# Comparing `tmp/gruel-4.1.2.tar.gz` & `tmp/gruel-4.2.0.tar.gz`

## Comparing `gruel-4.1.2.tar` & `gruel-4.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 gruel-4.1.2/src/gruel/__init__.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 gruel-4.1.2/src/gruel/brewer.py
--rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 gruel-4.1.2/src/gruel/core.py
--rw-r--r--   0        0        0    19712 2020-02-02 00:00:00.000000 gruel-4.1.2/src/gruel/crawler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gruel-4.1.2/src/gruel/py.typed
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 gruel-4.1.2/src/gruel/requests.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gruel-4.1.2/src/gruel/subgruel.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 gruel-4.1.2/src/gruel/template.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gruel-4.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gruel-4.1.2/LICENSE.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gruel-4.1.2/README.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 gruel-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 gruel-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 gruel-4.2.0/src/gruel/__init__.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 gruel-4.2.0/src/gruel/brewer.py
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 gruel-4.2.0/src/gruel/core.py
+-rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 gruel-4.2.0/src/gruel/crawler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gruel-4.2.0/src/gruel/py.typed
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 gruel-4.2.0/src/gruel/requests.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gruel-4.2.0/src/gruel/subgruel.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 gruel-4.2.0/src/gruel/template.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gruel-4.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gruel-4.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gruel-4.2.0/README.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 gruel-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 gruel-4.2.0/PKG-INFO
```

### Comparing `gruel-4.1.2/src/gruel/__init__.py` & `gruel-4.2.0/src/gruel/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     CrawlScraper,
     LimitCheckerMixin,
     SeleniumCrawler,
     UrlManager,
 )
 from .requests import Response, Session, request, retry_on_codes
 
-__version__ = "4.1.2"
+__version__ = "4.2.0"
 __all__ = [
     "Brewer",
     "GruelFinder",
     "Gruel",
     "ChoresMixin",
     "ParserMixin",
     "request",
```

### Comparing `gruel-4.1.2/src/gruel/brewer.py` & `gruel-4.2.0/src/gruel/brewer.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.2/src/gruel/core.py` & `gruel-4.2.0/src/gruel/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,23 @@
 
 class ParserMixin(abc.ABC):
     """Core parser functionality for scraper classes."""
 
     def __init__(self):
         super().__init__()
         self.flush_items()
+        self._show_parse_items_prog_bar = False
+
+    @property
+    def show_parse_items_prog_bar(self) -> bool:
+        return self._show_parse_items_prog_bar
+
+    @show_parse_items_prog_bar.setter
+    def show_parse_items_prog_bar(self, should_show: bool):
+        self._show_parse_items_prog_bar = should_show
 
     def flush_items(self):
         """Flush `parsable_items` and `parsed_items`."""
         self.parsable_items: list[Any] = []
         self.parsed_items: list[Any] = []
 
     @abc.abstractmethod
@@ -62,20 +71,18 @@
         >>>   try:
         >>>     return self.parse_item(item)
         >>>   except Exception as e:
         >>>     print(e)
         """
         return self.parse_item(item)
 
-    def parse_items(
-        self, parsable_items: Sequence[Any], show_progress: bool
-    ) -> list[Any]:
+    def parse_items(self, parsable_items: Sequence[Any]) -> list[Any]:
         """Parse items and return them."""
         parsed_items: list[Any] = []
-        for item in track(parsable_items, disable=not show_progress):
+        for item in track(parsable_items, disable=not self.show_parse_items_prog_bar):
             parsed_item = self.parse_item_wrapper(item)
             parsed_items.append(parsed_item)
         return parsed_items
 
 
 class ScraperMetricsMixin:
     """Mixin for various run time scraper stats."""
@@ -95,30 +102,63 @@
             self.fail_count > 0
             or self.failed_to_get_parsable_items
             or self.unexpected_failure_occured
         )
 
 
 class Gruel(ParserMixin, ScraperMetricsMixin, loggi.LoggerMixin, ChoresMixin):
-    def __init__(self, name: str | None = None, log_dir: Pathish = "logs"):
+    def __init__(
+        self,
+        name: str | None = None,
+        log_dir: Pathish = "logs",
+        show_parse_items_prog_bar: bool = False,
+    ):
         """
         :params:
         * `name`: The name of this scraper. If `None`, the name will be the stem of the file this class/subclass was defined in.
         i.e. A `Gruel` subclass located in a file called `myscraper.py` will have the name `"myscraper"`.
         * `log_dir`: The directory this scraper's logs should be saved to.
         """
         super().__init__()
         self._name = name
         self.init_logger(self.name, log_dir)
+        self.show_parse_items_prog_bar = show_parse_items_prog_bar
 
     @property
     def name(self) -> str:
         """Returns the name given to __init__ or the stem of the file this instance was defined in if one wasn't given."""
         return self._name or Pathier(inspect.getsourcefile(type(self))).stem  # type: ignore
 
+    def _fetch_and_parse(self):
+        """Fetch source content and pass to parsing workflow."""
+        try:
+            source = self.get_source()
+        except Exception as e:
+            self.logger.exception(f"Error getting source data.")
+        else:
+            self._parse_source(source)
+
+    def _parse_source(self, source: Any):
+        """
+        Run the parsing workflow and handle errors.
+        """
+        try:
+            self.parsable_items = self.get_parsable_items(source)
+            self.logger.info(
+                f"{self.name}:get_parsable_items() returned {len(self.parsable_items)} items."
+            )
+        except Exception:
+            self.failed_to_get_parsable_items = True
+            self.logger.exception(f"Error in {self.name}:get_parsable_items().")
+        else:
+            self.parsed_items = self.parse_items(self.parsable_items)
+            self.logger.info(
+                f"Scrape completed in {self.timer.elapsed_str} with {self.success_count} successes and {self.fail_count} failures."
+            )
+
     @abc.abstractmethod
     def get_source(self) -> Any:
         """Should fetch and return the raw data to be scraped.
 
         Typically would request a webpage and return the response."""
 
     @override
@@ -168,45 +208,26 @@
                 to a CA bundle to use. Defaults to ``True``.
         `stream`: if ``False``, the response content will be immediately downloaded.
         `cert`: if String, path to ssl client cert file (.pem). If Tuple, ('cert', 'key') pair.
         """
         kwargs["logger"] = self.logger
         return request(*args, **kwargs)
 
-    def scrape(self, parse_items_prog_bar_display: bool = False):
+    def scrape(self):
         """Run the scraper:
         1. prescrape chores
         2. get parsable items
         3. parse items
         4. store items
         5. postscrape chores"""
         try:
             self.timer.start()
             self.logger.info("Scrape started.")
             self.prescrape_chores()
-            try:
-                source = self.get_source()
-            except Exception as e:
-                self.logger.exception(f"Error getting source data.")
-            else:
-                try:
-                    self.parsable_items = self.get_parsable_items(source)
-                    self.logger.info(
-                        f"{self.name}:get_parsable_items() returned {len(self.parsable_items)} items."
-                    )
-                except Exception:
-                    self.failed_to_get_parsable_items = True
-                    self.logger.exception(f"Error in {self.name}:get_parsable_items().")
-                else:
-                    self.parsed_items = self.parse_items(
-                        self.parsable_items, parse_items_prog_bar_display
-                    )
-                    self.logger.info(
-                        f"Scrape completed in {self.timer.elapsed_str} with {self.success_count} successes and {self.fail_count} failures."
-                    )
+            self._fetch_and_parse()
             self.store_items(self.parsed_items)
         except Exception:
             self.unexpected_failure_occured = True
             self.logger.exception(f"Unexpected failure in {self.name}:scrape()")
         self.postscrape_chores()
         self.logger.close()
```

### Comparing `gruel-4.1.2/src/gruel/crawler.py` & `gruel-4.2.0/src/gruel/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             )
         except Exception as e:
             self.logger.exception(f"Error getting parsable items from `{source.url}`.")
         else:
             # Since likely usage is multithreaded,
             # don't want to pull from shared `self.parsed_items` container
             # when storing items
-            parsed_items = self.parse_items(parsable_items, False)
+            parsed_items = self.parse_items(parsable_items)
             for item in parsed_items:
                 self.parsed_items.append(item)
             self.store_items(parsed_items)
 
     @abc.abstractmethod
     def store_items(self, items: Sequence[Any]) -> None:
         """
```

### Comparing `gruel-4.1.2/src/gruel/requests.py` & `gruel-4.2.0/src/gruel/requests.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.2/src/gruel/subgruel.py` & `gruel-4.2.0/src/gruel/subgruel.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.2/src/gruel/template.py` & `gruel-4.2.0/src/gruel/template.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.2/LICENSE.txt` & `gruel-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gruel-4.1.2/pyproject.toml` & `gruel-4.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "gruel"
 description = "Another scraping framework"
-version = "4.1.2"
+version = "4.2.0"
 dependencies = ["pathier", "printbuddies", "younotyou", "noiftimer", "requests", "whosyouragent", "quickpool", "loggi", "beautifulsoup4", "rich", "scrapetools", "typing_extensions", "urllib3", "seleniumuser"]
 readme = "README.md"
 keywords = ["scrape", "scraping", "webscraping", "webscraper", "beautifulsoup", "framework"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10, <=3.12"
 
 [[project.authors]]
```

### Comparing `gruel-4.1.2/PKG-INFO` & `gruel-4.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gruel
-Version: 4.1.2
+Version: 4.2.0
 Summary: Another scraping framework
 Project-URL: Homepage, https://github.com/matt-manes/gruel
 Project-URL: Documentation, https://github.com/matt-manes/gruel/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gruel/tree/main/src/gruel
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: beautifulsoup,framework,scrape,scraping,webscraper,webscraping
```


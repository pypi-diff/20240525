# Comparing `tmp/secretscraper-1.3.9.7a2.tar.gz` & `tmp/secretscraper-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.9.7a2.tar", max compression
+gzip compressed data, was "secretscraper-1.4.tar", max compression
```

## Comparing `secretscraper-1.3.9.7a2.tar` & `secretscraper-1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.7a2/LICENSE
--rw-r--r--   0        0        0     9074 2024-05-24 03:17:08.607752 secretscraper-1.3.9.7a2/README.md
--rw-r--r--   0        0        0     1913 2024-05-24 08:06:04.088907 secretscraper-1.3.9.7a2/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-24 08:06:04.084309 secretscraper-1.3.9.7a2/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     8095 2024-05-24 07:55:26.370351 secretscraper-1.3.9.7a2/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.7a2/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2716 2024-05-24 03:03:31.799544 secretscraper-1.3.9.7a2/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.7a2/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    17291 2024-05-24 05:21:32.853650 secretscraper-1.3.9.7a2/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1503 2024-05-24 05:17:11.505719 secretscraper-1.3.9.7a2/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.7a2/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14636 2024-05-24 03:03:31.805841 secretscraper-1.3.9.7a2/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.7a2/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6774 2024-04-30 09:28:19.272007 secretscraper-1.3.9.7a2/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.7a2/src/secretscraper/log.py
--rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.7a2/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.7a2/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.7a2/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     4034 2024-05-24 08:05:45.193418 secretscraper-1.3.9.7a2/src/secretscraper/util.py
--rw-r--r--   0        0        0    10560 1970-01-01 00:00:00.000000 secretscraper-1.3.9.7a2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.4/LICENSE
+-rw-r--r--   0        0        0     9789 2024-05-25 15:21:16.098224 secretscraper-1.4/README.md
+-rw-r--r--   0        0        0     1906 2024-05-25 15:21:28.935811 secretscraper-1.4/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-05-25 15:21:33.253188 secretscraper-1.4/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     8126 2024-05-25 15:17:52.191299 secretscraper-1.4/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.4/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2716 2024-05-24 03:03:31.799544 secretscraper-1.4/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.4/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    17518 2024-05-25 15:25:58.666517 secretscraper-1.4/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1644 2024-05-25 14:38:52.673178 secretscraper-1.4/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.4/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14809 2024-05-25 15:17:52.196221 secretscraper-1.4/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.4/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6774 2024-04-30 09:28:19.272007 secretscraper-1.4/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.4/src/secretscraper/log.py
+-rw-r--r--   0        0        0    10048 2024-05-25 15:01:55.500803 secretscraper-1.4/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.4/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.4/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     4034 2024-05-24 08:05:45.193418 secretscraper-1.4/src/secretscraper/util.py
+-rw-r--r--   0        0        0    11269 1970-01-01 00:00:00.000000 secretscraper-1.4/PKG-INFO
```

### Comparing `secretscraper-1.3.9.7a2/LICENSE` & `secretscraper-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/README.md` & `secretscraper-1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                                example*
   -f, --url-file FILE          Target urls file, separated by line break
   -i, --config FILE            Set config file, defaults to settings.yml
   -m, --mode [1|2]             Set crawl mode, 1(normal) for max_depth=1,
                                2(thorough) for max_depth=2, default 1
   --max-page INTEGER           Max page number to crawl, default 100000
   --max-depth INTEGER          Max depth to crawl, default 1
-  -o, --outfile FILE           Output result to specified file
+  -o, --outfile FILE           Output result to specified file in csv format
   -s, --status TEXT            Filter response status to display, seperated by
                                commas, e.g. 200,300-400
   -x, --proxy TEXT             Set proxy, e.g. http://127.0.0.1:8080,
                                socks5://127.0.0.1:7890
   -H, --hide-regex             Hide regex search result
   -F, --follow-redirects       Follow redirects
   -u, --url TEXT               Target url
@@ -118,37 +118,47 @@
 The max depth is set to 1, which means only the start urls will be crawled. To change that, you can specify
 via `--max-depth <number>`. Or in a simpler way, use `-m 2` to run the crawler in thorough mode which is equivalent
 to `--max-depth 2`. By default the normal mode `-m 1` is adopted with max depth set to 1.
 ```bash
 secretscraper -u https://scrapeme.live/shop/ -m 2
 ```
 
-#### Write Results to File
+#### Write Results to Csv File
 ```bash
-secretscraper -u https://scrapeme.live/shop/ -o result.log
+secretscraper -u https://scrapeme.live/shop/ -o result.csv
 ```
 
 #### Hide Regex Result
 Use `-H` option to hide regex-matching results. Only found links will be displayed.
 ```bash
 secretscraper -u https://scrapeme.live/shop/ -H
 ```
 
 #### Extract secrets from local file
 ```bash
 secretscraper -l <dir or file>
 ```
 
+#### Switch to hyperscan
+I have implemented the regex matching functionality with both `hyperscan` and `re` module, `re` module is used as default, if you purse higher performance, you can switch to `hyperscan` by changing the `handler_type` to `hyperscan` in `settings.yml`.
+
+There are some pitfalls of `hyperscan` which you have to take caution to use it:
+1. not support regex group: you can not extract content by parentheses.
+2. different syntax from `re`
+
+You'd better write regex separately for the two regex engine.
+
 #### Customize Configuration
 The built-in config is shown as below. You can assign custom configuration via `-i settings.yml`.
 ```yaml
 verbose: false
 debug: false
 loglevel: critical
 logpath: log
+handler_type: re
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
 follow_redirects: true
 workers_num: 1000
@@ -227,14 +237,18 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.5.25 Version 1.4
+- Support csv output
+- Set `re` module as regex engine by default
+- Support to select regex engine by configuration `handler_type`
 ## 2024.4.30 Version 1.3.9
 - Add `--validate` option: Validate urls after the crawler finish, which helps reduce useless links
 - Optimize url collector
 - Optimize built-in regex
 ## 2024.4.29 Version 1.3.8
 - Optimize log output
 - Optimize the performance of `--debug` option
```

### Comparing `secretscraper-1.3.9.7a2/pyproject.toml` & `secretscraper-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.9.7.a2"
+version = "1.4"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/cmdline.py` & `secretscraper-1.4/src/secretscraper/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 @click.option(
     "--max-page", help="Max page number to crawl, default 100000", type=click.INT
 )
 @click.option("--max-depth", help="Max depth to crawl, default 1", type=click.INT)
 @click.option(
     "-o",
     "--outfile",
-    help="Output result to specified file",
+    help="Output result to specified file in csv format",
     type=click.Path(
         exists=False, file_okay=True, dir_okay=False, path_type=pathlib.Path
     ),
 )
 @click.option(
     "-s",
     "--status",
@@ -167,14 +167,15 @@
         return
     click.echo(f"Generating default configuration: {file.name}")
     file.write_text(
         r"""verbose: false
 debug: false
 loglevel: critical
 logpath: log
+handler_type: re
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
 follow_redirects: true
 workers_num: 1000
```

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/config/__init__.py` & `secretscraper-1.4/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/config/settings.yml` & `secretscraper-1.4/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/coroutinue.py` & `secretscraper-1.4/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/crawler.py` & `secretscraper-1.4/src/secretscraper/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,19 @@
             return
         logger.debug(f"Processing {url_node.url}")
         self.total_page += 1
         response = await self.fetch(url_node.url)
         if response is not None:  # and response.status == 200
             url_node.response_status = str(response.status_code)
             url_node.title = get_response_title(response)
+            try:
+                url_node.content_length = int(response.headers.get('content-length'))
+            except Exception:
+                pass
+            url_node.content_type = response.headers.get('content-type')
             response_text: str = response.text
             # try:
             #     response_text: str = await response.text(
             #         encoding="utf8", errors="ignore"
             #     )
             # except TimeoutError:
             #     logger.error(f"Timeout while reading response from {url_node.url}")
```

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/entity.py` & `secretscraper-1.4/src/secretscraper/entity.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     """
 
     url: str = field(hash=False, compare=False)
     url_object: ParseResult = field(hash=True, compare=True)
     response_status: str = field(default="Unknown", hash=False, compare=False)
     depth: int = field(default=0, hash=False, compare=False)
     parent: typing.Optional["URLNode"] = field(default=None, hash=False, compare=False)
-    title:str = field(hash=False, compare=False, default="")
+    content_length: int = field(hash=False, compare=False, default=-1)
+    content_type: str = field(hash=False, compare=False, default="")
+    title: str = field(hash=False, compare=False, default="")
 
     def __post_init__(self):
         if self.parent is not None and self.depth <= self.parent.depth:
             raise ValueError(
                 f"URLNode: depth({self.depth}) must be greater than that of parent({self.parent.depth})"
             )
```

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/exception.py` & `secretscraper-1.4/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/facade.py` & `secretscraper-1.4/src/secretscraper/facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,20 @@
 logger = logging.getLogger(__name__)
 
 warnings.filterwarnings("ignore")  # ignore all warnings
 
 
 def print_func(f: typing.IO, func: typing.Callable, content: str, **kwargs) -> None:
     func(content, **kwargs)
-    func(content, file=f, **kwargs)
+    if f is not None:
+        func(content, file=f, **kwargs)
 
 
 def print_func_colorful(
-    f: typing.IO,
+    f: typing.Optional[typing.IO],
     func: typing.Callable,
     content: str,
     fg: str = None,
     bg: str = None,
     blink=False,
     bold=False,
 ):
@@ -66,74 +67,79 @@
         :param custom_settings: dict
         :param print_func: must be partial of click.echo()
         """
         self.settings = full_settings
         self.custom_settings = custom_settings
         self.formatter = Formatter()
         self.hide_regex: bool = False
-        self.outfile = pathlib.Path(__file__).parent / "crawler.log"
+        self.outfile: typing.Optional[pathlib.Path] = None  # pathlib.Path(__file__).parent / "crawler.log"
         self.print_func = print_func
         self.debug: bool = False
         self.follow_redirects: bool = False
         self.detail_output: bool = False
         self.crawler: Crawler = self.create_crawler()
 
     def start(self):
         """Start the crawler and output"""
-        with self.outfile.open("w") as f:
-            try:
-
-                # print_func(f"Starting crawler...")
-                print_func_colorful(f,
-                                    self.print_func,
-                                    f"Target URLs: {', '.join(self.crawler.start_urls)}",
-                                    bold=True,
-                                    blink=True,
-                                    )
-                self.crawler.start()
-                self.crawler.start_validate()
-                if self.detail_output:
-                    # print_func_colorful(self.print_func,f"Total page: {self.crawler.total_page}")
-                    f.write(self.formatter.output_url_hierarchy(self.crawler.url_dict, True))
-
-                    if not self.hide_regex:
-                        print_func_colorful(f, self.print_func,
-                                            f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
-                                            )
-                    print_func_colorful(f, self.print_func, f"{self.formatter.output_js(self.crawler.js_dict)}")
-                    f.write(self.formatter.output_found_domains(list(self.crawler.found_urls), True))
-                else:
-                    # tidy output
-                    # URLs per domain
-                    domains = set()
-                    for url in self.crawler.start_urls:
-                        try:
-                            obj = urlparse(url)
-                            domain, _ = to_host_port(obj.netloc)
-                            if len(domain) > 0:
-                                domains.add(domain.strip())
-                        except:
-                            pass
-                    f.write(self.formatter.output_url_per_domain(domains, self.crawler.url_dict))
-                    # JS per domain
-                    f.write(self.formatter.output_url_per_domain(domains, self.crawler.js_dict, "JS"))
-                    # Domains
-                    f.write(self.formatter.output_found_domains(list(self.crawler.found_urls), True))
-                    # Secrets
-                    if not self.hide_regex:
-                        print_func_colorful(f, self.print_func,
-                                            f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
-                                            )
-            except KeyboardInterrupt:
-                self.print_func("\nExiting...")
-                self.crawler.close_all()
-            except Exception as e:
-                self.print_func(f"Unexpected error: {e}.\nExiting...")
-                self.crawler.close_all()
-                # raise FacadeException from e
+        # with self.outfile.open("w") as f:
+        f = None
+        try:
+
+            # print_func(f"Starting crawler...")
+            print_func_colorful(f,
+                                self.print_func,
+                                f"Target URLs: {', '.join(self.crawler.start_urls)}",
+                                bold=True,
+                                blink=True,
+                                )
+            self.crawler.start()
+            self.crawler.start_validate()
+            if self.detail_output:
+                # print_func_colorful(self.print_func,f"Total page: {self.crawler.total_page}")
+                self.formatter.output_url_hierarchy(self.crawler.url_dict, True)
+
+                if not self.hide_regex:
+                    print_func_colorful(f, self.print_func,
+                                        f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
+                                        )
+                print_func_colorful(f, self.print_func, f"{self.formatter.output_js(self.crawler.js_dict)}")
+                self.formatter.output_found_domains(list(self.crawler.found_urls), True)
+            else:
+                # tidy output
+                # URLs per domain
+                domains = set()
+                for url in self.crawler.start_urls:
+                    try:
+                        obj = urlparse(url)
+                        domain, _ = to_host_port(obj.netloc)
+                        if len(domain) > 0:
+                            domains.add(domain.strip())
+                    except:
+                        pass
+                self.formatter.output_url_per_domain(domains, self.crawler.url_dict)
+                # JS per domain
+                self.formatter.output_url_per_domain(domains, self.crawler.js_dict, "JS")
+                # Domains
+                self.formatter.output_found_domains(list(self.crawler.found_urls), True)
+                # Secrets
+                if not self.hide_regex:
+                    print_func_colorful(f, self.print_func,
+                                        f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
+                                        )
+            if self.outfile is not None:
+                self.formatter.output_csv(self.outfile, self.crawler.url_dict, self.crawler.url_secrets)
+                print_func_colorful(None, self.print_func, f"Save result to csv file {self.outfile.name}", fg="green",
+                                    bold=True)
+        except KeyboardInterrupt:
+            self.print_func("\nExiting...")
+            self.crawler.close_all()
+        except Exception as e:
+            self.print_func(f"Unexpected error: {e}.\nExiting...")
+            self.crawler.close_all()
+            # raise FacadeException from e
 
     def create_crawler(self) -> Crawler:
         """Create a Crawler"""
         # No validate
         if self.custom_settings.get("validate", False) is True:
             validate = True
         else:
@@ -256,15 +262,15 @@
         # Verbose
         verbose: typing.Optional[bool] = self.custom_settings.get("verbose", None)
         if verbose is not None:
             self.settings["verbose"] = verbose
 
         # Read rules from config file
         rules: typing.Dict[str, str] = read_rules_from_setting(self.settings)
-        handler_type = self.settings.get("handler_type", "regex")
+        handler_type = self.settings.get("handler_type", "re")
         if handler_type == "hyperscan":
             handler = get_regex_handler(rules)
             print_config(f"Using regex handler: Hyperscan")
         else:
             handler = get_regex_handler(rules, type_="regex", use_groups=True)
             print_config(f"Using regex handler: Re")
```

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/filter.py` & `secretscraper-1.4/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/handler.py` & `secretscraper-1.4/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/log.py` & `secretscraper-1.4/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/output_formatter.py` & `secretscraper-1.4/src/secretscraper/output_formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,16 @@
             return click.style(status, fg="yellow")
         elif 400 <= status < 500:
             return click.style(status, fg="magenta")
         else:
             return click.style(status, fg="red")
 
     def format_normal_result(self, content: str) -> str:
+        if content == "":
+            return ""
         return click.style(content, fg="bright_blue")
 
     def filter(self, url: URLNode) -> bool:
         """Determine whether a url should be displayed"""
         try:
             if int(url.response_status) == 404:  # filter 404 by default
                 return False
@@ -63,14 +65,21 @@
                     continue
                 else:
                     return False
             except ValueError:
                 return False  # default discard
         return True
 
+    def format_single_url(self, url: URLNode) -> str:
+        return self.format_normal_result(f"{str(url.url)}") \
+            + " [" \
+            + self.format_colorful_status(url.response_status) \
+            + "]" \
+            + f" [Content-Length: {self.format_normal_result(str(url.content_length)) if url.content_length > 0 else ''}] [Content-Type: {self.format_normal_result(url.content_type)}] [Title: {self.format_normal_result(url.title)}]"
+
     def output_found_domains(
         self, found_urls: typing.Iterable[URLNode], is_print: bool = False
     ) -> str:
         """Output the found domains"""
         if not is_print:
             urls = {str(url.url_object.netloc) for url in found_urls}
             found_urls_str = "\n".join(urls)
@@ -89,29 +98,26 @@
         self, url_dict: typing.Dict[URLNode, typing.Iterable[URLNode]], is_print: bool = False
     ) -> str:
         """Output the url hierarchy"""
         if not is_print:
             url_hierarchy = ""
             for base, urls in url_dict.items():
                 url_set = {
-                    f"{str(url.url)} [{str(url.response_status)}]"
+                    self.format_single_url(url)
                     for url in urls
                     if self.filter(url)
                 }
                 urls_str = "\n".join(url_set)
                 url_hierarchy += f"\n{len(url_set)} URLs from {base.url} [{str(base.response_status)}] (depth:{base.depth}):\n{urls_str}\n"
             return url_hierarchy
         else:
             url_hierarchy = ""
             for base, urls in url_dict.items():
                 url_set = {
-                    self.format_normal_result(f"{str(url.url)}")
-                    + " ["
-                    + self.format_colorful_status(url.response_status)
-                    + "]"
+                    self.format_single_url(url)
                     for url in urls
                     if self.filter(url)
                 }
                 urls_str = "\n".join(url_set)
                 url_hierarchy += f"\n{len(url_set)} URLs from {base.url} [{str(base.response_status)}] (depth:{base.depth}):\n{urls_str}"
                 click.echo(
                     f"\n{len(url_set)} URLs from {base.url} ["
@@ -144,18 +150,15 @@
             keys.remove("Other")
             keys.append("Other")
         for domain in keys:
             urls = domain_secrets[domain]
             if urls is None or len(urls) == 0:
                 continue
             url_set = {
-                self.format_normal_result(f"{str(url.url)}")
-                + " ["
-                + self.format_colorful_status(url.response_status)
-                + "]"
+                self.format_single_url(url)
                 for url in urls
                 if self.filter(url)
             }
             urls_str = "\n".join(url_set)
             url_hierarchy += f"\n{len(url_set)} {url_type} from {domain}:\n{urls_str}\n"
         click.echo(url_hierarchy)
 
@@ -223,7 +226,30 @@
                 }
                 secrets_str = "\n".join(secret_set)
                 s = click.style(f"\n{len(secret_set)} Secrets found in {str(path)}:", fg="cyan") + \
                     f"\n{secrets_str}\n"
                 result += s
                 click.echo(s)
         return result
+
+    def output_csv(
+        self,
+        outfile: pathlib.Path,
+        url_dict: typing.Dict[URLNode, typing.Iterable[URLNode]],
+        url_secrets: typing.Dict[URLNode, typing.Iterable[Secret]],
+
+    ) -> None:
+        import csv
+        with outfile.open("w", encoding='utf-8', errors='replace') as f:
+            writer = csv.writer(f)
+            writer.writerow(("URL", "Title", "Response Code", "Content Length", "Content Type", "Secrets"))
+            url_nodes: typing.Set[URLNode] = set()
+            for key, urls in url_dict.items():
+                url_nodes.add(key)
+                for url in urls:
+                    url_nodes.add(url)
+            for url in url_nodes:
+                row = [url.url, url.title, url.response_status, url.content_length, url.content_type]
+                if url in url_secrets:
+                    secrets = [f"{secret.type}: {secret.data}" for secret in url_secrets[url]]
+                    row += ['\n'.join(secrets)]
+                writer.writerow(row)
```

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/scanner.py` & `secretscraper-1.4/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/urlparser.py` & `secretscraper-1.4/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/src/secretscraper/util.py` & `secretscraper-1.4/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.7a2/PKG-INFO` & `secretscraper-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.9.7a2
+Version: 1.4
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -115,15 +115,15 @@
                                example*
   -f, --url-file FILE          Target urls file, separated by line break
   -i, --config FILE            Set config file, defaults to settings.yml
   -m, --mode [1|2]             Set crawl mode, 1(normal) for max_depth=1,
                                2(thorough) for max_depth=2, default 1
   --max-page INTEGER           Max page number to crawl, default 100000
   --max-depth INTEGER          Max depth to crawl, default 1
-  -o, --outfile FILE           Output result to specified file
+  -o, --outfile FILE           Output result to specified file in csv format
   -s, --status TEXT            Filter response status to display, seperated by
                                commas, e.g. 200,300-400
   -x, --proxy TEXT             Set proxy, e.g. http://127.0.0.1:8080,
                                socks5://127.0.0.1:7890
   -H, --hide-regex             Hide regex search result
   -F, --follow-redirects       Follow redirects
   -u, --url TEXT               Target url
@@ -146,37 +146,47 @@
 The max depth is set to 1, which means only the start urls will be crawled. To change that, you can specify
 via `--max-depth <number>`. Or in a simpler way, use `-m 2` to run the crawler in thorough mode which is equivalent
 to `--max-depth 2`. By default the normal mode `-m 1` is adopted with max depth set to 1.
 ```bash
 secretscraper -u https://scrapeme.live/shop/ -m 2
 ```
 
-#### Write Results to File
+#### Write Results to Csv File
 ```bash
-secretscraper -u https://scrapeme.live/shop/ -o result.log
+secretscraper -u https://scrapeme.live/shop/ -o result.csv
 ```
 
 #### Hide Regex Result
 Use `-H` option to hide regex-matching results. Only found links will be displayed.
 ```bash
 secretscraper -u https://scrapeme.live/shop/ -H
 ```
 
 #### Extract secrets from local file
 ```bash
 secretscraper -l <dir or file>
 ```
 
+#### Switch to hyperscan
+I have implemented the regex matching functionality with both `hyperscan` and `re` module, `re` module is used as default, if you purse higher performance, you can switch to `hyperscan` by changing the `handler_type` to `hyperscan` in `settings.yml`.
+
+There are some pitfalls of `hyperscan` which you have to take caution to use it:
+1. not support regex group: you can not extract content by parentheses.
+2. different syntax from `re`
+
+You'd better write regex separately for the two regex engine.
+
 #### Customize Configuration
 The built-in config is shown as below. You can assign custom configuration via `-i settings.yml`.
 ```yaml
 verbose: false
 debug: false
 loglevel: critical
 logpath: log
+handler_type: re
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
 follow_redirects: true
 workers_num: 1000
@@ -255,14 +265,18 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.5.25 Version 1.4
+- Support csv output
+- Set `re` module as regex engine by default
+- Support to select regex engine by configuration `handler_type`
 ## 2024.4.30 Version 1.3.9
 - Add `--validate` option: Validate urls after the crawler finish, which helps reduce useless links
 - Optimize url collector
 - Optimize built-in regex
 ## 2024.4.29 Version 1.3.8
 - Optimize log output
 - Optimize the performance of `--debug` option
```


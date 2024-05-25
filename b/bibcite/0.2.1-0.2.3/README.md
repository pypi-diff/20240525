# Comparing `tmp/bibcite-0.2.1.tar.gz` & `tmp/bibcite-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibcite-0.2.1.tar", last modified: Thu May 23 22:18:20 2024, max compression
+gzip compressed data, was "bibcite-0.2.3.tar", last modified: Sat May 25 21:33:09 2024, max compression
```

## Comparing `bibcite-0.2.1.tar` & `bibcite-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 22:18:20.490246 bibcite-0.2.1/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      905 2024-05-23 22:18:20.490246 bibcite-0.2.1/PKG-INFO
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 22:18:20.490246 bibcite-0.2.1/bibcite/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-05-23 17:02:29.000000 bibcite-0.2.1/bibcite/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      919 2024-05-23 18:16:53.000000 bibcite-0.2.1/bibcite/cli.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5252 2024-05-23 22:17:15.000000 bibcite-0.2.1/bibcite/work.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 22:18:20.490246 bibcite-0.2.1/bibcite.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      905 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      280 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      393 2024-05-23 22:18:05.000000 bibcite-0.2.1/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      585 2024-05-23 18:16:35.000000 bibcite-0.2.1/readme.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       27 2024-05-23 17:01:23.000000 bibcite-0.2.1/requirements.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-05-23 22:18:20.490246 bibcite-0.2.1/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-25 21:33:09.027620 bibcite-0.2.3/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      905 2024-05-25 21:33:09.027620 bibcite-0.2.3/PKG-INFO
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-25 21:33:09.023620 bibcite-0.2.3/bibcite/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-05-23 17:02:29.000000 bibcite-0.2.3/bibcite/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1047 2024-05-23 22:25:04.000000 bibcite-0.2.3/bibcite/cli.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5801 2024-05-24 01:04:15.000000 bibcite-0.2.3/bibcite/work.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-25 21:33:09.027620 bibcite-0.2.3/bibcite.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      905 2024-05-25 21:33:09.000000 bibcite-0.2.3/bibcite.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      280 2024-05-25 21:33:09.000000 bibcite-0.2.3/bibcite.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-25 21:33:09.000000 bibcite-0.2.3/bibcite.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-05-25 21:33:09.000000 bibcite-0.2.3/bibcite.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-05-25 21:33:09.000000 bibcite-0.2.3/bibcite.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2024-05-25 21:33:09.000000 bibcite-0.2.3/bibcite.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      393 2024-05-24 01:02:43.000000 bibcite-0.2.3/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      585 2024-05-23 18:16:35.000000 bibcite-0.2.3/readme.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       27 2024-05-23 17:01:23.000000 bibcite-0.2.3/requirements.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-05-25 21:33:09.027620 bibcite-0.2.3/setup.cfg
```

### Comparing `bibcite-0.2.1/PKG-INFO` & `bibcite-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibcite
-Version: 0.2.1
+Version: 0.2.3
 Summary: Generate bibtex citations from command line and instantly copies them to clipboard
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pyperclip
 Requires-Dist: tabulate
```

### Comparing `bibcite-0.2.1/bibcite/cli.py` & `bibcite-0.2.3/bibcite/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import argparse
 import pyperclip
 from tabulate import tabulate
 from bibcite.work import Work
 
 def main():
     parser = argparse.ArgumentParser(description='Generate BibTeX citations from a title.')
-    parser.add_argument('title', type=str, help='The title of the work to generate a BibTeX citation for.')
+    parser.add_argument('--title', type=str, help='The title of the work to generate a BibTeX citation for')
+    parser.add_argument('--author', type=str, help='The author of the work', default=None)
     args = parser.parse_args()
 
     text = "Bibcite: Bibtex citations from the command line\n"
     table = [[text]]
     print(tabulate(table, tablefmt="grid"))
 
-    title = args.title
+    title, author = args.title, args.author
     try:
         print(f'- Searching for title \"{title}\"')
-        work = Work.from_query(title=title)
+        work = Work.from_query(title=title, author=author)
     except Exception as e:
         print(f'- An error occurred while trying to find work with title \"{title}\": {repr(e)}')
         return
 
     bibtex = work.to_bibtex()
     print(f'- Found BibTeX citation: \n{bibtex}')
     pyperclip.copy(bibtex)
```

### Comparing `bibcite-0.2.1/bibcite/work.py` & `bibcite-0.2.3/bibcite/work.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,84 +19,96 @@
     pages : Optional[str] = None
     volume : Optional[str] = None
 
     @classmethod
     def from_query(cls, title : str,
                    work_type : Optional[str] = None,
                    author : Optional[str] = None) -> Work:
-        response = cls._search_request(search_expression=title)
+        response = cls._search_request(title=title, author=author)
         paper_dicts = response.json()['results']
 
         if len(paper_dicts) == 0:
             raise ValueError(f"No papers found with title {title}")
 
-        relevant_papers = [p for p in paper_dicts if title.lower() in p['title'].lower()]
+        def paper_title_matchs(p : dict) -> bool:
+            try:
+                return title.lower() in p['title'].lower()
+            except:
+                return False
+
+        relevant_papers = [p for p in paper_dicts if paper_title_matchs(p)]
         relevant_papers = [p for p in relevant_papers if not p['doi'] is None]
         # print(f'Relevant paper titles = {[p["title"] for p in relevant_papers]}')
 
         if len(relevant_papers) == 0:
             raise ValueError(f"No works or no works with doi found with title {title}")
 
         if work_type:
             relevant_papers = [p for p in relevant_papers if p['type'] == work_type]
-        if author:
-            relevant_papers = [p for p in relevant_papers if author in cls.get_author(p)]
         if len(relevant_papers) == 0:
             raise ValueError(f"No papers found with title {title} and author {author}")
 
         # print(f'Crossref item = {cls.get_crossref_item(paper_doi)}')
         crossref_item = cls.get_crossref_item(paper_doi=relevant_papers[0]['doi'])
         journal_item = crossref_item.get('container-title')
         if journal_item:
             journal = journal_item[0]
         else:
             journal = None
 
-        # print(f'Found crossref item = {crossref_item}')
-
         new_work = Work(title= crossref_item['title'][0],
                         authors= crossref_item['author'],
                         year=crossref_item['published']['date-parts'][0][0],
                         doi=crossref_item['DOI'],
                         url= crossref_item['URL'],
                         work_type= crossref_item['type'],
                         journal=journal,
                         pages= crossref_item.get('page'),
                         volume= crossref_item.get('volume'))
         return new_work
 
-    @staticmethod
-    def get_author(paper_dict : dict):
-        try:
-            author_name = paper_dict['authorships'][0]['raw_author_name']
-        except:
-            author_name = ''
-        return author_name
 
     @staticmethod
     def get_crossref_item(paper_doi : str) -> dict:
         url = f"https://api.crossref.org/works/{paper_doi}"
         response = requests.get(url)
         if response.status_code != 200:
             raise ValueError(f"Request failed with status code {response.status_code}")
         data = response.json()
         return data['message']
 
     @staticmethod
-    def _search_request(search_expression : str) -> Response:
+    def _search_request(title: str, author: str = None) -> Response:
+        author_url = 'https://api.openalex.org/authors'
+        conditional_author_filter = ''
+        if author:
+            author_search_params = {
+                'filter': f'display_name.search:{author}',
+                'per_page': 1
+            }
+            author_response = requests.get(author_url, params=author_search_params)
+            author_data = author_response.json()
+            # print(f'Author data results = {author_data["results"]}')
+            author_openalex_url = author_data['results'][0]['id']
+            author_id = author_openalex_url.split('/')[-1]
+            # print(f'Author id = {author_id}')
+            conditional_author_filter = f',authorships.author.id:{author_id}'
+
         works_url = 'https://api.openalex.org/works'
         results_per_page = 200
 
+        title_filter = f'default.search:{title}'
+
         search_params = {
-            'filter': f'title.search:{search_expression}',
+            'filter': f'{title_filter}{conditional_author_filter}',
             'sort': 'relevance_score:desc',
             'per_page': results_per_page,
         }
-        response = requests.get(works_url, params=search_params)
 
+        response = requests.get(works_url, params=search_params)
         return response
 
     # ---------------------------------------------------------
 
     def to_bibtex(self) -> str:
         if self.work_type == 'journal-article':
             bibtex_type = 'article'
@@ -134,14 +146,12 @@
 
 if __name__ == "__main__":
     # Error titles: Titles for which currently no citation can be generated
     # -> t1: Missing author
     # -> t2: DOI not found in Crossref
     t1 = "Fundamentals of Powder Diffraction and Structural Characterization of Materials"
     t2 = "Attention is all you need"
-    t3 = 'Supernova limits on muonic dark forces'
-    introd_work = Work.from_query(title=t3)
+    t3 = 'Supernova'
+    introd_work = Work.from_query(title=t3, author='Jonas Spinner')
     print(f'Paper doi is {introd_work.doi}')
-    print(f'Intro work bibtext = \n{introd_work.to_bibtex()}')
+    print(f'Intro work bibtext: \n{introd_work.to_bibtex()}')
     # print(Work.get_crossref_item(paper_doi='10.1063/1.2807734'))
-
-
```

### Comparing `bibcite-0.2.1/bibcite.egg-info/PKG-INFO` & `bibcite-0.2.3/bibcite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibcite
-Version: 0.2.1
+Version: 0.2.3
 Summary: Generate bibtex citations from command line and instantly copies them to clipboard
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pyperclip
 Requires-Dist: tabulate
```

### Comparing `bibcite-0.2.1/readme.md` & `bibcite-0.2.3/readme.md`

 * *Files identical despite different names*


# Comparing `tmp/librus_apix-1.0.2.post1.tar.gz` & `tmp/librus_apix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-1.0.2.post1.tar", last modified: Wed May 22 19:17:27 2024, max compression
+gzip compressed data, was "librus_apix-1.0.3.tar", last modified: Sat May 25 09:35:06 2024, max compression
```

## Comparing `librus_apix-1.0.2.post1.tar` & `librus_apix-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:17:27.092200 librus_apix-1.0.2.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 19:17:27.092200 librus_apix-1.0.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:17:27.088200 librus_apix-1.0.2.post1/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:17:27.092200 librus_apix-1.0.2.post1/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 19:17:27.000000 librus_apix-1.0.2.post1/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-22 19:17:27.000000 librus_apix-1.0.2.post1/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:17:27.000000 librus_apix-1.0.2.post1/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 19:17:27.000000 librus_apix-1.0.2.post1/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 19:17:27.000000 librus_apix-1.0.2.post1/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 19:17:27.092200 librus_apix-1.0.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:17:24.000000 librus_apix-1.0.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:35:06.422921 librus_apix-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 09:35:03.000000 librus_apix-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 09:35:06.422921 librus_apix-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-25 09:35:03.000000 librus_apix-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:35:06.422921 librus_apix-1.0.3/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:35:06.422921 librus_apix-1.0.3/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 09:35:03.000000 librus_apix-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-25 09:35:06.422921 librus_apix-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 09:35:03.000000 librus_apix-1.0.3/setup.py
```

### Comparing `librus_apix-1.0.2.post1/LICENSE` & `librus_apix-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/README.md` & `librus_apix-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/__init__.py` & `librus_apix-1.0.3/librus_apix/__init__.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/announcements.py` & `librus_apix-1.0.3/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/attendance.py` & `librus_apix-1.0.3/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/client.py` & `librus_apix-1.0.3/librus_apix/client.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/completed_lessons.py` & `librus_apix-1.0.3/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/exceptions.py` & `librus_apix-1.0.3/librus_apix/exceptions.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/grades.py` & `librus_apix-1.0.3/librus_apix/grades.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,23 @@
     ...
 except ParseError as e:
     # Handle parse error
     ...
 ```
 """
 import re
+from collections import defaultdict
+from dataclasses import dataclass
+from typing import DefaultDict, List, Tuple, Union
+
 from bs4 import BeautifulSoup, Tag
+
 from librus_apix.client import Client
+from librus_apix.exceptions import ArgumentError, ParseError
 from librus_apix.helpers import no_access_check
-from librus_apix.exceptions import ParseError, ArgumentError
-from typing import DefaultDict, Union, Tuple, List
-from dataclasses import dataclass
-from collections import defaultdict
 
 
 @dataclass
 class Gpa:
     """
     Represents the Semestral Grade for a specific semester and subject.
 
@@ -231,14 +233,16 @@
         semester_grades = box.select('td[class!="center micro screen-only"]')
         if len(semester_grades) < 9:
             continue
         average_grades = list(map(lambda x: x.text, box.select("td.right")))
         semesters = [semester_grades[1:4], semester_grades[4:7]]
         subject = _handle_subject(semester_grades)
         for semester_number, semester in enumerate(semesters):
+            if subject not in sem_grades[semester_number]:
+                sem_grades[semester_number][subject] = []
             for sg in semester:
                 grade_a_improved = sg.select(
                     "td[class!='center'] > span > span.grade-box > a"
                 )
                 grade_a = (
                     sg.select("td[class!='center'] > span.grade-box > a")
                     + grade_a_improved
```

### Comparing `librus_apix-1.0.2.post1/librus_apix/helpers.py` & `librus_apix-1.0.3/librus_apix/helpers.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/homework.py` & `librus_apix-1.0.3/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/messages.py` & `librus_apix-1.0.3/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/notifications.py` & `librus_apix-1.0.3/librus_apix/notifications.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/schedule.py` & `librus_apix-1.0.3/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/student_information.py` & `librus_apix-1.0.3/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/timetable.py` & `librus_apix-1.0.3/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix/urls.py` & `librus_apix-1.0.3/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/librus_apix.egg-info/SOURCES.txt` & `librus_apix-1.0.3/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.2.post1/setup.cfg` & `librus_apix-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = v1.0.2-1
+version = v1.0.3
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```


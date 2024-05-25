# Comparing `tmp/online_scheduler-0.6.tar.gz` & `tmp/online_scheduler-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-0.6.tar", last modified: Sat May 25 06:16:27 2024, max compression
+gzip compressed data, was "online_scheduler-0.7.tar", last modified: Sat May 25 06:58:54 2024, max compression
```

## Comparing `online_scheduler-0.6.tar` & `online_scheduler-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:16:27.525380 online_scheduler-0.6/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:16:27.525188 online_scheduler-0.6/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:16:27.524372 online_scheduler-0.6/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 05:23:08.000000 online_scheduler-0.6/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2855 2024-05-25 06:15:43.000000 online_scheduler-0.6/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:16:27.524937 online_scheduler-0.6/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:16:27.000000 online_scheduler-0.6/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 06:16:27.525417 online_scheduler-0.6/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 06:15:50.000000 online_scheduler-0.6/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:58:54.156858 online_scheduler-0.7/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:58:54.156648 online_scheduler-0.7/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:58:54.155577 online_scheduler-0.7/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 05:23:08.000000 online_scheduler-0.7/online_scheduler/__init__.py
+-rw-r--r--   0 endo       (501) staff       (20)     2443 2024-05-25 06:58:09.000000 online_scheduler-0.7/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:58:54.156362 online_scheduler-0.7/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:58:54.000000 online_scheduler-0.7/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 06:58:54.000000 online_scheduler-0.7/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 06:58:54.000000 online_scheduler-0.7/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:58:54.000000 online_scheduler-0.7/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:58:54.000000 online_scheduler-0.7/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 06:58:54.157097 online_scheduler-0.7/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 06:58:13.000000 online_scheduler-0.7/setup.py
```

### Comparing `online_scheduler-0.6/online_scheduler/online_scheduler.py` & `online_scheduler-0.7/online_scheduler/online_scheduler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 import os
 import csv
 import webbrowser
 
-class ScheduleManager:
-    def __init__(self):
-        if not os.path.exists("url.csv"):
-            self.create_empty_schedule()
-            print("url.csvを作成したので起動し直してください")
-            quit()
-
-        self.matrix = self.load_schedule_from_csv()
-        self.sch = [
-            ["1限 |", "2限 |", "3限 |", "4限 |", "5限 |", "6限 |"],
-            ["10", "11", "12", "13", "14", "15"],
-            ["20", "21", "22", "23", "24", "25"],
-            ["30", "31", "32", "33", "34", "35"],
-            ["40", "41", "42", "43", "44", "45"],
-            ["50", "51", "52", "53", "54", "55"]
-        ]
-        self.row = len(self.sch)
-        self.col = len(self.sch[0])
-
-    def create_empty_schedule(self):
-        with open("url.csv", "w", newline="") as f:
-            writer = csv.writer(f)
-            writer.writerows([[""] * 6] * 6)
-
-    def load_schedule_from_csv(self):
-        matrix = []
-        with open("url.csv", "r") as f:
-            for line in f:
-                data = line.rstrip("\n").split(",")
-                matrix.append(data)
-        return matrix
-
-    def display_schedule(self):
-        print("時限\t月\t火\t水\t木\t金")
-        print("-------------------------------------------------")
-        for j in range(self.row):
-            for i in range(self.col):
-                if len(self.matrix[i][j]) >= 3:
-                    self.sch[i][j] = "\033[34m" + self.sch[i][j] + "\033[0m"
-                print(self.sch[i][j], end="\t")
-            print("")
-
-    def edit_schedule(self):
-        while True:
-            print("マスを選択 or w")
-            a = input()
-            if a == "w":
-                self.save_schedule_to_csv()
-                break
-            else:
-                b = int(a[0])
-                c = int(a[1])
-                print("URLを貼り付けor エンターキーで削除 ")
-                d = input()
-                self.matrix[b][c] = d
-                if len(d) == 0:
-                    self.sch[b][c] = "\033[0m" + self.sch[b][c] + "\033[0m"
-                else:
-                    self.sch[b][c] = "\033[34m" + self.sch[b][c] + "\033[0m"
-                self.display_schedule()
-
-    def save_schedule_to_csv(self):
-        with open("url.csv", "w", newline="") as f:
-            writer = csv.writer(f)
-            writer.writerows(self.matrix)
-
-    def run(self):
-        self.display_schedule()
-        print("編集⇨ a\t編集終了⇨ w\tマスを入力⇨ ブラウザを起動")
-
-        action = input()
-        if action == "a":
-            self.edit_schedule()
+def main():
+    if not os.path.exists("url.csv"):
+        create_empty_csv()
+
+    matrix = load_schedule_from_csv()
+
+    Num = ["1限 |", "2限 |", "3限 |", "4限 |", "5限 |", "6限 |"]
+    Mon = ["10", "11", "12", "13", "14", "15"]
+    Tue = ["20", "21", "22", "23", "24", "25"]
+    Wed = ["30", "31", "32", "33", "34", "35"]
+    Thu = ["40", "41", "42", "43", "44", "45"]
+    Fri = ["50", "51", "52", "53", "54", "55"]
+    sch = [Num, Mon, Tue, Wed, Thu, Fri]
+
+    row = len(sch)
+    col = len(sch[0])
+
+    print_schedule(matrix, sch)
+
+    print("編集⇨ a\t編集終了⇨ w\tマスを入力⇨ ブラウザを起動")
+    a = input()
+
+    if a == "a":
+        edit_schedule(matrix, sch)
+    else:
+        open_browser(matrix, a)
+
+def create_empty_csv():
+    with open("url.csv", "w", newline="") as f:
+        writer = csv.writer(f)
+        writer.writerows([[""] * 6] * 6)
+    print("url.csvを作成したので起動し直してください")
+
+def load_schedule_from_csv():
+    matrix = []
+    with open("url.csv", "r") as f:
+        for line in f:
+            data = line.rstrip("\n").split(",")
+            matrix.append(data)
+    return matrix
+
+def print_schedule(matrix, sch):
+    print("時限\t月\t火\t水\t木\t金")
+    print("-------------------------------------------------")
+    for j in range(len(sch)):
+        for i in range(len(sch[0])):
+            if len(matrix[i][j]) >= 3:
+                sch[i][j] = "\033[34m" + sch[i][j] + "\033[0m"
+            print(sch[i][j], end="\t")
+        print("")
+
+def edit_schedule(matrix, sch):
+    while True:
+        print("マスを選択 or w")
+        a = input()
+        if a == "w":
+            save_schedule_to_csv(matrix)
+            break
         else:
-            b = int(action[0])
-            c = int(action[1])
-            webbrowser.open(self.matrix[b][c], 2)
+            b = int(a[0])
+            c = int(a[1])
+            print("URLを貼り付けor エンターキーで削除 ")
+            d = input()
+            matrix[b][c] = d
+            if len(d) == 0:
+                sch[b][c] = "\033[0m" + sch[b][c] + "\033[0m"
+            else:
+                sch[b][c] = "\033[34m" + sch[b][c] + "\033[0m"
+            print_schedule(matrix, sch)
+
+def save_schedule_to_csv(matrix):
+    with open("url.csv", "w", newline="") as f:
+        writer = csv.writer(f)
+        writer.writerows(matrix)
+
+def open_browser(matrix, a):
+    b = int(a[0])
+    c = int(a[1])
+    webbrowser.open(matrix[b][c], 2)
 
 if __name__ == "__main__":
-    schedule_manager = ScheduleManager()
-    schedule_manager.run()
+    main()
```

### Comparing `online_scheduler-0.6/setup.py` & `online_scheduler-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='0.6',
+    version='0.7',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```


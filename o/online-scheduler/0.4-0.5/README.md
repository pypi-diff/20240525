# Comparing `tmp/online_scheduler-0.4.tar.gz` & `tmp/online_scheduler-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-0.4.tar", last modified: Sat May 25 05:23:29 2024, max compression
+gzip compressed data, was "online_scheduler-0.5.tar", last modified: Sat May 25 06:09:02 2024, max compression
```

## Comparing `online_scheduler-0.4.tar` & `online_scheduler-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 05:23:29.150372 online_scheduler-0.4/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 05:23:29.150112 online_scheduler-0.4/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 05:23:29.149118 online_scheduler-0.4/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 05:23:08.000000 online_scheduler-0.4/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2824 2024-05-25 04:19:53.000000 online_scheduler-0.4/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 05:23:29.149811 online_scheduler-0.4/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 05:23:29.000000 online_scheduler-0.4/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 05:23:29.000000 online_scheduler-0.4/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 05:23:29.000000 online_scheduler-0.4/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 05:23:29.000000 online_scheduler-0.4/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 05:23:29.000000 online_scheduler-0.4/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 05:23:29.150418 online_scheduler-0.4/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 05:23:14.000000 online_scheduler-0.4/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:09:02.029644 online_scheduler-0.5/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:09:02.029456 online_scheduler-0.5/PKG-INFO
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:09:02.028649 online_scheduler-0.5/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)        0 2024-05-25 05:23:08.000000 online_scheduler-0.5/online_scheduler/__init__.py
+-rw-r--r--   0 endo       (501) staff       (20)     2538 2024-05-25 06:07:28.000000 online_scheduler-0.5/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 06:09:02.029226 online_scheduler-0.5/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 06:09:02.000000 online_scheduler-0.5/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 06:09:02.029685 online_scheduler-0.5/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 06:08:27.000000 online_scheduler-0.5/setup.py
```

### Comparing `online_scheduler-0.4/online_scheduler/online_scheduler.py` & `online_scheduler-0.5/online_scheduler/online_scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,88 +1,85 @@
+
 import os
-import csv
-import webbrowser
+if not os.path.exists("url.csv"):
+    import csv
+    f = open("url.csv", "w", newline="")
+    data1 = [ [ "", "", "", "", "", "" ],
+              [ "", "", "", "", "", "" ],
+              [ "", "", "", "", "", "" ],
+              [ "", "", "", "", "", "" ],
+              [ "", "", "", "", "", "" ],
+              [ "", "", "", "", "", "" ] ]
+    writer = csv.writer(f)
+    writer.writerows(data1)
+    f.close
+    print("url.csvを作成したので起動し直してください")
+    quit()
+
+matrix = []
+f = open("url.csv", "r")
+while True:
+    data = f.readline()
+    if data == "":
+        break
+    data = data.rstrip("\n")
+    line = data.split(",")
+    matrix.append(line)
+f.close
+
+Num = [ "1限 |", "2限 |", "3限 |", "4限 |", "5限 |", "6限 |" ]
+Mon = [ "10", "11", "12", "13", "14", "15" ]
+Tue = [ "20", "21", "22", "23", "24", "25" ]
+Wed = [ "30", "31", "32", "33", "34", "35" ]
+Thu = [ "40", "41", "42", "43", "44", "45" ]
+Fri = [ "50", "51", "52", "53", "54", "55" ]
+sch = [ Num, Mon, Tue, Wed, Thu, Fri ]
+
+row = len(sch)
+col = len(sch[0])
+
+print("時限\t月\t火\t水\t木\t金")
+print("-------------------------------------------------")
+for j in range(row):
+    for i in range(col):
+        if int(len(matrix[i][j])) >= 3:
+            sch[i][j] = "\033[34m" + sch[i][j] + "\033[0m"
+        print(sch[i][j], end="\t")
+    print("")
+print("編集⇨ a\t編集終了⇨ w\tマスを入力⇨ ブラウザを起動")
 
-def main():
-    if not os.path.exists("url.csv"):
-        f = open("url.csv", "w", newline="")
-        data1 = [["", "", "", "", "", ""],
-                 ["", "", "", "", "", ""],
-                 ["", "", "", "", "", ""],
-                 ["", "", "", "", "", ""],
-                 ["", "", "", "", "", ""],
-                 ["", "", "", "", "", ""]]
-        writer = csv.writer(f)
-        writer.writerows(data1)
-        f.close()
-        print("url.csvを作成したので起動し直してください")
-        quit()
+a = input()
+if a == "a":
 
-    matrix = []
-    f = open("url.csv", "r")
+    import csv
+    f = open("url.csv", "w", newline="")
     while True:
-        data = f.readline()
-        if data == "":
+        print("マスを選択 or w")
+        a = input()
+        if a == "w":
+            writer = csv.writer(f)
+            writer.writerows(matrix)
+            f.close
             break
-        data = data.rstrip("\n")
-        line = data.split(",")
-        matrix.append(line)
-    f.close()
-
-    Num = ["1限 |", "2限 |", "3限 |", "4限 |", "5限 |", "6限 |"]
-    Mon = ["10", "11", "12", "13", "14", "15"]
-    Tue = ["20", "21", "22", "23", "24", "25"]
-    Wed = ["30", "31", "32", "33", "34", "35"]
-    Thu = ["40", "41", "42", "43", "44", "45"]
-    Fri = ["50", "51", "52", "53", "54", "55"]
-    sch = [Num, Mon, Tue, Wed, Thu, Fri]
-
-    row = len(sch)
-    col = len(sch[0])
-
-    print("時限\t月\t火\t水\t木\t金")
-    print("-------------------------------------------------")
-    for j in range(row):
-        for i in range(col):
-            if int(len(matrix[i][j])) >= 3:
-                sch[i][j] = "\033[34m" + sch[i][j] + "\033[0m"
-            print(sch[i][j], end="\t")
-        print("")
-    print("編集⇨ a\t編集終了⇨ w\tマスを入力⇨ ブラウザを起動")
-
-    a = input()
-    if a == "a":
-        f = open("url.csv", "w", newline="")
-        while True:
-            print("マスを選択 or w")
-            a = input()
-            if a == "w":
-                writer = csv.writer(f)
-                writer.writerows(matrix)
-                f.close()
-                break
-                quit()
+            quit()
+        else:
+            b = a[0]
+            c = a[1]
+            print("URLを貼り付けor エンターキーで削除 ")
+            d = input()
+            matrix[int(b)][int(c)] = d
+            if int(len(d)) == int(0):
+                sch[int(b)][int(c)] = "\033[0m" + sch[int(b)][int(c)] + "\033[0m"
             else:
-                b = a[0]
-                c = a[1]
-                print("URLを貼り付けor エンターキーで削除 ")
-                d = input()
-                matrix[int(b)][int(c)] = d
-                if int(len(d)) == int(0):
-                    sch[int(b)][int(c)] = "\033[0m" + sch[int(b)][int(c)] + "\033[0m"
-                else:
-                    sch[int(b)][int(c)] = "\033[34m" + sch[int(b)][int(c)] + "\033[0m"
-                print("時限\t月\t火\t水\t木\t金")
-                print("-------------------------------------------------")
-                for j in range(row):
-                    for i in range(col):
-                        print(sch[i][j], end="\t")
-                    print("")
-    else:
-        b = a[0]
-        c = a[1]
-        webbrowser.open(matrix[int(b)][int(c)], 2)
-
-if __name__ == "__main__":
-    main()
-
-
+                sch[int(b)][int(c)] = "\033[34m" + sch[int(b)][int(c)] + "\033[0m"
+            print("時限\t月\t火\t水\t木\t金")
+            print("-------------------------------------------------")
+            for j in range(row):
+                for i in range(col):
+                    print(sch[i][j], end="\t")
+                print("")
+else:
+    b = a[0]
+    c = a[1]
+    
+    import webbrowser
+    webbrowser.open( matrix[int(b)][int(c)] , 2 )
```

### Comparing `online_scheduler-0.4/setup.py` & `online_scheduler-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='0.4',
+    version='0.5',
     description='Awesome library',
     url='https://github.com/2222041',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
```


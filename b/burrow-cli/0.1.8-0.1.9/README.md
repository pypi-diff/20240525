# Comparing `tmp/burrow_cli-0.1.8.tar.gz` & `tmp/burrow_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burrow_cli-0.1.8.tar", max compression
+gzip compressed data, was "burrow_cli-0.1.9.tar", max compression
```

## Comparing `burrow_cli-0.1.8.tar` & `burrow_cli-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1548 2024-05-25 08:31:19.597935 burrow_cli-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.8/burrow_cli/__init__.py
--rw-r--r--   0        0        0     7415 2024-05-24 14:47:03.700623 burrow_cli-0.1.8/burrow_cli/main.py
--rw-r--r--   0        0        0      602 2024-05-25 08:30:59.947178 burrow_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 burrow_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1616 2024-05-25 08:37:46.396589 burrow_cli-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.9/burrow_cli/__init__.py
+-rw-r--r--   0        0        0     7415 2024-05-24 14:47:03.700623 burrow_cli-0.1.9/burrow_cli/main.py
+-rw-r--r--   0        0        0      602 2024-05-25 08:41:55.487665 burrow_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 burrow_cli-0.1.9/PKG-INFO
```

### Comparing `burrow_cli-0.1.8/README.md` & `burrow_cli-0.1.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# Share part of your GPU with your friends!
+# Share part of your GPU with your friends using Burrow!
 
 * With Burrow, you can share part of your GPU with your friends with a single link! 🚀🔗
 * Work collaboratively in the same terminal, especially thanks to sshx.io 👨‍💻👩‍💻
 * With security in mind, Burrow uses sandbox Docker containers, so your friends can't access your local files. 🛡️🐳🔒
 
 # Install
 
 ## Prerequises
-
-* Burrow requires Docker to run. It will install Docker on your local machine if it's not already installed. The automated Docker installation only works on Ubuntu for now; if you are using other Linux distributions, you will need to install Docker yourself first.
+You need the following software installed in order to run Burrow, if you already have them installed you can skip this section.
+* Burrow requires __Docker__ to run
+* Burrow requires __Python3__ to run
 
 ## Install with a script
 
-Run the installation script (Only tested on Ubuntu22.04 for now, more coming)
+Run the installation script
 ```
-curl -sSL https://raw.githubusercontent.com/incomingflyingbrick/burrow-cli/main/install_burrow.sh | sudo sh
+curl -sSL https://raw.githubusercontent.com/incomingflyingbrick/burrow-cli/main/install_burrow.sh | sudo bash
 ```
 
 # Quick Start
-Launch a sharable GPU container with 3GB GRAM
 
+Launch a sharable GPU container with 3GB GRA
 ```bash
 burrow start 3gi
 ```
 
 List all running burrow container
 ```bash
 burrow list
@@ -45,15 +46,15 @@
 ## Ubuntu
 * Ubuntu Noble 24.04 (LTS)
 * Ubuntu Mantic 23.10 (EOL: July 12, 2024)
 * Ubuntu Jammy 22.04 (LTS)
 * Ubuntu Focal 20.04 (LTS)
 
 ## CentOS
-* CentOS 7 (EOL: June 30, 2024)
-* CentOS 8 (stream) (EOL: May 31, 2024)
-* CentOS 9 (stream)
+* CentOS 7 (EOL: June 30, 2024) (Needs to install python3 and git first)
+* CentOS 8 (stream) (EOL: May 31, 2024) (Needs to install python3 and git first)
+* CentOS 9 (stream) (Needs to install git first)
 
 
 ## Debian
-* Debian Bookworm 12 (stable)
-* Debian Bullseye 11 (oldstable)
+* Debian Bookworm 12 (stable) (Needs to install git first)
+* Debian Bullseye 11 (oldstable) (Needs to install git first)
```

### Comparing `burrow_cli-0.1.8/burrow_cli/main.py` & `burrow_cli-0.1.9/burrow_cli/main.py`

 * *Files identical despite different names*

### Comparing `burrow_cli-0.1.8/pyproject.toml` & `burrow_cli-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burrow-cli"
-version = "0.1.8"
+version = "0.1.9"
 description = "Burrow command line app, you can launch a fractional GPU contaienr with this app, and share a link of the container to your friends, you and your friends can work colloratively together"
 authors = ["Vurtne Saerdna <vurtnesaerdna@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 burrow = "burrow_cli.main:app"
```

### Comparing `burrow_cli-0.1.8/PKG-INFO` & `burrow_cli-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: burrow-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Burrow command line app, you can launch a fractional GPU contaienr with this app, and share a link of the container to your friends, you and your friends can work colloratively together
 Author: Vurtne Saerdna
 Author-email: vurtnesaerdna@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
-# Share part of your GPU with your friends!
+# Share part of your GPU with your friends using Burrow!
 
 * With Burrow, you can share part of your GPU with your friends with a single link! 🚀🔗
 * Work collaboratively in the same terminal, especially thanks to sshx.io 👨‍💻👩‍💻
 * With security in mind, Burrow uses sandbox Docker containers, so your friends can't access your local files. 🛡️🐳🔒
 
 # Install
 
 ## Prerequises
-
-* Burrow requires Docker to run. It will install Docker on your local machine if it's not already installed. The automated Docker installation only works on Ubuntu for now; if you are using other Linux distributions, you will need to install Docker yourself first.
+You need the following software installed in order to run Burrow, if you already have them installed you can skip this section.
+* Burrow requires __Docker__ to run
+* Burrow requires __Python3__ to run
 
 ## Install with a script
 
-Run the installation script (Only tested on Ubuntu22.04 for now, more coming)
+Run the installation script
 ```
-curl -sSL https://raw.githubusercontent.com/incomingflyingbrick/burrow-cli/main/install_burrow.sh | sudo sh
+curl -sSL https://raw.githubusercontent.com/incomingflyingbrick/burrow-cli/main/install_burrow.sh | sudo bash
 ```
 
 # Quick Start
-Launch a sharable GPU container with 3GB GRAM
 
+Launch a sharable GPU container with 3GB GRA
 ```bash
 burrow start 3gi
 ```
 
 List all running burrow container
 ```bash
 burrow list
@@ -62,15 +63,15 @@
 ## Ubuntu
 * Ubuntu Noble 24.04 (LTS)
 * Ubuntu Mantic 23.10 (EOL: July 12, 2024)
 * Ubuntu Jammy 22.04 (LTS)
 * Ubuntu Focal 20.04 (LTS)
 
 ## CentOS
-* CentOS 7 (EOL: June 30, 2024)
-* CentOS 8 (stream) (EOL: May 31, 2024)
-* CentOS 9 (stream)
+* CentOS 7 (EOL: June 30, 2024) (Needs to install python3 and git first)
+* CentOS 8 (stream) (EOL: May 31, 2024) (Needs to install python3 and git first)
+* CentOS 9 (stream) (Needs to install git first)
 
 
 ## Debian
-* Debian Bookworm 12 (stable)
-* Debian Bullseye 11 (oldstable)
+* Debian Bookworm 12 (stable) (Needs to install git first)
+* Debian Bullseye 11 (oldstable) (Needs to install git first)
```


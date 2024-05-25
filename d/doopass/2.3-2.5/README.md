# Comparing `tmp/doopass-2.3.tar.gz` & `tmp/doopass-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doopass-2.3.tar", last modified: Wed Feb 15 12:48:51 2023, max compression
+gzip compressed data, was "doopass-2.5.tar", last modified: Sat May 25 10:55:17 2024, max compression
```

## Comparing `doopass-2.3.tar` & `doopass-2.5.tar`

### file list

```diff
@@ -1,57 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:51.005375 doopass-2.3/
--rw-rw-rw-   0        0        0      134 2023-02-13 14:17:50.000000 doopass-2.3/.gitignore
--rw-rw-rw-   0        0        0    35150 2023-02-11 18:07:16.000000 doopass-2.3/LICENSE
--rw-rw-rw-   0        0        0     4406 2023-02-15 12:48:51.004354 doopass-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3817 2023-02-15 09:53:39.000000 doopass-2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:50.948472 doopass-2.3/assets/
--rw-rw-rw-   0        0        0    15600 2023-02-13 15:43:11.000000 doopass-2.3/assets/preview.png
--rw-rw-rw-   0        0        0     6691 2023-02-15 12:44:57.000000 doopass-2.3/assets/styles.css
--rw-rw-rw-   0        0        0      641 2023-02-15 08:53:26.000000 doopass-2.3/dependencies.txt
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:50.951471 doopass-2.3/doopass/
--rw-rw-rw-   0        0        0        0 2023-02-14 17:16:42.000000 doopass-2.3/doopass/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-02-15 10:03:22.000000 doopass-2.3/doopass/doopass.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:50.961473 doopass-2.3/doopass/src/
--rw-rw-rw-   0        0        0        0 2023-02-11 18:07:16.000000 doopass-2.3/doopass/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:50.972474 doopass-2.3/doopass/src/core/
--rw-rw-rw-   0        0        0        0 2023-02-11 18:07:16.000000 doopass-2.3/doopass/src/core/__init__.py
--rw-rw-rw-   0        0        0      976 2023-02-15 10:09:33.000000 doopass-2.3/doopass/src/core/app.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:50.984338 doopass-2.3/doopass/src/core/components/
--rw-rw-rw-   0        0        0     2482 2023-02-14 20:32:53.000000 doopass-2.3/doopass/src/core/components/backup_manage_menu.py
--rw-rw-rw-   0        0        0      890 2023-02-14 20:48:31.000000 doopass-2.3/doopass/src/core/components/login_page.py
--rw-rw-rw-   0        0        0     2394 2023-02-15 11:31:56.000000 doopass-2.3/doopass/src/core/components/login_page_container.py
--rw-rw-rw-   0        0        0      708 2023-02-14 20:41:49.000000 doopass-2.3/doopass/src/core/components/message.py
--rw-rw-rw-   0        0        0     1966 2023-02-13 10:45:15.000000 doopass-2.3/doopass/src/core/components/select_menu.py
--rw-rw-rw-   0        0        0      820 2023-02-11 18:07:16.000000 doopass-2.3/doopass/src/core/components/signup_page.py
--rw-rw-rw-   0        0        0     2403 2023-02-15 12:45:38.000000 doopass-2.3/doopass/src/core/components/store_handle_menu.py
--rw-rw-rw-   0        0        0     1127 2023-02-15 12:45:40.000000 doopass-2.3/doopass/src/core/components/store_handle_menu_item.py
--rw-rw-rw-   0        0        0     2303 2023-02-12 20:19:33.000000 doopass-2.3/doopass/src/core/components/store_pair_handle_page.py
--rw-rw-rw-   0        0        0      763 2023-02-15 08:41:17.000000 doopass-2.3/doopass/src/core/constants.py
--rw-rw-rw-   0        0        0      302 2023-02-11 18:07:16.000000 doopass-2.3/doopass/src/core/exceptions.py
--rw-rw-rw-   0        0        0     1275 2023-02-11 18:07:16.000000 doopass-2.3/doopass/src/core/password_validation.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:51.000485 doopass-2.3/doopass/src/core/screens/
--rw-rw-rw-   0        0        0        0 2023-02-11 18:07:16.000000 doopass-2.3/doopass/src/core/screens/__init__.py
--rw-rw-rw-   0        0        0     2172 2023-02-13 15:47:20.000000 doopass-2.3/doopass/src/core/screens/backup_manage_screen.py
--rw-rw-rw-   0        0        0     5652 2023-02-14 19:52:16.000000 doopass-2.3/doopass/src/core/screens/help_screen.py
--rw-rw-rw-   0        0        0      609 2023-02-14 20:48:29.000000 doopass-2.3/doopass/src/core/screens/login_screen.py
--rw-rw-rw-   0        0        0     1643 2023-02-15 11:32:16.000000 doopass-2.3/doopass/src/core/screens/main_menu_screen.py
--rw-rw-rw-   0        0        0     3004 2023-02-15 12:25:09.000000 doopass-2.3/doopass/src/core/screens/main_screen.py
--rw-rw-rw-   0        0        0      859 2023-02-14 20:45:32.000000 doopass-2.3/doopass/src/core/screens/message_screen.py
--rw-rw-rw-   0        0        0      872 2023-02-14 20:20:51.000000 doopass-2.3/doopass/src/core/screens/screen.py
--rw-rw-rw-   0        0        0     1534 2023-02-15 10:14:28.000000 doopass-2.3/doopass/src/core/screens/sign_up_screen.py
--rw-rw-rw-   0        0        0     5975 2023-02-15 12:46:11.000000 doopass-2.3/doopass/src/core/screens/store_handle_screen.py
--rw-rw-rw-   0        0        0     1795 2023-02-14 21:54:57.000000 doopass-2.3/doopass/src/core/screens/store_pair_handle_screen.py
--rw-rw-rw-   0        0        0     8532 2023-02-15 10:01:13.000000 doopass-2.3/doopass/src/core/store.py
--rw-rw-rw-   0        0        0     3833 2023-02-15 10:09:06.000000 doopass-2.3/doopass/src/core/store_backup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:51.002477 doopass-2.3/doopass/src/tests/
--rw-rw-rw-   0        0        0        0 2023-02-11 18:07:16.000000 doopass-2.3/doopass/src/tests/__init__.py
--rw-rw-rw-   0        0        0     3369 2023-02-13 07:06:04.000000 doopass-2.3/doopass/src/tests/store_test.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:48:50.960474 doopass-2.3/doopass.egg-info/
--rw-rw-rw-   0        0        0     4406 2023-02-15 12:48:50.000000 doopass-2.3/doopass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1538 2023-02-15 12:48:50.000000 doopass-2.3/doopass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 12:48:50.000000 doopass-2.3/doopass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-02-15 12:48:50.000000 doopass-2.3/doopass.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      608 2023-02-15 12:48:50.000000 doopass-2.3/doopass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-02-15 12:48:50.000000 doopass-2.3/doopass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      551 2023-02-11 18:07:16.000000 doopass-2.3/installing.txt
--rw-rw-rw-   0        0        0     1719 2023-02-15 08:54:29.000000 doopass-2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-15 12:48:51.005375 doopass-2.3/setup.cfg
+drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-25 10:55:17.847251 doopass-2.5/
+-rw-r--r--   0 doopath   (1000) doopath   (1000)      134 2023-02-27 08:33:02.000000 doopass-2.5/.gitignore
+-rw-r--r--   0 doopath   (1000) doopath   (1000)    35150 2023-02-27 08:33:02.000000 doopass-2.5/LICENSE
+-rw-r--r--   0 doopath   (1000) doopath   (1000)     5467 2024-05-25 10:55:17.846251 doopass-2.5/PKG-INFO
+-rw-r--r--   0 doopath   (1000) doopath   (1000)     3817 2023-02-27 08:33:02.000000 doopass-2.5/README.md
+drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-25 10:55:17.843251 doopass-2.5/assets/
+-rw-r--r--   0 doopath   (1000) doopath   (1000)    15600 2023-02-27 08:33:02.000000 doopass-2.5/assets/preview.png
+-rw-r--r--   0 doopath   (1000) doopath   (1000)     6691 2023-02-27 08:33:02.000000 doopass-2.5/assets/styles.css
+-rw-r--r--   0 doopath   (1000) doopath   (1000)      362 2024-05-25 10:44:01.000000 doopass-2.5/dependencies.txt
+-rw-r--r--   0 doopath   (1000) doopath   (1000)      330 2024-02-01 20:39:36.000000 doopass-2.5/deversion.py
+drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-25 10:55:17.844251 doopass-2.5/doopass/
+-rw-r--r--   0 doopath   (1000) doopath   (1000)        0 2023-02-27 08:33:02.000000 doopass-2.5/doopass/__init__.py
+-rw-r--r--   0 doopath   (1000) doopath   (1000)     1012 2024-05-25 10:52:29.000000 doopass-2.5/doopass/app.py
+-rw-r--r--   0 doopath   (1000) doopath   (1000)     1380 2024-05-25 10:52:29.000000 doopass-2.5/doopass/doopass.py
+drwxr-xr-x   0 doopath   (1000) doopath   (1000)        0 2024-05-25 10:55:17.845251 doopass-2.5/doopass.egg-info/
+-rw-r--r--   0 doopath   (1000) doopath   (1000)     5467 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/PKG-INFO
+-rw-r--r--   0 doopath   (1000) doopath   (1000)      367 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/SOURCES.txt
+-rw-r--r--   0 doopath   (1000) doopath   (1000)        1 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/dependency_links.txt
+-rw-r--r--   0 doopath   (1000) doopath   (1000)       49 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/entry_points.txt
+-rw-r--r--   0 doopath   (1000) doopath   (1000)      628 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/requires.txt
+-rw-r--r--   0 doopath   (1000) doopath   (1000)       15 2024-05-25 10:55:17.000000 doopass-2.5/doopass.egg-info/top_level.txt
+-rw-r--r--   0 doopath   (1000) doopath   (1000)      551 2023-02-27 08:33:02.000000 doopass-2.5/installing.txt
+-rw-r--r--   0 doopath   (1000) doopath   (1000)     1731 2024-05-25 10:55:02.000000 doopass-2.5/pyproject.toml
+-rw-r--r--   0 doopath   (1000) doopath   (1000)       38 2024-05-25 10:55:17.847251 doopass-2.5/setup.cfg
```

### Comparing `doopass-2.3/LICENSE` & `doopass-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `doopass-2.3/PKG-INFO` & `doopass-2.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,94 @@
-Metadata-Version: 2.1
-Name: doopass
-Version: 2.3
-Summary: Crossplatform TUI password manager written in python
-Author-email: Michael Nikishov <doopath@gmail.com>
-Project-URL: Homepage, https://github.com/doopath/PasswordManager
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PasswordManager
-
-## Preview
-
-![no image](https://raw.githubusercontent.com/doopath/PasswordManager/master/assets/preview.png)
-
-## Navigation
-
-<ul>
-  <li><a href="#preview">Preview</a></li>
-  <li><a href="#navigation">Navigation</a></li>
-  <li><a href="#description">Description</a></li>
-  <li><a href="#installation">Installation</a></li>
-  <li><a href="#navigation">Usage</a></li>
-  <li><a href="#about">About</a></li>
-</ul>
-
-## Description
-
-**Doopass** is a TUI password manager based on [_textual_](https://github.com/textualize/textual/) framework. It is run on **Windows**, **Linux** and **MacOS** (wherever python works). The old version (CLI) is actually on the [_cli_](https://github.com/doopath/PasswordManager/tree/cli) branch.
-
-## Installation
-
-_Python v3.11+_ should be installed on your system and available in the PATH as _python_.
-For better experience you could install one of [_NerdFonts_](https://www.nerdfonts.com/font-downloads) (_JetBrainsMono NF_ for example) and set this font for the terminal emulator where you run **Doopass**.
-Also it's highly recommended to use _PowerShell v7.0+_ and _Windows Terminal_ on **Windows**.
-
-**All platforms:**
-
-```bash
-pip install doopass==2.3
-```
-
-**Unix (specified):**
-
-```bash
-wget https://github.com/doopath/PasswordManager/releases/download/v2.3/Doopass-2.3-py3-none-any.whl
-pip install Doopass-2.3-py3-none-any.whl
-rm Doopass-2.3-py3-none-any.whl
-```
-
-**Windows (PowerShell) (specified):**
-
-```powershell
-Invoke-WebRequest https://github.com/doopath/PasswordManager/releases/download/v2.3/Doopass-2.3-py3-none-any.whl -OutFile Doopass-2.3-py3-none-any.whl
-pip install Doopass-2.3-py3-none-any.whl
-rm Doopass-2.3-py3-none-any.whl
-```
-
-**Build from source (Windows, Unix)**
-
-```bash
-git clone https://github.com/doopath/PasswordManager.git
-cd PasswordManager
-git checkout master
-python -m venv venv
-
-# For Unix (bash, zsh)
-source venv/bin/activate
-
-# For Windows (PowerShell)
-./venv/Scripts/Activate.ps1
-
-pip install -r dependencies.py
-python -m build
-deactivate
-pip install dist/Doopass-2.3-py3-none-any.whl
-```
-
-After building and installing you can delete the _PasswordManager_ dir.
-
-## Usage
-
-After installation of the **Doopass** you can run it by typing _doopass_ in the terminal. First of all after starting the **Doopass** at the first time you should create a store: press the _Init store_ button in the main menu and enter a password for the store. Every time you run **Doopass** you should _Log In_ to decrypt your store (because all your data is stored on your disk and encrypted). After that you will be able to manage the store (add, delete, update and copy key-value pairs). For better experience type `H` in the main menu to see the _help list_.
-
-More available actions:
-
-```
-Q or ESCAPE - quit the app
-SPACE - leave help screen
-H - open help screen
-DownArrow or TAB or J - focus next element
-UpArrow or Shift+TAB or K - focus previous element
-```
-
-Register of the key pressed doesn't matter, but be sure you are using english keyboard layout.
-
-## About
-
-Store format of the current version of **Doopass** is fully compatible with the older one ([_cli_](https://github.com/doopath/PasswordManager/tree/cli)). That means you can move the store.enc file from your cli version of the **Doopass** to the _~/doopass/appdata_ dir and you will able to use it.
-
-**Doopass** uses the _cryptography_ and _base64_ python libs for encrypting your data. It's safe to share your store.enc or backup of the store. You can upload your store.enc somewhere if it's necessary. If you have any ideas about making Doopass more safe please contact me or make a pull request.
-
-If you want to contribute you can make a pull request or create an issue. If you want to contact me you can write me on [Telegram](https://t.me/doopath) or Gmail: *doopath@gmail.com*.
+# PasswordManager
+
+## Preview
+
+![no image](https://raw.githubusercontent.com/doopath/PasswordManager/master/assets/preview.png)
+
+## Navigation
+
+<ul>
+  <li><a href="#preview">Preview</a></li>
+  <li><a href="#navigation">Navigation</a></li>
+  <li><a href="#description">Description</a></li>
+  <li><a href="#installation">Installation</a></li>
+  <li><a href="#navigation">Usage</a></li>
+  <li><a href="#about">About</a></li>
+</ul>
+
+## Description
+
+**Doopass** is a TUI password manager based on [_textual_](https://github.com/textualize/textual/) framework. It is run on **Windows**, **Linux** and **MacOS** (wherever python works). The old version (CLI) is actually on the [_cli_](https://github.com/doopath/PasswordManager/tree/cli) branch.
+
+## Installation
+
+_Python v3.11+_ should be installed on your system and available in the PATH as _python_.
+For better experience you could install one of [_NerdFonts_](https://www.nerdfonts.com/font-downloads) (_JetBrainsMono NF_ for example) and set this font for the terminal emulator where you run **Doopass**.
+Also it's highly recommended to use _PowerShell v7.0+_ and _Windows Terminal_ on **Windows**.
+
+**All platforms:**
+
+```bash
+pip install doopass==2.3
+```
+
+**Unix (specified):**
+
+```bash
+wget https://github.com/doopath/PasswordManager/releases/download/v2.3/Doopass-2.3-py3-none-any.whl
+pip install Doopass-2.3-py3-none-any.whl
+rm Doopass-2.3-py3-none-any.whl
+```
+
+**Windows (PowerShell) (specified):**
+
+```powershell
+Invoke-WebRequest https://github.com/doopath/PasswordManager/releases/download/v2.3/Doopass-2.3-py3-none-any.whl -OutFile Doopass-2.3-py3-none-any.whl
+pip install Doopass-2.3-py3-none-any.whl
+rm Doopass-2.3-py3-none-any.whl
+```
+
+**Build from source (Windows, Unix)**
+
+```bash
+git clone https://github.com/doopath/PasswordManager.git
+cd PasswordManager
+git checkout master
+python -m venv venv
+
+# For Unix (bash, zsh)
+source venv/bin/activate
+
+# For Windows (PowerShell)
+./venv/Scripts/Activate.ps1
+
+pip install -r dependencies.py
+python -m build
+deactivate
+pip install dist/Doopass-2.3-py3-none-any.whl
+```
+
+After building and installing you can delete the _PasswordManager_ dir.
+
+## Usage
+
+After installation of the **Doopass** you can run it by typing _doopass_ in the terminal. First of all after starting the **Doopass** at the first time you should create a store: press the _Init store_ button in the main menu and enter a password for the store. Every time you run **Doopass** you should _Log In_ to decrypt your store (because all your data is stored on your disk and encrypted). After that you will be able to manage the store (add, delete, update and copy key-value pairs). For better experience type `H` in the main menu to see the _help list_.
+
+More available actions:
+
+```
+Q or ESCAPE - quit the app
+SPACE - leave help screen
+H - open help screen
+DownArrow or TAB or J - focus next element
+UpArrow or Shift+TAB or K - focus previous element
+```
+
+Register of the key pressed doesn't matter, but be sure you are using english keyboard layout.
+
+## About
+
+Store format of the current version of **Doopass** is fully compatible with the older one ([_cli_](https://github.com/doopath/PasswordManager/tree/cli)). That means you can move the store.enc file from your cli version of the **Doopass** to the _~/doopass/appdata_ dir and you will able to use it.
+
+**Doopass** uses the _cryptography_ and _base64_ python libs for encrypting your data. It's safe to share your store.enc or backup of the store. You can upload your store.enc somewhere if it's necessary. If you have any ideas about making Doopass more safe please contact me or make a pull request.
+
+If you want to contribute you can make a pull request or create an issue. If you want to contact me you can write me on [Telegram](https://t.me/doopath) or Gmail: *doopath@gmail.com*.
```

#### html2text {}

```diff
@@ -1,16 +1,9 @@
-Metadata-Version: 2.1 Name: doopass Version: 2.3 Summary: Crossplatform TUI
-password manager written in python Author-email: Michael Nikishov
-gmail.com> Project-URL: Homepage, https://github.com/doopath/PasswordManager
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: GNU General Public License (GPL) Classifier: Operating System :: OS
-Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
-License-File: LICENSE # PasswordManager ## Preview ![no image](https://
-raw.githubusercontent.com/doopath/PasswordManager/master/assets/preview.png) ##
-Navigation
+# PasswordManager ## Preview ![no image](https://raw.githubusercontent.com/
+doopath/PasswordManager/master/assets/preview.png) ## Navigation
     * _P_r_e_v_i_e_w
     * _N_a_v_i_g_a_t_i_o_n
     * _D_e_s_c_r_i_p_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _A_b_o_u_t
 ## Description **Doopass** is a TUI password manager based on [_textual_]
```

### Comparing `doopass-2.3/assets/preview.png` & `doopass-2.5/assets/preview.png`

 * *Files identical despite different names*

### Comparing `doopass-2.3/assets/styles.css` & `doopass-2.5/assets/styles.css`

 * *Files identical despite different names*

### Comparing `doopass-2.3/doopass/doopass.py` & `doopass-2.5/doopass/doopass.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """ A python module that helps you to manage your secret data. """
 import logging
 import sys
+from typing import override
 
-from textual.cli import cli
+from doopass_libs.core.screens.main_screen import MainScreen
+from rich.console import RenderableType
+from textual.app import ReturnType
+from textual.screen import Screen as textaulScreen
 
-from doopass.src.core.app import App
-from doopass.src.core.screens.main_screen import MainScreen
-from doopass.src.core.screens.screen import Screen
+from doopass.app import App
 
 
 class Doopass(App):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
     def on_mount(self) -> None:
         main_screen = MainScreen(self)
         self.install_screen(main_screen, name="MainScreen")
         self.push_screen(main_screen)
         self.screen.styles.background = "black"
         logging.debug("The app has been launched")
 
+    @override
     def apply_screen(
-        self, screen: Screen, pop: bool = True, name: str | None = None
+            self, screen: textaulScreen, pop: bool = True, name: str | None = None
     ) -> None:
         screen.styles.background = "black"
 
         if name:
             self.app.install_screen(screen, name=name)
         else:
             self.app.install_screen(screen)
 
         if pop:
             self.app.pop_screen()
 
         self.app.push_screen(screen)
 
-    def exit(self, result=None, message=None) -> None:
+    def exit(self, result: ReturnType | None = None, return_code: int = 0, message: RenderableType | None = None,
+             **kwargs) -> None:
         logging.debug("App exited\n")
-        super().exit(result, message)
+        super().exit(result, return_code, message)
 
 
 def main() -> int:
-    cli.run(["run", "doopass.doopass:Doopass"])
-
+    app = Doopass()
+    app.run()
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `doopass-2.3/doopass/src/core/app.py` & `doopass-2.5/doopass/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 import os
 
+from doopass_libs.core import constants
+from doopass_libs.core.store import Store
 from textual import app
 from textual.screen import Screen
 
-from . import constants
-from .store import Store
-
 
 class App(app.App):
     CSS_PATH = "../assets/styles.css"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.store: Store | None
@@ -28,10 +27,10 @@
     def _init_appdir(self) -> None:
         if not os.path.exists(constants.APP_DIR):
             logging.debug("Creating the app directory")
             os.mkdir(constants.APP_DIR)
             logging.debug("The app directory has been created")
 
     def apply_screen(
-        self, screen: Screen, pop: bool = True, name: str | None = None
+            self, screen: Screen, pop: bool = True, name: str | None = None
     ) -> None:
         ...
```

### Comparing `doopass-2.3/doopass.egg-info/requires.txt` & `doopass-2.5/doopass.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -29,7 +29,8 @@
 rich==13.3.1
 six==1.16.0
 textual==0.10.1
 twine==4.0.2
 urllib3==1.26.14
 webencodings==0.5.1
 zipp==3.13.0
+doopass-libs==1.0.7
```

### Comparing `doopass-2.3/installing.txt` & `doopass-2.5/installing.txt`

 * *Files identical despite different names*

### Comparing `doopass-2.3/pyproject.toml` & `doopass-2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools', 'setuptools-scm']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'doopass'
-version = '2.3'
+version = '2.5'
 authors = [
   { name='Michael Nikishov', email='doopath@gmail.com' },
 ]
 description = 'Crossplatform TUI password manager written in python'
 readme = 'README.md'
 requires-python = '>=3.11'
 classifiers = [
@@ -49,19 +49,20 @@
     'rich==13.3.1',
     'six==1.16.0',
     'textual==0.10.1',
     'twine==4.0.2',
     'urllib3==1.26.14',
     'webencodings==0.5.1',
     'zipp==3.13.0',
+    'doopass-libs==1.0.7'
 ]
 
 [tool.setuptools.packages.find]
 where = ['.']
-include = ['doopass', 'doopass.src', 'assets']
+include = ['doopass', 'assets']
 
 [tool.setuptools.package-data]
 '*' = ['*.css', '*.png']
 
 [project.scripts]
 doopass = 'doopass.doopass:main'
```


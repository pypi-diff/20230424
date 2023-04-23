# Comparing `tmp/tkterm-0.0.0b1.tar.gz` & `tmp/tkterm-0.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Dhanoo\Documents\git\Ant-Shell\TkTerm\dist\tmp1xn_figb\tkterm-0.0.0b1.tar", last modified: Sun Apr 23 12:55:22 2023, max compression
+gzip compressed data, was "tkterm-0.0.0b2.tar", last modified: Sun Apr 23 23:18:13 2023, max compression
```

## Comparing `tkterm-0.0.0b1.tar` & `tkterm-0.0.0b2.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/
--rw-rw-rw-   0        0        0     1074 2023-04-23 12:24:00.000000 tkterm-0.0.0b1/LICENSE
--rw-rw-rw-   0        0        0       20 2023-04-23 12:28:21.000000 tkterm-0.0.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0     3806 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     2659 2023-04-23 12:40:10.000000 tkterm-0.0.0b1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0     1704 2023-04-23 12:54:12.000000 tkterm-0.0.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm/
-drwxrwxrwx   0        0        0        0 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm/backend/
--rw-rw-rw-   0        0        0      400 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/backend/InterpreterInterface.py
--rw-rw-rw-   0        0        0     1997 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/backend/InterpreterShell.py
--rw-rw-rw-   0        0        0     1446 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/backend/KThread.py
--rw-rw-rw-   0        0        0        0 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/backend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm/img/
--rw-rw-rw-   0        0        0     2456 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/app_icon.png
--rw-rw-rw-   0        0        0      264 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/case.png
--rw-rw-rw-   0        0        0      262 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/close.png
--rw-rw-rw-   0        0        0     1418 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/close_tab.png
--rw-rw-rw-   0        0        0    15607 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/hamburger.png
--rw-rw-rw-   0        0        0      581 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/linux.png
--rw-rw-rw-   0        0        0     1413 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/new_tab.png
--rw-rw-rw-   0        0        0      217 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/next.png
--rw-rw-rw-   0        0        0     1458 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/next_tab.png
--rw-rw-rw-   0        0        0    15403 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/plus.png
--rw-rw-rw-   0        0        0      219 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/prev.png
--rw-rw-rw-   0        0        0     1442 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/prev_tab.png
--rw-rw-rw-   0        0        0      215 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/regex.png
--rw-rw-rw-   0        0        0    23482 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/screenshot.jpg
--rw-rw-rw-   0        0        0      543 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/search.png
--rw-rw-rw-   0        0        0    27373 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/settings.png
--rw-rw-rw-   0        0        0    33172 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/snapshot1.png
--rw-rw-rw-   0        0        0    32868 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/snapshot2.png
--rw-rw-rw-   0        0        0     2518 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/warn.png
--rw-rw-rw-   0        0        0      807 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/img/windows.png
-drwxrwxrwx   0        0        0        0 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm/src/
--rw-rw-rw-   0        0        0     1506 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/src/Config.py
--rw-rw-rw-   0        0        0     3941 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/src/ExitDiaglogBox.py
--rw-rw-rw-   0        0        0     2346 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/src/Interpreter.py
--rw-rw-rw-   0        0        0     2850 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/src/Redirect.py
--rw-rw-rw-   0        0        0    14970 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/src/RightClickContextMenu.py
--rw-rw-rw-   0        0        0     9484 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/src/SearchBar.py
--rw-rw-rw-   0        0        0    29329 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/src/TerminalScreen.py
--rw-rw-rw-   0        0        0    16422 2023-04-23 12:27:54.000000 tkterm-0.0.0b1/tkterm/src/TerminalTab.py
--rw-rw-rw-   0        0        0     1604 2023-04-23 12:27:54.000000 tkterm-0.0.0b1/tkterm/src/Tooltip.py
--rw-rw-rw-   0        0        0      332 2023-04-23 12:27:54.000000 tkterm-0.0.0b1/tkterm/src/Utils.py
--rw-rw-rw-   0        0        0      295 2023-04-23 12:27:54.000000 tkterm-0.0.0b1/tkterm/src/__init__.py
--rw-rw-rw-   0        0        0     3265 2023-04-23 12:27:54.000000 tkterm-0.0.0b1/tkterm/tkterm.py
--rw-rw-rw-   0        0        0       88 2023-04-23 12:27:53.000000 tkterm-0.0.0b1/tkterm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3806 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 12:55:22.000000 tkterm-0.0.0b1/tkterm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:18:13.828050 tkterm-0.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-04-23 23:18:13.828050 tkterm-0.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 23:18:13.828050 tkterm-0.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:18:13.824050 tkterm-0.0.0b2/tkterm/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:18:13.824050 tkterm-0.0.0b2/tkterm/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/backend/InterpreterInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/backend/InterpreterShell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/backend/KThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:18:13.824050 tkterm-0.0.0b2/tkterm/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/app_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/case.png
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/close_tab.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/hamburger.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/linux.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/new_tab.png
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/next_tab.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/prev.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/prev_tab.png
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/regex.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23482 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/screenshot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/search.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33172 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/snapshot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32868 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/snapshot2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/warn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/img/windows.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:18:13.828050 tkterm-0.0.0b2/tkterm/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/ExitDiaglogBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/Interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/Redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/RightClickContextMenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/SearchBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29607 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/TerminalScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/TerminalTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/Tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/tkterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-23 23:18:01.000000 tkterm-0.0.0b2/tkterm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:18:13.824050 tkterm-0.0.0b2/tkterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-04-23 23:18:13.000000 tkterm-0.0.0b2/tkterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-23 23:18:13.000000 tkterm-0.0.0b2/tkterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:18:13.000000 tkterm-0.0.0b2/tkterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 23:18:13.000000 tkterm-0.0.0b2/tkterm.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tkterm-0.0.0b1/LICENSE` & `tkterm-0.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/PKG-INFO` & `tkterm-0.0.0b2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,137 @@
-Metadata-Version: 2.1
-Name: tkterm
-Version: 0.0.0b1
-Summary: Terminal emulator built on Tkinter library.
-Home-page: https://github.com/dhanoosu/tkterm
-Author: Dhanoo Surasarang
-Author-email: dhanoo.surasarang@gmail.com
-License: MIT
-Project-URL: Documentation, https://github.com/dhanoosu/TkTerm/blob/master/README.md
-Project-URL: Bug Tracker, https://github.com/dhanoosu/tkterm/issues
-Keywords: linux,shell,bash,cli,gui,terminal,command-line,tkinter,subprocess,tkinter-graphic-interface,terminal-emulator,ttk,commandprompt,tkinter-gui,tkinter-python,tkinter-terminal,tk-terminal,tkinter-shell,tkterminal
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# TkTerm - Tkinter Terminal Emulator
-A fully functional terminal emulator built on Tkinter library - perform all basic commands of a terminal
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/snapshot2.png">
-</p>
-
-Under the hood it executes commands using Python's *subprocess* module and spawn as a thread. Pressing `Ctrl-C` will terminate current running command. Supports Unix shells (`sh` and `bash`) and Window's Command Prompt (`cmd.exe`) commands.
-
-## Features
-- Compatible with Windows and Unix systems
-- Tabbed Terminal - `click & drag` to reorder, `middle-click` to close tab, `double-click` to rename
-- Return Code (RC) of previous run commands is shown at the bottom status bar
-- Settings to customise colours, font and cursor shape
-- **Ctrl-C** to kill current running process
-- **Ctrl-F** to search; supports case sensitivity and regex searches
-- **UP** and **DOWN** arrow keys to cycle between next and previous commands in history
-- Unix-like **tab completion** on files and directories
-- Handles **multiline commands** using caret character `^` or `\`
-
-## Requirements
-The Tkinter GUI library is built into Python, so no 3rd party library is required.
-
-Requires at least Python version 3.x and above.
-
-## Standalone usage
-Run standalone script simply with
-
-```bash
-$> python tkterm/tkterm.py
-```
-
-## Integration with other Tkinter application
-The Terminal is implemented as a `Frame` widget and can be easily be integrated to other Tkinter application by
-
-```python
-import tkinter as tk
-from tkinter import *
-from tkterm import Terminal
-
-root = tk.Tk()
-
-terminal = Terminal(root)
-terminal.pack(fill=BOTH, expand=True)
-
-root.mainloop()
-```
-
-## Customisation options
-Customise Terminal interface by `Right-click > Settings...`
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/settings.png">
-</p>
-
-**Note**: \
-Clicking `Save config` saves setting configuration to a file.\
-Tkterm will automatically load this file the next time it starts up.
-
-## Multiline command
-Long lines of command can be broken up using a caret. A caret at the line end appends the next line command with the current command.
-In Windows the caret is `^`, and UNIX is `\`.
-
-For multiline command to be considered there must be ***no** trailing space after the caret*, for example:
-
-- `$> ping ^` is considered
-- `$> ping ^ ` is **not** considered
-
-```bash
-$>> echo I ^
-> have apple ^
-> and banana
-I have apple and banana
-```
-
-## Links
-
-- **GitHub:** https://github.com/dhanoosu/TkTerm
-
-## Author
-
-Developed by Dhanoo Surasarang
-
-Github: [@dhanoosu](https://github.com/dhanoosu)
-
+Metadata-Version: 2.1
+Name: tkterm
+Version: 0.0.0b2
+Summary: Terminal emulator built on Tkinter library.
+Home-page: https://github.com/dhanoosu/tkterm
+Author: Dhanoo Surasarang
+Author-email: dhanoo.surasarang@gmail.com
+License: MIT
+Project-URL: Documentation, https://github.com/dhanoosu/TkTerm/blob/master/README.md
+Project-URL: Bug Tracker, https://github.com/dhanoosu/TkTerm/issues
+Keywords: linux,shell,bash,cli,gui,terminal,command-line,tkinter,subprocess,tkinter-graphic-interface,terminal-emulator,ttk,commandprompt,tkinter-gui,tkinter-python,tkinter-terminal,tk-terminal,tkinter-shell,tkterminal
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/tkterm)](https://pypi.org/project/tkterm)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tkterm)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
+
+# TkTerm - Tkinter Terminal Emulator
+A fully functional terminal emulator built on Tkinter library - perform all basic commands of a terminal
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/snapshot2.png">
+</p>
+
+Under the hood it executes commands using Python's *subprocess* module and spawn as a thread. Pressing `Ctrl-C` will terminate current running command. Supports Unix shells (`sh` and `bash`) and Window's Command Prompt (`cmd.exe`) commands.
+
+## Features
+- Compatible with Windows and Unix systems
+- Tabbed Terminal - `click & drag` to reorder, `middle-click` to close tab, `double-click` to rename
+- Return Code (RC) of previous run commands is shown at the bottom status bar
+- Settings to customise colours, font and cursor shape
+- **Ctrl-C** to kill current running process
+- **Ctrl-F** to search; supports case sensitivity and regex searches
+- **UP** and **DOWN** arrow keys to cycle between next and previous commands in history
+- Unix-like **tab completion** on files and directories
+- Handles **multiline commands** using caret character `^` or `\`
+
+## Requirements
+The Tkinter GUI library is built into Python, so no 3rd party library is required.
+
+Requires at least Python version 3.x and above.
+
+## Installation
+Get it from Github or PIP package manager
+
+```bash
+# From github
+git clone https://github.com/dhanoosu/TkTerm.git
+
+# From package manager
+pip install tkterm
+```
+
+## Standalone usage
+Navigate to downloaded folder and run script with
+
+```bash
+cd TkTerm
+
+# Either of these will work
+python tkterm
+python tkterm/tkterm.py
+```
+
+If package was installed via pip
+
+```bash
+python -m tkterm
+```
+
+## Integration with other Tkinter application
+The Terminal is implemented as a `Frame` widget and can easily be integrated to other Tkinter application by
+
+```python
+import tkinter as tk
+from tkinter import *
+from tkterm import Terminal
+
+root = tk.Tk()
+
+terminal = Terminal(root)
+terminal.pack(fill=BOTH, expand=True)
+
+root.mainloop()
+```
+
+> If downloaded via github append to system path before import
+> ```python
+> import sys
+> sys.path.insert(0, "./TkTerm")
+> from tkterm import Terminal
+> ```
+
+## Customisation options
+Customise Terminal interface by `Right-click > Settings...`
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/settings.png">
+</p>
+
+**Note**: \
+Clicking `Save config` saves setting configuration to a file.\
+Tkterm will automatically load this file the next time it starts up.
+
+## Multiline command
+Long lines of command can be broken up using a caret. A caret at the line end appends the next line command with the current command.
+In Windows the caret is `^`, and UNIX is `\`.
+
+For multiline command to be considered there must be ***no** trailing space after the caret*, for example:
+
+- `$> ping ^` is considered
+- `$> ping ^ ` is **not** considered
+
+```bash
+$>> echo I ^
+> have apple ^
+> and banana
+I have apple and banana
+```
+
+## Author
+
+Developed by Dhanoo Surasarang
+
+Github: [@dhanoosu](https://github.com/dhanoosu)
+
+## Links
+
+- **GitHub:** https://github.com/dhanoosu/TkTerm
```

### Comparing `tkterm-0.0.0b1/README.md` & `tkterm-0.0.0b2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![PyPI](https://img.shields.io/pypi/v/tkterm)](https://pypi.org/project/tkterm)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tkterm)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
+
 # TkTerm - Tkinter Terminal Emulator
 A fully functional terminal emulator built on Tkinter library - perform all basic commands of a terminal
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/snapshot2.png">
 </p>
 
@@ -19,37 +23,65 @@
 - Handles **multiline commands** using caret character `^` or `\`
 
 ## Requirements
 The Tkinter GUI library is built into Python, so no 3rd party library is required.
 
 Requires at least Python version 3.x and above.
 
+## Installation
+Get it from Github or PIP package manager
+
+```bash
+# From github
+git clone https://github.com/dhanoosu/TkTerm.git
+
+# From package manager
+pip install tkterm
+```
+
 ## Standalone usage
-Run standalone script simply with
+Navigate to downloaded folder and run script with
+
+```bash
+cd TkTerm
+
+# Either of these will work
+python tkterm
+python tkterm/tkterm.py
+```
+
+If package was installed via pip
 
 ```bash
-$> python tkterm/tkterm.py
+python -m tkterm
 ```
 
 ## Integration with other Tkinter application
-The Terminal is implemented as a `Frame` widget and can be easily be integrated to other Tkinter application by
+The Terminal is implemented as a `Frame` widget and can easily be integrated to other Tkinter application by
 
 ```python
 import tkinter as tk
 from tkinter import *
 from tkterm import Terminal
 
 root = tk.Tk()
 
 terminal = Terminal(root)
 terminal.pack(fill=BOTH, expand=True)
 
 root.mainloop()
 ```
 
+> If downloaded via github append to system path before import
+> ```python
+> import sys
+> sys.path.insert(0, "./TkTerm")
+> from tkterm import Terminal
+> ```
+
 ## Customisation options
 Customise Terminal interface by `Right-click > Settings...`
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/settings.png">
 </p>
 
@@ -69,16 +101,16 @@
 ```bash
 $>> echo I ^
 > have apple ^
 > and banana
 I have apple and banana
 ```
 
-## Links
-
-- **GitHub:** https://github.com/dhanoosu/TkTerm
-
 ## Author
 
 Developed by Dhanoo Surasarang
 
-Github: [@dhanoosu](https://github.com/dhanoosu)
+Github: [@dhanoosu](https://github.com/dhanoosu)
+
+## Links
+
+- **GitHub:** https://github.com/dhanoosu/TkTerm
```

### Comparing `tkterm-0.0.0b1/setup.py` & `tkterm-0.0.0b2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from tkterm import __version__
 from setuptools import setup, find_packages
 
 def read_from_file(path):
     """Return content from file"""
 
     with open(path, "r") as f:
         text = f.read()
 
     return text
 
 attrs = dict(
     name="tkterm",
-    version="0.0.0b1",
+    version=__version__,
     packages=find_packages(),
     include_package_data=True,
     long_description=read_from_file("README.md"),
     description="Terminal emulator built on Tkinter library.",
     long_description_content_type="text/markdown",
     author="Dhanoo Surasarang",
     author_email="dhanoo.surasarang@gmail.com",
@@ -38,24 +39,27 @@
         "tkinter-python",
         "tkinter-terminal",
         "tk-terminal",
         "tkinter-shell",
         "tkterminal"
     ],
     classifiers=[
-        # "Development Status :: 5 - Production/Stable",
-        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: MIT License",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3"
     ],
     project_urls={
         "Documentation": "https://github.com/dhanoosu/TkTerm/blob/master/README.md",
-        "Bug Tracker": "https://github.com/dhanoosu/tkterm/issues",
+        "Bug Tracker": "https://github.com/dhanoosu/TkTerm/issues",
     },
     include_package_data_info=True,
 )
 
+if "b" in __version__:
+    attrs["classifiers"].insert(0, "Development Status :: 4 - Beta")
+else:
+    attrs["classifiers"].insert(0, "Development Status :: 5 - Production/Stable")
+
 setup(**attrs)
```

### Comparing `tkterm-0.0.0b1/tkterm/backend/InterpreterShell.py` & `tkterm-0.0.0b2/tkterm/backend/InterpreterShell.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/backend/KThread.py` & `tkterm-0.0.0b2/tkterm/backend/KThread.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/app_icon.png` & `tkterm-0.0.0b2/tkterm/img/app_icon.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/close_tab.png` & `tkterm-0.0.0b2/tkterm/img/close_tab.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/hamburger.png` & `tkterm-0.0.0b2/tkterm/img/hamburger.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/linux.png` & `tkterm-0.0.0b2/tkterm/img/linux.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/new_tab.png` & `tkterm-0.0.0b2/tkterm/img/new_tab.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/next_tab.png` & `tkterm-0.0.0b2/tkterm/img/next_tab.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/plus.png` & `tkterm-0.0.0b2/tkterm/img/plus.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/prev_tab.png` & `tkterm-0.0.0b2/tkterm/img/prev_tab.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/screenshot.jpg` & `tkterm-0.0.0b2/tkterm/img/screenshot.jpg`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/search.png` & `tkterm-0.0.0b2/tkterm/img/search.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/settings.png` & `tkterm-0.0.0b2/tkterm/img/settings.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/snapshot1.png` & `tkterm-0.0.0b2/tkterm/img/snapshot1.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/snapshot2.png` & `tkterm-0.0.0b2/tkterm/img/snapshot2.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/warn.png` & `tkterm-0.0.0b2/tkterm/img/warn.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/img/windows.png` & `tkterm-0.0.0b2/tkterm/img/windows.png`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/src/Config.py` & `tkterm-0.0.0b2/tkterm/src/Config.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/src/ExitDiaglogBox.py` & `tkterm-0.0.0b2/tkterm/src/ExitDiaglogBox.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/src/Interpreter.py` & `tkterm-0.0.0b2/tkterm/src/Interpreter.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/src/Redirect.py` & `tkterm-0.0.0b2/tkterm/src/Redirect.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/src/RightClickContextMenu.py` & `tkterm-0.0.0b2/tkterm/src/RightClickContextMenu.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/src/SearchBar.py` & `tkterm-0.0.0b2/tkterm/src/SearchBar.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/src/TerminalScreen.py` & `tkterm-0.0.0b2/tkterm/src/TerminalScreen.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,16 @@
                 self.style.configure("Terminal.Vertical.TScrollbar", width=5)
                 self.style.map('Terminal.Vertical.TScrollbar',
                     background=[('active', "#3A3E48"), ('disabled', TkTermConfig.CONFIG["bg"])]
                 )
                 self.style.configure("Terminal.Vertical.TScrollbar", background="#3A3E48")
 
     def bind_keys(self):
+        self.TerminalScreen.bind("<FocusOut>",          self.focus_out)
+
         self.TerminalScreen.bind("<Return>",            self.do_keyReturn)
         self.TerminalScreen.bind("<Up>",                self.do_keyUpArrow)
         self.TerminalScreen.bind("<Down>",              self.do_keyDownArrow)
         self.TerminalScreen.bind("<BackSpace>",         self.do_keyBackspace)
         self.TerminalScreen.bind("<Delete>",            lambda event: "")
         self.TerminalScreen.bind("<End>",               lambda event: "")
         self.TerminalScreen.bind("<Left>",              self.do_keyLeftArrow)
@@ -377,14 +379,19 @@
             direction = 3
         if event.num == 4 or event.delta == 120:
             direction = -3
         self.TerminalScreen.yview_scroll(direction, UNITS)
 
         return "break"
 
+    def focus_out(self, event):
+        """When out of focus, store the last insertion index """
+
+        self.insertionIndex = self.TerminalScreen.index("insert")
+
     def do_keyPress(self, event):
 
         import string
 
         # The obvious information
         c = event.keysym
         s = event.state
@@ -639,14 +646,15 @@
 
     def do_leftClickRelease(self, *args):
 
         # Unhide cursor
         self.TerminalScreen["insertwidth"] = 1
         self.TerminalScreen["insertbackground"] = "white"
 
+        self.TerminalScreen.focus_set()
         self.TerminalScreen.mark_set("insert", self.insertionIndex)
 
     def do_middleClickRelease(self, *args):
 
         try:
             selected = self.TerminalScreen.selection_get()
         except Exception as e:
```

### Comparing `tkterm-0.0.0b1/tkterm/src/TerminalTab.py` & `tkterm-0.0.0b2/tkterm/src/TerminalTab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tkinter as tk
 from tkinter import *
 from tkinter import ttk
 
 import webbrowser
 
+from version import __version__
 from src.Utils import *
 from src.Config import TkTermConfig
 from src.TerminalScreen import TerminalWidget
 from src.SearchBar import SearchBar
 from src.RightClickContextMenu import RightClickContextMenu
 
 class TerminalTab(ttk.Notebook):
@@ -472,16 +473,17 @@
         frame = tk.Frame(self.parent, bg=INNER_BG)
         frame.place(relx=0.5, rely=0.5, anchor="center")
 
         # Inner frame
         frameInner = tk.Frame(frame, bg=INNER_BG)
         frameInner.pack(expand=True, fill=BOTH, padx=20, pady=20)
 
-        about_text = """
+        about_text = f"""
 TkTerm - Terminal Emulator built on Tkinter library
+Version: {__version__}
 
 Created by Dhanoo Surasarang
 Github @dhanoosu
 
 """
 
         labelIcon = tk.Label(frameInner, image=self.iconApp, bg=INNER_BG)
```

### Comparing `tkterm-0.0.0b1/tkterm/src/Tooltip.py` & `tkterm-0.0.0b2/tkterm/src/Tooltip.py`

 * *Files identical despite different names*

### Comparing `tkterm-0.0.0b1/tkterm/tkterm.py` & `tkterm-0.0.0b2/tkterm/tkterm.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from src.TerminalTab import TerminalTab
 from src.Interpreter import Interpreter
 from src.ExitDiaglogBox import ExitDiaglogBox
 from src.Utils import get_absolute_path
 from src.Config import TkTermConfig
 
 class Terminal(tk.Frame):
-
     """ Terminal widget """
 
     def __init__(self, parent, text=None, *args, **kwargs):
 
         super().__init__(parent, *args, **kwargs)
 
         self.splashText = text
@@ -86,21 +85,25 @@
         if self.scrollbar.get()[1] >= 1:
             self.TerminalScreen.see(END)
         # elif float(first_visible_line) >  1.0:
         #     self.TerminalScreen.see(float(first_visible_line)-1)
 
         # self.statusText.set(self.TerminalScreen.winfo_height())
 
-if __name__ == "__main__":
+def main():
+    """ Main function """
 
     root = tk.Tk()
     root.title("TkTerm - Terminal Emulator")
     root.geometry("700x400")
 
     terminal = Terminal(root)
     terminal.pack(expand=True, fill=BOTH)
 
     icon = PhotoImage(file=get_absolute_path(__file__, "icon.png"))
     root.iconphoto(False, icon)
 
     ExitDiaglogBox(root, icon)
-    root.mainloop()
+    root.mainloop()
+
+if __name__ == "__main__":
+    main()
```

### Comparing `tkterm-0.0.0b1/tkterm.egg-info/PKG-INFO` & `tkterm-0.0.0b2/tkterm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,137 @@
-Metadata-Version: 2.1
-Name: tkterm
-Version: 0.0.0b1
-Summary: Terminal emulator built on Tkinter library.
-Home-page: https://github.com/dhanoosu/tkterm
-Author: Dhanoo Surasarang
-Author-email: dhanoo.surasarang@gmail.com
-License: MIT
-Project-URL: Documentation, https://github.com/dhanoosu/TkTerm/blob/master/README.md
-Project-URL: Bug Tracker, https://github.com/dhanoosu/tkterm/issues
-Keywords: linux,shell,bash,cli,gui,terminal,command-line,tkinter,subprocess,tkinter-graphic-interface,terminal-emulator,ttk,commandprompt,tkinter-gui,tkinter-python,tkinter-terminal,tk-terminal,tkinter-shell,tkterminal
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# TkTerm - Tkinter Terminal Emulator
-A fully functional terminal emulator built on Tkinter library - perform all basic commands of a terminal
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/snapshot2.png">
-</p>
-
-Under the hood it executes commands using Python's *subprocess* module and spawn as a thread. Pressing `Ctrl-C` will terminate current running command. Supports Unix shells (`sh` and `bash`) and Window's Command Prompt (`cmd.exe`) commands.
-
-## Features
-- Compatible with Windows and Unix systems
-- Tabbed Terminal - `click & drag` to reorder, `middle-click` to close tab, `double-click` to rename
-- Return Code (RC) of previous run commands is shown at the bottom status bar
-- Settings to customise colours, font and cursor shape
-- **Ctrl-C** to kill current running process
-- **Ctrl-F** to search; supports case sensitivity and regex searches
-- **UP** and **DOWN** arrow keys to cycle between next and previous commands in history
-- Unix-like **tab completion** on files and directories
-- Handles **multiline commands** using caret character `^` or `\`
-
-## Requirements
-The Tkinter GUI library is built into Python, so no 3rd party library is required.
-
-Requires at least Python version 3.x and above.
-
-## Standalone usage
-Run standalone script simply with
-
-```bash
-$> python tkterm/tkterm.py
-```
-
-## Integration with other Tkinter application
-The Terminal is implemented as a `Frame` widget and can be easily be integrated to other Tkinter application by
-
-```python
-import tkinter as tk
-from tkinter import *
-from tkterm import Terminal
-
-root = tk.Tk()
-
-terminal = Terminal(root)
-terminal.pack(fill=BOTH, expand=True)
-
-root.mainloop()
-```
-
-## Customisation options
-Customise Terminal interface by `Right-click > Settings...`
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/settings.png">
-</p>
-
-**Note**: \
-Clicking `Save config` saves setting configuration to a file.\
-Tkterm will automatically load this file the next time it starts up.
-
-## Multiline command
-Long lines of command can be broken up using a caret. A caret at the line end appends the next line command with the current command.
-In Windows the caret is `^`, and UNIX is `\`.
-
-For multiline command to be considered there must be ***no** trailing space after the caret*, for example:
-
-- `$> ping ^` is considered
-- `$> ping ^ ` is **not** considered
-
-```bash
-$>> echo I ^
-> have apple ^
-> and banana
-I have apple and banana
-```
-
-## Links
-
-- **GitHub:** https://github.com/dhanoosu/TkTerm
-
-## Author
-
-Developed by Dhanoo Surasarang
-
-Github: [@dhanoosu](https://github.com/dhanoosu)
-
+Metadata-Version: 2.1
+Name: tkterm
+Version: 0.0.0b2
+Summary: Terminal emulator built on Tkinter library.
+Home-page: https://github.com/dhanoosu/tkterm
+Author: Dhanoo Surasarang
+Author-email: dhanoo.surasarang@gmail.com
+License: MIT
+Project-URL: Documentation, https://github.com/dhanoosu/TkTerm/blob/master/README.md
+Project-URL: Bug Tracker, https://github.com/dhanoosu/TkTerm/issues
+Keywords: linux,shell,bash,cli,gui,terminal,command-line,tkinter,subprocess,tkinter-graphic-interface,terminal-emulator,ttk,commandprompt,tkinter-gui,tkinter-python,tkinter-terminal,tk-terminal,tkinter-shell,tkterminal
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/tkterm)](https://pypi.org/project/tkterm)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tkterm)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
+
+# TkTerm - Tkinter Terminal Emulator
+A fully functional terminal emulator built on Tkinter library - perform all basic commands of a terminal
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/snapshot2.png">
+</p>
+
+Under the hood it executes commands using Python's *subprocess* module and spawn as a thread. Pressing `Ctrl-C` will terminate current running command. Supports Unix shells (`sh` and `bash`) and Window's Command Prompt (`cmd.exe`) commands.
+
+## Features
+- Compatible with Windows and Unix systems
+- Tabbed Terminal - `click & drag` to reorder, `middle-click` to close tab, `double-click` to rename
+- Return Code (RC) of previous run commands is shown at the bottom status bar
+- Settings to customise colours, font and cursor shape
+- **Ctrl-C** to kill current running process
+- **Ctrl-F** to search; supports case sensitivity and regex searches
+- **UP** and **DOWN** arrow keys to cycle between next and previous commands in history
+- Unix-like **tab completion** on files and directories
+- Handles **multiline commands** using caret character `^` or `\`
+
+## Requirements
+The Tkinter GUI library is built into Python, so no 3rd party library is required.
+
+Requires at least Python version 3.x and above.
+
+## Installation
+Get it from Github or PIP package manager
+
+```bash
+# From github
+git clone https://github.com/dhanoosu/TkTerm.git
+
+# From package manager
+pip install tkterm
+```
+
+## Standalone usage
+Navigate to downloaded folder and run script with
+
+```bash
+cd TkTerm
+
+# Either of these will work
+python tkterm
+python tkterm/tkterm.py
+```
+
+If package was installed via pip
+
+```bash
+python -m tkterm
+```
+
+## Integration with other Tkinter application
+The Terminal is implemented as a `Frame` widget and can easily be integrated to other Tkinter application by
+
+```python
+import tkinter as tk
+from tkinter import *
+from tkterm import Terminal
+
+root = tk.Tk()
+
+terminal = Terminal(root)
+terminal.pack(fill=BOTH, expand=True)
+
+root.mainloop()
+```
+
+> If downloaded via github append to system path before import
+> ```python
+> import sys
+> sys.path.insert(0, "./TkTerm")
+> from tkterm import Terminal
+> ```
+
+## Customisation options
+Customise Terminal interface by `Right-click > Settings...`
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/dhanoosu/TkTerm/master/tkterm/img/settings.png">
+</p>
+
+**Note**: \
+Clicking `Save config` saves setting configuration to a file.\
+Tkterm will automatically load this file the next time it starts up.
+
+## Multiline command
+Long lines of command can be broken up using a caret. A caret at the line end appends the next line command with the current command.
+In Windows the caret is `^`, and UNIX is `\`.
+
+For multiline command to be considered there must be ***no** trailing space after the caret*, for example:
+
+- `$> ping ^` is considered
+- `$> ping ^ ` is **not** considered
+
+```bash
+$>> echo I ^
+> have apple ^
+> and banana
+I have apple and banana
+```
+
+## Author
+
+Developed by Dhanoo Surasarang
+
+Github: [@dhanoosu](https://github.com/dhanoosu)
+
+## Links
+
+- **GitHub:** https://github.com/dhanoosu/TkTerm
```

### Comparing `tkterm-0.0.0b1/tkterm.egg-info/SOURCES.txt` & `tkterm-0.0.0b2/tkterm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 tkterm/__init__.py
+tkterm/__main__.py
+tkterm/icon.png
 tkterm/tkterm.py
+tkterm/version.py
 tkterm.egg-info/PKG-INFO
 tkterm.egg-info/SOURCES.txt
 tkterm.egg-info/dependency_links.txt
 tkterm.egg-info/top_level.txt
 tkterm/backend/InterpreterInterface.py
 tkterm/backend/InterpreterShell.py
 tkterm/backend/KThread.py
```


# Comparing `tmp/mote-gtest-gui-0.8.0.tar.gz` & `tmp/mote-gtest-gui-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mote-gtest-gui-0.8.0.tar", last modified: Sun Apr 23 18:31:43 2023, max compression
+gzip compressed data, was "mote-gtest-gui-0.8.1.tar", last modified: Mon Apr 24 19:08:38 2023, max compression
```

## Comparing `mote-gtest-gui-0.8.0.tar` & `mote-gtest-gui-0.8.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-23 18:31:43.830419 mote-gtest-gui-0.8.0/
--rw-r--r--   0 tom      (31978) tom       (2000)    35149 2023-03-12 12:42:14.000000 mote-gtest-gui-0.8.0/LICENSE
--rw-r--r--   0 tom      (31978) tom       (2000)      110 2023-04-23 18:25:01.000000 mote-gtest-gui-0.8.0/MANIFEST.in
--rw-r--r--   0 tom      (31978) tom       (2000)    28243 2023-04-23 18:31:43.830419 mote-gtest-gui-0.8.0/PKG-INFO
--rw-r--r--   0 tom      (31978) tom       (2000)     4897 2023-04-23 18:26:45.000000 mote-gtest-gui-0.8.0/README.md
--rw-r--r--   0 tom      (31978) tom       (2000)     2901 2023-04-23 18:25:01.000000 mote-gtest-gui-0.8.0/TODO.txt
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-23 18:31:43.826419 mote-gtest-gui-0.8.0/bin/
--rwxr-xr-x   0 tom      (31978) tom       (2000)     1280 2023-04-23 18:25:01.000000 mote-gtest-gui-0.8.0/bin/gtest_gui
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-23 18:31:43.830419 mote-gtest-gui-0.8.0/gtest_gui/
--rw-r--r--   0 tom      (31978) tom       (2000)       22 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.0/gtest_gui/__init__.py
--rw-r--r--   0 tom      (31978) tom       (2000)       31 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.0/gtest_gui/__main__.py
--rw-r--r--   0 tom      (31978) tom       (2000)      670 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.0/gtest_gui/bisect.py
--rwxr-xr-x   0 tom      (31978) tom       (2000)    14215 2023-04-23 18:22:19.000000 mote-gtest-gui-0.8.0/gtest_gui/config_db.py
--rw-r--r--   0 tom      (31978) tom       (2000)    12422 2023-04-23 18:25:01.000000 mote-gtest-gui-0.8.0/gtest_gui/dlg_browser.py
--rw-r--r--   0 tom      (31978) tom       (2000)    10132 2023-04-18 11:26:41.000000 mote-gtest-gui-0.8.0/gtest_gui/dlg_config.py
--rw-r--r--   0 tom      (31978) tom       (2000)     8073 2023-04-02 17:01:27.000000 mote-gtest-gui-0.8.0/gtest_gui/dlg_debug.py
--rw-r--r--   0 tom      (31978) tom       (2000)     7488 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.0/gtest_gui/dlg_font_sel.py
--rwxr-xr-x   0 tom      (31978) tom       (2000)    10929 2023-04-16 18:15:48.000000 mote-gtest-gui-0.8.0/gtest_gui/dlg_help.py
--rw-r--r--   0 tom      (31978) tom       (2000)     9212 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.0/gtest_gui/dlg_job_list.py
--rw-r--r--   0 tom      (31978) tom       (2000)    17288 2023-04-23 08:11:12.000000 mote-gtest-gui-0.8.0/gtest_gui/dlg_main.py
--rw-r--r--   0 tom      (31978) tom       (2000)    20826 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.0/gtest_gui/dlg_tc_list.py
--rw-r--r--   0 tom      (31978) tom       (2000)     1637 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.0/gtest_gui/fcntl.py
--rw-r--r--   0 tom      (31978) tom       (2000)    10319 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.0/gtest_gui/filter_expr.py
--rw-r--r--   0 tom      (31978) tom       (2000)    37515 2023-04-23 18:25:01.000000 mote-gtest-gui-0.8.0/gtest_gui/gtest.py
--rw-r--r--   0 tom      (31978) tom       (2000)    32768 2023-04-23 18:25:01.000000 mote-gtest-gui-0.8.0/gtest_gui/help_db.py
--rw-r--r--   0 tom      (31978) tom       (2000)     4120 2023-04-23 18:30:59.000000 mote-gtest-gui-0.8.0/gtest_gui/main.py
--rw-r--r--   0 tom      (31978) tom       (2000)     5357 2023-04-22 05:49:45.000000 mote-gtest-gui-0.8.0/gtest_gui/test_db.py
--rw-r--r--   0 tom      (31978) tom       (2000)     8434 2023-04-22 05:44:31.000000 mote-gtest-gui-0.8.0/gtest_gui/tk_utils.py
--rw-r--r--   0 tom      (31978) tom       (2000)    13123 2023-04-23 18:25:01.000000 mote-gtest-gui-0.8.0/gtest_gui/tool_tip_db.py
--rw-r--r--   0 tom      (31978) tom       (2000)     3594 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.0/gtest_gui/wid_status_line.py
--rw-r--r--   0 tom      (31978) tom       (2000)    35241 2023-04-23 18:25:01.000000 mote-gtest-gui-0.8.0/gtest_gui/wid_test_ctrl.py
--rw-r--r--   0 tom      (31978) tom       (2000)    31652 2023-04-22 05:49:45.000000 mote-gtest-gui-0.8.0/gtest_gui/wid_test_log.py
--rw-r--r--   0 tom      (31978) tom       (2000)    21045 2023-03-22 18:17:17.000000 mote-gtest-gui-0.8.0/gtest_gui/wid_text_sel.py
--rw-r--r--   0 tom      (31978) tom       (2000)     6032 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.0/gtest_gui/wid_tool_tip.py
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-23 18:31:43.830419 mote-gtest-gui-0.8.0/mote_gtest_gui.egg-info/
--rw-r--r--   0 tom      (31978) tom       (2000)    28243 2023-04-23 18:31:43.000000 mote-gtest-gui-0.8.0/mote_gtest_gui.egg-info/PKG-INFO
--rw-r--r--   0 tom      (31978) tom       (2000)      834 2023-04-23 18:31:43.000000 mote-gtest-gui-0.8.0/mote_gtest_gui.egg-info/SOURCES.txt
--rw-r--r--   0 tom      (31978) tom       (2000)        1 2023-04-23 18:31:43.000000 mote-gtest-gui-0.8.0/mote_gtest_gui.egg-info/dependency_links.txt
--rw-r--r--   0 tom      (31978) tom       (2000)        8 2023-04-23 18:31:43.000000 mote-gtest-gui-0.8.0/mote_gtest_gui.egg-info/requires.txt
--rw-r--r--   0 tom      (31978) tom       (2000)       10 2023-04-23 18:31:43.000000 mote-gtest-gui-0.8.0/mote_gtest_gui.egg-info/top_level.txt
--rw-r--r--   0 tom      (31978) tom       (2000)       38 2023-04-23 18:31:43.830419 mote-gtest-gui-0.8.0/setup.cfg
--rwxr-xr-x   0 tom      (31978) tom       (2000)     1538 2023-04-23 18:25:05.000000 mote-gtest-gui-0.8.0/setup.py
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/
+-rw-r--r--   0 tom      (31978) tom       (2000)    35149 2023-03-12 12:42:14.000000 mote-gtest-gui-0.8.1/LICENSE
+-rw-r--r--   0 tom      (31978) tom       (2000)      110 2023-04-23 09:14:13.000000 mote-gtest-gui-0.8.1/MANIFEST.in
+-rw-r--r--   0 tom      (31978) tom       (2000)    28541 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/PKG-INFO
+-rw-r--r--   0 tom      (31978) tom       (2000)     4976 2023-04-24 19:03:19.000000 mote-gtest-gui-0.8.1/README.md
+-rw-r--r--   0 tom      (31978) tom       (2000)     2901 2023-04-24 18:58:13.000000 mote-gtest-gui-0.8.1/TODO.txt
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-24 19:08:38.031321 mote-gtest-gui-0.8.1/bin/
+-rwxr-xr-x   0 tom      (31978) tom       (2000)     1280 2023-04-23 09:14:13.000000 mote-gtest-gui-0.8.1/bin/gtest_gui
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/gtest_gui/
+-rw-r--r--   0 tom      (31978) tom       (2000)       22 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.1/gtest_gui/__init__.py
+-rw-r--r--   0 tom      (31978) tom       (2000)       31 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.1/gtest_gui/__main__.py
+-rw-r--r--   0 tom      (31978) tom       (2000)      670 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.1/gtest_gui/bisect.py
+-rwxr-xr-x   0 tom      (31978) tom       (2000)    14215 2023-04-24 07:48:51.000000 mote-gtest-gui-0.8.1/gtest_gui/config_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    12432 2023-04-24 18:49:48.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_browser.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    10132 2023-04-18 11:26:41.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_config.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     8073 2023-04-02 17:01:27.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_debug.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     7488 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_font_sel.py
+-rwxr-xr-x   0 tom      (31978) tom       (2000)    10929 2023-04-16 18:15:48.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_help.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     9212 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_job_list.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    17290 2023-04-24 18:51:42.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_main.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    20826 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_tc_list.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     1637 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.1/gtest_gui/fcntl.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    10319 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/filter_expr.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    37727 2023-04-24 18:22:59.000000 mote-gtest-gui-0.8.1/gtest_gui/gtest.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    33151 2023-04-24 19:00:42.000000 mote-gtest-gui-0.8.1/gtest_gui/help_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     4120 2023-04-24 07:48:51.000000 mote-gtest-gui-0.8.1/gtest_gui/main.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     5357 2023-04-22 05:49:45.000000 mote-gtest-gui-0.8.1/gtest_gui/test_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     8434 2023-04-22 05:44:31.000000 mote-gtest-gui-0.8.1/gtest_gui/tk_utils.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    13123 2023-04-23 09:13:02.000000 mote-gtest-gui-0.8.1/gtest_gui/tool_tip_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     3594 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_status_line.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    35236 2023-04-24 18:30:17.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_test_ctrl.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    31652 2023-04-24 18:50:48.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_test_log.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    21045 2023-03-22 18:17:17.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_text_sel.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     6032 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_tool_tip.py
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/
+-rw-r--r--   0 tom      (31978) tom       (2000)    28541 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/PKG-INFO
+-rw-r--r--   0 tom      (31978) tom       (2000)      834 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)        1 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)        8 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/requires.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)       10 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/top_level.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)       38 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/setup.cfg
+-rwxr-xr-x   0 tom      (31978) tom       (2000)     1538 2023-04-24 18:51:56.000000 mote-gtest-gui-0.8.1/setup.py
```

### Comparing `mote-gtest-gui-0.8.0/LICENSE` & `mote-gtest-gui-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/PKG-INFO` & `mote-gtest-gui-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mote-gtest-gui
-Version: 0.8.0
+Version: 0.8.1
 Summary: Module tester's Gtest GUI is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
 Home-page: https://github.com/tomzox/gtest_gui
 Author: T. Zoerner
 Author-email: tomzox@gmail.com
 License: UNKNOWN
 Keywords: google-test,gtest,testing-tools,test-runners,tkinter,GUI
 Platform: posix
@@ -23,50 +23,50 @@
 
 Module-Tester's Gtest GUI
 =========================
 
 Description
 -----------
 
-Module-tester's GtestGui is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
+**Module-tester's GtestGui** is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
 
 The tool will work with any application with Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results, which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
 
 GtestGui typically is started with the path of an executable on the command line which is built using the gtest library. Using the "Run" button in the GUI, this executable can then be started and its progress be monitored live in the result log frame of the main window. Additional controls allow specifying options such as test case filter string and repetition count, which are forwarded to the executable via the respective "\ ``--gtest_*``" command line arguments.
 
-While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with *Trowser*, which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user *trowser.py*, but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening trace snippets.
+While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with *Trowser*, which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user *trowser.py*, but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening traces.
 
 Test control
 ------------
 
 The application main window consists of a menu bar, a frame containing test controls, a frame containing the test result log, and a text frame for trace preview. This chapter describes the top-most frame with the test controls.
 
 Test campaign control buttons
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Most prominent in the test control frame are the green buttons which directly control execution of the configured executable file:
+Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file:
 
 *Run*:
   Starts the text executable in a separate process, with its output redirected into a pipe which is read by GtestGui for progress monitoring. The output is also saved into a file.
 
   Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. Note after adding a new test case, use the *Refresh test case list* command in the *Control* menu to read the test case list, for allowing to use the new test case name in a filter pattern.
 
   Multiple processes are started if the *CPUs* value is larger than 1. Most of the time, GtestGui will use gtest's "sharding" feature, which assigns a static sub-set of tests to each process. However, if repetition count is larger than one and the number of configured CPUs is larger than the number of test cases, or if the remainder of division of test cases by CPUs is large, GtestGui may instead or additionally partition by repetitions.
 
   Note when a test process crashes, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
 
 *Stop*:
   Sends a TERM signal to the test processes and waits for them to finish. When termination takes a long time (possibly because the executable is hung) and the button is clicked a second time, a KILL signal is sent.
 
 *Resume*:
-  Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful in particular when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
+  Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
 
   This command will also use the same version of the test executable as used previously if option *Create copy of executable file* is enabled, see `Configuration`_. This allows resuming execution even when the executable at the configured path no longer exists, for example due to a failed build.
 
-  When resuming, scheduling cannot restart exactly where it was stopped due to limitations in gtest. If repetition count is 1, all test cases will be rescheduled. For higher repetition count, the the lowest number of remaining repetitions across all selected test cases is rescheduled.
+  When resuming, scheduling cannot restart exactly where it was stopped due to limitations in gtest. If repetition count is 1, all test cases will be rescheduled. For higher repetition count, the lowest number of remaining repetitions across all selected test cases is rescheduled.
 
 *Repeat*:
   Repeats the test cases marked manually for repetition via the result log, or all previously failed test cases if none were selected. This allows quick repetition of individual test cases without changing the test case filter.
 
 Test case filter
 ~~~~~~~~~~~~~~~~
 
@@ -108,18 +108,20 @@
   When enabled, "\ ``--gtest_also_run_disabled_tests``" option is set via the executable's command line. The option enables execution of test suites and individual test cases whose name starts with "\ ``DISABLED``".
 
   The option also affects test case filter and test case selection menus within GtestGui: When the option is not set, entering filter pattern "\ ``*DISABLED*``" would raise a warning that it matches no test cases (even if there are some with that name). The drop-down menu below the entry field would no show such names.
 
 *Break on failure*:
   When enabled, "\ ``--gtest_break_on_failure``" option is set via the executable's command line. This will cause SIGTRAP to be sent to the test process upon the first failure. As no debugger is attached, this will cause the process to crash.
 
-  When core dumps are enabled in the kernel, the core will be save by GtestGui and can be analyzed via the *Extract stack trace from core dump* command in the result log's context menu. When core dumps are not enabled, this option is probably not very useful.
+  When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the *Extract stack trace from core dump* command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 
 *Break on exception*:
-  When enabled, "\ ``--gtest_catch_exceptions=0``" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means the exception causes the process to terminate.
+  When enabled, "\ ``--gtest_catch_exceptions=0``" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means any exception not caught by the test case itself causes the test process to crash due to an unhandled exception.
+
+  When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the *Extract stack trace from core dump* command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 
 *Valgrind* and *Valgrind - 2nd option set*:
   The two valgrind options serve to run each execution of the test executable under valgrind using the configured command line. Notably, valgrind checks are performed across the complete lifetime of the test process, thus spanning all test cases or test repetitions. Therefore, if for example a memory leak is reported at the end, it cannot be determined which test case caused it (or it may even be caused by interaction of the test sequence.) Therefore valgrind errors are reported with a special entry in the result log. Some kind of errors such as invalid memory accesses can be mapped to test cases based on the position of the error report in the output stream. Note however that the position may not exactly reflect the timing of occurrence due to possible buffering in output streams within the test executable.) See `Result log`_ and `Configuration`_ for more details.
 
 Result log
 ----------
 
@@ -177,15 +179,15 @@
 
 Test management options
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 *Trace browser*
   This entry field selects the external application used for displaying trace files and trace snippets, when double-clicking on an entry in the result log. By default, trace browser *trowser.py* is used. You can either specify just the application file name, or its full path if it is not found via ``PATH`` configured in environment. The path of the trace file to be displayed will be appended to the given command line.
 
-  Currently the application path name or parameters cannot contain space characters, as these are assumed be be separators.
+  Currently the application path name or parameters cannot contain space characters, as these are assumed to be separators.
 
   Note for the Windows platform: When using the default of ``trowser.py``, you may need to insert the Python interpreter in front of "trowser.py", depending on your Python installation. In that case you need to add the full path to where ``trowser.py`` is installed.
 
   Enable option *Browser supports reading from STDIN* if the selected trace browser supports reading text from "standard input" via a pipeline. In this case filename "\ ``-``" is passed on the command line instead of a file name.  The default browser *trowser.py* supports this. When not enabled, GtestGui has to create temporary files for passing trace snippets to the browser application.
 
 *Pattern for seed*
   If a regular expression pattern is specified here, it will be applied to the trace of each test case. The string returned by the first match group (i.e. the first set of capturing parenthesis) will be shown in the corresponding result log as "seed". (This is intended for allowing repeat of a test sequence exactly even for test cases using randomness, by starting their PRNG with the same seed. This is not yet supported however, due to lack of an interface for passing a list of seed values via the GTest command line interface.)
@@ -203,15 +205,15 @@
   When enabled, a copy of the current executable under test is made within the configured trace directory. (Technically, the copy is achieved by creating a so-called "hard link", so that no additional disk space is needed.) This is recommended so that recompiling the executable does not affect the current test run (i.e. compilation may either fail with error "file busy" when tests are running, or tests may crash). This option is required for allowing to extract stack traces from core dump files taken from an older executable version. Note this option may not work when using trace directories in locations such as /tmp on UNIX-like systems, as these usually are configured to disallow executable files for security reasons.
 
 *Valgrind command line*
   *UNIX only:* Command lines to use for running test executables when one of the "Valgrind" options in the main window is enabled. The executable name and gtest options will be appended to the given command line.
 
   There are two separate entry fields, corresponding to the two check-buttons in the main window. This is intended for allowing to configure a configuration variant that runs faster and one that is slower but performs deeper analysis. By default, the command will perform check for memory leaks (notably at end of all test cases, not for individual test cases in a run of multiple tests) and for use of uninitialized memory. The second command line has additional options for tracking the origin of uninitialized memory.
 
-  Currently the path or parameters cannot contain space characters, as these are assumed be be separators.
+  Currently the path or parameters cannot contain space characters, as these are assumed to be separators.
 
 *Valgrind supports --exit-code*
   When this option is set, parameter "--error-exitcode=125" will be appended to the given valgrind command lines. This is required for detecting automatically that valgrind found errors during test execution. Only when enabled, result logs will report valgrind errors.
 
 The debugger used for extracting stack traces from core files (POSIX only) is currently not configurable; It is hard-coded to "\ ``gdb``", which should be somewhere in the ``PATH`` configured in environment.
 
 Caveats
```

### Comparing `mote-gtest-gui-0.8.0/README.md` & `mote-gtest-gui-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,19 @@
 complete set of tests and which kind of failures occur.  And it supports final
 quality checking in long-running, high-repetition test campaigns, optionally
 using valgrind or sanitizer builds.
 
 ## Installation
 
 GtestGui is available as package "mote-gtest-gui" ("Module tester's Gtest GUI")
-on [PyPi](https://pypi.org/project/mote-gtest-gui/)
+on [PyPi](https://pypi.org/project/mote-gtest-gui/). It can be installed using
+pip3:
+```console
+   pip3 install mote-gtest-gui
+```
 
 Python3 and the Python "tkinter" module are required. (The latter usually is
 part of default Python installation.)
 
 ## Usage
 
 Packages are not yet provided. To use the software, clone the repository and
```

### Comparing `mote-gtest-gui-0.8.0/TODO.txt` & `mote-gtest-gui-0.8.1/TODO.txt`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/bin/gtest_gui` & `mote-gtest-gui-0.8.1/bin/gtest_gui`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/bisect.py` & `mote-gtest-gui-0.8.1/gtest_gui/bisect.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/config_db.py` & `mote-gtest-gui-0.8.1/gtest_gui/config_db.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/dlg_browser.py` & `mote-gtest-gui-0.8.1/gtest_gui/dlg_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
 import os
+import re
 import subprocess
 import sys
 import tempfile
 import threading
 
 if (os.name == "posix"): import fcntl
```

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/dlg_config.py` & `mote-gtest-gui-0.8.1/gtest_gui/dlg_config.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/dlg_debug.py` & `mote-gtest-gui-0.8.1/gtest_gui/dlg_debug.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/dlg_font_sel.py` & `mote-gtest-gui-0.8.1/gtest_gui/dlg_font_sel.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/dlg_help.py` & `mote-gtest-gui-0.8.1/gtest_gui/dlg_help.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/dlg_job_list.py` & `mote-gtest-gui-0.8.1/gtest_gui/dlg_job_list.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/dlg_main.py` & `mote-gtest-gui-0.8.1/gtest_gui/dlg_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
         wid_about.wm_group(self.tk)
         wid_about.wm_title("About Gtest GUI")
 
         wid_lab1 = tk.Label(wid_about, text="Module tester's GoogleTest GUI",
                             font=tk_utils.font_bold)
         wid_lab1.pack(side=tk.TOP, pady=5)
 
-        wid_lab2 = tk.Label(wid_about, text="Version 0.8\n"
+        wid_lab2 = tk.Label(wid_about, text="Version 0.8.1\n"
                                             "Copyright (C) 2023 T. Zoerner")
         wid_lab2.pack(side=tk.TOP)
 
         url = "https://github.com/tomzox/gtest_gui"
         wid_lab3 = tk.Label(wid_about, text=url, fg="blue",
                             cursor="top_left_arrow")
         wid_lab3.pack(side=tk.TOP, pady=5)
```

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/dlg_tc_list.py` & `mote-gtest-gui-0.8.1/gtest_gui/dlg_tc_list.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/fcntl.py` & `mote-gtest-gui-0.8.1/gtest_gui/fcntl.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/filter_expr.py` & `mote-gtest-gui-0.8.1/gtest_gui/filter_expr.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/gtest.py` & `mote-gtest-gui-0.8.1/gtest_gui/gtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1064,9 +1064,14 @@
             if snippet_data:
                 snippet_data += buf_data[done_off : last_line_off]
             buf_data = buf_data[last_line_off:]
             file_off += last_line_off
 
 
 def gtest_automatic_import():
-    for file_name in gtest_control_search_trace_dirs():
-        gtest_import_result_file(file_name, True)
+    try:
+        for file_name in gtest_control_search_trace_dirs():
+            gtest_import_result_file(file_name, True)
+    except OSError as e:
+        tk_messagebox.showerror(parent=tk_utils.tk_top,
+                                message="Error during automatic import of trace files: " + str(e))
+        return
```

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/help_db.py` & `mote-gtest-gui-0.8.1/gtest_gui/help_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 helpSections[(1,2)] = '''Test case filter'''
 helpSections[(1,3)] = '''Test control options'''
 helpSections[(3,1)] = '''User-interface options'''
 helpSections[(3,2)] = '''Test management options'''
 
 helpTexts = {}
 helpTexts[0] = (('''Description''', 'title1'), ('''
-''', ''), ('''Module-tester's GtestGui is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
+''', ''), ('''Module-tester's GtestGui''', 'bold'), (''' is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
 ''', ''), ('''The tool will work with any application with Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results, which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
 ''', ''), ('''GtestGui typically is started with the path of an executable on the command line which is built using the gtest library. Using the "Run" button in the GUI, this executable can then be started and its progress be monitored live in the result log frame of the main window. Additional controls allow specifying options such as test case filter string and repetition count, which are forwarded to the executable via the respective "''', ''), ('''--gtest_*''', 'fixed'), ('''" command line arguments.
-''', ''), ('''While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with ''', ''), ('''Trowser''', 'underlined'), (''', which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user ''', ''), ('''trowser.py''', 'underlined'), (''', but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening trace snippets.
+''', ''), ('''While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with ''', ''), ('''Trowser''', 'underlined'), (''', which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user ''', ''), ('''trowser.py''', 'underlined'), (''', but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening traces.
 ''', ''), )
 
 helpTexts[1] = (('''Test control''', 'title1'), ('''
 ''', ''), ('''The application main window consists of a menu bar, a frame containing test controls, a frame containing the test result log, and a text frame for trace preview. This chapter describes the top-most frame with the test controls.
 ''', ''), ('''Test campaign control buttons''', 'title2'), ('''
-''', ''), ('''Most prominent in the test control frame are the green buttons which directly control execution of the configured executable file:
+''', ''), ('''Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file:
 ''', ''), ('''Run''', 'underlined'), (''':
 ''', ''), ('''Starts the text executable in a separate process, with its output redirected into a pipe which is read by GtestGui for progress monitoring. The output is also saved into a file.
 ''', 'indent'), ('''Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. Note after adding a new test case, use the ''', 'indent'), ('''Refresh test case list''', ('underlined', 'indent')), (''' command in the ''', 'indent'), ('''Control''', ('underlined', 'indent')), (''' menu to read the test case list, for allowing to use the new test case name in a filter pattern.
 ''', 'indent'), ('''Multiple processes are started if the ''', 'indent'), ('''CPUs''', ('underlined', 'indent')), (''' value is larger than 1. Most of the time, GtestGui will use gtest's "sharding" feature, which assigns a static sub-set of tests to each process. However, if repetition count is larger than one and the number of configured CPUs is larger than the number of test cases, or if the remainder of division of test cases by CPUs is large, GtestGui may instead or additionally partition by repetitions.
 ''', 'indent'), ('''Note when a test process crashes, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
 ''', 'indent'), ('''Stop''', 'underlined'), (''':
 ''', ''), ('''Sends a TERM signal to the test processes and waits for them to finish. When termination takes a long time (possibly because the executable is hung) and the button is clicked a second time, a KILL signal is sent.
 ''', 'indent'), ('''Resume''', 'underlined'), (''':
-''', ''), ('''Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful in particular when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
+''', ''), ('''Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
 ''', 'indent'), ('''This command will also use the same version of the test executable as used previously if option ''', 'indent'), ('''Create copy of executable file''', ('underlined', 'indent')), (''' is enabled, see ''', 'indent'), ('''Configuration''', ('href', 'indent')), ('''. This allows resuming execution even when the executable at the configured path no longer exists, for example due to a failed build.
-''', 'indent'), ('''When resuming, scheduling cannot restart exactly where it was stopped due to limitations in gtest. If repetition count is 1, all test cases will be rescheduled. For higher repetition count, the the lowest number of remaining repetitions across all selected test cases is rescheduled.
+''', 'indent'), ('''When resuming, scheduling cannot restart exactly where it was stopped due to limitations in gtest. If repetition count is 1, all test cases will be rescheduled. For higher repetition count, the lowest number of remaining repetitions across all selected test cases is rescheduled.
 ''', 'indent'), ('''Repeat''', 'underlined'), (''':
 ''', ''), ('''Repeats the test cases marked manually for repetition via the result log, or all previously failed test cases if none were selected. This allows quick repetition of individual test cases without changing the test case filter.
 ''', 'indent'), ('''Test case filter''', 'title2'), ('''
 ''', ''), ('''The entry field at the top of the test control frame allows specifying a test case filter, so that only a matching sub-set of test cases is run. The filter can be entered manually using the same syntax as the "''', ''), ('''--gtest-filter''', 'fixed'), ('''" command line option: The format of a filter expression is a ":"-separated list of test case names of wildcard patterns (positive patterns), optionally followed by a "-" and another ":"-separated pattern list (negative patterns). A test matches the filter if and only if it matches any of the positive patterns, but none of the negative ones. Wildcard characters are "*" (matching any sub-string) and "?" (matching any single character). As a special case, when no positive pattern is specified, all test cases are considered matching.
 ''', ''), ('''Alternatively, the test case filter can be modified via the drop-down menu below the entry field (which can be opened by the Cursor-Down key or a click on the drop-down button next to the entry field). The menu has entries for selecting and deselecting entries test suites as well as individual test cases. When modifying the filter this way, GtestGui will update the entry field with the shortest filter expression it can find using trailing wild card and negative patterns.
 ''', ''), ('''Yet another alternative for modifying test case filters is the test case list dialog, either via its context menu or the "Return" and "Delete" key bindings. Finally note any modification to the test case filter can be undone using "Control-Z" key binding in the entry field, or redone using "Control-Y" key binding.
 ''', ''), ('''Test control options''', 'title2'), ('''
@@ -63,17 +63,18 @@
 ''', 'indent'), ('''Shuffle execution order''', 'underlined'), (''':
 ''', ''), ('''When enabled, "''', 'indent'), ('''--gtest_shuffle''', ('fixed', 'indent')), ('''" option is set via the executable's command line. This option randomizes the order of test execution.
 ''', 'indent'), ('''Run disabled tests''', 'underlined'), (''':
 ''', ''), ('''When enabled, "''', 'indent'), ('''--gtest_also_run_disabled_tests''', ('fixed', 'indent')), ('''" option is set via the executable's command line. The option enables execution of test suites and individual test cases whose name starts with "''', 'indent'), ('''DISABLED''', ('fixed', 'indent')), ('''".
 ''', 'indent'), ('''The option also affects test case filter and test case selection menus within GtestGui: When the option is not set, entering filter pattern "''', 'indent'), ('''*DISABLED*''', ('fixed', 'indent')), ('''" would raise a warning that it matches no test cases (even if there are some with that name). The drop-down menu below the entry field would no show such names.
 ''', 'indent'), ('''Break on failure''', 'underlined'), (''':
 ''', ''), ('''When enabled, "''', 'indent'), ('''--gtest_break_on_failure''', ('fixed', 'indent')), ('''" option is set via the executable's command line. This will cause SIGTRAP to be sent to the test process upon the first failure. As no debugger is attached, this will cause the process to crash.
-''', 'indent'), ('''When core dumps are enabled in the kernel, the core will be save by GtestGui and can be analyzed via the ''', 'indent'), ('''Extract stack trace from core dump''', ('underlined', 'indent')), (''' command in the result log's context menu. When core dumps are not enabled, this option is probably not very useful.
+''', 'indent'), ('''When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the ''', 'indent'), ('''Extract stack trace from core dump''', ('underlined', 'indent')), (''' command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 ''', 'indent'), ('''Break on exception''', 'underlined'), (''':
-''', ''), ('''When enabled, "''', 'indent'), ('''--gtest_catch_exceptions=0''', ('fixed', 'indent')), ('''" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means the exception causes the process to terminate.
+''', ''), ('''When enabled, "''', 'indent'), ('''--gtest_catch_exceptions=0''', ('fixed', 'indent')), ('''" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means any exception not caught by the test case itself causes the test process to crash due to an unhandled exception.
+''', 'indent'), ('''When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the ''', 'indent'), ('''Extract stack trace from core dump''', ('underlined', 'indent')), (''' command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 ''', 'indent'), ('''Valgrind''', 'underlined'), (''' and ''', ''), ('''Valgrind - 2nd option set''', 'underlined'), (''':
 ''', ''), ('''The two valgrind options serve to run each execution of the test executable under valgrind using the configured command line. Notably, valgrind checks are performed across the complete lifetime of the test process, thus spanning all test cases or test repetitions. Therefore, if for example a memory leak is reported at the end, it cannot be determined which test case caused it (or it may even be caused by interaction of the test sequence.) Therefore valgrind errors are reported with a special entry in the result log. Some kind of errors such as invalid memory accesses can be mapped to test cases based on the position of the error report in the output stream. Note however that the position may not exactly reflect the timing of occurrence due to possible buffering in output streams within the test executable.) See ''', 'indent'), ('''Result log''', ('href', 'indent')), (''' and ''', 'indent'), ('''Configuration''', ('href', 'indent')), (''' for more details.
 ''', 'indent'), )
 
 helpTexts[2] = (('''Result log''', 'title1'), ('''
 ''', ''), ('''The result log frame is located in the middle of the main window. When started for the first time, the log is usually empty. However, results can also be imported via the command line, for example from a file that contains output from a test executable that was redirected into a file. The result log may also show results from a previous run of GtestGui, if auto-import is enabled in ''', ''), ('''Configuration''', 'href'), ('''.
 ''', ''), ('''The result log contains one line for each ''', ''), ('''[ OK ]''', 'fixed'), (''', ''', ''), ('''[ SKIPPED ]''', 'fixed'), (''' and ''', ''), ('''[ FAILED ]''', 'fixed'), (''' line in the test application's gtest-generated output. The test executable's output stream is redirected to a pipe that is read continuously by GtestGui for this purpose. GtestGui also stores this output to a file, so that the trace output between ''', ''), ('''[ RUN ]''', 'fixed'), (''' and verdict text line can be opened in a trace browser.
@@ -103,15 +104,15 @@
 ''', 'indent'), ('''Show test controls''', 'underlined'), (''':
 ''', ''), ('''This option can be unchecked for temporarily hiding the test control frame in the main window. This allows for more space for the result log during result analysis. This option is not stored in persistent configuration and will always be enabled upon start of the application. Note while the controls are not shown, some operations are still possible via key bindings as well as the ''', 'indent'), ('''Control''', ('underlined', 'indent')), (''' menu.
 ''', 'indent'), ('''Show tool-tip popups''', 'underlined'), (''':
 ''', ''), ('''The option can be unchecked to disable display of "tool-tip" popup windows when hovering with the mouse on labels or check-buttons in the main window and dialogs which have such built-in help. Changes of the option are stored in the configuration file, so that it is persistent. This may be useful once you are sufficiently familiar with the tool.
 ''', 'indent'), ('''Test management options''', 'title2'), ('''
 ''', ''), ('''Trace browser''', 'underlined'), ('''
 ''', ''), ('''This entry field selects the external application used for displaying trace files and trace snippets, when double-clicking on an entry in the result log. By default, trace browser ''', 'indent'), ('''trowser.py''', ('underlined', 'indent')), (''' is used. You can either specify just the application file name, or its full path if it is not found via ''', 'indent'), ('''PATH''', ('fixed', 'indent')), (''' configured in environment. The path of the trace file to be displayed will be appended to the given command line.
-''', 'indent'), ('''Currently the application path name or parameters cannot contain space characters, as these are assumed be be separators.
+''', 'indent'), ('''Currently the application path name or parameters cannot contain space characters, as these are assumed to be separators.
 ''', 'indent'), ('''Note for the Windows platform: When using the default of ''', 'indent'), ('''trowser.py''', ('fixed', 'indent')), (''', you may need to insert the Python interpreter in front of "trowser.py", depending on your Python installation. In that case you need to add the full path to where ''', 'indent'), ('''trowser.py''', ('fixed', 'indent')), (''' is installed.
 ''', 'indent'), ('''Enable option ''', 'indent'), ('''Browser supports reading from STDIN''', ('underlined', 'indent')), (''' if the selected trace browser supports reading text from "standard input" via a pipeline. In this case filename "''', 'indent'), ('''-''', ('fixed', 'indent')), ('''" is passed on the command line instead of a file name.  The default browser ''', 'indent'), ('''trowser.py''', ('underlined', 'indent')), (''' supports this. When not enabled, GtestGui has to create temporary files for passing trace snippets to the browser application.
 ''', 'indent'), ('''Pattern for seed''', 'underlined'), ('''
 ''', ''), ('''If a regular expression pattern is specified here, it will be applied to the trace of each test case. The string returned by the first match group (i.e. the first set of capturing parenthesis) will be shown in the corresponding result log as "seed". (This is intended for allowing repeat of a test sequence exactly even for test cases using randomness, by starting their PRNG with the same seed. This is not yet supported however, due to lack of an interface for passing a list of seed values via the GTest command line interface.)
 ''', 'indent'), ('''Directory for trace files''', 'underlined'), ('''
 ''', ''), ('''Specifies the directory where to store temporary files for trace output and core dump files collected from the executable under test. If empty, the current working directory at the time of starting GtestGui is used. Note sub-directories will be created in the given directory for each executable file version. If you want to use the "copy executable" option, the specified directory needs to be in the same filesystem as the executables. If you want to keep core dumps, the directory needs to be in the same filesystem as the working directory (because they will be moved, not copied due to size.)
 ''', 'indent'), ('''Automatically remove trace files of passed tests upon exit''', 'underlined'), ('''
@@ -119,15 +120,15 @@
 ''', 'indent'), ('''Automatically import trace files upon start''', 'underlined'), ('''
 ''', ''), ('''When enabled, all trace files found in sub-directories under the configured trace directory are read after starting GtestGui. Test case results found in the files are shown in the result log window.
 ''', 'indent'), ('''Create copy of executable under test''', 'underlined'), ('''
 ''', ''), ('''When enabled, a copy of the current executable under test is made within the configured trace directory. (Technically, the copy is achieved by creating a so-called "hard link", so that no additional disk space is needed.) This is recommended so that recompiling the executable does not affect the current test run (i.e. compilation may either fail with error "file busy" when tests are running, or tests may crash). This option is required for allowing to extract stack traces from core dump files taken from an older executable version. Note this option may not work when using trace directories in locations such as /tmp on UNIX-like systems, as these usually are configured to disallow executable files for security reasons.
 ''', 'indent'), ('''Valgrind command line''', 'underlined'), ('''
 ''', ''), ('''UNIX only:''', ('underlined', 'indent')), (''' Command lines to use for running test executables when one of the "Valgrind" options in the main window is enabled. The executable name and gtest options will be appended to the given command line.
 ''', 'indent'), ('''There are two separate entry fields, corresponding to the two check-buttons in the main window. This is intended for allowing to configure a configuration variant that runs faster and one that is slower but performs deeper analysis. By default, the command will perform check for memory leaks (notably at end of all test cases, not for individual test cases in a run of multiple tests) and for use of uninitialized memory. The second command line has additional options for tracking the origin of uninitialized memory.
-''', 'indent'), ('''Currently the path or parameters cannot contain space characters, as these are assumed be be separators.
+''', 'indent'), ('''Currently the path or parameters cannot contain space characters, as these are assumed to be separators.
 ''', 'indent'), ('''Valgrind supports --exit-code''', 'underlined'), ('''
 ''', ''), ('''When this option is set, parameter "--error-exitcode=125" will be appended to the given valgrind command lines. This is required for detecting automatically that valgrind found errors during test execution. Only when enabled, result logs will report valgrind errors.
 ''', 'indent'), ('''The debugger used for extracting stack traces from core files (POSIX only) is currently not configurable; It is hard-coded to "''', ''), ('''gdb''', 'fixed'), ('''", which should be somewhere in the ''', ''), ('''PATH''', 'fixed'), (''' configured in environment.
 ''', ''), )
 
 helpTexts[4] = (('''Caveats''', 'title1'), ('''
 ''', ''), ('''This chapter lists notable limitations that are not easy to overcome due to design choices.
```

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/main.py` & `mote-gtest-gui-0.8.1/gtest_gui/main.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/test_db.py` & `mote-gtest-gui-0.8.1/gtest_gui/test_db.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/tk_utils.py` & `mote-gtest-gui-0.8.1/gtest_gui/tk_utils.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/tool_tip_db.py` & `mote-gtest-gui-0.8.1/gtest_gui/tool_tip_db.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/wid_status_line.py` & `mote-gtest-gui-0.8.1/gtest_gui/wid_status_line.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/wid_test_ctrl.py` & `mote-gtest-gui-0.8.1/gtest_gui/wid_test_ctrl.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,18 +332,18 @@
             if len(tc_list) > 1 and (rep_cnt > 1):
                 if max_cnt < min_cnt + 2:
                     return ("%d of %d test case runs\n%d of %d repetitions" %
                             (totals[5], totals[4], min_cnt, rep_cnt))
                 else:
                     return ("%d of %d test case runs\n%d..%d of %d repetitions" %
                             (totals[5], totals[4], min_cnt, max_cnt, rep_cnt))
-            elif len(tc_list) > 1:
-                return "%d of %d test case runs" % (totals[5], totals[4])
-            else:
+            elif rep_cnt > 1:
                 return "%d of %d repetitions" % (min_cnt, rep_cnt)
+            else:
+                return "%d of %d test case runs" % (totals[5], totals[4])
         else:
             return ""
 
 
     def __update_campaign_status(self):
         # Update counters in status frame
         totals = test_db.campaign_stats
```

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/wid_test_log.py` & `mote-gtest-gui-0.8.1/gtest_gui/wid_test_log.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/wid_text_sel.py` & `mote-gtest-gui-0.8.1/gtest_gui/wid_text_sel.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/gtest_gui/wid_tool_tip.py` & `mote-gtest-gui-0.8.1/gtest_gui/wid_tool_tip.py`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/mote_gtest_gui.egg-info/PKG-INFO` & `mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mote-gtest-gui
-Version: 0.8.0
+Version: 0.8.1
 Summary: Module tester's Gtest GUI is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
 Home-page: https://github.com/tomzox/gtest_gui
 Author: T. Zoerner
 Author-email: tomzox@gmail.com
 License: UNKNOWN
 Keywords: google-test,gtest,testing-tools,test-runners,tkinter,GUI
 Platform: posix
@@ -23,50 +23,50 @@
 
 Module-Tester's Gtest GUI
 =========================
 
 Description
 -----------
 
-Module-tester's GtestGui is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
+**Module-tester's GtestGui** is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
 
 The tool will work with any application with Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results, which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
 
 GtestGui typically is started with the path of an executable on the command line which is built using the gtest library. Using the "Run" button in the GUI, this executable can then be started and its progress be monitored live in the result log frame of the main window. Additional controls allow specifying options such as test case filter string and repetition count, which are forwarded to the executable via the respective "\ ``--gtest_*``" command line arguments.
 
-While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with *Trowser*, which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user *trowser.py*, but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening trace snippets.
+While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with *Trowser*, which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user *trowser.py*, but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening traces.
 
 Test control
 ------------
 
 The application main window consists of a menu bar, a frame containing test controls, a frame containing the test result log, and a text frame for trace preview. This chapter describes the top-most frame with the test controls.
 
 Test campaign control buttons
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Most prominent in the test control frame are the green buttons which directly control execution of the configured executable file:
+Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file:
 
 *Run*:
   Starts the text executable in a separate process, with its output redirected into a pipe which is read by GtestGui for progress monitoring. The output is also saved into a file.
 
   Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. Note after adding a new test case, use the *Refresh test case list* command in the *Control* menu to read the test case list, for allowing to use the new test case name in a filter pattern.
 
   Multiple processes are started if the *CPUs* value is larger than 1. Most of the time, GtestGui will use gtest's "sharding" feature, which assigns a static sub-set of tests to each process. However, if repetition count is larger than one and the number of configured CPUs is larger than the number of test cases, or if the remainder of division of test cases by CPUs is large, GtestGui may instead or additionally partition by repetitions.
 
   Note when a test process crashes, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
 
 *Stop*:
   Sends a TERM signal to the test processes and waits for them to finish. When termination takes a long time (possibly because the executable is hung) and the button is clicked a second time, a KILL signal is sent.
 
 *Resume*:
-  Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful in particular when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
+  Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
 
   This command will also use the same version of the test executable as used previously if option *Create copy of executable file* is enabled, see `Configuration`_. This allows resuming execution even when the executable at the configured path no longer exists, for example due to a failed build.
 
-  When resuming, scheduling cannot restart exactly where it was stopped due to limitations in gtest. If repetition count is 1, all test cases will be rescheduled. For higher repetition count, the the lowest number of remaining repetitions across all selected test cases is rescheduled.
+  When resuming, scheduling cannot restart exactly where it was stopped due to limitations in gtest. If repetition count is 1, all test cases will be rescheduled. For higher repetition count, the lowest number of remaining repetitions across all selected test cases is rescheduled.
 
 *Repeat*:
   Repeats the test cases marked manually for repetition via the result log, or all previously failed test cases if none were selected. This allows quick repetition of individual test cases without changing the test case filter.
 
 Test case filter
 ~~~~~~~~~~~~~~~~
 
@@ -108,18 +108,20 @@
   When enabled, "\ ``--gtest_also_run_disabled_tests``" option is set via the executable's command line. The option enables execution of test suites and individual test cases whose name starts with "\ ``DISABLED``".
 
   The option also affects test case filter and test case selection menus within GtestGui: When the option is not set, entering filter pattern "\ ``*DISABLED*``" would raise a warning that it matches no test cases (even if there are some with that name). The drop-down menu below the entry field would no show such names.
 
 *Break on failure*:
   When enabled, "\ ``--gtest_break_on_failure``" option is set via the executable's command line. This will cause SIGTRAP to be sent to the test process upon the first failure. As no debugger is attached, this will cause the process to crash.
 
-  When core dumps are enabled in the kernel, the core will be save by GtestGui and can be analyzed via the *Extract stack trace from core dump* command in the result log's context menu. When core dumps are not enabled, this option is probably not very useful.
+  When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the *Extract stack trace from core dump* command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 
 *Break on exception*:
-  When enabled, "\ ``--gtest_catch_exceptions=0``" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means the exception causes the process to terminate.
+  When enabled, "\ ``--gtest_catch_exceptions=0``" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means any exception not caught by the test case itself causes the test process to crash due to an unhandled exception.
+
+  When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the *Extract stack trace from core dump* command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 
 *Valgrind* and *Valgrind - 2nd option set*:
   The two valgrind options serve to run each execution of the test executable under valgrind using the configured command line. Notably, valgrind checks are performed across the complete lifetime of the test process, thus spanning all test cases or test repetitions. Therefore, if for example a memory leak is reported at the end, it cannot be determined which test case caused it (or it may even be caused by interaction of the test sequence.) Therefore valgrind errors are reported with a special entry in the result log. Some kind of errors such as invalid memory accesses can be mapped to test cases based on the position of the error report in the output stream. Note however that the position may not exactly reflect the timing of occurrence due to possible buffering in output streams within the test executable.) See `Result log`_ and `Configuration`_ for more details.
 
 Result log
 ----------
 
@@ -177,15 +179,15 @@
 
 Test management options
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 *Trace browser*
   This entry field selects the external application used for displaying trace files and trace snippets, when double-clicking on an entry in the result log. By default, trace browser *trowser.py* is used. You can either specify just the application file name, or its full path if it is not found via ``PATH`` configured in environment. The path of the trace file to be displayed will be appended to the given command line.
 
-  Currently the application path name or parameters cannot contain space characters, as these are assumed be be separators.
+  Currently the application path name or parameters cannot contain space characters, as these are assumed to be separators.
 
   Note for the Windows platform: When using the default of ``trowser.py``, you may need to insert the Python interpreter in front of "trowser.py", depending on your Python installation. In that case you need to add the full path to where ``trowser.py`` is installed.
 
   Enable option *Browser supports reading from STDIN* if the selected trace browser supports reading text from "standard input" via a pipeline. In this case filename "\ ``-``" is passed on the command line instead of a file name.  The default browser *trowser.py* supports this. When not enabled, GtestGui has to create temporary files for passing trace snippets to the browser application.
 
 *Pattern for seed*
   If a regular expression pattern is specified here, it will be applied to the trace of each test case. The string returned by the first match group (i.e. the first set of capturing parenthesis) will be shown in the corresponding result log as "seed". (This is intended for allowing repeat of a test sequence exactly even for test cases using randomness, by starting their PRNG with the same seed. This is not yet supported however, due to lack of an interface for passing a list of seed values via the GTest command line interface.)
@@ -203,15 +205,15 @@
   When enabled, a copy of the current executable under test is made within the configured trace directory. (Technically, the copy is achieved by creating a so-called "hard link", so that no additional disk space is needed.) This is recommended so that recompiling the executable does not affect the current test run (i.e. compilation may either fail with error "file busy" when tests are running, or tests may crash). This option is required for allowing to extract stack traces from core dump files taken from an older executable version. Note this option may not work when using trace directories in locations such as /tmp on UNIX-like systems, as these usually are configured to disallow executable files for security reasons.
 
 *Valgrind command line*
   *UNIX only:* Command lines to use for running test executables when one of the "Valgrind" options in the main window is enabled. The executable name and gtest options will be appended to the given command line.
 
   There are two separate entry fields, corresponding to the two check-buttons in the main window. This is intended for allowing to configure a configuration variant that runs faster and one that is slower but performs deeper analysis. By default, the command will perform check for memory leaks (notably at end of all test cases, not for individual test cases in a run of multiple tests) and for use of uninitialized memory. The second command line has additional options for tracking the origin of uninitialized memory.
 
-  Currently the path or parameters cannot contain space characters, as these are assumed be be separators.
+  Currently the path or parameters cannot contain space characters, as these are assumed to be separators.
 
 *Valgrind supports --exit-code*
   When this option is set, parameter "--error-exitcode=125" will be appended to the given valgrind command lines. This is required for detecting automatically that valgrind found errors during test execution. Only when enabled, result logs will report valgrind errors.
 
 The debugger used for extracting stack traces from core files (POSIX only) is currently not configurable; It is hard-coded to "\ ``gdb``", which should be somewhere in the ``PATH`` configured in environment.
 
 Caveats
```

### Comparing `mote-gtest-gui-0.8.0/mote_gtest_gui.egg-info/SOURCES.txt` & `mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.0/setup.py` & `mote-gtest-gui-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                               stdout=subprocess.PIPE, text=True, check=True)
     long_description = proc_rst.stdout
 else:
     long_description = None
 
 setup(
     name='mote-gtest-gui',
-    version='0.8.0',
+    version='0.8.1',
     packages=['gtest_gui'],
     scripts=['bin/gtest_gui'],
 
     install_requires=['trowser'],
 
     author='T. Zoerner',
     author_email='tomzox@gmail.com',
```


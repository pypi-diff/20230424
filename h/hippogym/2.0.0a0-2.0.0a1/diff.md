# Comparing `tmp/hippogym-2.0.0a0.tar.gz` & `tmp/hippogym-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hippogym-2.0.0a0.tar", last modified: Tue Mar  7 06:22:12 2023, max compression
+gzip compressed data, was "hippogym-2.0.0a1.tar", last modified: Mon Apr 24 11:33:40 2023, max compression
```

## Comparing `hippogym-2.0.0a0.tar` & `hippogym-2.0.0a1.tar`

### file list

```diff
@@ -1,103 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.991278 hippogym-2.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.995278 hippogym-2.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/.github/workflows/python-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/.github/workflows/python-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/.github/workflows/python_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/.github/workflows/python_tests_end_to_end.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.995278 hippogym-2.0.0a0/StepFiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/StepFiles/exampleConsent.html
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/StepFiles/exampleQuiz.html
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/StepFiles/exampleSurvey.html
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/StepFiles/exampleThank.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.995278 hippogym-2.0.0a0/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    19099 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/assets/class_diagram.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.995278 hippogym-2.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/docs/UML_class_diagram.uxf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.995278 hippogym-2.0.0a0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/examples/crafting_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/examples/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/examples/lunar_lander.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/examples/minigrid_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/examples/text_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.995278 hippogym-2.0.0a0/img/
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/img/NickNissen.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/img/icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/img/icon_light.png
--rw-r--r--   0 runner    (1001) docker     (123)    46665 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/img/logo_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)    44138 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/img/logo_vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/img/words_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/img/words_vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/requirements-examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.991278 hippogym-2.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.995278 hippogym-2.0.0a0/src/hippogym/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/bucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/communicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/hippogym.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/message_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/src/hippogym/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/recorder/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/recorder/uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/src/hippogym/trialsteps/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/trialsteps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/trialsteps/gymstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/trialsteps/trialstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/src/hippogym/ui_elements/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/src/hippogym/ui_elements/building_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/building_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/building_blocks/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/building_blocks/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/game_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/info_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/text_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/src/hippogym/ui_elements/ui_element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.995278 hippogym-2.0.0a0/src/hippogym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-03-07 06:22:11.000000 hippogym-2.0.0a0/src/hippogym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-03-07 06:22:11.000000 hippogym-2.0.0a0/src/hippogym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 06:22:11.000000 hippogym-2.0.0a0/src/hippogym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-07 06:22:11.000000 hippogym-2.0.0a0/src/hippogym.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-07 06:22:11.000000 hippogym-2.0.0a0/src/hippogym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-07 06:22:11.000000 hippogym-2.0.0a0/src/hippogym.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/tests/end_to_end/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/end_to_end/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/end_to_end/custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/end_to_end/test_crafting.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/end_to_end/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/end_to_end/test_minigrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/end_to_end/test_text_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/fakes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/unit/test_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/unit/test_events_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/unit/test_hippogym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 06:22:11.999278 hippogym-2.0.0a0/tests/unit/ui_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/unit/ui_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/unit/ui_elements/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/unit/ui_elements/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-07 06:21:47.000000 hippogym-2.0.0a0/tests/unit/ui_elements/test_ui_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.812371 hippogym-2.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.816371 hippogym-2.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.github/workflows/python-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.github/workflows/python-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.github/workflows/python_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.github/workflows/python_tests_end_to_end.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.816371 hippogym-2.0.0a1/StepFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/StepFiles/exampleConsent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/StepFiles/exampleQuiz.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/StepFiles/exampleSurvey.html
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/StepFiles/exampleThank.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.816371 hippogym-2.0.0a1/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    19099 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/assets/class_diagram.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.824371 hippogym-2.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/docs/UML_class_diagram.uxf
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/docs/backend_success_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)  6002564 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/docs/lunar_human_demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)  1863460 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/docs/minigrid_human_demo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.824371 hippogym-2.0.0a1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/examples/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/examples/hcraft_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/examples/lunar_lander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/examples/minigrid_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/icon_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46665 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/logo_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44138 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/logo_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/words_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/words_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/requirements-examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.812371 hippogym-2.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/bucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/hippogym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym/trialsteps/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/trialsteps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/trialsteps/gymstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/trialsteps/trialstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym/ui_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/game_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/info_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/text_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/ui_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/tests/end_to_end/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/test_crafting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/test_minigrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/fakes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/test_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/test_events_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/test_hippogym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/tests/unit/ui_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/ui_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/ui_elements/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/ui_elements/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/ui_elements/test_ui_element.py
```

### Comparing `hippogym-2.0.0a0/.github/workflows/python-coverage.yml` & `hippogym-2.0.0a1/.github/workflows/python-coverage.yml`

 * *Files 14% similar despite different names*

```diff
@@ -18,13 +18,13 @@
           pip install .
       - name: Install tests dependencies
         run: |
           pip install -r requirements-dev.txt
           pip install -r requirements-examples.txt
       - name: Build coverage using pytest-cov
         run: |
-          pytest --cov=src --cov-report=xml tests
+          pytest --cov=hippogym --cov-report=xml tests
       - name: Codacy Coverage Reporter
         uses: codacy/codacy-coverage-reporter-action@v1.3.0
         with:
           project-token: ${{ secrets.CODACY_PROJECT_TOKEN }}
           coverage-reports: coverage.xml
```

### Comparing `hippogym-2.0.0a0/.github/workflows/python-pypi.yml` & `hippogym-2.0.0a1/.github/workflows/python-pypi.yml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/.github/workflows/python_tests.yml` & `hippogym-2.0.0a1/.github/workflows/python_tests.yml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/.gitignore` & `hippogym-2.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/LICENSE` & `hippogym-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/StepFiles/exampleConsent.html` & `hippogym-2.0.0a1/StepFiles/exampleConsent.html`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/StepFiles/exampleQuiz.html` & `hippogym-2.0.0a1/StepFiles/exampleQuiz.html`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/StepFiles/exampleSurvey.html` & `hippogym-2.0.0a1/StepFiles/exampleSurvey.html`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/assets/class_diagram.pdf` & `hippogym-2.0.0a1/assets/class_diagram.pdf`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/config.yml` & `hippogym-2.0.0a1/config.yml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/docs/UML_class_diagram.uxf` & `hippogym-2.0.0a1/docs/UML_class_diagram.uxf`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/examples/crafting_example.py` & `hippogym-2.0.0a1/examples/hcraft_example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-""" This examples require to have install the crafting environment.
+""" This examples require to have install the hcraft dependency.
 
 ```bash
-pip install git+https://github.com/IRLL/Crafting.git#egg=crafting
+pip install hcraft[gui]
 ```
 
 """
 
 from copy import copy
 import logging
 from typing import Optional, Tuple
 
 import pygame
 from pygame.event import Event
 from pygame.locals import MOUSEBUTTONDOWN, MOUSEBUTTONUP, MOUSEMOTION
 
-import gym
-from crafting import CraftingEnv
-from crafting.render.human import get_human_action
+from hcraft import HcraftEnv
+from hcraft.render.human import get_human_action
 
 from hippogym import HippoGym, Agent
 from hippogym.trialsteps import GymStep
 
 logging.basicConfig(level=logging.INFO)
 LOGGER = logging.getLogger(__name__)
 
 
-class HumanCraftingAgent(Agent):
+class HumanHCraftAgent(Agent):
     def __init__(self, observation_space=None, action_space=None) -> None:
         self.trialstep: Optional["GymStep"] = None
         self.action = None
         super().__init__(observation_space, action_space)
 
     def message_to_event(self, event_type, event_data) -> Optional[Event]:
         window_size = self.trialstep.render_window.size
@@ -55,23 +54,23 @@
                 rel["xMovement"] / window_size[0],
                 rel["yMovement"] / window_size[1],
             )
             rel_abs = rel_to_abs_coords(*rel_relative)
             return Event(pygame_event_type, pos=pos_abs, rel=rel_abs, button=button)
         return Event(pygame_event_type, pos=pos_abs, button=1)
 
-    def on_mouse_event(self, event_type: "MouseEvent", event_data):
+    def on_mouse_event(self, event_type, event_data):
         # Create fake pygame mouse event
         fake_event = self.message_to_event(event_type, event_data)
 
         if fake_event is None:
             return
 
         # Get action from crafting rendering
-        env: CraftingEnv = self.trialstep.env
+        env: HcraftEnv = self.trialstep.env
         action = get_human_action(
             env,
             additional_events=[fake_event],
             can_be_none=True,
         )
         if action:
             self.action = action
@@ -80,20 +79,15 @@
         if self.action is not None:
             action = copy(self.action)
             self.action = None
             return action
         return self.action
 
 
-class MineCraftingStep(GymStep):
-    def __init__(self, agent, render_mode: str = "rgb_array"):
-        self.score = 0
-        env = gym.make("MineCrafting-v1")
-        super().__init__(env, agent)
-
+class HCraftStep(GymStep):
     def run(self) -> None:
         self.env.reset()
         self.env.render()
         self.render_window.set_size(*pygame_screen_size())
         return super().run()
 
 
@@ -112,17 +106,17 @@
     Returns:
         Tuple[int, int]: Absolute pixel coordinates on the pygame window.
     """
     width, height = pygame_screen_size()
     return int(x_rel * width), int(y_rel * height)
 
 
-def build_experiment(render_mode: str = "rgb_array") -> HippoGym:
-    agent = HumanCraftingAgent()
-    lunarstep = MineCraftingStep(agent, render_mode=render_mode)
+def build_experiment() -> HippoGym:
+    agent = HumanHCraftAgent()
+    lunarstep = HCraftStep("MineHcraft-v1", agent)
     return HippoGym(lunarstep)
 
 
 def main():
     hippo = build_experiment()
     hippo.start()
```

### Comparing `hippogym-2.0.0a0/examples/grid.py` & `hippogym-2.0.0a1/examples/grid.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/examples/lunar_lander.py` & `hippogym-2.0.0a1/examples/lunar_lander.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from copy import copy
 from enum import Enum
 import logging
 
 from hippogym import HippoGym, HumanAgent
 from hippogym.ui_elements import InfoPanel, ControlPanel, standard_controls
 from hippogym.trialsteps import GymStep
+from hippogym.recorder import JsonRecorder
 
 logging.basicConfig(level=logging.INFO)
 LOGGER = logging.getLogger(__name__)
 
 
 class LunarLanderAction(Enum):
     NOOP = 0
@@ -60,57 +60,69 @@
 
     def reset(self):
         self.last_action = self.default_action
         super().reset()
 
 
 class LunarLanderV2Step(GymStep):
-    def __init__(self, agent):
+    def __init__(self, agent, experiment_name: str):
         self.info_panel = InfoPanel(
             text="Use keyboard to play the game",
             items=["s = down", "a = left", "d = right"],
         )
         self.control_panel = ControlPanel(buttons=standard_controls)
+        self.recorder = JsonRecorder(
+            records_path="records", experiment_name=experiment_name
+        )
         self.score = 0
         super().__init__(
             "LunarLander-v2",
             agent,
             ui_elements=[self.info_panel, self.control_panel],
         )
 
     def step(
         self,
+        episode: int,
+        step: int,
         observation,
         action,
         new_observation,
         reward: float,
         done: bool,
         info: dict,
     ) -> None:
+        self.score += reward
 
         if done:
-            self.info_panel.update(key_value={"Score": reward})
+            self.info_panel.update(key_value={"Score": self.score})
+            self.recorder.record(
+                data={
+                    "Episode": episode,
+                    "Score": self.score,
+                },
+                user_id=self.user_id,
+            )
             self.score = 0
             return
 
         observation_msg = ", ".join([f"{x:.2f}" for x in new_observation])
         observation_msg = f"[{observation_msg}]"
-        self.score += reward
         self.info_panel.update(
             key_value={
                 "Score": self.score,
                 "Reward": reward,
                 "Observation": observation_msg,
             },
         )
 
 
 def build_experiment() -> HippoGym:
     agent = HumanAgentToggling()
-    lunarstep = LunarLanderV2Step(agent)
+    lunarstep = LunarLanderV2Step(agent, experiment_name="lunar_human")
     return HippoGym(lunarstep)
 
 
 def main():
     hippo = build_experiment()
     hippo.start()
```

### Comparing `hippogym-2.0.0a0/examples/minigrid_example.py` & `hippogym-2.0.0a1/examples/minigrid_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """ To try this example you must install the minigrid environment
 
 ```bash
-pip install git+https://github.com/Farama-Foundation/Minigrid.git
+pip install gymnasium minigrid
 ```
 
 """
 
 from enum import Enum
 import logging
 
 import gymnasium as gym
 from minigrid.minigrid_env import MiniGridEnv
+from minigrid.core.actions import Actions
 
 from hippogym import HippoGym, HumanAgent
 from hippogym.ui_elements import InfoPanel, ControlPanel, Button
 from hippogym.trialsteps import GymStep
 
 
 logging.basicConfig(level=logging.DEBUG)
@@ -58,22 +59,23 @@
             self.env,
             agent,
             ui_elements=[self.info_panel, self.control_panel],
         )
 
     def step(
         self,
+        episode:int,
+        step:int,
         observation,
         action,
         new_observation,
         reward: float,
         done: bool,
         info: dict,
     ) -> None:
-
         if done:
             self.info_panel.update(key_value={"Score": reward})
             self.score = 0
             return
 
         observation_msg = f"Step={self.env.step_count}, Reward={reward}"
         observation_msg = f"[{observation_msg}]"
@@ -89,33 +91,32 @@
     def send_render(self):
         rgb_frame = self.env.get_frame(tile_size=64, agent_pov=True)
         render = self.render_window.convert_numpy_array_to_base64(rgb_frame)
         self.render_window.update(image=render)
 
 
 def build_experiment() -> HippoGym:
-
     keyboard_to_value = {
         "ArrowRight": HumanValue.RIGHT,
         "ArrowLeft": HumanValue.LEFT,
         "ArrowUp": HumanValue.UP,
         " ": HumanValue.TOGGLE,
         "c": HumanValue.PICKUP,
         "v": HumanValue.DROP,
         "Enter": HumanValue.END,
     }
 
     value_to_action = {
-        HumanValue.LEFT: MiniGridEnv.Actions.left.value,
-        HumanValue.RIGHT: MiniGridEnv.Actions.right.value,
-        HumanValue.UP: MiniGridEnv.Actions.forward.value,
-        HumanValue.TOGGLE: MiniGridEnv.Actions.toggle.value,
-        HumanValue.PICKUP: MiniGridEnv.Actions.pickup.value,
-        HumanValue.DROP: MiniGridEnv.Actions.drop.value,
-        HumanValue.END: MiniGridEnv.Actions.done.value,
+        HumanValue.LEFT: Actions.left.value,
+        HumanValue.RIGHT: Actions.right.value,
+        HumanValue.UP: Actions.forward.value,
+        HumanValue.TOGGLE: Actions.toggle.value,
+        HumanValue.PICKUP: Actions.pickup.value,
+        HumanValue.DROP: Actions.drop.value,
+        HumanValue.END: Actions.done.value,
     }
 
     agent = HumanAgent(HumanValue, value_to_action, keyboard_to_value)
     minigrid = MiniGridStep(agent)
     return HippoGym(minigrid)
```

### Comparing `hippogym-2.0.0a0/img/icon_dark.png` & `hippogym-2.0.0a1/img/icon_dark.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/img/icon_light.png` & `hippogym-2.0.0a1/img/icon_light.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/img/logo_horizontal.png` & `hippogym-2.0.0a1/img/logo_horizontal.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/img/logo_vertical.png` & `hippogym-2.0.0a1/img/logo_vertical.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/img/words_horizontal.png` & `hippogym-2.0.0a1/img/words_horizontal.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/img/words_vertical.png` & `hippogym-2.0.0a1/img/words_vertical.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/pyproject.toml` & `hippogym-2.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/agent.py` & `hippogym-2.0.0a1/src/hippogym/agent.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/bucketer.py` & `hippogym-2.0.0a1/src/hippogym/bucketer.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/communicator.py` & `hippogym-2.0.0a1/src/hippogym/communicator.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/event_handler.py` & `hippogym-2.0.0a1/src/hippogym/event_handler.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/hippogym.py` & `hippogym-2.0.0a1/src/hippogym/hippogym.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
         if user_id in self.trials:
             raise ValueError(f"{user_id=} already in trial")
 
         new_trial_process = Process(
             name="Trial",
             target=trial.build_and_run,
-            args=(in_q, out_q),
+            args=(user_id, in_q, out_q),
         )
 
         self.trials[user_id] = new_trial_process
         self._trial_seed += 1
         new_trial_process.start()
         return in_q, out_q
```

### Comparing `hippogym-2.0.0a0/src/hippogym/log.py` & `hippogym-2.0.0a1/src/hippogym/log.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/message_handler.py` & `hippogym-2.0.0a1/src/hippogym/message_handler.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/trial.py` & `hippogym-2.0.0a1/src/hippogym/trial.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,30 @@
     """A single experiment instance."""
 
     def __init__(self, steps: List["TrialStep"]) -> None:
         self.steps = steps
         self.in_q: Optional[Queue] = None
         self.out_q: Optional[Queue] = None
 
-    def build(self, in_q: Queue, out_q: Queue):
+    def build(self, user_id: str, in_q: Queue, out_q: Queue):
         """Build trial events architecture."""
+        self.user_id = user_id
         self.in_q = in_q
         self.out_q = out_q
 
     def run(self):
         """Run the Trial step by step."""
         for step in self.steps:
             event_handler = EventHandler(self.in_q, self.out_q)
-            step.build(event_handler)
+            step.build(self.user_id, event_handler)
             step.run()
 
-    def build_and_run(self, in_q: Queue, out_q: Queue):
+    def build_and_run(self, user_id: str, in_q: Queue, out_q: Queue):
         """Build then run the Trial step by step."""
-        self.build(in_q, out_q)
+        self.build(user_id, in_q, out_q)
         self.run()
 
 
 class TrialConfig:
     """Configuration to generate independant Trial instances."""
 
     def __init__(self, steps: List["TrialStep"]) -> None:
```

### Comparing `hippogym-2.0.0a0/src/hippogym/trialsteps/gymstep.py` & `hippogym-2.0.0a1/src/hippogym/trialsteps/gymstep.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,30 +36,32 @@
         )
         if ui_elements is None:
             ui_elements = []
         if self.render_window not in ui_elements:
             ui_elements.append(self.render_window)
         super().__init__(ui_elements)
         if isinstance(env, str):
-            env = gym.make(env, render_mode="rgb_array", **kwargs)
+            env = gym.make(env, **kwargs)
         self.env = env
         self.agent = agent
         self.agent.set_spaces(self.env.observation_space, self.env.action_space)
 
         self.stop = False
         self.run_from_start = run_from_start
         self.running = self.run_from_start
 
-    def build(self, event_handler: "EventHandler") -> None:
+    def build(self, user_id: str, event_handler: "EventHandler") -> None:
         """Initialize queues and message handler thread."""
-        super().build(event_handler)
+        super().build(user_id, event_handler)
         self.agent.build(self)
 
     def step(
         self,
+        episode: int,
+        step: int,
         observation: Observation,
         action: Action,
         new_observation: Observation,
         reward: float,
         done: bool,
         info: dict,
     ) -> None:
@@ -75,38 +77,49 @@
         """
 
     def run(self) -> None:
         self.stop = False
         self.running = self.run_from_start
 
         observation, info = self.gym_reset()
+        step = 0
+        episode = 0
 
         while not self.stop:
             self.send_render()
             while self.running:
-
                 action = None
                 while action is None:
                     self.event_handler.trigger_events()
                     action = self.agent.act(observation)
+                    step += 1
 
                 new_observation, reward, terminated, truncated, info = self.gym_step(
                     action
                 )
                 done = terminated or truncated
                 LOGGER.debug("GymStep action was taken: %s. Reward: %f", action, reward)
 
                 self.step(
-                    observation, action, new_observation, reward, terminated, info
+                    episode,
+                    step,
+                    observation,
+                    action,
+                    new_observation,
+                    reward,
+                    terminated,
+                    info,
                 )
 
                 if done:
                     self.stop = True
                     observation, info = self.gym_reset()
                     self.agent.reset()
+                    step = 0
+                    episode += 1
 
                 observation = new_observation
                 self.send_render()
                 time.sleep(0.03)
             time.sleep(1)
         self.env.close()
 
@@ -127,12 +140,14 @@
         if len(reset_data) == 2 and isinstance(reset_data[1], dict):
             return reset_data
         observation = reset_data
         info = {}
         return observation, info
 
     def send_render(self):
-        rgb_array = self.env.render()
-        if not isinstance(rgb_array, np.ndarray):
+        rgb_array = self.env.render(mode="rgb_array")
+        try:
+            rgb_array = np.array(rgb_array)
+        except:
             raise TypeError("Env render should output a numpy array.")
         render = self.render_window.convert_numpy_array_to_base64(rgb_array)
         self.render_window.update(image=render)
```

### Comparing `hippogym-2.0.0a0/src/hippogym/trialsteps/trialstep.py` & `hippogym-2.0.0a1/src/hippogym/trialsteps/trialstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,20 @@
     from hippogym.ui_elements.ui_element import UIElement
 
 
 class TrialStep(ABC):
     """Abstract class for single trial step."""
 
     def __init__(self) -> None:
+        self.user_id = None
         self.event_handler: Optional[EventHandler] = None
 
-    def build(self, event_handler: EventHandler) -> None:
+    def build(self, user_id: str, event_handler: EventHandler) -> None:
         """Build the TrialStep events architecture."""
+        self.user_id = user_id
         self.event_handler = event_handler
 
     @abstractmethod
     def run(self) -> None:
         """Run the trial step"""
 
 
@@ -38,17 +40,17 @@
 class InteractiveStep(TrialStep):
     """A step where user interacts with hippogym UIElements."""
 
     def __init__(self, ui_elements: List["UIElement"]) -> None:
         self.ui_elements: List["UIElement"] = ui_elements
         super().__init__()
 
-    def build(self, event_handler: EventHandler) -> None:
+    def build(self, user_id: str, event_handler: EventHandler) -> None:
         """Initialize multiprocessing queues."""
-        super().build(event_handler)
+        super().build(user_id, event_handler)
         for ui_element in self.ui_elements:
             ui_element.build(self)
         self.send()
 
     def send(self) -> None:
         """Send ui_elements to frontend."""
         for ui_element in self.ui_elements:
```

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/__init__.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/building_blocks/button.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/button.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/building_blocks/slider.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/slider.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/control_panel.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/control_panel.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/game_window.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/game_window.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/grid.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/grid.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/info_panel.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/info_panel.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/text_box.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/text_box.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym/ui_elements/ui_element.py` & `hippogym-2.0.0a1/src/hippogym/ui_elements/ui_element.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/src/hippogym.egg-info/SOURCES.txt` & `hippogym-2.0.0a1/src/hippogym.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 .github/workflows/python_tests_end_to_end.yml
 StepFiles/exampleConsent.html
 StepFiles/exampleQuiz.html
 StepFiles/exampleSurvey.html
 StepFiles/exampleThank.html
 assets/class_diagram.pdf
 docs/UML_class_diagram.uxf
-examples/crafting_example.py
+docs/backend_success_example.png
+docs/lunar_human_demo.gif
+docs/minigrid_human_demo.gif
 examples/grid.py
+examples/hcraft_example.py
 examples/lunar_lander.py
 examples/minigrid_example.py
-examples/text_box.py
-img/NickNissen.jpeg
 img/icon_dark.png
 img/icon_light.png
 img/logo_horizontal.png
 img/logo_vertical.png
 img/words_horizontal.png
 img/words_vertical.png
 src/hippogym/__init__.py
@@ -37,24 +38,22 @@
 src/hippogym/agent.py
 src/hippogym/bucketer.py
 src/hippogym/communicator.py
 src/hippogym/event_handler.py
 src/hippogym/hippogym.py
 src/hippogym/log.py
 src/hippogym/message_handler.py
+src/hippogym/recorder.py
 src/hippogym/trial.py
 src/hippogym.egg-info/PKG-INFO
 src/hippogym.egg-info/SOURCES.txt
 src/hippogym.egg-info/dependency_links.txt
 src/hippogym.egg-info/entry_points.txt
 src/hippogym.egg-info/requires.txt
 src/hippogym.egg-info/top_level.txt
-src/hippogym/recorder/__init__.py
-src/hippogym/recorder/recorder.py
-src/hippogym/recorder/uploader.py
 src/hippogym/trialsteps/__init__.py
 src/hippogym/trialsteps/gymstep.py
 src/hippogym/trialsteps/trialstep.py
 src/hippogym/ui_elements/__init__.py
 src/hippogym/ui_elements/control_panel.py
 src/hippogym/ui_elements/game_window.py
 src/hippogym/ui_elements/grid.py
@@ -67,15 +66,14 @@
 tests/__init__.py
 tests/fakes.py
 tests/end_to_end/__init__.py
 tests/end_to_end/custom_checks.py
 tests/end_to_end/test_crafting.py
 tests/end_to_end/test_grid.py
 tests/end_to_end/test_minigrid.py
-tests/end_to_end/test_text_box.py
 tests/unit/__init__.py
 tests/unit/test_event_handler.py
 tests/unit/test_events_dispatch.py
 tests/unit/test_hippogym.py
 tests/unit/ui_elements/__init__.py
 tests/unit/ui_elements/test_button.py
 tests/unit/ui_elements/test_slider.py
```

### Comparing `hippogym-2.0.0a0/tests/end_to_end/custom_checks.py` & `hippogym-2.0.0a1/tests/end_to_end/custom_checks.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/tests/fakes.py` & `hippogym-2.0.0a1/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/tests/unit/test_event_handler.py` & `hippogym-2.0.0a1/tests/unit/test_event_handler.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/tests/unit/test_events_dispatch.py` & `hippogym-2.0.0a1/tests/unit/test_events_dispatch.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,24 +32,24 @@
         self.uie1 = DummyUIElement("UIE1")
         self.uie2 = DummyUIElement("UIE2")
 
     def test_UIElements_send(self):
         """Anything sent by a UIElement should go in the output queue."""
 
         intstep = DummyInteractiveStep([self.uie1, self.uie2])
-        intstep.build(self.event_handler)
+        intstep.build("dummy_user", self.event_handler)
 
         expected_msgs = {}
         for ui_element in (self.uie1, self.uie2):
             ui_element.send()
             expected_msgs[ui_element.name] = {
                 ui_element.name: {"name": ui_element.name}
             }
 
-        time.sleep(0.1) # Let queue update
+        time.sleep(0.1)  # Let queue update
         messages_recv = []
         while not self.out_q.empty():
             message_recv = self.out_q.get_nowait()
             messages_recv.append(message_recv)
 
         for _, message in expected_msgs.items():
             check.is_in(message, messages_recv)
@@ -57,20 +57,20 @@
     def test_UIElements_recv(self, mocker: MockerFixture):
         """UIElements should recieve messages of topics they are subscribed to."""
 
         self.uie1.emitter.emit = mocker.MagicMock()
         self.uie2.emitter.emit = mocker.MagicMock()
 
         intstep = DummyInteractiveStep([self.uie1])
-        intstep.build(self.event_handler)
+        intstep.build("dummy_user", self.event_handler)
 
         expected_args = ("ui.ButtonEvent", "BUTTONPRESSED", "clickme")
         self.in_q.put({"ButtonEvent": {"BUTTONPRESSED": "clickme"}})
 
-        time.sleep(0.1) # Let queue update
+        time.sleep(0.1)  # Let queue update
         self.event_handler.trigger_events()
 
         assert self.uie1.emitter.emit.called, "UIElement emitter was not called"
 
         check.equal(
             self.uie1.emitter.emit.call_args.args,
             expected_args,
```

### Comparing `hippogym-2.0.0a0/tests/unit/test_hippogym.py` & `hippogym-2.0.0a1/tests/unit/test_hippogym.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/tests/unit/ui_elements/test_button.py` & `hippogym-2.0.0a1/tests/unit/ui_elements/test_button.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/tests/unit/ui_elements/test_slider.py` & `hippogym-2.0.0a1/tests/unit/ui_elements/test_slider.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a0/tests/unit/ui_elements/test_ui_element.py` & `hippogym-2.0.0a1/tests/unit/ui_elements/test_ui_element.py`

 * *Files identical despite different names*


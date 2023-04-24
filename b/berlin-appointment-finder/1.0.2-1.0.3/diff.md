# Comparing `tmp/berlin-appointment-finder-1.0.2.tar.gz` & `tmp/berlin-appointment-finder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berlin-appointment-finder-1.0.2.tar", last modified: Tue Apr 11 08:51:13 2023, max compression
+gzip compressed data, was "berlin-appointment-finder-1.0.3.tar", last modified: Mon Apr 24 09:24:04 2023, max compression
```

## Comparing `berlin-appointment-finder-1.0.2.tar` & `berlin-appointment-finder-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-11 08:51:13.929165 berlin-appointment-finder-1.0.2/
--rw-------   0 nicolas    (501) staff       (20)     1073 2022-01-25 21:16:12.000000 berlin-appointment-finder-1.0.2/LICENSE
--rw-r--r--   0 nicolas    (501) staff       (20)     2358 2023-04-11 08:51:13.928381 berlin-appointment-finder-1.0.2/PKG-INFO
--rw-------   0 nicolas    (501) staff       (20)     1965 2023-04-05 11:56:10.000000 berlin-appointment-finder-1.0.2/README.md
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-11 08:51:13.879540 berlin-appointment-finder-1.0.2/appointments/
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-04-11 08:41:36.000000 berlin-appointment-finder-1.0.2/appointments/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     6729 2023-04-05 14:58:26.000000 berlin-appointment-finder-1.0.2/appointments/appointments.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-11 08:51:13.926106 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)     2358 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      389 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-05 11:21:55.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/not-zip-safe
--rw-r--r--   0 nicolas    (501) staff       (20)       85 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/requires.txt
--rw-r--r--   0 nicolas    (501) staff       (20)       13 2023-04-11 08:51:13.000000 berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/top_level.txt
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-11 08:51:13.926954 berlin-appointment-finder-1.0.2/bin/
--rwxr-xr-x   0 nicolas    (501) staff       (20)     2259 2023-04-05 12:26:04.000000 berlin-appointment-finder-1.0.2/bin/appointments
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-04-11 08:51:13.929367 berlin-appointment-finder-1.0.2/setup.cfg
--rw-r--r--   0 nicolas    (501) staff       (20)      857 2023-04-11 08:49:57.000000 berlin-appointment-finder-1.0.2/setup.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-24 09:24:04.357942 berlin-appointment-finder-1.0.3/
+-rw-------   0 nicolas    (501) staff       (20)     1073 2022-01-25 21:16:12.000000 berlin-appointment-finder-1.0.3/LICENSE
+-rw-r--r--   0 nicolas    (501) staff       (20)     2996 2023-04-24 09:24:04.357245 berlin-appointment-finder-1.0.3/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     2603 2023-04-16 12:00:04.000000 berlin-appointment-finder-1.0.3/README.md
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-24 09:24:04.349013 berlin-appointment-finder-1.0.3/appointments/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-04-11 08:41:36.000000 berlin-appointment-finder-1.0.3/appointments/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     7145 2023-04-24 09:20:58.000000 berlin-appointment-finder-1.0.3/appointments/appointments.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-24 09:24:04.354962 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)     2996 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)      389 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-05 11:21:55.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/not-zip-safe
+-rw-r--r--   0 nicolas    (501) staff       (20)       85 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/requires.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)       13 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-24 09:24:04.355827 berlin-appointment-finder-1.0.3/bin/
+-rwxr-xr-x   0 nicolas    (501) staff       (20)     2259 2023-04-05 12:26:04.000000 berlin-appointment-finder-1.0.3/bin/appointments
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-04-24 09:24:04.358156 berlin-appointment-finder-1.0.3/setup.cfg
+-rw-r--r--   0 nicolas    (501) staff       (20)      857 2023-04-24 09:21:23.000000 berlin-appointment-finder-1.0.3/setup.py
```

### Comparing `berlin-appointment-finder-1.0.2/LICENSE` & `berlin-appointment-finder-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `berlin-appointment-finder-1.0.2/PKG-INFO` & `berlin-appointment-finder-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin-appointment-finder
-Version: 1.0.2
+Version: 1.0.3
 Summary: Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets
 Home-page: https://github.com/nicbou/burgeramt-appointments-websockets
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -14,53 +14,61 @@
 
 This server looks for Bürgeramt appointment every few seconds. You can make it look for any kind of appointment.
 
 This is the code behind All About Berlin's [Bürgeramt appointment finder](https://allaboutberlin.com/tools/appointment-finder).
 
 If this tool helped you, [make a donation](https://allaboutberlin.com/donate). Building things for Berliners is my full time job.
 
+## What this tool does
+
+This tool looks for appointments on service.berlin.de every 3 minutes. When it finds an appointment, it makes a sound. It can be used as a command line tool, or as the backend for a [web-based tool](https://allaboutberlin.com/tools/appointment-finder).
+
+This tool can't book the appointment for you. It can't look for Ausländerbehörde appointments. These features will not be implemented.
+
 ## Setup
 
 ### 1. Install the script
 
 Run this command in your terminal:
 
 ```bash
 # It might be called 'pip3' on your computer
 pip install berlin-appointment-finder
 ```
 
 You need Python 3 on your computer. If you have macOS or Linux, you already have it. If you have Windows, you're on your own.
 
+If you get a `error: legacy-install-feature`, try some of the [solutions listed here](https://sebhastian.com/python-error-legacy-install-failure/). Do not open an issue; the problem is not related to this project.
+
 ### 2. Find the appointment type you need
 
 Pick a service from the [list of services on Berlin.de](https://service.berlin.de/dienstleistungen/), and copy the URL. For example, `https://service.berlin.de/dienstleistung/120686/` for the *[Anmeldung](https://allaboutberlin.com/glossary/Anmeldung)*.
 
 ### 3. Run the script
 
 Run this command and follow the instructions on your screen:
 
 ```bash
 appointments
 ```
 
-The script will check Berlin.de every 3 minutes. When it finds appointments, it lists them. Just keep an eye on the terminal.
+The script will check Berlin.de every 3 minutes. When it finds appointments, it lists them. Just keep an eye on the terminal. It will also emit a sound.
 
 ## Instructions for nerds
 
 This script can be configured with command line arguments or environment variables.
 
 Type `appointments --help` to see available command line arguments.
 
 These are the available environment variables:
 
-    ```bash
-    BOOKING_TOOL_EMAIL=your@email.com
-    BOOKING_TOOL_ID=johnsmith-dev
-    BOOKING_TOOL_URL=https://service.berlin.de/dienstleistung/120686/
-    ```
+```bash
+BOOKING_TOOL_EMAIL=your@email.com
+BOOKING_TOOL_ID=johnsmith-dev
+BOOKING_TOOL_URL=https://service.berlin.de/dienstleistung/120686/
+```
 
 The script broadcasts broadcasts the appointments it finds with websockets. By default, it broadcasts them on port 80.
 
 A Dockerfile is supplied in this repo. It's the same one I use on All About Berlin.
 
 The polling rate is limited to 180 seconds (3 minutes), as required by the Berlin.de IKT-ZMS team (ikt-zms@seninnds.berlin.de).
```

### Comparing `berlin-appointment-finder-1.0.2/README.md` & `berlin-appointment-finder-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,53 +2,61 @@
 
 This server looks for Bürgeramt appointment every few seconds. You can make it look for any kind of appointment.
 
 This is the code behind All About Berlin's [Bürgeramt appointment finder](https://allaboutberlin.com/tools/appointment-finder).
 
 If this tool helped you, [make a donation](https://allaboutberlin.com/donate). Building things for Berliners is my full time job.
 
+## What this tool does
+
+This tool looks for appointments on service.berlin.de every 3 minutes. When it finds an appointment, it makes a sound. It can be used as a command line tool, or as the backend for a [web-based tool](https://allaboutberlin.com/tools/appointment-finder).
+
+This tool can't book the appointment for you. It can't look for Ausländerbehörde appointments. These features will not be implemented.
+
 ## Setup
 
 ### 1. Install the script
 
 Run this command in your terminal:
 
 ```bash
 # It might be called 'pip3' on your computer
 pip install berlin-appointment-finder
 ```
 
 You need Python 3 on your computer. If you have macOS or Linux, you already have it. If you have Windows, you're on your own.
 
+If you get a `error: legacy-install-feature`, try some of the [solutions listed here](https://sebhastian.com/python-error-legacy-install-failure/). Do not open an issue; the problem is not related to this project.
+
 ### 2. Find the appointment type you need
 
 Pick a service from the [list of services on Berlin.de](https://service.berlin.de/dienstleistungen/), and copy the URL. For example, `https://service.berlin.de/dienstleistung/120686/` for the *[Anmeldung](https://allaboutberlin.com/glossary/Anmeldung)*.
 
 ### 3. Run the script
 
 Run this command and follow the instructions on your screen:
 
 ```bash
 appointments
 ```
 
-The script will check Berlin.de every 3 minutes. When it finds appointments, it lists them. Just keep an eye on the terminal.
+The script will check Berlin.de every 3 minutes. When it finds appointments, it lists them. Just keep an eye on the terminal. It will also emit a sound.
 
 ## Instructions for nerds
 
 This script can be configured with command line arguments or environment variables.
 
 Type `appointments --help` to see available command line arguments.
 
 These are the available environment variables:
 
-    ```bash
-    BOOKING_TOOL_EMAIL=your@email.com
-    BOOKING_TOOL_ID=johnsmith-dev
-    BOOKING_TOOL_URL=https://service.berlin.de/dienstleistung/120686/
-    ```
+```bash
+BOOKING_TOOL_EMAIL=your@email.com
+BOOKING_TOOL_ID=johnsmith-dev
+BOOKING_TOOL_URL=https://service.berlin.de/dienstleistung/120686/
+```
 
 The script broadcasts broadcasts the appointments it finds with websockets. By default, it broadcasts them on port 80.
 
 A Dockerfile is supplied in this repo. It's the same one I use on All About Berlin.
 
 The polling rate is limited to 180 seconds (3 minutes), as required by the Berlin.de IKT-ZMS team (ikt-zms@seninnds.berlin.de).
```

### Comparing `berlin-appointment-finder-1.0.2/appointments/appointments.py` & `berlin-appointment-finder-1.0.3/appointments/appointments.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,24 @@
             chime.error()
         return {
             'time': datetime_to_json(datetime.now()),
             'status': 502,
             'message': 'Could not fetch results from Berlin.de - Got connection error.',
             'appointmentDates': [],
         }
+    except asyncio.exceptions.TimeoutError:
+        logger.warning(f"Got Timeout on response from Berlin.de. Checking in {refresh_delay} seconds")
+        if not quiet:
+            chime.error()
+        return {
+            'time': datetime_to_json(datetime.now()),
+            'status': 504,
+            'message': f'Could not fetch results from Berlin.de. - Timeout',
+            'appointmentDates': [],
+        }
     except Exception as err:
         logger.exception("Could not fetch results due to an unexpected error.")
         if not quiet:
             chime.error()
         return {
             'time': datetime_to_json(datetime.now()),
             'status': 500,
```

### Comparing `berlin-appointment-finder-1.0.2/berlin_appointment_finder.egg-info/PKG-INFO` & `berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin-appointment-finder
-Version: 1.0.2
+Version: 1.0.3
 Summary: Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets
 Home-page: https://github.com/nicbou/burgeramt-appointments-websockets
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -14,53 +14,61 @@
 
 This server looks for Bürgeramt appointment every few seconds. You can make it look for any kind of appointment.
 
 This is the code behind All About Berlin's [Bürgeramt appointment finder](https://allaboutberlin.com/tools/appointment-finder).
 
 If this tool helped you, [make a donation](https://allaboutberlin.com/donate). Building things for Berliners is my full time job.
 
+## What this tool does
+
+This tool looks for appointments on service.berlin.de every 3 minutes. When it finds an appointment, it makes a sound. It can be used as a command line tool, or as the backend for a [web-based tool](https://allaboutberlin.com/tools/appointment-finder).
+
+This tool can't book the appointment for you. It can't look for Ausländerbehörde appointments. These features will not be implemented.
+
 ## Setup
 
 ### 1. Install the script
 
 Run this command in your terminal:
 
 ```bash
 # It might be called 'pip3' on your computer
 pip install berlin-appointment-finder
 ```
 
 You need Python 3 on your computer. If you have macOS or Linux, you already have it. If you have Windows, you're on your own.
 
+If you get a `error: legacy-install-feature`, try some of the [solutions listed here](https://sebhastian.com/python-error-legacy-install-failure/). Do not open an issue; the problem is not related to this project.
+
 ### 2. Find the appointment type you need
 
 Pick a service from the [list of services on Berlin.de](https://service.berlin.de/dienstleistungen/), and copy the URL. For example, `https://service.berlin.de/dienstleistung/120686/` for the *[Anmeldung](https://allaboutberlin.com/glossary/Anmeldung)*.
 
 ### 3. Run the script
 
 Run this command and follow the instructions on your screen:
 
 ```bash
 appointments
 ```
 
-The script will check Berlin.de every 3 minutes. When it finds appointments, it lists them. Just keep an eye on the terminal.
+The script will check Berlin.de every 3 minutes. When it finds appointments, it lists them. Just keep an eye on the terminal. It will also emit a sound.
 
 ## Instructions for nerds
 
 This script can be configured with command line arguments or environment variables.
 
 Type `appointments --help` to see available command line arguments.
 
 These are the available environment variables:
 
-    ```bash
-    BOOKING_TOOL_EMAIL=your@email.com
-    BOOKING_TOOL_ID=johnsmith-dev
-    BOOKING_TOOL_URL=https://service.berlin.de/dienstleistung/120686/
-    ```
+```bash
+BOOKING_TOOL_EMAIL=your@email.com
+BOOKING_TOOL_ID=johnsmith-dev
+BOOKING_TOOL_URL=https://service.berlin.de/dienstleistung/120686/
+```
 
 The script broadcasts broadcasts the appointments it finds with websockets. By default, it broadcasts them on port 80.
 
 A Dockerfile is supplied in this repo. It's the same one I use on All About Berlin.
 
 The polling rate is limited to 180 seconds (3 minutes), as required by the Berlin.de IKT-ZMS team (ikt-zms@seninnds.berlin.de).
```

### Comparing `berlin-appointment-finder-1.0.2/bin/appointments` & `berlin-appointment-finder-1.0.3/bin/appointments`

 * *Files identical despite different names*

### Comparing `berlin-appointment-finder-1.0.2/setup.py` & `berlin-appointment-finder-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name='berlin-appointment-finder',
-    version='1.0.2',
+    version='1.0.3',
     description='Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nicbou/burgeramt-appointments-websockets',
     author='Nicolas Bouliane',
     author_email='contact@nicolasbouliane.com',
     license='MIT',
```


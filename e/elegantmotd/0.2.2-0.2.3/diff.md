# Comparing `tmp/elegantmotd-0.2.2.tar.gz` & `tmp/elegantmotd-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegantmotd-0.2.2.tar", max compression
+gzip compressed data, was "elegantmotd-0.2.3.tar", max compression
```

## Comparing `elegantmotd-0.2.2.tar` & `elegantmotd-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      785 2023-04-24 12:09:05.925360 elegantmotd-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1626 2023-04-24 09:49:46.346640 elegantmotd-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-04-24 09:50:20.677486 elegantmotd-0.2.2/src/elegantmotd/__init__.py
--rw-r--r--   0        0        0      212 2023-04-24 08:04:35.982872 elegantmotd-0.2.2/src/elegantmotd/constants.py
--rw-r--r--   0        0        0      845 2023-04-24 09:50:20.670118 elegantmotd-0.2.2/src/elegantmotd/cpu.py
--rw-r--r--   0        0        0     1068 2023-04-24 08:04:35.982872 elegantmotd-0.2.2/src/elegantmotd/disk.py
--rw-r--r--   0        0        0      308 2023-04-24 08:04:35.982872 elegantmotd-0.2.2/src/elegantmotd/load.py
--rw-r--r--   0        0        0      379 2023-04-24 08:04:35.982872 elegantmotd-0.2.2/src/elegantmotd/loggedinusers.py
--rw-r--r--   0        0        0     1468 2023-04-24 08:04:35.982872 elegantmotd-0.2.2/src/elegantmotd/memory.py
--rw-r--r--   0        0        0     2189 2023-04-24 12:08:12.745157 elegantmotd-0.2.2/src/elegantmotd/motd.py
--rw-r--r--   0        0        0      519 2023-04-24 08:04:35.986528 elegantmotd-0.2.2/src/elegantmotd/network.py
--rw-r--r--   0        0        0      291 2023-04-24 08:04:35.987213 elegantmotd-0.2.2/src/elegantmotd/process.py
--rw-r--r--   0        0        0      345 2023-04-24 08:04:35.987213 elegantmotd-0.2.2/src/elegantmotd/sysinfo.py
--rw-r--r--   0        0        0     1455 2023-04-24 08:04:35.987770 elegantmotd-0.2.2/src/elegantmotd/temperature.py
--rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 elegantmotd-0.2.2/setup.py
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 elegantmotd-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      785 2023-04-24 12:12:52.679061 elegantmotd-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1626 2023-04-24 09:49:46.346640 elegantmotd-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 09:50:20.677486 elegantmotd-0.2.3/src/elegantmotd/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-24 08:04:35.982872 elegantmotd-0.2.3/src/elegantmotd/constants.py
+-rw-r--r--   0        0        0      845 2023-04-24 09:50:20.670118 elegantmotd-0.2.3/src/elegantmotd/cpu.py
+-rw-r--r--   0        0        0     1068 2023-04-24 08:04:35.982872 elegantmotd-0.2.3/src/elegantmotd/disk.py
+-rw-r--r--   0        0        0      308 2023-04-24 08:04:35.982872 elegantmotd-0.2.3/src/elegantmotd/load.py
+-rw-r--r--   0        0        0      379 2023-04-24 08:04:35.982872 elegantmotd-0.2.3/src/elegantmotd/loggedinusers.py
+-rw-r--r--   0        0        0     1468 2023-04-24 08:04:35.982872 elegantmotd-0.2.3/src/elegantmotd/memory.py
+-rw-r--r--   0        0        0     2198 2023-04-24 12:12:35.623458 elegantmotd-0.2.3/src/elegantmotd/motd.py
+-rw-r--r--   0        0        0      519 2023-04-24 08:04:35.986528 elegantmotd-0.2.3/src/elegantmotd/network.py
+-rw-r--r--   0        0        0      291 2023-04-24 08:04:35.987213 elegantmotd-0.2.3/src/elegantmotd/process.py
+-rw-r--r--   0        0        0      345 2023-04-24 08:04:35.987213 elegantmotd-0.2.3/src/elegantmotd/sysinfo.py
+-rw-r--r--   0        0        0     1455 2023-04-24 08:04:35.987770 elegantmotd-0.2.3/src/elegantmotd/temperature.py
+-rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 elegantmotd-0.2.3/setup.py
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 elegantmotd-0.2.3/PKG-INFO
```

### Comparing `elegantmotd-0.2.2/pyproject.toml` & `elegantmotd-0.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elegantmotd"
-version = "0.2.2"
+version = "0.2.3"
 authors = ["Emerick Biron <emerick.biron@gmail.com>"]
 readme = "README.md"
 description = "A visually appealing and informative Message of the Day (MOTD) generator for Linux systems."
 homepage = "https://github.com/emerick-biron/elegantmotd"
 repository = "https://github.com/emerick-biron/elegantmotd.git"
 keywords = ["motd", "system", "information", "console", "dashboard"]
 license = "MIT"
```

### Comparing `elegantmotd-0.2.2/README.md` & `elegantmotd-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.2/src/elegantmotd/cpu.py` & `elegantmotd-0.2.3/src/elegantmotd/cpu.py`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.2/src/elegantmotd/disk.py` & `elegantmotd-0.2.3/src/elegantmotd/disk.py`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.2/src/elegantmotd/memory.py` & `elegantmotd-0.2.3/src/elegantmotd/memory.py`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.2/src/elegantmotd/motd.py` & `elegantmotd-0.2.3/src/elegantmotd/motd.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,8 +64,9 @@
     table.add_column("Info", style="bold CYAN")
     table.add_column("Value", style="bold WHITE")
 
     sysinfos = [Load(), Disk(), Memory(), Temperature(), Process(), LoggedInUsers(), Network(), CPU()]
 
     [table.add_row(f"{info}:", sysinfo.infos[info]) for sysinfo in sysinfos for info in sysinfo.infos]
 
-    console.print(table, end="\n\n")
+    console.print(table)
+    console.print()
```

### Comparing `elegantmotd-0.2.2/src/elegantmotd/network.py` & `elegantmotd-0.2.3/src/elegantmotd/network.py`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.2/src/elegantmotd/temperature.py` & `elegantmotd-0.2.3/src/elegantmotd/temperature.py`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.2.2/setup.py` & `elegantmotd-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'rich>=13.3.4,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['elegantmotd = elegantmotd.motd:display']}
 
 setup_kwargs = {
     'name': 'elegantmotd',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'A visually appealing and informative Message of the Day (MOTD) generator for Linux systems.',
     'long_description': '# ElegantMOTD\n\nElegantMOTD is a Python-based Message of the Day (MOTD) generator for displaying system information in a visually\nappealing and informative manner. It works on Linux systems and provides details such as system load, disk usage, memory\nusage, swap usage, temperature, network interfaces, CPU usage, and more.\n\n## Features\n\n- Rich, colorful text-based output.\n- Displays various system information.\n- Customizable display options.\n- Easy to use and integrate into your system.\n\n## Installation\n- Clone this repository:\n```bash\ngit clone https://github.com/yourusername/elegantmotd.git\ncd elegantmotd\n```\n- Create a virtual environment and activate it:\n\n```bash\npython3 -m venv venv\nsource venv/bin/activate\n```\n\n- Install the required dependencies:\n```bash\npoetry build \n```\n\n## Usage\n\nTo display the Message of the Day, run the following command:\n\n```bash\nelegantmotd\n```\n\n## Customization\n\nYou can customize the output by modifying the `motd.py` file and adding or removing system information modules as per your preference. The available modules are:\n\n- Load\n- Disk\n- Memory\n- Temperature\n- Process\n- LoggedInUsers\n- Network\n- CPU\n\nTo add or remove a module, simply add or remove the corresponding import statement and the respective class instance from the `sysinfos` list in the `display()` function.\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n',
     'author': 'Emerick Biron',
     'author_email': 'emerick.biron@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/emerick-biron/elegantmotd',
```

### Comparing `elegantmotd-0.2.2/PKG-INFO` & `elegantmotd-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elegantmotd
-Version: 0.2.2
+Version: 0.2.3
 Summary: A visually appealing and informative Message of the Day (MOTD) generator for Linux systems.
 Home-page: https://github.com/emerick-biron/elegantmotd
 License: MIT
 Keywords: motd,system,information,console,dashboard
 Author: Emerick Biron
 Author-email: emerick.biron@gmail.com
 Requires-Python: >=3.10,<4.0
```


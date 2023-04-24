# Comparing `tmp/yokkaichi-1.2.2.tar.gz` & `tmp/yokkaichi-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.2.2.tar", last modified: Fri Mar 10 22:54:10 2023, max compression
+gzip compressed data, was "yokkaichi-1.3.tar", last modified: Mon Apr 24 16:57:56 2023, max compression
```

## Comparing `yokkaichi-1.2.2.tar` & `yokkaichi-1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-03-10 22:54:10.643539 yokkaichi-1.2.2/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1210 2022-06-23 18:02:35.000000 yokkaichi-1.2.2/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2726 2023-03-10 22:54:10.643539 yokkaichi-1.2.2/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1954 2023-03-10 22:19:25.000000 yokkaichi-1.2.2/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-03-10 22:54:10.643539 yokkaichi-1.2.2/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1407 2023-03-10 22:53:34.000000 yokkaichi-1.2.2/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-03-10 22:54:10.640206 yokkaichi-1.2.2/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2782 2023-03-02 21:12:52.000000 yokkaichi-1.2.2/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     6398 2023-03-06 21:41:52.000000 yokkaichi-1.2.2/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-01-14 23:17:48.000000 yokkaichi-1.2.2/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     7846 2023-03-10 22:53:34.000000 yokkaichi-1.2.2/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-03-10 22:53:34.000000 yokkaichi-1.2.2/yokkaichi/_version.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-03-10 22:54:10.643539 yokkaichi-1.2.2/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2726 2023-03-10 22:54:10.000000 yokkaichi-1.2.2/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      309 2023-03-10 22:54:10.000000 yokkaichi-1.2.2/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-03-10 22:54:10.000000 yokkaichi-1.2.2/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       54 2023-03-10 22:54:10.000000 yokkaichi-1.2.2/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-03-10 22:54:10.000000 yokkaichi-1.2.2/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 16:57:56.282512 yokkaichi-1.3/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.3/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2710 2023-04-24 16:57:56.282512 yokkaichi-1.3/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1954 2023-03-10 22:19:25.000000 yokkaichi-1.3/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-04-24 16:57:56.282512 yokkaichi-1.3/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1389 2023-04-09 23:36:24.000000 yokkaichi-1.3/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 16:57:56.282512 yokkaichi-1.3/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2967 2023-04-09 23:36:24.000000 yokkaichi-1.3/yokkaichi/MasscanScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     6489 2023-04-09 23:36:24.000000 yokkaichi-1.3/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-01-14 23:17:48.000000 yokkaichi-1.3/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     7971 2023-04-09 23:36:24.000000 yokkaichi-1.3/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       20 2023-04-24 16:56:31.000000 yokkaichi-1.3/yokkaichi/_version.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       54 2023-04-09 23:36:24.000000 yokkaichi-1.3/yokkaichi/rich_console.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 16:57:56.282512 yokkaichi-1.3/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2710 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      335 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       50 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.2.2/PKG-INFO` & `yokkaichi-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.2.2
+Version: 1.3
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yokkaichi-1.2.2/README.md` & `yokkaichi-1.3/README.md`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.2.2/setup.py` & `yokkaichi-1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     version=version,
     description="Shodan-like server scanner for Minecraft (formely mcserverscanner)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Oreeeee",
     url="https://github.com/Oreeeee/yokkaichi",
     install_requires=[
-        "colorama",
+        "rich",
         "mcstatus",
         "ip2location",
         "python-masscan",
         "requests",
     ],
     classifiers=[
         "Environment :: Console",
-        "License :: OSI Approved :: The Unlicense (Unlicense)",
+        "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

### Comparing `yokkaichi-1.2.2/yokkaichi/MasscanScan.py` & `yokkaichi-1.3/yokkaichi/MasscanScan.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from .rich_console import console
 from pathlib import Path
-import colorama as clr
 import platform
 import masscan
 import json
 
 
 class MasscanScan:
     def __init__(self, ip_list, port_list, masscan_args, masscan_output):
@@ -42,28 +42,29 @@
 
         return mas_port_list
 
     def save_output(self, masscan_results):
         Path(self.masscan_output).touch()
         with open(self.masscan_output, "w") as f:
             f.write(json.dumps(masscan_results, indent=4))
-        print(
-            clr.Fore.GREEN
-            + f"Saved masscan results to {self.masscan_output}"
-            + clr.Fore.RESET
+        console.print(
+            f"Saved masscan results to [bold cyan]{self.masscan_output}[/bold cyan]",
+            style="green",
         )
 
     def start_scan(self):
-        print(
-            clr.Fore.BLUE
-            + f"Starting masscan with {len(self.ip_list)} entries and {len(self.port_list)} ports"
-            + clr.Fore.RESET
+        console.print(
+            f"Starting masscan with [bold white]{len(self.ip_list)}[/bold white] entries and [bold white]{len(self.port_list)}[/bold white] ports",
+            style="cyan",
         )
         if platform.system() == "Windows":
-            print("If the scanning doesn't work, start this script as admin!")
+            console.print(
+                "If the scanning doesn't work, start this script as admin!",
+                style="bold yellow",
+            )
             self.mas.scan(
                 self.mas_ip_list, ports=self.mas_port_list, arguments=self.masscan_args
             )
         else:
             self.mas.scan(
                 self.mas_ip_list,
                 ports=self.mas_port_list,
@@ -76,16 +77,17 @@
 
         online_ip_amount = len(masscan_results["scan"])
         # Calculate open port amount
         open_port_amount = 0
         for online_ip in masscan_results["scan"]:
             open_port_amount += len(masscan_results["scan"][online_ip])
 
-        print(
-            clr.Fore.GREEN + f"{open_port_amount} ports open on {online_ip_amount} IPs"
+        console.print(
+            f"[bold white]{open_port_amount}[/bold white] ports open on [bold white]{online_ip_amount}[/bold white] IPs",
+            style="green",
         )
 
         # Save the results if provided
         if self.masscan_output != "":
             self.save_output(masscan_results)
 
         return masscan_results
```

### Comparing `yokkaichi-1.2.2/yokkaichi/ServerScan.py` & `yokkaichi-1.3/yokkaichi/ServerScan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Import modules
 from mcstatus import BedrockServer, JavaServer
+from .rich_console import console
 from datetime import datetime
-import colorama as clr
 import IP2Location
 import threading
 import json
 import ast
 
 
 class ServerScan:
@@ -30,23 +30,25 @@
         self.output_file = output_file
 
         self.results = {"server_list": []}
         self.lock = threading.Lock()
 
     def start_scan(self, thread_count):
         if self.ip2location_db_file != "":
-            print(clr.Fore.CYAN + "Loading IP2Location database")
+            console.print("Loading IP2Location database", style="cyan")
             if self.ip2location_cache:
                 self.ip2location_db = IP2Location.IP2Location(
                     self.ip2location_db_file, "SHARED_MEMORY"
                 )
             else:
                 self.ip2location_db = IP2Location.IP2Location(self.ip2location_db_file)
 
-        print(clr.Fore.CYAN + f"Loading {thread_count} threads!")
+        console.print(
+            f"Loading [bold white]{thread_count}[/bold white] threads!", style="cyan"
+        )
 
         thread_list = []
 
         for _ in range(thread_count):
             thread = threading.Thread(target=self.scan_server)
             thread_list.append(thread)
 
@@ -54,15 +56,17 @@
             thread.start()
 
         for thread in thread_list:
             thread.join()
 
         # Show results
         server_count = len(self.results["server_list"])
-        print(clr.Fore.MAGENTA + f"{server_count} servers found")
+        console.print(
+            f"[bold white]{server_count}[/bold white] servers found", style="magenta"
+        )
 
     def scan_server(self):
         # Scan servers from masscan list
         if self.masscan_list != None:
             self.scan_masscan()
         if self.ip_list != None:
             self.scan_ip_list()
@@ -71,70 +75,68 @@
         while True:
             # Select the first IP from the list and get the port list
             with self.lock:
                 try:
                     ip = list(self.masscan_list["scan"].keys())[0]
                 except IndexError:
                     print(
-                        clr.Fore.WHITE
-                        + f"No more IPs in masscan in thread {threading.current_thread().name}"
+                        f"No more IPs in masscan in thread {threading.current_thread().name}"
                     )
                     return
                 ports = []
                 for port_info in self.masscan_list["scan"][ip]:
                     ports.append(port_info["port"])
                 self.masscan_list["scan"].pop(ip)
 
             for port in ports:
                 for server_platform in self.platforms:
                     try:
                         self.check_server(ip, port, server_platform)
                     except Exception:
                         with self.lock:
-                            print(
-                                clr.Fore.RED
-                                + f"[-] {ip}:{port} for {server_platform} is offline!"
+                            console.print(
+                                f"[-] {ip}:{port} for {server_platform} is offline!",
+                                style="red",
                             )
 
     def scan_ip_list(self):
         while True:
-            try:
-                with self.lock:
+            with self.lock:
+                try:
                     ip = self.ip_list[0]
                     self.ip_list.pop(0)
-            except IndexError:
-                print(
-                    clr.Fore.WHITE
-                    + f"No more IPs in IP list in thread {threading.current_thread().name}"
-                )
-                return
+                except IndexError:
+                    print(
+                        f"No more IPs in IP list in thread {threading.current_thread().name}"
+                    )
+                    return
 
             for port in self.ports:
                 for server_platform in self.platforms:
                     try:
                         self.check_server(ip, port, server_platform)
                     except Exception as e:
                         with self.lock:
-                            print(
-                                clr.Fore.RED
-                                + f"[-] {ip}:{port} for {server_platform} is offline!"
+                            console.print(
+                                f"[-] {ip}:{port} for {server_platform} is offline!",
+                                style="red",
                             )
 
     def check_server(self, ip, port, server_platform):
         if server_platform == "Java":
             server_lookup = JavaServer.lookup(f"{ip}:{port}")
         if server_platform == "Bedrock":
             server_lookup = BedrockServer.lookup(f"{ip}:{port}")
 
         # Get player list
         if self.query:
             try:
                 player_list = server_lookup.query().players.names
             except Exception as e:
-                print(clr.Fore.YELLOW + f"[!] Query failed for {ip}:{port}")
+                console.print(f"[!] Query failed for {ip}:{port}", style="yellow")
                 player_list = None
         else:
             player_list = None
 
         server_info = {
             "ip": ip,
             "port": port,
@@ -156,16 +158,16 @@
         if server_platform == "Bedrock":
             server_info["motd"] = server_lookup.status().motd
             server_info["version"] = ""
             server_info["online_players"] = server_lookup.status().players_online
             server_info["max_players"] = server_lookup.status().players_max
 
         with self.lock:
-            print(
-                clr.Fore.GREEN + f"[+] {server_platform} server found at {ip}:{port}!"
+            console.print(
+                f"[+] {server_platform} server found at {ip}:{port}!", style="green"
             )
             self.add_to_file(server_info)
 
     def get_location_data(self, ip):
         if self.ip2location_db_file == "":
             # Return None if the database doesn't exist
             return None
```

### Comparing `yokkaichi-1.2.2/yokkaichi/__main__.py` & `yokkaichi-1.3/yokkaichi/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Import modules
 from .MasscanScan import MasscanScan
 from .ServerScan import ServerScan
 from ._version import __version__
-import colorama as clr
+from .rich_console import console
 import platform
 import argparse
 import requests
 import pathlib
 
 
 def get_country_ips(countries):
@@ -14,15 +14,18 @@
     for country in countries:
         # Download CIDRs for country
         cidr_list = requests.get(
             f"https://raw.githubusercontent.com/herrbischoff/country-ip-blocks/master/ipv4/{country.lower()}.cidr"
         )
         # Check is the country valid
         if cidr_list.text == "404: Not Found":
-            print(clr.Fore.RED + f"{country} is not a proper 2-letter code!")
+            console.print(
+                f"[bold white]{country}[/bold white] is not a proper 2-letter code!",
+                style="red",
+            )
             continue
         # Add IPs to IP list
         for ip in cidr_list.text.splitlines():
             country_ip_list.append(ip)
 
     return country_ip_list
 
@@ -32,26 +35,28 @@
     # Load file
     try:
         with open(ip_list_location, "r") as f:
             ip_list = f.readlines()
             for ip in ip_list:
                 ips.append(ip.strip())
     except FileNotFoundError:
-        print(clr.Back.RED + clr.Fore.WHITE + "ERROR! IP LIST/MASSCAN LIST NOT FOUND!")
+        console.print("ERROR! IP LIST/MASSCAN LIST NOT FOUND!", style="red")
         exit(1)
 
     return ips
 
 
 def parse_port_range(unparsed_args: str) -> list:
     def verify_ints(port: any) -> None:
         try:
             int(port)
         except TypeError:
-            print(clr.Fore.RED + f"Couldn't parse: {port}" + clr.Fore.RESET)
+            console.print(
+                f"Couldn't parse: [bold white]{port}[/bold white]", style="red"
+            )
             exit(1)
 
     ports: list[int] = []
     # Parse all separate port/ranges, separated by commas
     separate_values: list[str] = unparsed_args.split(",")
     # Parse all ranges
     for value in separate_values:
@@ -73,55 +78,51 @@
 
     return list(set(ports))
 
 
 def main():
     if args.show_version:
         # Show the version and exit
-        print(
-            f"yokkaichi {__version__} on {platform.python_implementation()} {platform.python_version()}"
+        console.print(
+            f"yokkaichi [bold cyan]{__version__}[/bold cyan] on [bold cyan]{platform.python_implementation()} {platform.python_version()}[/bold cyan]",
+            style="green",
         )
         exit()
 
-    if platform.system() == "Windows":
-        # Init colorama if on Windows
-        clr.init()
-
     # Check does output file exists
     if pathlib.Path(args.output_file).is_file():
-        if (
-            input(
-                clr.Fore.YELLOW
-                + "Output file exists. Continuing will overwrite this file. Proceed? (y/n) "
-            )
-            == "n"
-        ):
+        console.print(
+            "Output file exists. Continuing will overwrite this file. Proceed? (y/n) ",
+            style="yellow",
+            end="",
+        )
+        if input() == "n":
             exit(0)
     else:
         # Touch the file
         pathlib.Path(args.output_file).touch()
 
     # Check does IP2Location db exist
     if args.ip2location_db != "" and not pathlib.Path(args.ip2location_db).is_file():
-        print(clr.Fore.RED + "This IP2Location DB doesn't exist")
+        console.print("This IP2Location DB doesn't exist", style="bold red")
         exit(1)
 
     ports = parse_port_range(args.ports)
 
     # Add platforms to a list
     platforms = []
     if args.java:
         platforms.append("Java")
     if args.bedrock:
         platforms.append("Bedrock")
 
     if args.ip_list != "":
-        print(clr.Fore.CYAN + "Loading IPs")
+        console.print("Loading IPs", style="cyan")
         ip_list = load_ip_list(args.ip_list)
-        print(clr.Fore.GREEN + f"Loaded {len(ip_list)} IPs")
+        console.print(f"Loaded {len(ip_list)} IPs", style="green")
     else:
         ip_list = None
 
     if args.masscan:
         masscan_ips_from_file = []
         masscan_ips_for_countries = []
         if args.masscan_ip_list != "":
```

### Comparing `yokkaichi-1.2.2/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.3/yokkaichi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.2.2
+Version: 1.3
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


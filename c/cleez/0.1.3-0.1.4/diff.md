# Comparing `tmp/cleez-0.1.3.tar.gz` & `tmp/cleez-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleez-0.1.3.tar", max compression
+gzip compressed data, was "cleez-0.1.4.tar", max compression
```

## Comparing `cleez-0.1.3.tar` & `cleez-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.3/LICENSE
--rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.3/README.rst
--rw-r--r--   0        0        0     3364 2023-04-23 09:08:34.038374 cleez-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.3/src/cleez/__init__.py
--rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.3/src/cleez/actions.py
--rw-r--r--   0        0        0     4666 2023-04-23 08:52:49.436377 cleez-0.1.3/src/cleez/cleez.py
--rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.3/src/cleez/colors.py
--rw-r--r--   0        0        0     1237 2023-04-18 13:52:32.245318 cleez-0.1.3/src/cleez/command.py
--rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.3/src/cleez/exceptions.py
--rw-r--r--   0        0        0     2692 2023-04-17 19:57:10.619068 cleez-0.1.3/src/cleez/help.py
--rw-r--r--   0        0        0    16860 2023-04-23 09:07:58.541193 cleez-0.1.3/src/cleez/testing.py
--rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 cleez-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.4/LICENSE
+-rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.4/README.rst
+-rw-r--r--   0        0        0     3368 2023-04-24 08:39:56.663490 cleez-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.4/src/cleez/__init__.py
+-rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.4/src/cleez/actions.py
+-rw-r--r--   0        0        0     4952 2023-04-24 08:31:13.115187 cleez-0.1.4/src/cleez/cleez.py
+-rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.4/src/cleez/colors.py
+-rw-r--r--   0        0        0     1752 2023-04-24 08:30:16.438456 cleez-0.1.4/src/cleez/command.py
+-rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.4/src/cleez/exceptions.py
+-rw-r--r--   0        0        0     2707 2023-04-24 08:22:54.099009 cleez-0.1.4/src/cleez/help.py
+-rw-r--r--   0        0        0    11768 2023-04-24 08:31:38.016892 cleez-0.1.4/src/cleez/testing.py
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.4/PKG-INFO
```

### Comparing `cleez-0.1.3/LICENSE` & `cleez-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cleez-0.1.3/README.rst` & `cleez-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `cleez-0.1.3/pyproject.toml` & `cleez-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "cleez"
-version = "0.1.3"
+version = "0.1.4"
 homepage = "https://github.com/abilian/cleez"
 description = "Simple class-based CLI framework."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
@@ -23,25 +23,25 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 termcolor = "^2.2.0"
 
 # Temp (for debugging)
 snoop = "^0.4.3"
-click = "^8.1.3"
 
 [tool.poetry.group.dev.dependencies]
 ## Standard cruft
 abilian-devtools = "*"
 
 # Cruft (project templates management)
 cruft = "*"
 toml = "*"
 
 ## /standard cruft
+devtools = "^0.11.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # ---
```

### Comparing `cleez-0.1.3/src/cleez/actions.py` & `cleez-0.1.4/src/cleez/actions.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.3/src/cleez/cleez.py` & `cleez-0.1.4/src/cleez/cleez.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         # self.common_options(args)
         if "_command" not in args:
             self.help_maker.print_help(self)
             sys.exit()  # exit 0 or exit 1 ?
 
         self.call_command(args._command, args)
 
-    def main(self, args, prog_name):
+    def main(self, args, prog_name, **extra):
         return self.run(args)
 
     def scan(self, module_name: str):
         root_module = importlib.import_module(module_name)
         root_module_name = root_module.__name__
         root_path = Path(root_module.__file__).parent  # type: ignore
         for _, module_name, _ in iter_modules([str(root_path)]):
@@ -74,14 +74,20 @@
         if isabstract(command_class):
             return
 
         self.commands.append(command_class(self))
 
     def add_option(self, *args, **kwargs):
         if args and isinstance(args[0], Option):
+            assert (
+                len(args) == 1
+            ), f"Only one option can be added at a time (got {len(args):d})"
+            assert (
+                not kwargs
+            ), "Cannot pass keyword arguments when adding an option object"
             option = args[0]
             self.options.append(option)
         else:
             self.options.append(Option(*args, **kwargs))
 
     #
     # Internal API
@@ -92,17 +98,18 @@
                 return command
         raise KeyError(f"Command {name} not found")
 
     def make_parser(self):
         parser = MyArgParser()
         subparsers = parser.add_subparsers(parser_class=MyArgParser)
 
-        for command in sorted(self.commands, key=lambda c: len(c.name.split(" "))):
-            if " " in command.name:
-                main_cmd, sub_cms = command.name.split(" ")
+        for command in sorted(self.commands, key=len):
+            if command.is_subcommand():
+                main_cmd = command.main_command_name()
+                # sub_cmd = command.subcommand_name()
                 parent_command = self.get_command(main_cmd)
                 if not parent_command.subparsers:
                     raise ParserBuildError(
                         f"Parent command '{main_cmd}' has not subparsers"
                     )
                 command.add_subparser_to(parent_command.subparsers)
             else:
```

### Comparing `cleez-0.1.3/src/cleez/command.py` & `cleez-0.1.4/src/cleez/command.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,28 +24,51 @@
         self.subparsers = None
 
     @abstractmethod
     def run(self, *args, **kwargs):
         raise NotImplementedError
 
     def add_subparser_to(self, subparsers):
-        name = self.name.split(" ")[-1]
+        name = self.split()[-1]
 
         subparser = subparsers.add_parser(name, help=self.__doc__)
         subparser.set_defaults(_command=self)
 
         for argument in self.arguments:
             subparser.add_argument(*argument.args, **argument.kwargs)
 
         for option in self.options:
             subparser.add_argument(*option.args, **option.kwargs)
 
-        if " " not in self.name:
+        if not self.is_subcommand():
             self.subparsers = subparser.add_subparsers()
 
+    def is_subcommand(self):
+        return " " in self.name
+
+    def main_command_name(self):
+        return self.split()[0]
+
+    def subcommand_name(self):
+        return self.split()[1]
+
+    def __len__(self):
+        return len(self.split())
+
+    def split(self):
+        args = self.name.split(" ")
+        assert len(args) in {
+            1,
+            2,
+        }, (
+            "Command name must be composed of one or "
+            "two words (i.e. '<command> <subcommand>')"
+        )
+        return args
+
 
 class Argument:
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
```

### Comparing `cleez-0.1.3/src/cleez/help.py` & `cleez-0.1.4/src/cleez/help.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,18 @@
             print(f"  {blue(option.args[0])}  {option.kwargs['help']}")
         print()
 
     def print_commands(self, commands: list[Command]):
         print(bold("Available commands:"))
 
         commands = self.get_commands(commands)
-        simple_commands = [command for command in commands if " " not in command.name]
-        complex_commands = [command for command in commands if " " in command.name]
+        simple_commands = [
+            command for command in commands if not command.is_subcommand()
+        ]
+        complex_commands = [command for command in commands if command.is_subcommand()]
 
         self.print_simple_commands_help(simple_commands)
         self.print_complex_commands_help(complex_commands)
 
     def print_simple_commands_help(self, commands: list[Command]):
         if not commands:
             return
@@ -53,24 +55,24 @@
             print(f"  {blue(cmd_name)}  {help}")
 
     def print_complex_commands_help(self, commands: list[Command]):
         if not commands:
             return
         max_command_length = max(len(command.name) for command in commands)
         w = max_command_length
-        groups = groupby(commands, lambda command: command.name.split(" ")[0])
+        groups = groupby(commands, lambda command: command.main_command_name())
         for group_name, group in groups:
             print()
             print(f" {green(group_name)}")
 
             for command in group:
                 cmd_name = f"{command.name:<{w}}"
                 help = (command.__doc__ or "").split("\n")[0].strip()
                 print(f"  {blue(cmd_name)}  {help}")
 
     def get_commands(self, commands: list[Command]):
         def sorter(command):
-            return len(command.name.split(" ")), command.name
+            return len(command), command.name
 
         commands = [command for command in commands if command.name]
         commands = [command for command in commands if not command.hide_from_help]
         return sorted(commands, key=sorter)
```

### Comparing `cleez-0.1.3/PKG-INFO` & `cleez-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleez
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple class-based CLI framework.
 Home-page: https://github.com/abilian/cleez
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: snoop (>=0.4.3,<0.5.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Description-Content-Type: text/x-rst
 
 =====
 Cleez
 =====
```


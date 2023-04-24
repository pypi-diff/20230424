# Comparing `tmp/sysrsync-1.1.0.tar.gz` & `tmp/sysrsync-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrsync-1.1.0.tar", max compression
+gzip compressed data, was "sysrsync-1.1.1.tar", max compression
```

## Comparing `sysrsync-1.1.0.tar` & `sysrsync-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1078 2020-03-04 11:23:57.493668 sysrsync-1.1.0/LICENSE
--rw-r--r--   0        0        0     6080 2022-05-29 22:46:43.120632 sysrsync-1.1.0/README.md
--rw-r--r--   0        0        0      443 2022-05-29 22:45:30.459056 sysrsync-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       53 2020-03-04 11:23:57.493668 sysrsync-1.1.0/sysrsync/__init__.py
--rw-r--r--   0        0        0     1798 2022-05-29 22:45:30.459056 sysrsync-1.1.0/sysrsync/command_maker.py
--rw-r--r--   0        0        0      364 2021-09-12 21:08:21.391439 sysrsync-1.1.0/sysrsync/exceptions.py
--rw-r--r--   0        0        0        0 2020-03-04 11:23:57.493668 sysrsync-1.1.0/sysrsync/helpers/__init__.py
--rw-r--r--   0        0        0      850 2021-09-12 21:08:21.391439 sysrsync-1.1.0/sysrsync/helpers/directories.py
--rw-r--r--   0        0        0      485 2021-12-28 20:02:11.822578 sysrsync-1.1.0/sysrsync/helpers/iterators.py
--rw-r--r--   0        0        0     1100 2022-05-29 22:45:30.459056 sysrsync-1.1.0/sysrsync/helpers/rsync.py
--rw-r--r--   0        0        0      760 2022-05-29 22:45:30.459056 sysrsync-1.1.0/sysrsync/runner.py
--rw-r--r--   0        0        0     6995 2022-05-29 22:47:49.816991 sysrsync-1.1.0/setup.py
--rw-r--r--   0        0        0     6706 2022-05-29 22:47:49.817179 sysrsync-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-03-04 11:23:57.493668 sysrsync-1.1.1/LICENSE
+-rw-r--r--   0        0        0     6501 2023-04-24 14:27:42.227836 sysrsync-1.1.1/README.md
+-rw-r--r--   0        0        0      443 2023-04-24 14:27:54.181523 sysrsync-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       53 2020-03-04 11:23:57.493668 sysrsync-1.1.1/sysrsync/__init__.py
+-rw-r--r--   0        0        0     1812 2023-04-24 14:27:42.227836 sysrsync-1.1.1/sysrsync/command_maker.py
+-rw-r--r--   0        0        0      364 2021-09-12 21:08:21.391439 sysrsync-1.1.1/sysrsync/exceptions.py
+-rw-r--r--   0        0        0        0 2020-03-04 11:23:57.493668 sysrsync-1.1.1/sysrsync/helpers/__init__.py
+-rw-r--r--   0        0        0      850 2021-09-12 21:08:21.391439 sysrsync-1.1.1/sysrsync/helpers/directories.py
+-rw-r--r--   0        0        0      485 2021-12-28 20:02:11.822578 sysrsync-1.1.1/sysrsync/helpers/iterators.py
+-rw-r--r--   0        0        0     1100 2022-05-29 23:01:46.680328 sysrsync-1.1.1/sysrsync/helpers/rsync.py
+-rw-r--r--   0        0        0      760 2022-05-29 23:01:46.680328 sysrsync-1.1.1/sysrsync/runner.py
+-rw-r--r--   0        0        0     7423 1970-01-01 00:00:00.000000 sysrsync-1.1.1/setup.py
+-rw-r--r--   0        0        0     7178 1970-01-01 00:00:00.000000 sysrsync-1.1.1/PKG-INFO
```

### Comparing `sysrsync-1.1.0/LICENSE` & `sysrsync-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sysrsync-1.1.0/README.md` & `sysrsync-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sysrsync
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 Simple and safe native rsync wrapper for Python 3
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=gchamon_sysrsync&metric=alert_status)](https://sonarcloud.io/dashboard?id=gchamon_sysrsync)
 
 ## Requirements
 
@@ -147,17 +147,20 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://github.com/plazmakeks"><img src="https://avatars.githubusercontent.com/u/25690073?v=4?s=100" width="100px;" alt=""/><br /><sub><b>plazmakeks</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=plazmakeks" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/plazmakeks"><img src="https://avatars.githubusercontent.com/u/25690073?v=4?s=100" width="100px;" alt="plazmakeks"/><br /><sub><b>plazmakeks</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=plazmakeks" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://stevehenderson.github.io/"><img src="https://avatars.githubusercontent.com/u/2936416?v=4?s=100" width="100px;" alt="Steve Henderson"/><br /><sub><b>Steve Henderson</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=stevehenderson" title="Code">💻</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `sysrsync-1.1.0/sysrsync/command_maker.py` & `sysrsync-1.1.1/sysrsync/command_maker.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     source, destination = sanitize_trailing_slash(source, destination, sync_source_contents)
 
     exclusions_options = (get_exclusions(exclusions)
                           if exclusions
                           else [])
 
     rsh = (get_rsh_command(private_key, rsh_port, strict_host_key_checking)
-           if any((private_key, rsh_port, strict_host_key_checking))
+           if any((private_key, rsh_port, (strict_host_key_checking is not None)))
            else [])
 
     if options is None:
         options = []
 
     return ['rsync',
             *options,
```

### Comparing `sysrsync-1.1.0/sysrsync/helpers/directories.py` & `sysrsync-1.1.1/sysrsync/helpers/directories.py`

 * *Files identical despite different names*

### Comparing `sysrsync-1.1.0/sysrsync/helpers/rsync.py` & `sysrsync-1.1.1/sysrsync/helpers/rsync.py`

 * *Files identical despite different names*

### Comparing `sysrsync-1.1.0/sysrsync/runner.py` & `sysrsync-1.1.1/sysrsync/runner.py`

 * *Files identical despite different names*

### Comparing `sysrsync-1.1.0/setup.py` & `sysrsync-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['toml>=0.10.0,<0.11.0']
 
 setup_kwargs = {
     'name': 'sysrsync',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'Simple and safe python wrapper for calling system rsync',
-    'long_description': '# sysrsync\n<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->\n[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)\n<!-- ALL-CONTRIBUTORS-BADGE:END -->\nSimple and safe native rsync wrapper for Python 3\n\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=gchamon_sysrsync&metric=alert_status)](https://sonarcloud.io/dashboard?id=gchamon_sysrsync)\n\n## Requirements\n\n* rsync\n* python 3.6+\n\n**development**:\n\n* poetry (be sure to have both poetry and pip upgraded to the latest version)\n\n## Installation\n\n`pip install sysrsync`\n\n## Basic rules\n\n- Syncs source contents by default, so it adds a trailing slash to the end of source, unless `sync_source_contents=False` is specified\n- Removes trailing slash from destination\n- Extra arguments are put right after `rsync`\n- Breaks if `source_ssh` and `destination_ssh` are both set\n\n## Usage\n\n* Basic file sync\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/foo.txt\',\n             destination=\'/home/server/bar\')\n# runs \'rsync /home/users/foo.txt /home/server/files\'\n```\n\n* sync whole folder\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/\',\n             sync_source_contents=False)\n# runs \'rsync /home/user/files /home/server\'\n```\n\n* sync folder contents\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/\',\n             sync_source_contents=True)\n# runs \'rsync /home/user/files/ /home/server\'\n```\n\n* ssh with options\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/files\',\n             destination_ssh=\'myserver\',\n             options=[\'-a\'])\n# runs \'rsync -a /home/users/files/ myserver:/home/server/files\'\n```\n\n* exclusions\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/files\',\n             destination_ssh=\'myserver\',\n             options=[\'-a\'],\n             exclusions=[\'file_to_exclude\', \'unwanted_file\'])\n# runs \'rsync -a /home/user/files/ myserver:/home/server/files --exclude file_to_exclude --exclude unwanted_file\'\n```\n* Private key\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/files\',\n             destination_ssh=\'myserver\',\n             private_key="totally_secure_key")\n# runs \'rsync --rsh=\'ssh -i totally_secure_key\' /home/user/files/ myserver:/home/server/files\'\n```\n\n## API\n\n`sysrsync.run`\n\n| argument  | type | default | description |\n| --------- | ---- | ------- | ----------- |\n| cwd  | str  | `os.getcwd()` | working directory in which subprocess will run the rsync command |\n| strict  | bool | `True` | raises `RsyncError` when rsync return code is different than 0  |\n| verbose | bool | `False` | verbose mode: currently prints rsync command before executing |\n| **kwargs | dict | Not Applicable | arguments that will be forwarded to call to `sysrsync.get_rsync_command` |\n\n**returns**: `subprocess.CompletedProcess`\n\n**raises**:\n- `RsyncError` when `strict = True` and rsync return code is different than 0 ([Success](https://lxadm.com/Rsync_exit_codes#List_of_standard_rsync_exit_codes))\n\n`sysrsync.get_rsync_command`\n\n| argument  | type | default | description |\n| --------- | ---- | ------- | ----------- |\n| source | str | - | Source folder or file |\n| destination | str | - | Destination folder |\n| source_ssh | Optional[str] | None | Remote ssh client where source is located |\n| destination_ssh | Optional[str] | None | Remote ssh client where destination is located |\n| exclusions | Optional[Iterable[str]] | None | List of excluded patterns as in rsync\'s `--exclude` |\n| sync_source_contents | bool | True | Abstracts the elusive trailing slash behaviour that `source` normally has when using rsync directly, i.e. when a trailing slash is present in `source`, the folder\'s content is synchronized with destination. When no trailing slash is present, the folder itself is synchronized with destination. |\n| options | Optional[Iterable[str]] | None | List of options to be used right after rsync call, e.g. `[\'-a\', \'-v\']` translates to `rsync -a -v` |\n| private_key | Optional[str] | None | Configures an explicit key to be used with rsync --rsh command |\n| rsh_port |\xa0Optional[int] | None | Specify port to be used for --rsh command |\n| strict_host_key_checking | Optional[bool] | None | set StrictHostKeyChecking property for rsh #cf. https://superuser.com/questions/125324/how-can-i-avoid-sshs-host-verification-for-known-hosts |\n\n**returns**: `List[str]` -> the compiled list of commands to be used directly in `subprocess.run`\n\n**raises**:\n- `RemotesError` when both `source_ssh` and `destination_ssh` are set. Normally linux rsync distribution disallows source and destination to be both remotes.\n- `PrivateKeyError` when `private_key` doesn\'t exist\n\n# Contributing\n\n- Fork project\n- Install dependencies with `poetry install`\n- Make changes\n- Lint with `poetry run pylint ./sysrsync`\n- Test with `poetry run python -m unittest`\n- Run end-to-end tests with `bash end-to-end-tests/run-tests.sh`\n- Submit changes with a pull request\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://github.com/plazmakeks"><img src="https://avatars.githubusercontent.com/u/25690073?v=4?s=100" width="100px;" alt=""/><br /><sub><b>plazmakeks</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=plazmakeks" title="Code">💻</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n',
+    'long_description': '# sysrsync\n<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->\n[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)\n<!-- ALL-CONTRIBUTORS-BADGE:END -->\nSimple and safe native rsync wrapper for Python 3\n\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=gchamon_sysrsync&metric=alert_status)](https://sonarcloud.io/dashboard?id=gchamon_sysrsync)\n\n## Requirements\n\n* rsync\n* python 3.6+\n\n**development**:\n\n* poetry (be sure to have both poetry and pip upgraded to the latest version)\n\n## Installation\n\n`pip install sysrsync`\n\n## Basic rules\n\n- Syncs source contents by default, so it adds a trailing slash to the end of source, unless `sync_source_contents=False` is specified\n- Removes trailing slash from destination\n- Extra arguments are put right after `rsync`\n- Breaks if `source_ssh` and `destination_ssh` are both set\n\n## Usage\n\n* Basic file sync\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/foo.txt\',\n             destination=\'/home/server/bar\')\n# runs \'rsync /home/users/foo.txt /home/server/files\'\n```\n\n* sync whole folder\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/\',\n             sync_source_contents=False)\n# runs \'rsync /home/user/files /home/server\'\n```\n\n* sync folder contents\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/\',\n             sync_source_contents=True)\n# runs \'rsync /home/user/files/ /home/server\'\n```\n\n* ssh with options\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/files\',\n             destination_ssh=\'myserver\',\n             options=[\'-a\'])\n# runs \'rsync -a /home/users/files/ myserver:/home/server/files\'\n```\n\n* exclusions\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/files\',\n             destination_ssh=\'myserver\',\n             options=[\'-a\'],\n             exclusions=[\'file_to_exclude\', \'unwanted_file\'])\n# runs \'rsync -a /home/user/files/ myserver:/home/server/files --exclude file_to_exclude --exclude unwanted_file\'\n```\n* Private key\n\n```python\nimport sysrsync\n\nsysrsync.run(source=\'/home/user/files\',\n             destination=\'/home/server/files\',\n             destination_ssh=\'myserver\',\n             private_key="totally_secure_key")\n# runs \'rsync --rsh=\'ssh -i totally_secure_key\' /home/user/files/ myserver:/home/server/files\'\n```\n\n## API\n\n`sysrsync.run`\n\n| argument  | type | default | description |\n| --------- | ---- | ------- | ----------- |\n| cwd  | str  | `os.getcwd()` | working directory in which subprocess will run the rsync command |\n| strict  | bool | `True` | raises `RsyncError` when rsync return code is different than 0  |\n| verbose | bool | `False` | verbose mode: currently prints rsync command before executing |\n| **kwargs | dict | Not Applicable | arguments that will be forwarded to call to `sysrsync.get_rsync_command` |\n\n**returns**: `subprocess.CompletedProcess`\n\n**raises**:\n- `RsyncError` when `strict = True` and rsync return code is different than 0 ([Success](https://lxadm.com/Rsync_exit_codes#List_of_standard_rsync_exit_codes))\n\n`sysrsync.get_rsync_command`\n\n| argument  | type | default | description |\n| --------- | ---- | ------- | ----------- |\n| source | str | - | Source folder or file |\n| destination | str | - | Destination folder |\n| source_ssh | Optional[str] | None | Remote ssh client where source is located |\n| destination_ssh | Optional[str] | None | Remote ssh client where destination is located |\n| exclusions | Optional[Iterable[str]] | None | List of excluded patterns as in rsync\'s `--exclude` |\n| sync_source_contents | bool | True | Abstracts the elusive trailing slash behaviour that `source` normally has when using rsync directly, i.e. when a trailing slash is present in `source`, the folder\'s content is synchronized with destination. When no trailing slash is present, the folder itself is synchronized with destination. |\n| options | Optional[Iterable[str]] | None | List of options to be used right after rsync call, e.g. `[\'-a\', \'-v\']` translates to `rsync -a -v` |\n| private_key | Optional[str] | None | Configures an explicit key to be used with rsync --rsh command |\n| rsh_port |\xa0Optional[int] | None | Specify port to be used for --rsh command |\n| strict_host_key_checking | Optional[bool] | None | set StrictHostKeyChecking property for rsh #cf. https://superuser.com/questions/125324/how-can-i-avoid-sshs-host-verification-for-known-hosts |\n\n**returns**: `List[str]` -> the compiled list of commands to be used directly in `subprocess.run`\n\n**raises**:\n- `RemotesError` when both `source_ssh` and `destination_ssh` are set. Normally linux rsync distribution disallows source and destination to be both remotes.\n- `PrivateKeyError` when `private_key` doesn\'t exist\n\n# Contributing\n\n- Fork project\n- Install dependencies with `poetry install`\n- Make changes\n- Lint with `poetry run pylint ./sysrsync`\n- Test with `poetry run python -m unittest`\n- Run end-to-end tests with `bash end-to-end-tests/run-tests.sh`\n- Submit changes with a pull request\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/plazmakeks"><img src="https://avatars.githubusercontent.com/u/25690073?v=4?s=100" width="100px;" alt="plazmakeks"/><br /><sub><b>plazmakeks</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=plazmakeks" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://stevehenderson.github.io/"><img src="https://avatars.githubusercontent.com/u/2936416?v=4?s=100" width="100px;" alt="Steve Henderson"/><br /><sub><b>Steve Henderson</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=stevehenderson" title="Code">💻</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n',
     'author': 'Gabriel Chamon',
     'author_email': 'gchamon@live.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/gchamon/sysrsync',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `sysrsync-1.1.0/PKG-INFO` & `sysrsync-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: sysrsync
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple and safe python wrapper for calling system rsync
 Home-page: https://github.com/gchamon/sysrsync
 Author: Gabriel Chamon
 Author-email: gchamon@live.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: toml (>=0.10.0,<0.11.0)
 Description-Content-Type: text/markdown
 
 # sysrsync
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 Simple and safe native rsync wrapper for Python 3
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=gchamon_sysrsync&metric=alert_status)](https://sonarcloud.io/dashboard?id=gchamon_sysrsync)
 
 ## Requirements
 
@@ -164,17 +165,20 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://github.com/plazmakeks"><img src="https://avatars.githubusercontent.com/u/25690073?v=4?s=100" width="100px;" alt=""/><br /><sub><b>plazmakeks</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=plazmakeks" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/plazmakeks"><img src="https://avatars.githubusercontent.com/u/25690073?v=4?s=100" width="100px;" alt="plazmakeks"/><br /><sub><b>plazmakeks</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=plazmakeks" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://stevehenderson.github.io/"><img src="https://avatars.githubusercontent.com/u/2936416?v=4?s=100" width="100px;" alt="Steve Henderson"/><br /><sub><b>Steve Henderson</b></sub></a><br /><a href="https://github.com/gchamon/sysrsync/commits?author=stevehenderson" title="Code">💻</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```


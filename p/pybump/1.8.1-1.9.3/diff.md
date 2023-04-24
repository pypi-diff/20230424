# Comparing `tmp/pybump-1.8.1-py3-none-any.whl.zip` & `tmp/pybump-1.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 21070 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-05 13:16 src/__init__.py
--rw-r--r--  2.0 unx    24845 b- defN 22-Mar-05 13:16 src/pybump.py
--rw-r--r--  2.0 unx     2806 b- defN 22-Mar-05 13:16 test/__init__.py
--rw-r--r--  2.0 unx    12354 b- defN 22-Mar-05 13:16 test/test_pybump.py
--rw-r--r--  2.0 unx    10792 b- defN 22-Mar-05 13:16 test/test_pybump_patch_validator.py
--rw-r--r--  2.0 unx    15185 b- defN 22-Mar-05 13:16 test/test_simulate_pybump.py
--rw-r--r--  2.0 unx    10759 b- defN 22-Mar-05 13:16 pybump-1.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4521 b- defN 22-Mar-05 13:16 pybump-1.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Mar-05 13:16 pybump-1.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 22-Mar-05 13:16 pybump-1.8.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 22-Mar-05 13:16 pybump-1.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      944 b- defN 22-Mar-05 13:16 pybump-1.8.1.dist-info/RECORD
-12 files, 82351 bytes uncompressed, 19498 bytes compressed:  76.3%
+Zip file size: 22317 bytes, number of entries: 14
+-rw-r--r--  2.0 unx        0 b- defN 22-Nov-12 13:18 src/__init__.py
+-rw-r--r--  2.0 unx    12821 b- defN 22-Nov-12 13:18 src/pybump.py
+-rw-r--r--  2.0 unx     8067 b- defN 22-Nov-12 13:18 src/pybump_patch.py
+-rw-r--r--  2.0 unx     5201 b- defN 22-Nov-12 13:18 src/pybump_version.py
+-rw-r--r--  2.0 unx     3013 b- defN 22-Nov-12 13:18 test/__init__.py
+-rw-r--r--  2.0 unx    12354 b- defN 22-Nov-12 13:18 test/test_pybump.py
+-rw-r--r--  2.0 unx    11292 b- defN 22-Nov-12 13:18 test/test_pybump_patch_validator.py
+-rw-r--r--  2.0 unx    15185 b- defN 22-Nov-12 13:18 test/test_simulate_pybump.py
+-rw-r--r--  2.0 unx    10759 b- defN 22-Nov-12 13:18 pybump-1.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3991 b- defN 22-Nov-12 13:18 pybump-1.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Nov-12 13:18 pybump-1.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 22-Nov-12 13:18 pybump-1.9.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 22-Nov-12 13:18 pybump-1.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1098 b- defN 22-Nov-12 13:18 pybump-1.9.3.dist-info/RECORD
+14 files, 83925 bytes uncompressed, 20513 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,37 +1,43 @@
 Filename: src/__init__.py
 Comment: 
 
 Filename: src/pybump.py
 Comment: 
 
+Filename: src/pybump_patch.py
+Comment: 
+
+Filename: src/pybump_version.py
+Comment: 
+
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_pybump.py
 Comment: 
 
 Filename: test/test_pybump_patch_validator.py
 Comment: 
 
 Filename: test/test_simulate_pybump.py
 Comment: 
 
-Filename: pybump-1.8.1.dist-info/LICENSE
+Filename: pybump-1.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: pybump-1.8.1.dist-info/METADATA
+Filename: pybump-1.9.3.dist-info/METADATA
 Comment: 
 
-Filename: pybump-1.8.1.dist-info/WHEEL
+Filename: pybump-1.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: pybump-1.8.1.dist-info/entry_points.txt
+Filename: pybump-1.9.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pybump-1.8.1.dist-info/top_level.txt
+Filename: pybump-1.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pybump-1.8.1.dist-info/RECORD
+Filename: pybump-1.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/pybump.py

```diff
@@ -1,352 +1,22 @@
 import argparse
 import os
 import re
 from sys import stderr
 
 import yaml
 from pkg_resources import get_distribution, DistributionNotFound
+try:
+    from .pybump_version import PybumpVersion
+except ImportError:
+    from pybump_version import PybumpVersion
 
 regex_version_pattern = re.compile(r"((?:__)?version(?:__)? ?= ?[\"'])(.+?)([\"'])")
 
 
-class PybumpVersion(object):
-
-    def __init__(self, version):
-        self.__prefix = False
-        self.__version = [0, 0, 0]
-        self.__release = None
-        self.__metadata = None
-        self.__valid_sem_ver = False
-        self.__invalid_version = None
-        self.validate_semantic_string(version)
-
-    def validate_semantic_string(self, version):
-        """
-        init the PybumpVersion object by getting a plain text version string,
-        init will check if input string is a semantic version
-        semver defined here: https://github.com/semver/semver/blob/master/semver.md,
-        The version is allowed a lower case 'v' character.
-        search a match according to the regular expression, so for example '1.1.2-prerelease+meta' is valid,
-        then make sure there is and exact single match and validate if each of x,y,z is an integer.
-
-        in case a non valid version passed, 'valid_sem_ver' will stay False
-
-        :param version: string
-        """
-        orig_version = version
-        # only if passed version is non empty string
-        if type(version) == str and len(version) != 0:
-            # In case the version if of type 'v2.2.5' then save 'v' prefix and cut it for further 'semver' validation
-            if version[0] == 'v':
-                version = version[1:]
-                self.__prefix = True
-
-            semver_regex = re.compile(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)"  # Match x.y.z
-                                      # Match -sometext-12.here
-                                      r"(?:-((?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)"
-                                      r"(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?"
-                                      # Match +more.123.here
-                                      r"(?:\+([0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$")
-            # returns a list of tuples, for example [('2', '2', '7', 'alpha', '')]
-            match = semver_regex.findall(version)
-
-            # if there was no match using 'semver_regex', then empty list returned
-            if len(match) != 0:
-                try:
-                    self.__version = [int(n) for n in match[0][:3]]
-
-                    self.__release = match[0][3]
-                    self.__metadata = match[0][4]
-
-                    self.__valid_sem_ver = True
-                    self.__invalid_version = None
-                    return True
-                except ValueError:
-                    pass
-        self.__valid_sem_ver = False
-        self.__invalid_version = orig_version
-        return False
-
-    @property
-    def version(self):
-        return self.__version
-
-    @property
-    def prefix(self):
-        return self.__prefix
-
-    @property
-    def release(self):
-        return self.__release
-
-    @release.setter
-    def release(self, value):
-        self.__release = value
-        # re validate that updated version with new release is still valid
-        self.validate_semantic_string(self.__str__())
-
-    @property
-    def metadata(self):
-        return self.__metadata
-
-    @metadata.setter
-    def metadata(self, value):
-        # re validate that updated version with new metadata is still valid
-        self.__metadata = value
-        self.validate_semantic_string(self.__str__())
-
-    @property
-    def invalid_version(self):
-        return self.__invalid_version
-
-    def __str__(self):
-        """
-        reconstruct version to string, if releases or metadata passed, override the one that is part of object
-        :return: string
-        """
-        result_string = ''
-        if self.prefix:
-            result_string = 'v'
-        result_string += '.'.join(str(x) for x in self.__version)
-
-        if self.release:
-            result_string += '-' + self.release
-
-        if self.metadata:
-            result_string += '+' + self.metadata
-
-        return result_string
-
-    def bump_version(self, level):
-        """
-        Perform ++1 action on the array [x, y, z] cell,
-        :param level: string represents major|minor|patch
-        :return: int array with new value
-        """
-        if level == 'major':
-            self.__version[0] += 1
-            self.__version[1] = 0
-            self.__version[2] = 0
-        elif level == 'minor':
-            self.__version[1] += 1
-            self.__version[2] = 0
-        elif level == 'patch':
-            self.__version[2] += 1
-        else:
-            raise ValueError("Error, invalid level: '{}', "
-                             "should be major|minor|patch.".format(level))
-
-        return self.__version
-
-    def is_larger_then(self, other_version):
-        """
-        return True if current version is higher the 'other',
-        :param other_version: PybumpVersion object
-        :return: boolean
-        """
-        return self.__version > other_version.version
-
-    def is_valid_semantic_version(self):
-        return self.__valid_sem_ver
-
-    def print_invalid_version(self):
-        print("Invalid semantic version format: {}\n"
-              "Make sure to comply with https://semver.org/ "
-              "(lower case 'v' prefix is allowed)".format(self.__invalid_version),
-              file=stderr)
-
-
-class PybumpPatchableVersion(object):
-    def __init__(self, package_name, version):
-        self.__package_name = package_name
-        self.__version = version
-        self.patchable = False
-        self.latest_patch = None
-
-    @property
-    def package_name(self):
-        return self.__package_name
-
-    @property
-    def version(self):
-        return self.__version
-
-    def identify_possible_patch(self, releases_list):
-        """
-        check if there is a possible patch version (in releases_list) newer then self.__version,
-        get list of semantic versions, for example ['0.1.2', '0.1.3', '0.3.1', '0.3.2']
-
-        :param releases_list: list of strings
-        """
-        if not releases_list:
-            raise ValueError('releases_list cannot be empty')
-
-        # assume self.__version is the latest version
-        latest_patch_version = self.__version
-
-        for release in releases_list:
-            release_patch_candidate = PybumpVersion(release)
-
-            if not release_patch_candidate.is_valid_semantic_version():
-                # current 'release' does not meet semantic version, skip
-                continue
-
-            # check if version_to_patch is patchable
-            if not self.is_patchable(release_patch_candidate.version, self.__version.version):
-                continue
-
-            # at this point possible patch version found, so if version_to_patch is [0, 3, 1],
-            # and current iteration over releases_list is [0, 3, 2] then it matches for a patch,
-            # but there also might be a release with version [0, 3, 3] and even newer, we need to find most recent.
-            # calculate highest value found for patch (for cases when the 'releases' is not sorted)
-            if release_patch_candidate.version[2] > latest_patch_version.version[2]:
-                latest_patch_version = release_patch_candidate
-
-        if latest_patch_version.is_larger_then(self.__version):
-            self.patchable = True
-        else:
-            self.patchable = False
-        self.latest_patch = latest_patch_version
-
-    def get_dict(self):
-        return {
-            "package_name": self.package_name,
-            "version": str(self.version),
-            "patchable": self.patchable,
-            "latest_patch": str(self.latest_patch)
-        }
-
-    def __str__(self):
-        return str(self.get_dict())
-
-    @staticmethod
-    def is_patchable(x, y):
-        """
-        takes two lists, and checks if second list is patchable,
-        a version is patchable only if major and minor values equal but patch value is higher in first version,
-        for example:
-        x = [0, 4, 8] y = [0, 4, 6] returns True
-        x = [0, 4, 5] y = [0, 4, 6] returns False
-        x = [2, 1, 1] y = [2, 4, 1] returns False
-        :param x: list of ints
-        :param y: list of ints
-        :return: boolean
-        """
-        return x[0] == y[0] and x[1] == y[1] and x[2] > y[2]
-
-
-def get_pypi_package_releases(package_name):
-    """
-    calls PYPI json api as described here
-    https://wiki.python.org/moin/PyPIJSON
-    https://warehouse.readthedocs.io/api-reference/json.html
-    :param package_name: string, pypi project name
-    :return: json with pypi project response
-    """
-    import requests
-
-    result = requests.get('https://pypi.org/pypi/{}/json'.format(package_name))
-    if result.status_code != 200:
-        print('error occurred fetching package {} from PYPI.\n'
-              'response is: {}'.format(package_name, result.reason))
-        raise requests.exceptions.RequestException
-    return result.json()
-
-
-def get_setup_py_install_requires(content):
-    """
-    Extract 'install_requires' value using regex from 'content',
-    function will return a list of python packages:
-    ['package_a', 'package_b==1.5.6', 'package_c>=3.0']
-
-    :param content: the content of a setup.py file
-    :return: list on strings, install_requires values as list
-    """
-    # use DOTALL https://docs.python.org/3/library/re.html#re.DOTALL to include new lines
-    regex_install_requires_pattern = re.compile(r"install_requires=(.*?)],", flags=re.DOTALL)
-    version_match = regex_install_requires_pattern.findall(content)
-
-    if len(version_match) > 1:
-        raise RuntimeError("More than one 'install_requires' found: {0}".format(version_match))
-    if not version_match:
-        # 'install_requires' missing from setup.py file, just return empty array
-        return []
-
-    # add ending ']' since regex will not include it
-    found_install_requires = version_match[0] + ']'
-
-    # convert found_install_requires values into an array and return
-    from ast import literal_eval
-    return literal_eval(found_install_requires)
-
-
-def get_versions_from_requirements(requirements_list):
-    """
-    as described here https://pip.pypa.io/en/stable/reference/pip_install/#example-requirements-file
-    python versions requirement may appear in the form of:
-    docopt == 0.6.1             # Version Matching. Must be version 0.6.1
-    keyring >= 4.1.1            # Minimum version 4.1.1
-    coverage != 3.5             # Version Exclusion. Anything except version 3.5
-    pybump ~= 1.1               # Compatible release. Same as >= 1.1, == 1.*
-
-    the function is interested only in exact version match (case '=='), and will not consider '!=' patching
-    brake python requirements list, in the form of ['package_a', 'package_b==1.5.6', 'package_c>=3.0'],
-    for example
-    ['pyyaml==5.3.1', 'pybump', 'GitPython>=3.1']
-    :param requirements_list: list of strings
-    :return: list of PybumpPatchableVersion objects in the form of:
-        [PybumpPatchableVersion, PybumpPatchableVersion, PybumpPatchableVersion, ]
-    """
-    dependencies = []
-    for req in requirements_list:
-        # split name from version by all allowed operators
-        package_array = re.split("==|>=|~=", req)
-
-        package_name = package_array[0].strip()
-        if len(package_array) == 1:
-            # if package has no locked version or has >= type for current package, of type 'package>=2.7' its invalid
-            version = PybumpVersion('latest')
-        else:  # else the object will have a (probably) valid semantic version
-            version = PybumpVersion(package_array[1].strip())
-
-        # append current package
-        dependencies.append(PybumpPatchableVersion(package_name, version))
-
-    return dependencies
-
-
-def check_available_python_patches(setup_py_content=None):
-    """
-    get the content of setup.py file and return a list of dicts with possible patchable dependencies versions,
-    return will be in the form of:
-    [
-        {'package_name': 'pyyaml', 'version': '5.3.1', 'patchable': False, 'latest_patch': '5.3.1'},
-        {'package_name': 'GitPython', 'version': '3.1.7', 'patchable': True, 'latest_patch': '3.1.12'}
-    ]
-    :param setup_py_content: content of setup.py file
-    :return: list of dicts
-    """
-    requirements_list = get_setup_py_install_requires(setup_py_content)
-    requirements_versions = get_versions_from_requirements(requirements_list)
-
-    patchable_packages_array = []
-    for requirement in requirements_versions:
-        if requirement.version.is_valid_semantic_version():
-            # get current package info (as json) from pypi api
-            package_releases = get_pypi_package_releases(requirement.package_name)
-
-            # convert keys of the 'releases' dict, into a list (only version numbers),
-            releases_list = package_releases.get('releases').keys()  # releases_list is a list of strings
-            requirement.identify_possible_patch(releases_list)
-            patchable_packages_array.append(requirement.get_dict())
-
-    return patchable_packages_array
-
-
 def is_valid_helm_chart(content):
     """
     Check if input dictionary contains mandatory keys of a Helm Chart.yaml file,
     as documented here https://helm.sh/docs/topics/charts/#the-chartyaml-file
     :param content: parsed YAML file as dictionary of key values
     :return: True if dict contains mandatory values, else False
     """
@@ -474,15 +144,15 @@
 
     parser.add_argument('--version', action='version',
                         version='%(prog)s {}'.format(get_self_version('pybump')),
                         help='Print version and exit')
     parser.add_argument('--verify', required=False,
                         help='Verify if input string is a valid semantic version')
 
-    # Define parses that is shared, and will be used as 'parent' parser to all others
+    # Define parses that are shared, and will be used as 'parent' parser to all others
     base_sub_parser = argparse.ArgumentParser(add_help=False)
     base_sub_parser.add_argument('--file', help='Path to Chart.yaml/setup.py/VERSION file', required=True)
     base_sub_parser.add_argument('--app-version', action='store_true',
                                  help='Bump Helm chart appVersion, relevant only for Chart.yaml files', required=False)
 
     # Sub-parser for bump version command
     parser_bump = subparsers.add_parser('bump', parents=[base_sub_parser])
@@ -503,16 +173,16 @@
 
     # Sub-parser for get version command
     parser_get = subparsers.add_parser('get', parents=[base_sub_parser])
     parser_get.add_argument('--sem-ver', action='store_true', help='Get the main version only', required=False)
     parser_get.add_argument('--release', action='store_true', help='Get the version release only', required=False)
     parser_get.add_argument('--metadata', action='store_true', help='Get the version metadata only', required=False)
 
-    # Sub-parser for version latest patch verification command
-    subparsers.add_parser('patch-update', parents=[base_sub_parser])
+    # Sub-parser for version the latest patch verification command
+    # subparsers.add_parser('patch-update', parents=[base_sub_parser])
 
     args = vars(parser.parse_args())
 
     # Case where no args passed, sub_command is mandatory
     if args['sub_command'] is None:
         if args['verify']:
             version = PybumpVersion(args['verify'])
@@ -520,80 +190,89 @@
                 print('{} is valid'.format(version.__str__()))
             else:
                 version.print_invalid_version()
                 exit(1)
         else:
             parser.print_help()
         exit(0)
+    # elif args['sub_command'] == 'patch-update':
+    #     with open(args['file'], 'r') as stream:
+    #         filename, file_extension = os.path.splitext(args['file'])
+    #         file_base_name = os.path.basename(filename)
+    #         file_content = stream.read()
+    #
+    #     requirements = []
+    #     if file_base_name == 'python':
+    #         requirements = pybump_patch.get_setup_py_install_requires(file_content)
+    #     elif file_base_name == 'requirements':
+    #         requirements = [line.rstrip() for line in file_content.splitlines()]
+    #     else:
+    #       print('currently only python.py or requirements.txt pypi packages supported for latest patch verifications')
+    #       exit(1)
+    #
+    #     print(pybump_patch.check_available_python_patches(requirements_list=requirements))
+    else:
+        # Read current version from the given file
+        file_data = read_version_from_file(args['file'], args['app_version'])
+        file_content = file_data.get('file_content')
+        version_object = PybumpVersion(file_data.get('version'))
 
-    # Read current version from the given file
-    file_data = read_version_from_file(args['file'], args['app_version'])
-    file_content = file_data.get('file_content')
-    file_type = file_data.get('file_type')
-    version_object = PybumpVersion(file_data.get('version'))
-
-    if not version_object.is_valid_semantic_version():
-        version_object.print_invalid_version()
-        exit(1)
-
-    if args['sub_command'] == 'patch-update':
-        if file_type == 'python':
-            print(check_available_python_patches(setup_py_content=file_content))
-        else:
-            print('currently only python pypi packages supported for latest patch verifications')
+        if not version_object.is_valid_semantic_version():
+            version_object.print_invalid_version()
             exit(1)
-    elif args['sub_command'] == 'get':
-        if args['sem_ver']:
-            # Join the array of current_version_dict by dots
-            print('.'.join(str(x) for x in version_object.version))
-        elif args['release']:
-            print(version_object.release)
-        elif args['metadata']:
-            print(version_object.metadata)
+
+        if args['sub_command'] == 'get':
+            if args['sem_ver']:
+                # Join the array of current_version_dict by dots
+                print('.'.join(str(x) for x in version_object.version))
+            elif args['release']:
+                print(version_object.release)
+            elif args['metadata']:
+                print(version_object.metadata)
+            else:
+                print(version_object.__str__())
         else:
-            print(version_object.__str__())
-    else:
-        # Set new_version to be invalid first
-        new_version = None
+            # Set new_version to be invalid first
+            new_version = None
 
-        # Set the 'new_version' value
-        if args['sub_command'] == 'set':
-            # Case set-version argument passed, just set the new version with its value
-            if args['set_version']:
-                new_version = PybumpVersion(args['set_version'])
-            # Case the 'auto' flag was set, set release with current git branch name and metadata with hash
-            elif args['auto']:
-                from git import Repo, InvalidGitRepositoryError
-                # get the directory path of current working file
-                file_dirname_path = os.path.dirname(args['file'])
-                try:
-                    repo = Repo(path=file_dirname_path, search_parent_directories=True)
-                    # update current version release and metadata with relevant git values
+            # Set the 'new_version' value
+            if args['sub_command'] == 'set':
+                # Case set-version argument passed, just set the new version with its value
+                if args['set_version']:
+                    new_version = PybumpVersion(args['set_version'])
+                # Case the 'auto' flag was set, set release with current git branch name and metadata with hash
+                elif args['auto']:
+                    from git import Repo, InvalidGitRepositoryError
+                    # get the directory path of current working file
+                    file_dirname_path = os.path.dirname(args['file'])
                     try:
-                        version_object.release = str(repo.active_branch.commit)
-                    except TypeError:
-                        version_object.release = str(repo.head.object.hexsha)
-                    new_version = version_object
-                except InvalidGitRepositoryError:
-                    print("{} is not a valid git repo".format(file_dirname_path), file=stderr)
+                        repo = Repo(path=file_dirname_path, search_parent_directories=True)
+                        # update current version release and metadata with relevant git values
+                        try:
+                            version_object.release = str(repo.active_branch.commit)
+                        except TypeError:
+                            version_object.release = str(repo.head.object.hexsha)
+                        new_version = version_object
+                    except InvalidGitRepositoryError:
+                        print("{} is not a valid git repo".format(file_dirname_path), file=stderr)
+                        exit(1)
+                # Should never reach this point due to argparse mutual exclusion, but set safety if statement anyway
+                else:
+                    print("set-version or auto flags are mandatory", file=stderr)
                     exit(1)
-            # Should never reach this point due to argparse mutual exclusion, but set safety if statement anyway
-            else:
-                print("set-version or auto flags are mandatory", file=stderr)
+            else:  # bump version ['sub_command'] == 'bump'
+                # Only bump value of the 'version' key
+                version_object.bump_version(args['level'])
+                new_version = version_object
+            # new_version should never be None at this point, but check this anyway
+            if not new_version or not new_version.is_valid_semantic_version():
+                new_version.print_invalid_version()
                 exit(1)
-        else:  # bump version ['sub_command'] == 'bump'
-            # Only bump value of the 'version' key
-            version_object.bump_version(args['level'])
-            new_version = version_object
-        # new_version should never be None at this point, but check this anyway
-        if not new_version or not new_version.is_valid_semantic_version():
-            new_version.print_invalid_version()
-            exit(1)
-        # Write the new version with relevant content back to the file
-        write_version_to_file(args['file'], file_content, new_version.__str__(), args['app_version'])
+            # Write the new version with relevant content back to the file
+            write_version_to_file(args['file'], file_content, new_version.__str__(), args['app_version'])
 
-        if args['quiet'] is False:
-            print(new_version)
+            if args['quiet'] is False:
+                print(new_version)
 
 
 if __name__ == "__main__":
     main()
```

## test/__init__.py

```diff
@@ -1,7 +1,13 @@
+# make sure to import package directory whe running tests from root dir
+import os
+import sys
+
+ROOT = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..')
+sys.path.append(os.path.join(ROOT, 'src'))
 
 valid_helm_chart = {'apiVersion': 'v1',
                     'appVersion': '1.0',
                     'description': 'A Helm chart for Kubernetes',
                     'name': 'test',
                     'version': '0.1.0'}
 invalid_helm_chart = {'apiVersion': 'v1',
```

## test/test_pybump_patch_validator.py

```diff
@@ -1,231 +1,233 @@
-import json
-import unittest
-from unittest import mock
-
-from src.pybump import get_setup_py_install_requires, get_versions_from_requirements, \
-    get_pypi_package_releases, check_available_python_patches, PybumpVersion, PybumpPatchableVersion
-
-from . import valid_setup_py, valid_setup_py_2, invalid_setup_py_1, invalid_setup_py_2
-
-
-def mocked__pypi_requests(*args):
-    class MockResponse:
-        def __init__(self, json_data, status_code, reason='OK'):
-            self.json_data = json_data
-            self.status_code = status_code
-            self.reason = reason
-
-        def json(self):
-            return self.json_data
-
-    if args[0] == 'https://pypi.org/pypi/pybump/json':
-        with open('test/test_content_files/pypi_mocks/pypi_pybump_api_result.json') as json_file:
-            data = json.load(json_file)
-        return MockResponse(data, 200)
-
-    if args[0] == 'https://pypi.org/pypi/GitPython/json':
-        with open('test/test_content_files/pypi_mocks/pypi_gitpython_api_result.json') as json_file:
-            data = json.load(json_file)
-        return MockResponse(data, 200)
-
-    if args[0] == 'https://pypi.org/pypi/package_b/json':
-        with open('test/test_content_files/pypi_mocks/pypi_pybump_api_result.json') as json_file:
-            data = json.load(json_file)
-        return MockResponse(data, 200)
-
-    if args[0] == 'https://pypi.org/pypi/SOME_not_ex1st1ng_pypi_package/json':
-        return MockResponse(None, 404, 'Not Found')
-
-    return MockResponse(None, 404)
-
-
-class PyBumpPatcherTest(unittest.TestCase):
-
-    def setUp(self):
-        version_invalid_1 = PybumpVersion('latest')
-        version_invalid_2 = PybumpVersion('some_text>=more_text')
-
-        self.version_0_3_0 = PybumpVersion('0.3.0')
-        self.version_0_3_1 = PybumpVersion('v0.3.1')
-        self.version_0_3_2 = PybumpVersion('0.3.2')
-        self.version_0_3_8 = PybumpVersion('0.3.8')
-        self.version_0_4_2 = PybumpVersion('0.4.2')
-        self.version_1_3_3 = PybumpVersion('1.3.3')
-
-        self.package_a_0_3_0 = PybumpPatchableVersion('package_a', self.version_0_3_0)
-        self.package_b_0_3_1 = PybumpPatchableVersion('package_b', self.version_0_3_1)
-        self.package_c_0_3_2 = PybumpPatchableVersion('package_b', self.version_0_3_2)
-        self.package_d_0_4_2 = PybumpPatchableVersion('package_c', self.version_0_4_2)
-        self.package_invalid_a = PybumpPatchableVersion('package_invalid_a', version_invalid_1)
-        self.package_invalid_b = PybumpPatchableVersion('package_invalid_b', version_invalid_2)
-
-    def test_get_dict(self):
-        self.assertEqual(self.package_a_0_3_0.get_dict(),
-                         {'latest_patch': 'None',
-                          'package_name': 'package_a',
-                          'patchable': False,
-                          'version': '0.3.0'})
-        self.assertEqual(self.package_invalid_a.get_dict(),
-                         {'latest_patch': 'None',
-                          'package_name': 'package_invalid_a',
-                          'patchable': False,
-                          'version': '0.0.0'})
-
-    def test_str(self):
-        self.assertEqual(
-            str(self.package_a_0_3_0),
-            "{'package_name': 'package_a', 'version': '0.3.0', 'patchable': False, 'latest_patch': 'None'}")
-        self.assertEqual(
-            str(self.package_invalid_a),
-            "{'package_name': 'package_invalid_a', 'version': '0.0.0', 'patchable': False, 'latest_patch': 'None'}")
-
-    def test_get_setup_py_install_requires(self):
-        # should return empty list since valid_setup_py missing the install_requires=[] key
-        self.assertEqual(get_setup_py_install_requires(valid_setup_py), [])
-
-        self.assertEqual(get_setup_py_install_requires(valid_setup_py_2), ['pyyaml', 'pybump==1.3.3'])
-
-        # invalid_setup_py_1 should return empty list even when install_requires misspelled
-        self.assertEqual(get_setup_py_install_requires(invalid_setup_py_1), [])
-
-        with self.assertRaises(RuntimeError):
-            get_setup_py_install_requires(invalid_setup_py_2)
-
-    def test_get_versions_from_requirements(self):
-        """
-        get_versions_from_requirements function should return list of dicts in the form of:
-        [PybumpPatchableVersion, PybumpPatchableVersion, ]
-        will test against the values returned inside the PybumpVersion object
-        """
-        result = get_versions_from_requirements(
-            ['pyyaml', 'pybump==1.3.3', 'package_a >= 5.7', 'package_b~=1.1', 'package_c!=4.5.5', 'just_text=1']
-        )
-
-        # pyyaml
-        self.assertEqual(result[0].package_name, 'pyyaml')
-        self.assertEqual(result[0].version.version, [0, 0, 0])
-        self.assertEqual(result[0].version.release, None)
-        self.assertFalse(result[0].version.is_valid_semantic_version())
-
-        # pybump
-        self.assertEqual(result[1].package_name, 'pybump')
-        self.assertEqual(result[1].version.version, [1, 3, 3])
-        self.assertEqual(result[1].version.release, '')
-        self.assertTrue(result[1].version.is_valid_semantic_version())
-
-        # package_a
-        self.assertEqual(result[2].package_name, 'package_a')
-        self.assertEqual(result[2].version.version, [0, 0, 0])
-        self.assertEqual(result[2].version.release, None)
-        self.assertFalse(result[2].version.is_valid_semantic_version())
-
-        # package_b
-        self.assertEqual(result[3].package_name, 'package_b')
-        self.assertEqual(result[3].version.version, [0, 0, 0])
-        self.assertEqual(result[3].version.release, None)
-        self.assertFalse(result[3].version.is_valid_semantic_version())
-
-        # package_c
-        self.assertEqual(result[4].package_name, 'package_c!=4.5.5')
-        self.assertEqual(result[4].version.version, [0, 0, 0])
-        self.assertEqual(result[4].version.release, None)
-        self.assertFalse(result[4].version.is_valid_semantic_version())
-
-        # just_text
-        self.assertEqual(result[5].package_name, 'just_text=1')
-        self.assertEqual(result[5].version.version, [0, 0, 0])
-        self.assertEqual(result[5].version.release, None)
-        self.assertFalse(result[5].version.is_valid_semantic_version())
-
-        # test passing empty list
-        self.assertEqual(
-            get_versions_from_requirements([]),
-            []
-        )
-
-        with self.assertRaises(TypeError):
-            get_versions_from_requirements(None)
-            get_versions_from_requirements('str')
-
-    def test_identify_possible_patch(self):
-        # test package_a_0_3_0 case when version is patchable
-        self.assertFalse(self.package_a_0_3_0.patchable)
-        self.package_a_0_3_0.identify_possible_patch(['0.1.2', '0.1.3', '0.3.1', '0.3.2'])
-        self.assertTrue(self.package_a_0_3_0.patchable)
-        self.assertEqual(self.package_a_0_3_0.latest_patch.version, self.version_0_3_2.version)
-
-        # test package_b_0_3_1 NOT sorted list case
-        self.assertFalse(self.package_b_0_3_1.patchable)
-        self.package_b_0_3_1.identify_possible_patch(['0.3.2', '0.1.2', '0.1.3', '0.3.1'])
-        self.assertTrue(self.package_b_0_3_1.patchable)
-        self.assertEqual(self.package_b_0_3_1.latest_patch.version, self.version_0_3_2.version)
-
-        self.package_b_0_3_1.identify_possible_patch(['0.2.2', 'text', None])
-        self.assertFalse(self.package_b_0_3_1.patchable)
-        self.assertEqual(self.package_b_0_3_1.latest_patch.version, self.version_0_3_1.version)
-
-        # test package_b_0_3_1 NOT sorted list case
-        self.package_b_0_3_1.identify_possible_patch(['4.2.2', '0.3.8', '0.1.2', '0.1.3', '0.3.1'])
-        self.assertTrue(self.package_b_0_3_1.patchable)
-        self.assertEqual(self.package_b_0_3_1.latest_patch.version, self.version_0_3_8.version)
-
-        # pass empty list
-        with self.assertRaises(ValueError):
-            self.package_b_0_3_1.identify_possible_patch([])
-
-        # test version that is already latest
-        self.package_c_0_3_2.identify_possible_patch(['0.1.2', '0.1.3', '0.3.1', '0.3.2'])
-        self.assertFalse(self.package_c_0_3_2.patchable)
-        self.assertEqual(self.package_c_0_3_2.latest_patch.version, self.version_0_3_2.version)
-
-        # test not patchable version
-        self.package_d_0_4_2.identify_possible_patch(['4.2.2', '0.3.8', '0.1.2', '0.1.3', '0.3.1'])
-        self.assertFalse(self.package_d_0_4_2.patchable)
-        self.assertEqual(self.package_d_0_4_2.latest_patch.version, self.version_0_4_2.version)
-
-        self.assertFalse(self.package_invalid_b.patchable)
-        self.package_invalid_b.identify_possible_patch(['4.2.2', '0.3.8', '0.1.2', '0.1.3', '0.3.1'])
-        self.assertFalse(self.package_invalid_b.patchable)
-        self.assertEqual(self.package_invalid_b.latest_patch.invalid_version, 'some_text>=more_text')
-
-    def test_is_patchable(self):
-        self.assertTrue(PybumpPatchableVersion.is_patchable([0, 4, 5], [0, 4, 1]))
-        self.assertFalse(PybumpPatchableVersion.is_patchable([2, 1, 2], [2, 4, 2]))
-        self.assertFalse(PybumpPatchableVersion.is_patchable([0, 4, 5], [0, 4, 6]))
-        self.assertFalse(PybumpPatchableVersion.is_patchable([0, 0, 1], [0, 0, 1]))
-
-    @mock.patch('requests.get', side_effect=mocked__pypi_requests)
-    def test_get_pypi_package_releases(self, mock_get):
-        # mock request to https://pypi.org/pypi/pybump/json
-        json_data = get_pypi_package_releases('pybump')
-
-        with open('test/test_content_files/pypi_mocks/pypi_pybump_api_result.json') as json_file:
-            data = json.load(json_file)
-        self.assertEqual(json_data, data)
-
-        # test request to https://pypi.org/pypi/SOME_not_ex1st1ng_pypi_package/json
-        from requests.exceptions import RequestException
-        with self.assertRaises(RequestException):
-            get_pypi_package_releases('SOME_not_ex1st1ng_pypi_package')
-
-        # make sure we mocked 3 tests
-        self.assertEqual(len(mock_get.call_args_list), 2)
-
-    @mock.patch('requests.get', side_effect=mocked__pypi_requests)
-    def test_check_available_python_patches(self, mock_get):
-        # the test_valid_setup.py file contains 2 dependencies
-        with open('test/test_content_files/test_valid_setup.py') as py_content:
-            setup_py_content = py_content.read()
-        self.assertEqual(
-            check_available_python_patches(setup_py_content),
-            [
-                {'package_name': 'pybump', 'version': '1.3.1', 'patchable': True, 'latest_patch': '1.3.8'},
-                {'package_name': 'GitPython', 'version': '3.1.7', 'patchable': True, 'latest_patch': '3.1.12'},
-            ])
-
-        # make sure we check (mocked) 2 packages
-        self.assertEqual(len(mock_get.call_args_list), 2)
-
-
-if __name__ == '__main__':
-    unittest.main()
+# import json
+# import unittest
+# from unittest import mock
+#
+# from src.pybump import PybumpVersion
+# from src.pybump_patch import get_setup_py_install_requires, get_versions_from_requirements, \
+#     get_pypi_package_releases, check_available_python_patches, PybumpPatchableVersion
+#
+# from . import valid_setup_py, valid_setup_py_2, invalid_setup_py_1, invalid_setup_py_2
+#
+#
+# def mocked__pypi_requests(*args):
+#     class MockResponse:
+#         def __init__(self, json_data, status_code, reason='OK'):
+#             self.json_data = json_data
+#             self.status_code = status_code
+#             self.reason = reason
+#
+#         def json(self):
+#             return self.json_data
+#
+#     if args[0] == 'https://pypi.org/pypi/pybump/json':
+#         with open('test/test_content_files/pypi_mocks/pypi_pybump_api_result.json') as json_file:
+#             data = json.load(json_file)
+#         return MockResponse(data, 200)
+#
+#     if args[0] == 'https://pypi.org/pypi/GitPython/json':
+#         with open('test/test_content_files/pypi_mocks/pypi_gitpython_api_result.json') as json_file:
+#             data = json.load(json_file)
+#         return MockResponse(data, 200)
+#
+#     if args[0] == 'https://pypi.org/pypi/package_b/json':
+#         with open('test/test_content_files/pypi_mocks/pypi_pybump_api_result.json') as json_file:
+#             data = json.load(json_file)
+#         return MockResponse(data, 200)
+#
+#     if args[0] == 'https://pypi.org/pypi/SOME_not_ex1st1ng_pypi_package/json':
+#         return MockResponse(None, 404, 'Not Found')
+#
+#     return MockResponse(None, 404)
+#
+#
+# class PyBumpPatcherTest(unittest.TestCase):
+#
+#     def setUp(self):
+#         version_invalid_1 = PybumpVersion('latest')
+#         version_invalid_2 = PybumpVersion('some_text>=more_text')
+#
+#         self.version_0_3_0 = PybumpVersion('0.3.0')
+#         self.version_0_3_1 = PybumpVersion('v0.3.1')
+#         self.version_0_3_2 = PybumpVersion('0.3.2')
+#         self.version_0_3_8 = PybumpVersion('0.3.8')
+#         self.version_0_4_2 = PybumpVersion('0.4.2')
+#         self.version_1_3_3 = PybumpVersion('1.3.3')
+#
+#         self.package_a_0_3_0 = PybumpPatchableVersion('package_a', self.version_0_3_0)
+#         self.package_b_0_3_1 = PybumpPatchableVersion('package_b', self.version_0_3_1)
+#         self.package_c_0_3_2 = PybumpPatchableVersion('package_b', self.version_0_3_2)
+#         self.package_d_0_4_2 = PybumpPatchableVersion('package_c', self.version_0_4_2)
+#         self.package_invalid_a = PybumpPatchableVersion('package_invalid_a', version_invalid_1)
+#         self.package_invalid_b = PybumpPatchableVersion('package_invalid_b', version_invalid_2)
+#
+#     def test_get_dict(self):
+#         self.assertEqual(self.package_a_0_3_0.get_dict(),
+#                          {'latest_patch': 'None',
+#                           'package_name': 'package_a',
+#                           'patchable': False,
+#                           'version': '0.3.0'})
+#         self.assertEqual(self.package_invalid_a.get_dict(),
+#                          {'latest_patch': 'None',
+#                           'package_name': 'package_invalid_a',
+#                           'patchable': False,
+#                           'version': '0.0.0'})
+#
+#     def test_str(self):
+#         self.assertEqual(
+#             str(self.package_a_0_3_0),
+#             "{'package_name': 'package_a', 'version': '0.3.0', 'patchable': False, 'latest_patch': 'None'}")
+#         self.assertEqual(
+#             str(self.package_invalid_a),
+#             "{'package_name': 'package_invalid_a', 'version': '0.0.0', 'patchable': False, 'latest_patch': 'None'}")
+#
+#     def test_get_setup_py_install_requires(self):
+#         # should return empty list since valid_setup_py missing the install_requires=[] key
+#         self.assertEqual(get_setup_py_install_requires(valid_setup_py), [])
+#
+#         self.assertEqual(get_setup_py_install_requires(valid_setup_py_2), ['pyyaml', 'pybump==1.3.3'])
+#
+#         # invalid_setup_py_1 should return empty list even when install_requires misspelled
+#         self.assertEqual(get_setup_py_install_requires(invalid_setup_py_1), [])
+#
+#         with self.assertRaises(RuntimeError):
+#             get_setup_py_install_requires(invalid_setup_py_2)
+#
+#     def test_get_versions_from_requirements(self):
+#         """
+#         get_versions_from_requirements function should return list of dicts in the form of:
+#         [PybumpPatchableVersion, PybumpPatchableVersion, ]
+#         will test against the values returned inside the PybumpVersion object
+#         """
+#         result = get_versions_from_requirements(
+#             ['pyyaml', 'pybump==1.3.3', 'package_a >= 5.7', 'package_b~=1.1', 'package_c!=4.5.5', 'just_text=1']
+#         )
+#
+#         # pyyaml
+#         self.assertEqual(result[0].package_name, 'pyyaml')
+#         self.assertEqual(result[0].version.version, [0, 0, 0])
+#         self.assertEqual(result[0].version.release, None)
+#         self.assertFalse(result[0].version.is_valid_semantic_version())
+#
+#         # pybump
+#         self.assertEqual(result[1].package_name, 'pybump')
+#         self.assertEqual(result[1].version.version, [1, 3, 3])
+#         self.assertEqual(result[1].version.release, '')
+#         self.assertTrue(result[1].version.is_valid_semantic_version())
+#
+#         # package_a
+#         self.assertEqual(result[2].package_name, 'package_a')
+#         self.assertEqual(result[2].version.version, [0, 0, 0])
+#         self.assertEqual(result[2].version.release, None)
+#         self.assertFalse(result[2].version.is_valid_semantic_version())
+#
+#         # package_b
+#         self.assertEqual(result[3].package_name, 'package_b')
+#         self.assertEqual(result[3].version.version, [0, 0, 0])
+#         self.assertEqual(result[3].version.release, None)
+#         self.assertFalse(result[3].version.is_valid_semantic_version())
+#
+#         # package_c
+#         self.assertEqual(result[4].package_name, 'package_c!=4.5.5')
+#         self.assertEqual(result[4].version.version, [0, 0, 0])
+#         self.assertEqual(result[4].version.release, None)
+#         self.assertFalse(result[4].version.is_valid_semantic_version())
+#
+#         # just_text
+#         self.assertEqual(result[5].package_name, 'just_text=1')
+#         self.assertEqual(result[5].version.version, [0, 0, 0])
+#         self.assertEqual(result[5].version.release, None)
+#         self.assertFalse(result[5].version.is_valid_semantic_version())
+#
+#         # test passing empty list
+#         self.assertEqual(
+#             get_versions_from_requirements([]),
+#             []
+#         )
+#
+#         with self.assertRaises(TypeError):
+#             get_versions_from_requirements(None)
+#             get_versions_from_requirements('str')
+#
+#     def test_identify_possible_patch(self):
+#         # test package_a_0_3_0 case when version is patchable
+#         self.assertFalse(self.package_a_0_3_0.patchable)
+#         self.package_a_0_3_0.identify_possible_patch(['0.1.2', '0.1.3', '0.3.1', '0.3.2'])
+#         self.assertTrue(self.package_a_0_3_0.patchable)
+#         self.assertEqual(self.package_a_0_3_0.latest_patch.version, self.version_0_3_2.version)
+#
+#         # test package_b_0_3_1 NOT sorted list case
+#         self.assertFalse(self.package_b_0_3_1.patchable)
+#         self.package_b_0_3_1.identify_possible_patch(['0.3.2', '0.1.2', '0.1.3', '0.3.1'])
+#         self.assertTrue(self.package_b_0_3_1.patchable)
+#         self.assertEqual(self.package_b_0_3_1.latest_patch.version, self.version_0_3_2.version)
+#
+#         self.package_b_0_3_1.identify_possible_patch(['0.2.2', 'text', None])
+#         self.assertFalse(self.package_b_0_3_1.patchable)
+#         self.assertEqual(self.package_b_0_3_1.latest_patch.version, self.version_0_3_1.version)
+#
+#         # test package_b_0_3_1 NOT sorted list case
+#         self.package_b_0_3_1.identify_possible_patch(['4.2.2', '0.3.8', '0.1.2', '0.1.3', '0.3.1'])
+#         self.assertTrue(self.package_b_0_3_1.patchable)
+#         self.assertEqual(self.package_b_0_3_1.latest_patch.version, self.version_0_3_8.version)
+#
+#         # pass empty list
+#         with self.assertRaises(ValueError):
+#             self.package_b_0_3_1.identify_possible_patch([])
+#
+#         # test version that is already latest
+#         self.package_c_0_3_2.identify_possible_patch(['0.1.2', '0.1.3', '0.3.1', '0.3.2'])
+#         self.assertFalse(self.package_c_0_3_2.patchable)
+#         self.assertEqual(self.package_c_0_3_2.latest_patch.version, self.version_0_3_2.version)
+#
+#         # test not patchable version
+#         self.package_d_0_4_2.identify_possible_patch(['4.2.2', '0.3.8', '0.1.2', '0.1.3', '0.3.1'])
+#         self.assertFalse(self.package_d_0_4_2.patchable)
+#         self.assertEqual(self.package_d_0_4_2.latest_patch.version, self.version_0_4_2.version)
+#
+#         self.assertFalse(self.package_invalid_b.patchable)
+#         self.package_invalid_b.identify_possible_patch(['4.2.2', '0.3.8', '0.1.2', '0.1.3', '0.3.1'])
+#         self.assertFalse(self.package_invalid_b.patchable)
+#         self.assertEqual(self.package_invalid_b.latest_patch.invalid_version, 'some_text>=more_text')
+#
+#     def test_is_patchable(self):
+#         self.assertTrue(PybumpPatchableVersion.is_patchable([0, 4, 5], [0, 4, 1]))
+#         self.assertFalse(PybumpPatchableVersion.is_patchable([2, 1, 2], [2, 4, 2]))
+#         self.assertFalse(PybumpPatchableVersion.is_patchable([0, 4, 5], [0, 4, 6]))
+#         self.assertFalse(PybumpPatchableVersion.is_patchable([0, 0, 1], [0, 0, 1]))
+#
+#     @mock.patch('requests.get', side_effect=mocked__pypi_requests)
+#     def test_get_pypi_package_releases(self, mock_get):
+#         # mock request to https://pypi.org/pypi/pybump/json
+#         json_data = get_pypi_package_releases('pybump')
+#
+#         with open('test/test_content_files/pypi_mocks/pypi_pybump_api_result.json') as json_file:
+#             data = json.load(json_file)
+#         self.assertEqual(json_data, data)
+#
+#         # test request to https://pypi.org/pypi/SOME_not_ex1st1ng_pypi_package/json
+#         from requests.exceptions import RequestException
+#         with self.assertRaises(RequestException):
+#             get_pypi_package_releases('SOME_not_ex1st1ng_pypi_package')
+#
+#         # make sure we mocked 3 tests
+#         self.assertEqual(len(mock_get.call_args_list), 2)
+#
+#     @mock.patch('requests.get', side_effect=mocked__pypi_requests)
+#     def test_check_available_python_patches(self, mock_get):
+#         # the test_valid_setup.py file contains 2 dependencies
+#         with open('test/test_content_files/test_valid_setup.py') as py_content:
+#             setup_py_content = py_content.read()
+#             aaa = get_setup_py_install_requires(setup_py_content)
+#         self.assertEqual(
+#             check_available_python_patches(aaa),
+#             [
+#                 {'package_name': 'pybump', 'version': '1.3.1', 'patchable': True, 'latest_patch': '1.3.8'},
+#                 {'package_name': 'GitPython', 'version': '3.1.7', 'patchable': True, 'latest_patch': '3.1.12'},
+#             ])
+#
+#         # make sure we check (mocked) 2 packages
+#         self.assertEqual(len(mock_get.call_args_list), 2)
+#
+#
+# if __name__ == '__main__':
+#     unittest.main()
```

## Comparing `pybump-1.8.1.dist-info/LICENSE` & `pybump-1.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pybump-1.8.1.dist-info/METADATA` & `pybump-1.9.3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pybump
-Version: 1.8.1
+Version: 1.9.3
 Summary: Python version bumper
 Home-page: https://github.com/ArieLevs/PyBump
 Author: Arie Lev
 Author-email: levinsonarie@gmail.com
 License: Apache License 2.0
 Keywords: bump,version,appVersion,versioning,helm,charts,setup.py,promote
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: pyyaml (==5.4.1)
-Requires-Dist: GitPython (==3.1.27)
-Requires-Dist: requests (==2.25.1)
+Requires-Dist: pyyaml (==6.0)
+Requires-Dist: GitPython (==3.1.29)
 
 Python Version Bumper
 =====================
 .. image:: https://github.com/arielevs/pybump/workflows/Python%20package/badge.svg
     :alt: Build
     :target: https://pypi.org/project/pybump/
 
@@ -45,20 +44,14 @@
     :target: https://pypi.org/project/pybump/
 
 Simple python code to bump kubernetes package manager Helm charts.yaml, VERSION and setup.py files versions.
 
 | Versions must match semver 2.0.0: https://github.com/semver/semver/blob/master/semver.md
 | Version is allowed a lower case 'v' character for example: ``v1.5.4-beta2``
 
-| Continuous integration dependencies check:
-| the ``patch-update`` argument will check dependencies in target file and suggest only patchable versions,
-| The main purpose it to provide a way to constantly scan dependencies updates, and patch them once available.
-| For example, this package has a dependencies ``pyyaml``, and a version with ``5.3.1``,
-| once a new patch i released at PYPI, it will detect it and return for example ``5.3.7``.
-
 Install
 -------
 ``pip install pybump``
 
 Usage
 -----
 | **bump** version:
@@ -75,18 +68,14 @@
  * NOTE - This can be dangerous as the `auto` flag might detect a git repo you were not intended to bump,
    make sure the bumped file is really a child in the git repo you intended to bump.
 
 | **get** current version:
 | ``pybump get --file PATH_TO_CHART.YAML``
 |
 
-| **patch-verification**:
-| ``pybump patch-update --file PATH_TO_SETUP.PY``
-|
-
 | update Helm chart **appVersion**:
 | in order to bump/get/set the Helm chart appVersion value just add the ``--app-version`` flag
 | ``pybump bump [-h] --file PATH_TO_CHART.YAML --level {major,minor,patch} [--quiet] [--app-version]``
 
  * note that the --app-version flag is relevant only for Helm chart.yaml files and has not effect on other cases.
 
 Examples
@@ -118,9 +107,7 @@
 
 | Case: ``version: 1.0.13``
 | ``pybump get --file Chart.yaml`` will return ``1.0.13``
 |
 
 | Case: ``version: 1.0.13+some-metadata``
 | ``pybump get --file Chart.yaml --release`` will return ``some``
-
-
```

## Comparing `pybump-1.8.1.dist-info/RECORD` & `pybump-1.9.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-src/pybump.py,sha256=jwrRfDc_Vd8Oee1FzZrAdf4s-n3ZhI5brbw43qR203k,24845
-test/__init__.py,sha256=RAcc3Acl--C-2HtOiKn7huILfsrW7xzkSkR4looxLQ4,2806
+src/pybump.py,sha256=B_UeaErZnseJQOCJc9Rv9Ilbt0i8omrLIfYpGiqcvog,12821
+src/pybump_patch.py,sha256=bQ2YTRfzXpT8j2RTLQQiMeWWAc8Ck2V5SJAIQ0j_hR8,8067
+src/pybump_version.py,sha256=18Npku57VZblQfe4a7rDamHmbpFQNAY4ltUJtka5yy4,5201
+test/__init__.py,sha256=3OA3Aa2eC2YAcWgQDeN1JpLvP1EVZrSlitpsbdXZVO0,3013
 test/test_pybump.py,sha256=dk8o8vmmFH2OOwqcld-4pr7JJFd2BXK2UIlJ6LntQIQ,12354
-test/test_pybump_patch_validator.py,sha256=O1HXPeWe7mMvj1PaGbiZrsNd1QCi_Y5BA02FjRNBvJ4,10792
+test/test_pybump_patch_validator.py,sha256=uaE0GEgLesQwauWi3qtWLpY9LB7JPqatjbu8Ws-qob8,11292
 test/test_simulate_pybump.py,sha256=BJNDf1OS9SM17t2GDsXRgXyE-2uGo4_17eC6fxlPH2A,15185
-pybump-1.8.1.dist-info/LICENSE,sha256=a51oCHpBvC241HTra8pAx_H70YFc0bJ0s3dsn6Gljlc,10759
-pybump-1.8.1.dist-info/METADATA,sha256=tNH5SkvbfzMV6gTG5kl8QyiIVA55W6lTTxiu79hPakk,4521
-pybump-1.8.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pybump-1.8.1.dist-info/entry_points.txt,sha256=suHzZkorfPm4CsHJxx6uzwsuQbGJr3LJB3oyopa2Zp8,44
-pybump-1.8.1.dist-info/top_level.txt,sha256=ko5Zp-GH1-aCqmTB-_pzAfcKWZ9D29cRgzo8EmAy2_k,9
-pybump-1.8.1.dist-info/RECORD,,
+pybump-1.9.3.dist-info/LICENSE,sha256=a51oCHpBvC241HTra8pAx_H70YFc0bJ0s3dsn6Gljlc,10759
+pybump-1.9.3.dist-info/METADATA,sha256=WbBwPzl_vpaiaRxD5j9NW4NVhMwS0qrH6PCYxPkk8kM,3991
+pybump-1.9.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pybump-1.9.3.dist-info/entry_points.txt,sha256=DbwrnsPKlOUkLOsXlVgR3WGbV_zK9wxW7WEMlEUsHhQ,43
+pybump-1.9.3.dist-info/top_level.txt,sha256=ko5Zp-GH1-aCqmTB-_pzAfcKWZ9D29cRgzo8EmAy2_k,9
+pybump-1.9.3.dist-info/RECORD,,
```


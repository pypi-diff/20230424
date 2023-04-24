# Comparing `tmp/labcrawler-1.0.0.tar.gz` & `tmp/labcrawler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcrawler-1.0.0.tar", last modified: Sat Apr 22 03:10:25 2023, max compression
+gzip compressed data, was "labcrawler-1.0.1.tar", last modified: Mon Apr 24 01:40:10 2023, max compression
```

## Comparing `labcrawler-1.0.0.tar` & `labcrawler-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.270439 labcrawler-1.0.0/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-1.0.0/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-22 03:09:31.000000 labcrawler-1.0.0/MANIFEST.in
--rw-r--r--   0 francispotter   (501) staff       (20)    13528 2023-04-22 03:10:25.269366 labcrawler-1.0.0/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)    13246 2023-04-22 03:09:31.000000 labcrawler-1.0.0/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.263841 labcrawler-1.0.0/labcrawler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-1.0.0/labcrawler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/_legacy.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3509 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/analysis.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5354 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/cli.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-1.0.0/labcrawler/gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3040 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/gitlab_ci_data_loader.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-1.0.0/labcrawler/gitlab_repository_files_extractor.py
--rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/project_data_file.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.268015 labcrawler-1.0.0/labcrawler/templates/
--rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/templates/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/templates/labcrawler.json.template
--rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/templates/meltano.yml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.266020 labcrawler-1.0.0/labcrawler.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)    13528 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      689 2023-04-22 03:09:31.000000 labcrawler-1.0.0/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-22 03:10:25.270633 labcrawler-1.0.0/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.268436 labcrawler-1.0.0/test/
--rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-1.0.0/test/test_gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-22 03:10:05.000000 labcrawler-1.0.0/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 01:40:10.713647 labcrawler-1.0.1/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-1.0.1/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-22 03:09:31.000000 labcrawler-1.0.1/MANIFEST.in
+-rw-r--r--   0 francispotter   (501) staff       (20)    13695 2023-04-24 01:40:10.713257 labcrawler-1.0.1/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)    13413 2023-04-24 01:28:44.000000 labcrawler-1.0.1/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 01:40:10.707635 labcrawler-1.0.1/labcrawler/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-1.0.1/labcrawler/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-22 03:09:31.000000 labcrawler-1.0.1/labcrawler/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-22 03:09:31.000000 labcrawler-1.0.1/labcrawler/_legacy.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3573 2023-04-24 01:27:34.000000 labcrawler-1.0.1/labcrawler/analysis.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5351 2023-04-24 00:51:06.000000 labcrawler-1.0.1/labcrawler/cli.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-1.0.1/labcrawler/gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3131 2023-04-24 00:56:03.000000 labcrawler-1.0.1/labcrawler/gitlab_ci_data_loader.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-1.0.1/labcrawler/gitlab_repository_files_extractor.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-22 03:09:31.000000 labcrawler-1.0.1/labcrawler/project_data_file.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 01:40:10.711921 labcrawler-1.0.1/labcrawler/templates/
+-rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-22 03:09:31.000000 labcrawler-1.0.1/labcrawler/templates/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-22 03:09:31.000000 labcrawler-1.0.1/labcrawler/templates/labcrawler.json.template
+-rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-22 03:09:31.000000 labcrawler-1.0.1/labcrawler/templates/meltano.yml
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 01:40:10.710392 labcrawler-1.0.1/labcrawler.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)    13695 2023-04-24 01:40:10.000000 labcrawler-1.0.1/labcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-04-24 01:40:10.000000 labcrawler-1.0.1/labcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-24 01:40:10.000000 labcrawler-1.0.1/labcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-04-24 01:40:10.000000 labcrawler-1.0.1/labcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-04-24 01:40:10.000000 labcrawler-1.0.1/labcrawler.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-04-24 01:40:10.000000 labcrawler-1.0.1/labcrawler.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      689 2023-04-22 03:09:31.000000 labcrawler-1.0.1/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-24 01:40:10.713751 labcrawler-1.0.1/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 01:40:10.712473 labcrawler-1.0.1/test/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-1.0.1/test/test_gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-24 01:39:56.000000 labcrawler-1.0.1/version
```

### Comparing `labcrawler-1.0.0/LICENSE` & `labcrawler-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.0/PKG-INFO` & `labcrawler-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -146,43 +146,52 @@
 2. Joins raw DataFrames into slightly-more-useful DataFrames with specific names for each datatype
 3. Outputs how many rows are in each DataFrame, with the variable name for each
 4. Starts a Python command-line Python interpreter for querying the resulting DataFrames using Pandas operations
 
 
 ``` python
 
+# List the projects
+projects[['name']]
+
 # See what columns are available in any table
 projects.columns
 
 # View just certain columns from a table
-projects[['path_with_namespace','merge_requests_enabled']]
+projects[['path_with_namespace','merge_method']]
 
 # See how many of each value are included
-projects.value_counts(['merge_requests_enabled'])
+projects.value_counts(['merge_method'])
 
 # Count the total of unmerged branches
 len(branches.loc[~branches['merged']])
 
 # View the number of unmerged branches by project
-branches.loc[~branches['merged']].value_counts(['project_path_with_namespace'])
+branches.loc[~branches['merged']].value_counts(['project_name'])
 
 # See who has access to a project
-project_members.query('project_path_with_namespace == "<replace-with-project-path>"')[['user_username','access_level_name']]
+project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
 
 # See who has access to a group
-group_members.query('group_path == "<replace-with-group-path>"')[['username','access_level_name']]
+group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
 
 # How many have each access level
 group_members.value_counts(['access_level_name'])
 
 # Who are the owners and maintainers?
-group_members.query('group_path == "<replace-with-group-path>" and access_level_name in {"Owner","Maintainer}')[['username','access_level_name']]
+group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
 
 # See the GitLab CI configuration file path for projects
-projects[['path_with_namespace','ci_config_path']]
+projects[['name','ci_config_path']]
+
+# Which projects have CI configuration at all
+ci_config_paths.query("main.notnull()")[['project_name']]
+
+# Projects without any CI configuration
+ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
 
 # See who has edited the CI configuration file
 ci_config_committers
 ```
 
 If you want to see all of the rows when performing queries, rather than just a sample, try:
```

### Comparing `labcrawler-1.0.0/README.md` & `labcrawler-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,43 +136,52 @@
 2. Joins raw DataFrames into slightly-more-useful DataFrames with specific names for each datatype
 3. Outputs how many rows are in each DataFrame, with the variable name for each
 4. Starts a Python command-line Python interpreter for querying the resulting DataFrames using Pandas operations
 
 
 ``` python
 
+# List the projects
+projects[['name']]
+
 # See what columns are available in any table
 projects.columns
 
 # View just certain columns from a table
-projects[['path_with_namespace','merge_requests_enabled']]
+projects[['path_with_namespace','merge_method']]
 
 # See how many of each value are included
-projects.value_counts(['merge_requests_enabled'])
+projects.value_counts(['merge_method'])
 
 # Count the total of unmerged branches
 len(branches.loc[~branches['merged']])
 
 # View the number of unmerged branches by project
-branches.loc[~branches['merged']].value_counts(['project_path_with_namespace'])
+branches.loc[~branches['merged']].value_counts(['project_name'])
 
 # See who has access to a project
-project_members.query('project_path_with_namespace == "<replace-with-project-path>"')[['user_username','access_level_name']]
+project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
 
 # See who has access to a group
-group_members.query('group_path == "<replace-with-group-path>"')[['username','access_level_name']]
+group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
 
 # How many have each access level
 group_members.value_counts(['access_level_name'])
 
 # Who are the owners and maintainers?
-group_members.query('group_path == "<replace-with-group-path>" and access_level_name in {"Owner","Maintainer}')[['username','access_level_name']]
+group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
 
 # See the GitLab CI configuration file path for projects
-projects[['path_with_namespace','ci_config_path']]
+projects[['name','ci_config_path']]
+
+# Which projects have CI configuration at all
+ci_config_paths.query("main.notnull()")[['project_name']]
+
+# Projects without any CI configuration
+ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
 
 # See who has edited the CI configuration file
 ci_config_committers
 ```
 
 If you want to see all of the rows when performing queries, rather than just a sample, try:
```

### Comparing `labcrawler-1.0.0/labcrawler/_legacy.py` & `labcrawler-1.0.1/labcrawler/_legacy.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.0/labcrawler/analysis.py` & `labcrawler-1.0.1/labcrawler/analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     projects:DataFrame = None
     branches:DataFrame = None
     merge_requests:DataFrame = None
     project_members:DataFrame = None
     group_members:DataFrame = None
     users:DataFrame = None
     ci_config_committers:DataFrame = None
-    ci_config_includes:DataFrame = None
+    ci_config_paths:DataFrame = None
 
 def datatypes():
     annotations = get_annotations(DataSet)
     return  [n for n in annotations if annotations[n] == DataFrame]
 
 DATATYPES = datatypes()
 
@@ -45,16 +45,17 @@
                 [50, 'Owner']], columns = ['id', 'name']).set_index('id')
         if isinstance(raw.groups, DataFrame):
                 self.groups = raw.groups.set_index('id')
         if isinstance(raw.projects, DataFrame):
                 self.projects = raw.projects.set_index('id')
         if isinstance(raw.users, DataFrame):
                 self.users = raw.users.set_index('id')
-        self.branches = raw.branches.set_index('project_id').\
-                join(self.projects[['name','path_with_namespace']].add_prefix('project_'))
+        if isinstance(raw.branches, DataFrame):
+                self.branches = raw.branches.set_index('project_id').\
+                        join(self.projects[['name','path_with_namespace']].add_prefix('project_'))
         if isinstance(raw.merge_requests, DataFrame):
                 self.merge_requests = raw.merge_requests.set_index('project_id').\
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'))
         if isinstance(raw.project_members, DataFrame):
                 self.project_members = raw.project_members.\
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'), on='project_id').\
                         join(self.users[['username']].add_prefix('user_'), on='user_id').\
@@ -62,16 +63,16 @@
         if isinstance(raw.group_members, DataFrame):
                 self.group_members = raw.group_members.\
                         join(self.groups[['path']].add_prefix('group_'), on='group_id').\
                         join(self.access_levels[['name']].add_prefix('access_level_'), on='access_level')
         if isinstance(raw.ci_config_committers, DataFrame):
                 self.ci_config_committers = raw.ci_config_committers.\
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'), on='project_id' )
-        if isinstance(raw.ci_config_includes, DataFrame):
-                self.ci_config_includes = raw.ci_config_includes.\
-                        join(self.projects[['name','path_with_namespace']].add_prefix('project_'), on='project_id' )
+        if isinstance(raw.ci_config_paths, DataFrame):
+                self.ci_config_paths = raw.ci_config_paths.\
+                        join(self.projects[['name','path_with_namespace']].add_prefix('project_'), on='project_id', how='right')
         
         for datatype in DATATYPES:
             df = getattr(self, datatype)
             if df is not None:
                 df.index.name = 'id'
```

### Comparing `labcrawler-1.0.0/labcrawler/cli.py` & `labcrawler-1.0.1/labcrawler/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         # Cheap and easy cli argument: give me PROJECT_ID to limit scope
         self.grab_token()
         if 'PROJECT_ID' in os.environ:
             loader = GitLabCIDataLoader(self.config, \
                     project_id=os.environ['PROJECT_ID'])
         else:
             loader = GitLabCIDataLoader(self.config)
-        loader.load_includes()
+        loader.load_files()
         loader.load_blames()
 
     def analyze(self):
         raw = RawDataSet(self.config['output_dir'])
         assembled = AssembledDataSet(raw)
         values = vars(assembled)
         banner = "\n".join([f"{len(values[t].index)} {t}" for t in values])
```

### Comparing `labcrawler-1.0.0/labcrawler/gitlab_ci_config.py` & `labcrawler-1.0.1/labcrawler/gitlab_ci_config.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.0/labcrawler/gitlab_ci_data_loader.py` & `labcrawler-1.0.1/labcrawler/gitlab_ci_data_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,32 +19,34 @@
             self.project_ids = [int(project_id)]    
         else:
             self.project_ids = [p['id'] for p in self.project_file.projects_data]
         self.extractor = GitLabRepositoryFilesExtractor( \
                 gitlab_private_token = environ['GITLAB_PRIVATE_TOKEN'], \
                 gitlab_api_url = config['api_url'] )
 
-    def load_includes(self):
-        """Load the includes (and accidentally full CI config content)"""
-        contents = []  # For a future feature where we write the contents
-        includes = []
+    def load_files(self):
+        """Load the main CI config file and the local includes"""
+        paths = []
         for project_id in self.project_ids:
             project_data = self.project_file.get_project_data(project_id)
+            main_ci_config_path = project_data['ci_config_path'] or '.gitlab-ci.yml'
             ci_config_file_content = self.extractor.extract_file_content( \
                     project_id = project_data['id'], \
                     branch = project_data['default_branch'], \
-                    repo_path = project_data['ci_config_path'] or '.gitlab-ci.yml' )
-            contents.append(ci_config_file_content)
-            ci_config = GitLabCIConfig(ci_config_file_content)
-            if ci_config.locals:
-                for localfile in ci_config.locals:
-                    includes.append({'project_id': project_data['id'], \
-                            'local_include': localfile})
-        self.write_csv(includes, 'ci_config_includes', \
-                ['project_id','local_include'])
+                    repo_path = main_ci_config_path )
+            if ci_config_file_content:
+                paths.append({'project_id': project_data['id'], \
+                        'main': main_ci_config_path})
+                ci_config = GitLabCIConfig(ci_config_file_content)
+                if ci_config.locals:
+                    for localfile in ci_config.locals:
+                        paths.append({'project_id': project_data['id'], \
+                                'local_include': localfile})
+        self.write_csv(paths, 'ci_config_paths', \
+                ['project_id','main','local_include'])
 
     def load_blames(self):
         """Find committer information for main CI config file"""
         committers = []
         for project_id in self.project_ids:
             project_data = self.project_file.get_project_data(project_id)
             project_committers = self.extractor.extract_blamed_committers( \
```

### Comparing `labcrawler-1.0.0/labcrawler/gitlab_repository_files_extractor.py` & `labcrawler-1.0.1/labcrawler/gitlab_repository_files_extractor.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.0/labcrawler/templates/meltano.yml` & `labcrawler-1.0.1/labcrawler/templates/meltano.yml`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.0/labcrawler.egg-info/PKG-INFO` & `labcrawler-1.0.1/labcrawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -146,43 +146,52 @@
 2. Joins raw DataFrames into slightly-more-useful DataFrames with specific names for each datatype
 3. Outputs how many rows are in each DataFrame, with the variable name for each
 4. Starts a Python command-line Python interpreter for querying the resulting DataFrames using Pandas operations
 
 
 ``` python
 
+# List the projects
+projects[['name']]
+
 # See what columns are available in any table
 projects.columns
 
 # View just certain columns from a table
-projects[['path_with_namespace','merge_requests_enabled']]
+projects[['path_with_namespace','merge_method']]
 
 # See how many of each value are included
-projects.value_counts(['merge_requests_enabled'])
+projects.value_counts(['merge_method'])
 
 # Count the total of unmerged branches
 len(branches.loc[~branches['merged']])
 
 # View the number of unmerged branches by project
-branches.loc[~branches['merged']].value_counts(['project_path_with_namespace'])
+branches.loc[~branches['merged']].value_counts(['project_name'])
 
 # See who has access to a project
-project_members.query('project_path_with_namespace == "<replace-with-project-path>"')[['user_username','access_level_name']]
+project_members.query('project_name == "<project-name>"')[['user_username','access_level_name']]
 
 # See who has access to a group
-group_members.query('group_path == "<replace-with-group-path>"')[['username','access_level_name']]
+group_members.query('group_path == "<group-path>"')[['username','access_level_name']]
 
 # How many have each access level
 group_members.value_counts(['access_level_name'])
 
 # Who are the owners and maintainers?
-group_members.query('group_path == "<replace-with-group-path>" and access_level_name in {"Owner","Maintainer}')[['username','access_level_name']]
+group_members.query('group_path == "<group-path>" and access_level_name in ["Owner","Maintainer"]')[['username','access_level_name']]
 
 # See the GitLab CI configuration file path for projects
-projects[['path_with_namespace','ci_config_path']]
+projects[['name','ci_config_path']]
+
+# Which projects have CI configuration at all
+ci_config_paths.query("main.notnull()")[['project_name']]
+
+# Projects without any CI configuration
+ci_config_paths.query("main.isnull() and local_include.isnull()")[['project_name']]
 
 # See who has edited the CI configuration file
 ci_config_committers
 ```
 
 If you want to see all of the rows when performing queries, rather than just a sample, try:
```

### Comparing `labcrawler-1.0.0/labcrawler.egg-info/SOURCES.txt` & `labcrawler-1.0.1/labcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.0/pyproject.toml` & `labcrawler-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.0/test/test_gitlab_ci_config.py` & `labcrawler-1.0.1/test/test_gitlab_ci_config.py`

 * *Files identical despite different names*


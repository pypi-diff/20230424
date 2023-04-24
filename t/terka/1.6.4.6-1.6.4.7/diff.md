# Comparing `tmp/terka-1.6.4.6.tar.gz` & `tmp/terka-1.6.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.4.6.tar", last modified: Sun Apr 23 14:27:29 2023, max compression
+gzip compressed data, was "terka-1.6.4.7.tar", last modified: Mon Apr 24 18:41:26 2023, max compression
```

## Comparing `terka-1.6.4.6.tar` & `terka-1.6.4.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:27:29.391401 terka-1.6.4.6/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-23 14:27:29.391401 terka-1.6.4.6/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-23 14:27:29.391401 terka-1.6.4.6/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      903 2023-04-23 14:27:25.000000 terka-1.6.4.6/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:27:29.387401 terka-1.6.4.6/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 14:06:23.000000 terka-1.6.4.6/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:27:29.387401 terka-1.6.4.6/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.6/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16083 2023-04-23 14:14:21.000000 terka-1.6.4.6/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-23 14:10:47.000000 terka-1.6.4.6/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:27:29.391401 terka-1.6.4.6/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.6/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.6/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41005 2023-04-23 14:11:14.000000 terka-1.6.4.6/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.6/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.6/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      961 2023-04-23 14:11:41.000000 terka-1.6.4.6/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.6/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:27:29.391401 terka-1.6.4.6/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.6/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.6/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.6/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.6/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-23 14:12:42.000000 terka-1.6.4.6/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      955 2023-04-23 14:12:46.000000 terka-1.6.4.6/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.6/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.4.6/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.6/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-23 14:13:11.000000 terka-1.6.4.6/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:27:29.391401 terka-1.6.4.6/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.6/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-23 14:13:55.000000 terka-1.6.4.6/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:27:29.391401 terka-1.6.4.6/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.6/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    27276 2023-04-23 14:14:50.000000 terka-1.6.4.6/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-23 14:14:34.000000 terka-1.6.4.6/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.6/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.6/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     1433 2023-04-23 14:27:11.000000 terka-1.6.4.6/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7747 2023-04-23 14:24:46.000000 terka-1.6.4.6/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:27:29.387401 terka-1.6.4.6/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-23 14:27:29.000000 terka-1.6.4.6/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-23 14:27:29.000000 terka-1.6.4.6/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-23 14:27:29.000000 terka-1.6.4.6/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-23 14:27:29.000000 terka-1.6.4.6/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-23 14:27:29.000000 terka-1.6.4.6/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-23 14:27:29.000000 terka-1.6.4.6/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 18:41:26.596121 terka-1.6.4.7/
+-rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-24 18:41:26.596121 terka-1.6.4.7/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-24 18:41:26.596121 terka-1.6.4.7/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      905 2023-04-24 18:41:17.000000 terka-1.6.4.7/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 18:41:26.592121 terka-1.6.4.7/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 14:06:23.000000 terka-1.6.4.7/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 18:41:26.592121 terka-1.6.4.7/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.7/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16083 2023-04-23 14:14:21.000000 terka-1.6.4.7/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-23 14:10:47.000000 terka-1.6.4.7/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 18:41:26.596121 terka-1.6.4.7/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.7/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.7/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41005 2023-04-23 14:11:14.000000 terka-1.6.4.7/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.7/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.7/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      961 2023-04-23 14:11:41.000000 terka-1.6.4.7/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.7/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 18:41:26.596121 terka-1.6.4.7/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.7/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.7/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.7/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.7/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-23 14:12:42.000000 terka-1.6.4.7/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      955 2023-04-23 14:12:46.000000 terka-1.6.4.7/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.7/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2242 2023-04-24 06:38:30.000000 terka-1.6.4.7/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.7/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-23 14:13:11.000000 terka-1.6.4.7/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 18:41:26.596121 terka-1.6.4.7/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.7/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-23 14:13:55.000000 terka-1.6.4.7/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 18:41:26.596121 terka-1.6.4.7/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.7/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27276 2023-04-23 14:14:50.000000 terka-1.6.4.7/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-23 14:14:34.000000 terka-1.6.4.7/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.7/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.7/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     1427 2023-04-24 18:36:30.000000 terka-1.6.4.7/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7747 2023-04-23 14:24:46.000000 terka-1.6.4.7/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-24 18:41:26.592121 terka-1.6.4.7/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      294 2023-04-24 18:41:26.000000 terka-1.6.4.7/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-24 18:41:26.000000 terka-1.6.4.7/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-24 18:41:26.000000 terka-1.6.4.7/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-04-24 18:41:26.000000 terka-1.6.4.7/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-24 18:41:26.000000 terka-1.6.4.7/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-24 18:41:26.000000 terka-1.6.4.7/terka.egg-info/top_level.txt
```

### Comparing `terka-1.6.4.6/setup.py` & `terka-1.6.4.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.4.6",
+    version="1.6.4.7",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
@@ -20,11 +20,11 @@
     install_requires=[
         "sqlalchemy", "pyaml", "rich", "textual==0.5.0", "plotext==5.2.8"
     ],
     setup_requires=["pytest-runner"],
     tests_requires=["pytest"],
     entry_points={
         "console_scripts": [
-            "terka=src.entrypoints.cli:main"
+            "terka=terka.entrypoints.cli:main"
         ]
     }
 )
```

### Comparing `terka-1.6.4.6/terka/adapters/orm.py` & `terka-1.6.4.7/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/adapters/repository.py` & `terka-1.6.4.7/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/collaborators.py` & `terka-1.6.4.7/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/commands.py` & `terka-1.6.4.7/terka/domain/commands.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/commentary.py` & `terka-1.6.4.7/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/epic.py` & `terka-1.6.4.7/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/event_history.py` & `terka-1.6.4.7/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/project.py` & `terka-1.6.4.7/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/sprint.py` & `terka-1.6.4.7/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/story.py` & `terka-1.6.4.7/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/tag.py` & `terka-1.6.4.7/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/domain/task.py` & `terka-1.6.4.7/terka/domain/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,21 @@
         else:
             self.due_date = due_date
         self.status = self._validate_status(status)
         if priority and priority not in [p.name for p in TaskPriority]:
             raise ValueError(f"{priority} is invalid priority")
         else:
             self.priority = priority
+        self.commentaries: Optional[Set[TaskCommentaries]] = None
+        self.history: Optional[Set[TaskHistory]] = None
+
+    @property
+    def last_modified(self):
+        # TODO: return 
+        pass
 
     def _validate_status(self, status):
         if status and status not in [s.name for s in TaskStatus if s.name != "DELETED"]:
             raise ValueError(f"{status} is invalid status")
         else:
             return status
```

### Comparing `terka-1.6.4.6/terka/domain/time_tracker.py` & `terka-1.6.4.7/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/entrypoints/cli.py` & `terka-1.6.4.7/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/service_layer/printer.py` & `terka-1.6.4.7/terka/service_layer/printer.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/service_layer/services.py` & `terka-1.6.4.7/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/service_layer/ui.py` & `terka-1.6.4.7/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/service_layer/vertical_layout.css` & `terka-1.6.4.7/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka/service_layer/views.py` & `terka-1.6.4.7/terka/service_layer/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,12 +40,12 @@
     return [dict(r) for r in results]
 
 
 def external_connectors_asana_tasks(session, project_id: str) -> List[Dict[int, str]]:
     results = session.execute(
         """
     SELECT
-        id, asana_project_id
-    FROM 'external_connectors.asana.projects'
+        id, asana_task_id
+    FROM 'external_connectors.asana.tasks'
     WHERE project = :project_id
     """, dict(project_id=project_id))
     return [dict(r) for r in results]
```

### Comparing `terka-1.6.4.6/terka/utils.py` & `terka-1.6.4.7/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.6/terka.egg-info/SOURCES.txt` & `terka-1.6.4.7/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/opx_plus-0.1.1.tar.gz` & `tmp/opx_plus-0.1.2.tar.gz`

## Comparing `opx_plus-0.1.1.tar` & `opx_plus-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/.name
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/OPX_Plus.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.1/src/OPX_Plus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opx_plus-0.1.1/src/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 opx_plus-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 opx_plus-0.1.1/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 opx_plus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 opx_plus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.DS_Store
+-rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.2/opx_plus.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 opx_plus-0.1.2/requirements.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 opx_plus-0.1.2/top_level.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/OPX_Plus.iml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opx_plus-0.1.2/src/__init__.py
+-rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.2/src/opx_plus.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 opx_plus-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 opx_plus-0.1.2/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 opx_plus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 opx_plus-0.1.2/PKG-INFO
```

### Comparing `opx_plus-0.1.1/.DS_Store` & `opx_plus-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.1/.idea/workspace.xml` & `opx_plus-0.1.2/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `opx_plus-0.1.1/.idea/workspace.xml` & `opx_plus-0.1.2/.idea/workspace.xml`

```diff
@@ -1,41 +1,48 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="e970cb05-7d56-441a-b2e6-7549de815664" name="Changes" comment="Missed a function in the README.">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+    <list default="true" id="e970cb05-7d56-441a-b2e6-7549de815664" name="Changes" comment="trying some suggestions from jeffrey to make the module install proerply..">
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2OZQewtSMVMqAR3KnAsv3cYG0Po"/>
-  <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
+  <component name="ProjectLevelVcsManager" settingsEditedManually="true">
+    <ConfirmationsSetting value="2" id="Add"/>
+  </component>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;ASKED_ADD_EXTERNAL_FILES&quot;: &quot;true&quot;,
-    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "ASKED_ADD_EXTERNAL_FILES": "true",
+    "RunOnceActivity.OpenProjectViewOnStart": "true",
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "last_opened_file_path": "/Users/stevenwilson/PycharmProjects/opx_plus"
   }
-}</component>
+}]]></component>
+  <component name="RecentsManager">
+    <key name="CopyFile.RECENT_KEYS">
+      <recent name="$PROJECT_DIR$"/>
+    </key>
+  </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="e970cb05-7d56-441a-b2e6-7549de815664" name="Changes" comment=""/>
       <created>1681765722599</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
@@ -86,15 +93,29 @@
     <task id="LOCAL-00007" summary="Missed a function in the README.">
       <created>1681828151662</created>
       <option name="number" value="00007"/>
       <option name="presentableId" value="LOCAL-00007"/>
       <option name="project" value="LOCAL"/>
       <updated>1681828151662</updated>
     </task>
-    <option name="localTasksCounter" value="8"/>
+    <task id="LOCAL-00008" summary="update version fix, replace _ with - in the .toml name">
+      <created>1681836997393</created>
+      <option name="number" value="00008"/>
+      <option name="presentableId" value="LOCAL-00008"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1681836997393</updated>
+    </task>
+    <task id="LOCAL-00009" summary="trying some suggestions from jeffrey to make the module install proerply..">
+      <created>1682289337736</created>
+      <option name="number" value="00009"/>
+      <option name="presentableId" value="LOCAL-00009"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1682289337737</updated>
+    </task>
+    <option name="localTasksCounter" value="10"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
@@ -107,10 +128,12 @@
   <component name="VcsManagerConfiguration">
     <MESSAGE value="git commit"/>
     <MESSAGE value="git commit test 2"/>
     <MESSAGE value="Write README"/>
     <MESSAGE value="I accidentally pasted over a function (copy_over_and_down_formulas -&gt; paste_csv_vals_to_sheet) definition... Fixed!"/>
     <MESSAGE value="List dependencies in README"/>
     <MESSAGE value="Missed a function in the README."/>
-    <option name="LAST_COMMIT_MESSAGE" value="Missed a function in the README."/>
+    <MESSAGE value="update version fix, replace _ with - in the .toml name"/>
+    <MESSAGE value="trying some suggestions from jeffrey to make the module install proerply.."/>
+    <option name="LAST_COMMIT_MESSAGE" value="trying some suggestions from jeffrey to make the module install proerply.."/>
   </component>
 </project>
```

### Comparing `opx_plus-0.1.1/src/OPX_Plus.py` & `opx_plus-0.1.2/opx_plus.py`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.1/LICENSE.txt` & `opx_plus-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.1/README.md` & `opx_plus-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.1/PKG-INFO` & `opx_plus-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: OPX-Plus
-Version: 0.1.1
+Name: opx_plus
+Version: 0.1.2
 Summary: Adds additional functionality on top of OpenPyXL
 Project-URL: Homepage, https://github.com/StevenWilson9/OPX_Plus
 Project-URL: Bug Tracker, https://github.com/StevenWilson9/OPX_Plus/issues
 Author: Steven Wilson
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: openpyxl~=3.0.9
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 OPX_Plus (OpenPyXL Plus) is an extension to [OpenPyXL](https://pypi.org/project/openpyxl/), a module for reading and writing .xlsx and similar files. **OPX_Plus** adds functions centred around creating regular reports based on a template file. You can log issues on the [GitHub page](https://github.com/StevenWilson9/OPX_Plus/issues).
 
 ### Has the Following Dependencies
```


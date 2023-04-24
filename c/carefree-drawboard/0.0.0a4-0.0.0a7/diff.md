# Comparing `tmp/carefree-drawboard-0.0.0a4.tar.gz` & `tmp/carefree-drawboard-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.0a4.tar", last modified: Tue Apr 18 10:07:58 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.0a7.tar", last modified: Mon Apr 24 10:38:20 2023, max compression
```

## Comparing `carefree-drawboard-0.0.0a4.tar` & `carefree-drawboard-0.0.0a7.tar`

### file list

```diff
@@ -1,192 +1,197 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.854997 carefree-drawboard-0.0.0a4/
--rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/LICENSE
--rw-rw-rw-   0        0        0      121 2023-04-18 10:04:06.000000 carefree-drawboard-0.0.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0     9076 2023-04-18 10:07:58.854997 carefree-drawboard-0.0.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     8793 2023-04-18 02:22:15.000000 carefree-drawboard-0.0.0a4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.781726 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     9076 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5363 2023-04-18 10:07:58.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.783719 carefree-drawboard-0.0.0a4/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.786709 carefree-drawboard-0.0.0a4/cfdraw/.web/
--rw-rw-rw-   0        0        0      121 2023-04-18 05:54:36.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1628 2023-04-18 02:10:06.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.789699 carefree-drawboard-0.0.0a4/cfdraw/.web/src/
--rw-rw-rw-   0        0        0      895 2023-04-18 10:06:42.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/BoardPanel.tsx
--rw-rw-rw-   0        0        0     5434 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.794683 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     2174 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0     5947 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.750433 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.794683 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/icons/arrow-down.svg
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.798669 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0      353 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.799667 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFInput.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.800663 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFText.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.802656 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     2940 2023-04-17 06:33:19.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5003 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useUndoRedo.ts
--rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.806643 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2283 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0     6568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.810629 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/
--rw-rw-rw-   0        0        0     2839 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/AddPlugin.tsx
--rw-rw-rw-   0        0        0      870 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4801 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      879 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3545 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1067 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1101 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     6511 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     5093 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2366 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0      906 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.813619 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0     3607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2064 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1951 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
--rw-rw-rw-   0        0        0     1602 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
--rw-rw-rw-   0        0        0      258 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.814615 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.817607 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0     2318 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.818604 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.819600 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0      922 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     3555 2023-04-17 15:25:00.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.821593 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      880 2023-04-17 14:19:55.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.826578 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     3348 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/metaFields.ts
--rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.832561 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0     1431 2023-04-17 09:56:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/_python.ts
--rw-rw-rw-   0        0        0     1495 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/init.ts
--rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/plugins.ts
--rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.835551 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0      466 2023-04-17 06:32:01.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0     1849 2023-04-18 03:53:52.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   214083 2023-04-18 03:11:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a4/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.837544 carefree-drawboard-0.0.0a4/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     3022 2023-04-18 07:46:59.000000 carefree-drawboard-0.0.0a4/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.840534 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      118 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     1944 2023-04-18 06:33:13.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/plugins.py
--rw-rw-rw-   0        0        0     5713 2023-04-17 13:23:53.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     1813 2023-04-18 02:06:49.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     2974 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0      519 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     3485 2023-04-18 08:00:45.000000 carefree-drawboard-0.0.0a4/cfdraw/cli.py
--rw-rw-rw-   0        0        0     2226 2023-04-18 07:55:50.000000 carefree-drawboard-0.0.0a4/cfdraw/config.py
--rw-rw-rw-   0        0        0     1479 2023-04-18 07:48:42.000000 carefree-drawboard-0.0.0a4/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.841530 carefree-drawboard-0.0.0a4/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0     6203 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.843524 carefree-drawboard-0.0.0a4/cfdraw/plugins/
--rw-rw-rw-   0        0        0      113 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/__init__.py
--rw-rw-rw-   0        0        0     4367 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.843524 carefree-drawboard-0.0.0a4/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     2407 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/factory.py
--rw-rw-rw-   0        0        0     1956 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/meta.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.845027 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0       71 2023-04-13 03:23:59.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/fields.py
--rw-rw-rw-   0        0        0      671 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/text_area.py
--rw-rw-rw-   0        0        0      795 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/timer.py
--rw-rw-rw-   0        0        0     1090 2023-04-17 09:56:46.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/sync.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.847024 carefree-drawboard-0.0.0a4/cfdraw/schema/
--rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0     9673 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/plugins.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.849017 carefree-drawboard-0.0.0a4/cfdraw/server/
--rw-rw-rw-   0        0        0     1194 2023-04-18 09:42:33.000000 carefree-drawboard-0.0.0a4/cfdraw/server/__init__.py
--rw-rw-rw-   0        0        0     1185 2023-04-18 07:04:07.000000 carefree-drawboard-0.0.0a4/cfdraw/server/http.py
--rw-rw-rw-   0        0        0      381 2023-04-18 07:40:33.000000 carefree-drawboard-0.0.0a4/cfdraw/server/index.py
--rw-rw-rw-   0        0        0     1459 2023-04-18 07:40:19.000000 carefree-drawboard-0.0.0a4/cfdraw/server/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.854001 carefree-drawboard-0.0.0a4/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     2781 2023-04-18 07:55:53.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     3667 2023-04-17 13:24:23.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2733 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-04-18 10:07:58.855994 carefree-drawboard-0.0.0a4/setup.cfg
--rw-rw-rw-   0        0        0     1054 2023-04-18 10:07:27.000000 carefree-drawboard-0.0.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.891778 carefree-drawboard-0.0.0a7/
+-rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a7/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-04-18 10:04:06.000000 carefree-drawboard-0.0.0a7/MANIFEST.in
+-rw-rw-rw-   0        0        0     8996 2023-04-24 10:38:20.891778 carefree-drawboard-0.0.0a7/PKG-INFO
+-rw-rw-rw-   0        0        0     8713 2023-04-24 10:36:28.000000 carefree-drawboard-0.0.0a7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.820781 carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     8996 2023-04-24 10:38:18.000000 carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5639 2023-04-24 10:38:20.000000 carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:38:18.000000 carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:38:18.000000 carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-04-24 10:38:18.000000 carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 10:38:18.000000 carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.822778 carefree-drawboard-0.0.0a7/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.827778 carefree-drawboard-0.0.0a7/cfdraw/.web/
+-rw-rw-rw-   0        0        0      121 2023-04-18 05:54:36.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1628 2023-04-18 02:10:06.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.830778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0      977 2023-04-24 08:35:50.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     1454 2023-04-24 07:30:21.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/BoardPanel.tsx
+-rw-rw-rw-   0        0        0     5803 2023-04-24 07:18:40.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.835778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     2249 2023-04-19 04:21:39.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0     5952 2023-04-23 08:04:37.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1292 2023-04-24 04:34:26.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.792781 carefree-drawboard-0.0.0a7/cfdraw/.web/src/assets/
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.835778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/assets/icons/arrow-down.svg
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.839779 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0      723 2023-04-22 13:46:05.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      640 2023-04-24 02:04:13.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFCircularProgress.tsx
+-rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.840778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFInput.tsx
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.841778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFSelect/
+-rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFSelect/index.scss
+-rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFSelect/index.tsx
+-rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFText.tsx
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.844778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     2940 2023-04-17 06:33:19.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     5241 2023-04-24 07:07:26.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.848778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2302 2023-04-23 08:04:44.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0     7075 2023-04-21 10:12:04.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     1788 2023-04-24 03:25:59.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.854779 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/
+-rw-rw-rw-   0        0        0     2806 2023-04-23 04:26:50.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      876 2023-04-23 04:26:57.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4807 2023-04-23 04:27:02.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      852 2023-04-23 04:27:13.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     3471 2023-04-23 04:27:24.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1081 2023-04-23 04:27:32.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1121 2023-04-23 04:21:09.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     1309 2023-04-24 04:42:50.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/MetaPlugin.tsx
+-rw-rw-rw-   0        0        0     6478 2023-04-23 04:27:51.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     5072 2023-04-24 04:34:26.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     2372 2023-04-23 04:28:10.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0     1251 2023-04-24 08:34:30.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.857778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0      685 2023-04-21 06:07:38.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
+-rw-rw-rw-   0        0        0     3923 2023-04-24 04:50:52.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+-rw-rw-rw-   0        0        0     2855 2023-04-24 07:25:56.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1945 2023-04-24 04:47:37.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+-rw-rw-rw-   0        0        0     1755 2023-04-24 04:48:29.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0      851 2023-04-24 04:49:31.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.859778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.862778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0    11005 2023-04-24 10:31:02.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0     7028 2023-04-24 06:13:05.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0      225 2023-04-21 05:52:53.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/hooks.ts
+-rw-rw-rw-   0        0        0     2343 2023-04-24 04:34:26.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.863778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.864778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0     1028 2023-04-19 04:57:46.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     2546 2023-04-24 07:30:12.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.865778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-04-17 14:19:55.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.867778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     3848 2023-04-24 04:08:32.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1758 2023-04-24 04:08:41.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/metaFields.ts
+-rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3137 2023-04-24 06:12:21.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.874778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0     1531 2023-04-24 07:46:09.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/_python.ts
+-rw-rw-rw-   0        0        0      586 2023-04-24 06:37:16.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/debug.ts
+-rw-rw-rw-   0        0        0     1495 2023-04-21 10:35:17.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/init.ts
+-rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     1561 2023-04-24 08:27:40.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/pluginVisible.ts
+-rw-rw-rw-   0        0        0     2505 2023-04-24 08:59:38.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/plugins.ts
+-rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     6076 2023-04-24 07:30:05.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/socket.ts
+-rw-rw-rw-   0        0        0     3845 2023-04-24 08:00:35.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2031 2023-04-24 04:34:26.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/ui.ts
+-rw-rw-rw-   0        0        0      866 2023-04-23 10:06:41.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/user.ts
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.876778 carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0      533 2023-04-24 02:26:58.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1091 2023-04-24 04:41:20.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     1849 2023-04-18 03:53:52.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   214083 2023-04-18 03:11:54.000000 carefree-drawboard-0.0.0a7/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      487 2023-04-24 10:12:18.000000 carefree-drawboard-0.0.0a7/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.877778 carefree-drawboard-0.0.0a7/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-23 08:15:58.000000 carefree-drawboard-0.0.0a7/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.880778 carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      139 2023-04-23 08:15:42.000000 carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-04-21 12:01:39.000000 carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/assets.py
+-rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     5713 2023-04-19 04:49:15.000000 carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     5918 2023-04-24 09:42:11.000000 carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/queue.py
+-rw-rw-rw-   0        0        0     2158 2023-04-19 04:21:46.000000 carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     3323 2023-04-24 09:42:32.000000 carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0     1392 2023-04-24 01:32:44.000000 carefree-drawboard-0.0.0a7/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     3333 2023-04-22 02:31:01.000000 carefree-drawboard-0.0.0a7/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2245 2023-04-21 12:04:53.000000 carefree-drawboard-0.0.0a7/cfdraw/config.py
+-rw-rw-rw-   0        0        0     1456 2023-04-21 11:42:04.000000 carefree-drawboard-0.0.0a7/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.881778 carefree-drawboard-0.0.0a7/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a7/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a7/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0     6847 2023-04-24 01:38:38.000000 carefree-drawboard-0.0.0a7/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.883778 carefree-drawboard-0.0.0a7/cfdraw/plugins/
+-rw-rw-rw-   0        0        0       92 2023-04-23 04:40:40.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4944 2023-04-24 10:13:38.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.883778 carefree-drawboard-0.0.0a7/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-04-22 12:17:12.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.885778 carefree-drawboard-0.0.0a7/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0      100 2023-04-23 09:08:34.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-04-23 09:30:55.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/middlewares/fields.py
+-rw-rw-rw-   0        0        0      728 2023-04-24 01:32:44.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/middlewares/send_message.py
+-rw-rw-rw-   0        0        0      500 2023-04-23 09:31:13.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/middlewares/text_area.py
+-rw-rw-rw-   0        0        0      962 2023-04-23 10:00:12.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/middlewares/timer.py
+-rw-rw-rw-   0        0        0      920 2023-04-23 10:00:12.000000 carefree-drawboard-0.0.0a7/cfdraw/plugins/sync.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.886778 carefree-drawboard-0.0.0a7/cfdraw/schema/
+-rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a7/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a7/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0    12906 2023-04-24 01:32:44.000000 carefree-drawboard-0.0.0a7/cfdraw/schema/plugins.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:38:20.890778 carefree-drawboard-0.0.0a7/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     6414 2023-04-23 02:50:50.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/data_structures.py
+-rw-rw-rw-   0        0        0     2622 2023-04-22 02:30:59.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0     1691 2023-04-24 10:15:42.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/misc.py
+-rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     3667 2023-04-17 13:24:23.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2691 2023-04-23 10:00:12.000000 carefree-drawboard-0.0.0a7/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-04-24 10:38:20.894779 carefree-drawboard-0.0.0a7/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-04-24 10:37:23.000000 carefree-drawboard-0.0.0a7/setup.py
```

### Comparing `carefree-drawboard-0.0.0a4/LICENSE` & `carefree-drawboard-0.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/PKG-INFO` & `carefree-drawboard-0.0.0a7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a4
+Version: 0.0.0a7
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,20 +12,20 @@
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
+### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
@@ -57,34 +57,34 @@
 
 Create a folder (e.g., `my_fancy_app`) wherever you like, get into it, and run
 
 ```bash
 cfdraw init
 ```
 
-> When you run this command for the first time, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
-
 This command will write two files to your folder (`my_fancy_app`). After which you can run the app in development mode:
 
 ```bash
 cfdraw run
 ```
 
+> When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
+
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
-> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dropping on directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
+> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
 
 ## Examples
 
-* [Getting Started](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
+* [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
-* [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
+* [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
@@ -98,18 +98,16 @@
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
 * **GitHub Discussions**: Currently the best way to chat around.
 * **GitHub Issues**: Bugs! Fixes! PRs!.
 
 Apart from these:
+* It might be the best to start from the [Contributing](https://github.com/carefree0910/carefree-drawboard/wiki/Contributing) Wiki page.
 * If you are truly an enthusiast, you may check out our [Roadmap](https://github.com/carefree0910/carefree-drawboard/wiki/Roadmap), pick up what you are interested, and create the corresponding PR!
-* If you are familiar with `React`, you may check out the [Customizations](https://github.com/carefree0910/carefree-drawboard/wiki/Customizations) documentation and try to customize your own plugins and have fun!
-
-> It is also recommended to start from the [Development Guide](https://github.com/carefree0910/carefree-drawboard/wiki/Development-Guide)!
 
 ### Style Guide
 
 If you are still interested: `carefree-drawboard` 🎨 adopted [`black`](https://github.com/psf/black) and [`mypy`](https://github.com/python/mypy) to stylize its codes, so you may need to check the format, coding style and type hint with them before your codes could actually be merged.
 
 ## Q&A
 
@@ -125,20 +123,20 @@
 
 > 🎨 (Artist Palette) - This emoji represents creativity, design, and artistic expression, which are all key aspects of the `carefree-drawboard` 🎨 platform.
 
 Cool!
 
 ### Will there be a Discord Community?
 
-Unfortunately I'm Chinese and I can hardly access to Discord. 🤣 Even if there are someone kindly enough to build one up for me, I can hardly connect to it so it will be impossible for me to stay tuned.
-
-If you are kind enough please use the **GitHub Discussions**, or maybe there are other Discord replacements? I don't know, help!!!
+Many thanks to [JSDu](https://github.com/JamesBonddu), who created a [Discord channel](https://discord.gg/UkfpFFmNd2) for my projects!!
 
 如果有热心观众对这个项目感兴趣并愿意帮忙建立一个中文社区，欢迎联系我，我会非常感激的！！
 
+**更新：** 热心观众（[JSDu](https://github.com/JamesBonddu)）出现啦！非常感谢！！！（猛戳[这里](https://discord.gg/UkfpFFmNd2)加入我们！）
+
 ### Why do you build this project?
 
 > Also check [Design Philosophy](https://github.com/carefree0910/carefree-drawboard/wiki/Design-Philosophy).
 
 In short, I believe that:
 * Infinite Drawboard can unleash Infinite possibilities.
 * If we can use `Python` to interact with it and even craft new plugins for it, it will be even better.
```

### Comparing `carefree-drawboard-0.0.0a4/README.md` & `carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+Metadata-Version: 2.1
+Name: carefree-drawboard
+Version: 0.0.0a7
+Summary: 🎨 Infinite Drawboard in Python
+Author: carefree0910
+Author-email: syameimaru.saki@gmail.com
+Keywords: python carefree-learn drawboard
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # carefree-drawboard 🎨
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
+### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
@@ -47,34 +57,34 @@
 
 Create a folder (e.g., `my_fancy_app`) wherever you like, get into it, and run
 
 ```bash
 cfdraw init
 ```
 
-> When you run this command for the first time, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
-
 This command will write two files to your folder (`my_fancy_app`). After which you can run the app in development mode:
 
 ```bash
 cfdraw run
 ```
 
+> When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
+
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
-> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dropping on directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
+> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
 
 ## Examples
 
-* [Getting Started](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
+* [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
-* [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
+* [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
@@ -88,18 +98,16 @@
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
 * **GitHub Discussions**: Currently the best way to chat around.
 * **GitHub Issues**: Bugs! Fixes! PRs!.
 
 Apart from these:
+* It might be the best to start from the [Contributing](https://github.com/carefree0910/carefree-drawboard/wiki/Contributing) Wiki page.
 * If you are truly an enthusiast, you may check out our [Roadmap](https://github.com/carefree0910/carefree-drawboard/wiki/Roadmap), pick up what you are interested, and create the corresponding PR!
-* If you are familiar with `React`, you may check out the [Customizations](https://github.com/carefree0910/carefree-drawboard/wiki/Customizations) documentation and try to customize your own plugins and have fun!
-
-> It is also recommended to start from the [Development Guide](https://github.com/carefree0910/carefree-drawboard/wiki/Development-Guide)!
 
 ### Style Guide
 
 If you are still interested: `carefree-drawboard` 🎨 adopted [`black`](https://github.com/psf/black) and [`mypy`](https://github.com/python/mypy) to stylize its codes, so you may need to check the format, coding style and type hint with them before your codes could actually be merged.
 
 ## Q&A
 
@@ -115,20 +123,20 @@
 
 > 🎨 (Artist Palette) - This emoji represents creativity, design, and artistic expression, which are all key aspects of the `carefree-drawboard` 🎨 platform.
 
 Cool!
 
 ### Will there be a Discord Community?
 
-Unfortunately I'm Chinese and I can hardly access to Discord. 🤣 Even if there are someone kindly enough to build one up for me, I can hardly connect to it so it will be impossible for me to stay tuned.
-
-If you are kind enough please use the **GitHub Discussions**, or maybe there are other Discord replacements? I don't know, help!!!
+Many thanks to [JSDu](https://github.com/JamesBonddu), who created a [Discord channel](https://discord.gg/UkfpFFmNd2) for my projects!!
 
 如果有热心观众对这个项目感兴趣并愿意帮忙建立一个中文社区，欢迎联系我，我会非常感激的！！
 
+**更新：** 热心观众（[JSDu](https://github.com/JamesBonddu)）出现啦！非常感谢！！！（猛戳[这里](https://discord.gg/UkfpFFmNd2)加入我们！）
+
 ### Why do you build this project?
 
 > Also check [Design Philosophy](https://github.com/carefree0910/carefree-drawboard/wiki/Design-Philosophy).
 
 In short, I believe that:
 * Infinite Drawboard can unleash Infinite possibilities.
 * If we can use `Python` to interact with it and even craft new plugins for it, it will be even better.
```

### Comparing `carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.0a7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,21 @@
-Metadata-Version: 2.1
-Name: carefree-drawboard
-Version: 0.0.0a4
-Summary: 🎨 Infinite Drawboard in Python
-Author: carefree0910
-Author-email: syameimaru.saki@gmail.com
-Keywords: python carefree-learn drawboard
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # carefree-drawboard 🎨
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
+### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
@@ -57,34 +47,34 @@
 
 Create a folder (e.g., `my_fancy_app`) wherever you like, get into it, and run
 
 ```bash
 cfdraw init
 ```
 
-> When you run this command for the first time, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
-
 This command will write two files to your folder (`my_fancy_app`). After which you can run the app in development mode:
 
 ```bash
 cfdraw run
 ```
 
+> When you run this command for the first time and have not called `cfdraw install` before, we will use `yarn` to install the JavaScript dependencies for you, which may be quite slow!
+
 And you should see your app running at http://localhost:5123. Now you can play with the generated `app.py` file and see warm reload (yeah, not hot enough because we rely on the `reload` provided by `uvicorn` 🤣).
 
-> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dropping on directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
+> Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/232184463-627c2cd7-728a-49ce-93c6-7c878edc27b9.mp4)
 
 ## Examples
 
-* [Getting Started](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
+* [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
 * [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
 * [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
-* [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
+* [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
 * [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
 * [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
@@ -98,18 +88,16 @@
 
 Contributions are truly welcomed! Here are some good (common) ways to get started:
 
 * **GitHub Discussions**: Currently the best way to chat around.
 * **GitHub Issues**: Bugs! Fixes! PRs!.
 
 Apart from these:
+* It might be the best to start from the [Contributing](https://github.com/carefree0910/carefree-drawboard/wiki/Contributing) Wiki page.
 * If you are truly an enthusiast, you may check out our [Roadmap](https://github.com/carefree0910/carefree-drawboard/wiki/Roadmap), pick up what you are interested, and create the corresponding PR!
-* If you are familiar with `React`, you may check out the [Customizations](https://github.com/carefree0910/carefree-drawboard/wiki/Customizations) documentation and try to customize your own plugins and have fun!
-
-> It is also recommended to start from the [Development Guide](https://github.com/carefree0910/carefree-drawboard/wiki/Development-Guide)!
 
 ### Style Guide
 
 If you are still interested: `carefree-drawboard` 🎨 adopted [`black`](https://github.com/psf/black) and [`mypy`](https://github.com/python/mypy) to stylize its codes, so you may need to check the format, coding style and type hint with them before your codes could actually be merged.
 
 ## Q&A
 
@@ -125,20 +113,20 @@
 
 > 🎨 (Artist Palette) - This emoji represents creativity, design, and artistic expression, which are all key aspects of the `carefree-drawboard` 🎨 platform.
 
 Cool!
 
 ### Will there be a Discord Community?
 
-Unfortunately I'm Chinese and I can hardly access to Discord. 🤣 Even if there are someone kindly enough to build one up for me, I can hardly connect to it so it will be impossible for me to stay tuned.
-
-If you are kind enough please use the **GitHub Discussions**, or maybe there are other Discord replacements? I don't know, help!!!
+Many thanks to [JSDu](https://github.com/JamesBonddu), who created a [Discord channel](https://discord.gg/UkfpFFmNd2) for my projects!!
 
 如果有热心观众对这个项目感兴趣并愿意帮忙建立一个中文社区，欢迎联系我，我会非常感激的！！
 
+**更新：** 热心观众（[JSDu](https://github.com/JamesBonddu)）出现啦！非常感谢！！！（猛戳[这里](https://discord.gg/UkfpFFmNd2)加入我们！）
+
 ### Why do you build this project?
 
 > Also check [Design Philosophy](https://github.com/carefree0910/carefree-drawboard/wiki/Design-Philosophy).
 
 In short, I believe that:
 * Infinite Drawboard can unleash Infinite possibilities.
 * If we can use `Python` to interact with it and even craft new plugins for it, it will be even better.
```

### Comparing `carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.0a7/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 cfdraw/.web/src/actions/importMeta.ts
 cfdraw/.web/src/actions/managePlugins.ts
 cfdraw/.web/src/actions/manageProjects.ts
 cfdraw/.web/src/actions/update.ts
 cfdraw/.web/src/actions/uploadImage.ts
 cfdraw/.web/src/assets/icons/arrow-down.svg
 cfdraw/.web/src/components/CFButton.tsx
+cfdraw/.web/src/components/CFCircularProgress.tsx
 cfdraw/.web/src/components/CFDivider.tsx
 cfdraw/.web/src/components/CFHeading.tsx
 cfdraw/.web/src/components/CFImageUploader.tsx
 cfdraw/.web/src/components/CFInput.tsx
 cfdraw/.web/src/components/CFSlider.tsx
 cfdraw/.web/src/components/CFSwitch.tsx
 cfdraw/.web/src/components/CFText.tsx
@@ -54,15 +55,14 @@
 cfdraw/.web/src/components/CFSelect/index.scss
 cfdraw/.web/src/components/CFSelect/index.tsx
 cfdraw/.web/src/hooks/useFileDropper.ts
 cfdraw/.web/src/hooks/useGridLines.ts
 cfdraw/.web/src/hooks/useInitBoard.ts
 cfdraw/.web/src/hooks/usePreventDefaults.ts
 cfdraw/.web/src/hooks/usePython.ts
-cfdraw/.web/src/hooks/useUndoRedo.ts
 cfdraw/.web/src/lang/add.ts
 cfdraw/.web/src/lang/brush.ts
 cfdraw/.web/src/lang/download.ts
 cfdraw/.web/src/lang/index.ts
 cfdraw/.web/src/lang/nodeEditor.ts
 cfdraw/.web/src/lang/plugins.ts
 cfdraw/.web/src/lang/projects.ts
@@ -72,27 +72,30 @@
 cfdraw/.web/src/plugins/AddPlugin.tsx
 cfdraw/.web/src/plugins/ArrangePlugin.tsx
 cfdraw/.web/src/plugins/BrushPlugin.tsx
 cfdraw/.web/src/plugins/DeletePlugin.tsx
 cfdraw/.web/src/plugins/DownloadPlugin.tsx
 cfdraw/.web/src/plugins/GroupPlugin.tsx
 cfdraw/.web/src/plugins/LinksPlugin.tsx
+cfdraw/.web/src/plugins/MetaPlugin.tsx
 cfdraw/.web/src/plugins/ProjectPlugin.tsx
 cfdraw/.web/src/plugins/SettingsPlugin.tsx
 cfdraw/.web/src/plugins/TextEditorPlugin.tsx
 cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
 cfdraw/.web/src/plugins/index.tsx
-cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
-cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
-cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
-cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
+cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
+cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
 cfdraw/.web/src/plugins/_python/hooks.ts
 cfdraw/.web/src/plugins/components/Floating.tsx
 cfdraw/.web/src/plugins/components/Link.tsx
 cfdraw/.web/src/plugins/components/Render.tsx
+cfdraw/.web/src/plugins/components/hooks.ts
 cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
 cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
 cfdraw/.web/src/plugins/components/Fields/TextField.tsx
 cfdraw/.web/src/plugins/components/Fields/index.tsx
 cfdraw/.web/src/plugins/components/Fields/utils.ts
 cfdraw/.web/src/plugins/utils/factory.ts
 cfdraw/.web/src/plugins/utils/renderFilters.ts
@@ -103,57 +106,60 @@
 cfdraw/.web/src/schema/_python.ts
 cfdraw/.web/src/schema/meta.ts
 cfdraw/.web/src/schema/metaFields.ts
 cfdraw/.web/src/schema/misc.ts
 cfdraw/.web/src/schema/plugins.ts
 cfdraw/.web/src/schema/requests.ts
 cfdraw/.web/src/stores/_python.ts
+cfdraw/.web/src/stores/debug.ts
 cfdraw/.web/src/stores/gridLines.ts
 cfdraw/.web/src/stores/hooks.ts
 cfdraw/.web/src/stores/init.ts
 cfdraw/.web/src/stores/meta.ts
+cfdraw/.web/src/stores/pluginVisible.ts
 cfdraw/.web/src/stores/plugins.ts
 cfdraw/.web/src/stores/projects.ts
+cfdraw/.web/src/stores/socket.ts
 cfdraw/.web/src/stores/theme.ts
 cfdraw/.web/src/stores/ui.ts
+cfdraw/.web/src/stores/user.ts
 cfdraw/.web/src/utils/bem.ts
 cfdraw/.web/src/utils/constants.ts
 cfdraw/.web/src/utils/event.ts
 cfdraw/.web/src/utils/misc.ts
 cfdraw/.web/src/utils/toast.ts
 cfdraw/app/__init__.py
 cfdraw/app/app.py
 cfdraw/app/schema.py
 cfdraw/app/endpoints/__init__.py
+cfdraw/app/endpoints/assets.py
 cfdraw/app/endpoints/base.py
-cfdraw/app/endpoints/plugins.py
 cfdraw/app/endpoints/project.py
+cfdraw/app/endpoints/queue.py
 cfdraw/app/endpoints/upload.py
 cfdraw/app/endpoints/websocket.py
 cfdraw/parsers/__init__.py
 cfdraw/parsers/chakra.py
 cfdraw/parsers/noli.py
 cfdraw/plugins/__init__.py
 cfdraw/plugins/base.py
 cfdraw/plugins/factory.py
-cfdraw/plugins/meta.py
 cfdraw/plugins/sync.py
 cfdraw/plugins/community/__init__.py
 cfdraw/plugins/middlewares/__init__.py
 cfdraw/plugins/middlewares/fields.py
+cfdraw/plugins/middlewares/send_message.py
 cfdraw/plugins/middlewares/text_area.py
 cfdraw/plugins/middlewares/timer.py
 cfdraw/schema/__init__.py
 cfdraw/schema/fields.py
 cfdraw/schema/plugins.py
-cfdraw/server/__init__.py
-cfdraw/server/http.py
-cfdraw/server/index.py
-cfdraw/server/socket.py
 cfdraw/utils/__init__.py
 cfdraw/utils/cache.py
 cfdraw/utils/console.py
+cfdraw/utils/data_structures.py
 cfdraw/utils/exec.py
+cfdraw/utils/misc.py
 cfdraw/utils/prerequisites.py
 cfdraw/utils/processes.py
 cfdraw/utils/server.py
 cfdraw/utils/template.py
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/package.json` & `carefree-drawboard-0.0.0a7/cfdraw/.web/package.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/App.tsx`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import { Flex } from "@chakra-ui/react";
 import { observer } from "mobx-react-lite";
 
 import { langStore } from "@carefree0910/business";
 
+import { useWebSocket } from "./stores/socket";
+import { useUserInitialization } from "./stores/user";
 import { useInitBoard } from "./hooks/useInitBoard";
 import { useFileDropper } from "./hooks/useFileDropper";
 import { useGridLines } from "./hooks/useGridLines";
 import { usePreventDefaults } from "./hooks/usePreventDefaults";
-import { useUndoRedo } from "./hooks/useUndoRedo";
 import { useSyncPython } from "./hooks/usePython";
 import BoardPanel from "./BoardPanel";
 
 function App() {
+  useWebSocket();
+  useUserInitialization();
   useSyncPython();
   useInitBoard();
   useFileDropper(langStore.tgt);
   useGridLines();
-  useUndoRedo();
   usePreventDefaults();
 
   return (
     <Flex h="100vh" className="p-editor" direction="column" userSelect="none">
       <Flex w="100%" flex={1}>
         <BoardPanel />
       </Flex>
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/BoardPanel.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/BoardPanel.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import { BOARD_CONTAINER_ID } from "@/utils/constants";
 import { makePlugin } from "@/plugins";
 
 function BoardPanel() {
   const ref = useRef(null);
   const isReady = useIsReady();
   const { boardBg } = themeStore.styles;
-  const Wrapper = pythonStore.globalSettings.useStrictMode ? React.StrictMode : React.Fragment;
+  const Wrapper = pythonStore.globalSettings?.useStrictMode ? React.StrictMode : React.Fragment;
 
   return (
     <>
       <Flex h="100%" flex={1} direction="column">
         <Box w="100%" h="100%" bg={boardBg}>
           <Box id={BOARD_CONTAINER_ID} visibility={isReady ? "visible" : "hidden"}></Box>
         </Box>
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/_settings.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/_settings.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 import type { AvailablePlugins, IMakePlugin } from "@/schema/plugins";
 
 export const reactPluginSettings: IMakePlugin<AvailablePlugins>[] = [
   {
+    type: "meta",
+    props: {
+      nodeConstraint: "singleNode",
+      renderInfo: {
+        w: 400,
+        h: 400,
+        offsetY: 48,
+        src: "https://ailab-huawei-cdn.nolibox.com/upload/images/0ec1b08f9c3e4ef4813ecb80bebf3b42.png",
+        pivot: "rt",
+        follow: true,
+      },
+      pluginInfo: {},
+    },
+  },
+  {
     type: "settings",
     props: {
       nodeConstraint: "none",
       renderInfo: {
         w: 300,
         h: 400,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/49223052f17f4f249c56ba00f43b3043.png",
@@ -14,113 +29,113 @@
       },
       pluginInfo: {},
     },
   },
   {
     type: "project",
     props: {
-      offsetY: 64,
       nodeConstraint: "none",
       renderInfo: {
         w: 300,
         h: 400,
+        offsetY: 64,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/255c1c20b5754815b759969218f8a87c.png",
         pivot: "rt",
         follow: false,
       },
       pluginInfo: {},
     },
   },
   {
     type: "add",
     props: {
       p: "14px",
-      offsetY: 120,
       nodeConstraint: "none",
       renderInfo: {
         w: 300,
         h: 225,
+        offsetY: 120,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/81a82eca03224bc2bb8de65c08f2f48a.png",
         pivot: "rt",
         follow: false,
       },
       pluginInfo: {},
     },
   },
   {
     type: "arrange",
     props: {
-      offsetY: 48,
       nodeConstraint: "multiNode",
       renderInfo: {
         w: 0,
         h: 0,
+        offsetY: 48,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/7fcc3fb8a25248b0a1f2ca68b0c975f4.png",
         pivot: "rt",
         follow: true,
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
     type: "undo",
     props: {
       p: "14px",
-      offsetX: -28,
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
+        offsetX: -28,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/069122c037d34d97ba10157438af131b.png",
         pivot: "top",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
     type: "redo",
     props: {
       p: "14px",
-      offsetX: 28,
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
+        offsetX: 28,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/4c0b2343838344fdb574520006aa83c9.png",
         pivot: "top",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
     type: "download",
     props: {
-      offsetY: -48,
       nodeConstraint: "anyNode",
       renderInfo: {
         w: 240,
         h: 230,
+        offsetY: -48,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/d871d80a875146fa8aabc09fbbdef47e.png",
         pivot: "rb",
         follow: true,
       },
       pluginInfo: {},
     },
   },
   {
     type: "delete",
     props: {
-      offsetY: -48,
       nodeConstraint: "anyNode",
       renderInfo: {
         w: 0,
         h: 0,
+        offsetY: -48,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/384b2261faa748e6b57e14e697e19520.png",
         pivot: "lb",
         follow: true,
       },
       pluginInfo: {},
       noExpand: true,
     },
@@ -174,19 +189,19 @@
   },
   {
     type: "brush",
     props: {
       p: "0px",
       pl: "10px",
       pr: "7px",
-      offsetY: 176,
       nodeConstraint: "none",
       renderInfo: {
         w: 300,
         h: 220,
+        offsetY: 176,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/static/brush.svg",
         pivot: "rt",
         follow: false,
       },
       pluginInfo: {},
     },
   },
@@ -203,34 +218,34 @@
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
     type: "email",
     props: {
-      offsetX: -120,
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
+        offsetX: -120,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/7ff42ebb21664a9abb55331463951126.png",
         pivot: "rb",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
     type: "github",
     props: {
-      offsetX: -64,
       nodeConstraint: "none",
       renderInfo: {
         w: 0,
         h: 0,
+        offsetX: -64,
         src: "https://ailab-huawei-cdn.nolibox.com/upload/images/4fb8d24d515744f6ac6836b3ba12a649.png",
         pivot: "rb",
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/export.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import { INode, ISingleNode, Lang, toJsonBlob } from "@carefree0910/core";
 import { ExportBlobOptions, exportBlob, exportNodes } from "@carefree0910/svg";
 import { translate } from "@carefree0910/business";
 
 import type { DownloadFormat, IToast, ImageFormat } from "@/schema/misc";
 import { toast } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
+import { Requests } from "@/requests/actions";
 import { uploadImage } from "./uploadImage";
 
 const isImage = (format: DownloadFormat) => format === "JPG" || format === "PNG";
-const toJpegUrl = (url: string) => `${url}?jpeg=True`;
+
+function fetchImage(data: { url: string; jpeg: boolean }): Promise<Blob> {
+  return Requests.postJson<Blob>("_python", "/fetch_image", data, "blob");
+}
 
 export type IExportBlob = ExportBlobOptions & { t: IToast; lang: Lang };
 export class Exporter {
   static async exportBlob(
     nodes: ISingleNode[],
     { t, lang, ...others }: IExportBlob,
   ): Promise<Blob | void> {
@@ -26,33 +30,30 @@
   static async exportOne(
     t: IToast,
     lang: Lang,
     node: INode,
     format: ImageFormat,
     exportOriginalSize: boolean,
   ): Promise<Blob | void> {
+    const jpeg = format === "JPG";
     if (isImage(format) && node.type === "image" && exportOriginalSize) {
-      let url = node.renderParams.src;
-      if (format === "JPG") {
-        url = toJpegUrl(url);
-      }
-      return fetch(url).then((res) => res.blob());
+      return fetchImage({ url: node.renderParams.src, jpeg });
     }
     const bounding = node.bbox.bounding.toAABB();
     const targetNodes = node.type === "group" ? node.allChildrenNodes : [node];
     if (isImage(format)) {
       const blob = await Exporter.exportBlob(targetNodes, {
         t,
         lang,
         exportOptions: { exportBox: bounding },
       });
       if (!blob || format !== "JPG") return blob;
       const res = await uploadImage(t, lang, blob, { failed: async () => void 0 });
       if (!res) return;
-      return fetch(toJpegUrl(res.url)).then((res) => res.blob());
+      return fetchImage({ url: res.url, jpeg: true });
     }
     const res = await exportNodes(targetNodes, { exportBox: bounding });
     if (!res) {
       toast(t, "error", translate(Toast_Words["export-blob-error-message"], lang));
       return;
     }
     return toJsonBlob(res.svg.svg());
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/importMeta.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import { Dictionary, RectangleShapeNode, getRandomHash, shallowCopy } from "@carefree0910/core";
 import { BoardStore, translate, useAddNode } from "@carefree0910/business";
 
-import type { IMetaData, MetaType } from "@/schema/meta";
+import type { IMetaData, IPythonFieldsMetaData, MetaType } from "@/schema/meta";
 import type { IImportMeta } from "@/schema/meta";
 import { toast } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { themeStore } from "@/stores/theme";
 import { updateMeta } from "./update";
 import { addNewText } from "./addText";
 import { addNewImage, getNewRectangle, INewRectangle, NewImageInfo } from "./addImage";
@@ -24,27 +24,28 @@
   updateMeta(alias, node.params.meta);
 }
 
 const consumers: Record<MetaType, (input: IImportMeta<any>) => void> = {
   upload: consumeUpload,
   "add.text": consumeAddText,
   "add.sketch.path": consumeAddSketchPath,
-  "python.httpFields": consumePythonHttpFields,
+  "python.fields": consumePythonFields,
 };
 function consumeUpload({ t, lang, type, metaData }: IImportMeta<"upload">): void {
   const success = async () => {
     toast(t, "success", translate(Toast_Words["upload-image-success-message"], lang));
     updateTimestamps(newAlias);
   };
   const failed = async () => {
     toast(t, "error", translate(Toast_Words["upload-image-error-message"], lang));
   };
   const { w, h, url, isDrag } = metaData;
   const prefix = isDrag ? "drag-" : "";
   const newAlias = `${prefix}upload.${getRandomHash()}`;
+  metaData.alias = newAlias;
   const bboxInfo: NewImageInfo = { w, h };
   addNewImage(newAlias, url, {
     info: bboxInfo,
     meta: { type, data: metaData },
     callbacks: { success, failed },
     noSelect: false,
   });
@@ -57,63 +58,56 @@
     toast(t, "success", translate(Toast_Words["add-text-success-message"], lang));
     updateTimestamps(newAlias);
   };
   const failed = async () => {
     toast(t, "error", translate(Toast_Words["add-text-error-message"], lang));
   };
   const { addText } = useAddNode({ success, failed });
+  metaData.alias = newAlias;
   addText({ trace: true })({
     alias: newAlias,
     initColor: textColor,
     lang,
     autoFit: true,
     meta: { type, data: metaData },
   });
 }
 function consumeAddSketchPath(): void {
   throw Error("Add sketch path by `importMeta` is not supported yet.");
 }
-function consumePythonHttpFields({
-  t,
-  lang,
-  type,
-  metaData,
-}: IImportMeta<"python.httpFields">): void {
+function consumePythonFields({ t, lang, type, metaData }: IImportMeta<"python.fields">): void {
   const success = async () => {
     toast(t, "success", translate(Toast_Words["generate-image-success-message"], lang));
   };
   const failed = async (err: any) => {
     toast(
       t,
       "error",
       `${translate(Toast_Words["post-python-http-fields-plugin-error-message"], lang)} (${err})`,
     );
   };
-  const getNewAlias = () => `python.httpFields.${metaData.identifier}.${getRandomHash()}`;
+  const getNewAlias = () => `${type}.${metaData.identifier}.${getRandomHash()}`;
+  interface IPack<R> {
+    data: R;
+    alias: string;
+    rectangle: RectangleShapeNode;
+    metaData: IPythonFieldsMetaData;
+  }
   function gatherPacks<T, R>(
     responses: T[],
     getRectangleInfo: (res: T) => INewRectangle,
     getData: (res: T) => R,
-  ): {
-    data: R;
-    alias: string;
-    rectangle: RectangleShapeNode;
-    metaData: Dictionary<any>;
-  }[] {
-    const packs: {
-      data: R;
-      alias: string;
-      rectangle: RectangleShapeNode;
-      metaData: Dictionary<any>;
-    }[] = [];
+  ): IPack<R>[] {
+    const packs: IPack<R>[] = [];
     responses.forEach((res, i) => {
       const newAlias = getNewAlias();
       const rectangle = getNewRectangle(`${i}.${getRandomHash()}`, getRectangleInfo(res));
       const iMetaData = shallowCopy(metaData);
       iMetaData.response.value = metaData.response.value[i] as any;
+      iMetaData.alias = newAlias;
       iMetaData.timestamp = Date.now();
       packs.push({ data: getData(res), alias: newAlias, rectangle, metaData: iMetaData });
     });
     return packs;
   }
   function getCallbacks(isLast: boolean) {
     return { success: isLast ? success : async () => void 0, failed };
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import { runInAction } from "mobx";
 
 import type { AvailablePluginsAndPythonPlugins } from "@/schema/plugins";
 import { reactPluginSettings } from "@/_settings";
 import { usePythonPluginSettings } from "@/stores/_python";
-import { setPluginVisible, setPythonPluginVisible } from "@/stores/plugins";
+import { setPluginVisible, setPythonPluginVisible } from "@/stores/pluginVisible";
 import { floatingControlEvent } from "@/plugins/components/Floating";
 
 function setAllPlugins(visible: boolean, except?: AvailablePluginsAndPythonPlugins[]) {
   runInAction(() => {
     reactPluginSettings.forEach(({ type }) => {
       if (except?.includes(type)) return;
       if (!["settings", "undo", "redo"].includes(type)) {
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFSelect/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useInitBoard.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/useInitBoard.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/hooks/usePython.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import { useCallback, useEffect } from "react";
+import { useCallback } from "react";
 
 import { BBox, INode, INodes, Logger } from "@carefree0910/core";
 
 import type { IMeta } from "@/schema/meta";
 import type {
   INodeData,
-  IPythonResponse,
-  IPythonRequest,
-  IUseHttpPython,
+  IPythonSocketRequest,
   IUsePythonInfo,
+  IUseSocketPython,
+  IPythonOnSocketMessage,
 } from "@/schema/_python";
+import { userStore } from "@/stores/user";
+import { debugStore } from "@/stores/debug";
 import { IPythonStore, updatePythonStore } from "@/stores/_python";
-import { Requests } from "@/requests/actions";
-import { useWebSocket } from "@/requests/hooks";
+import { useWebSocketHook } from "@/requests/hooks";
 import { uploadImage } from "@/actions/uploadImage";
 import { Exporter, IExportBlob } from "@/actions/export";
 
 type IGetNodeData = IExportBlob & { exportBox: BBox };
 async function getNodeData(node: INode | null, opt: IGetNodeData): Promise<INodeData> {
   if (!node) return {};
   const { x, y } = node.position;
@@ -50,112 +51,122 @@
 async function getPythonRequest({
   node,
   nodes,
   identifier,
   getExtraRequestData,
   opt,
 }: Omit<IUsePythonInfo, "endpoint" | "isInvisible"> & {
-  opt: IGetNodeData;
-}): Promise<IPythonRequest> {
-  const nodeData = await getNodeData(node, opt);
-  const nodeDataList = nodes.length <= 1 ? [] : await getNodeDataList(nodes, opt);
+  opt: IExportBlob;
+}): Promise<Omit<IPythonSocketRequest, "hash">> {
+  const exportBox = new INodes(nodes).bbox;
+  const getNodeDataOpt: IGetNodeData = { exportBox, ...opt };
+  const nodeData = await getNodeData(node, getNodeDataOpt);
+  const nodeDataList = nodes.length <= 1 ? [] : await getNodeDataList(nodes, getNodeDataOpt);
   return {
+    userId: userStore.userId,
     identifier,
     nodeData,
     nodeDataList,
     extraData: getExtraRequestData ? getExtraRequestData() : {},
   };
 }
 
-export function useHttpPython<R>({
+/**
+ * this function will integrate a simple but useful retry mechanism, so we only need to
+ * focus on the core logics in `onMessage` function.
+ */
+export function useSocketPython<R>({
   t,
   lang,
+  hash,
   node,
   nodes,
   endpoint,
   identifier,
   isInvisible,
   updateInterval,
-  forceNotSend,
-  onUseHttpPythonSuccess,
-  onUseHttpPythonError,
-  beforeRequest,
   getExtraRequestData,
-}: IUseHttpPython<R>) {
+  onMessage,
+  onSocketError,
+}: IUseSocketPython<R>) {
   const deps = [
+    t,
+    lang,
+    hash,
     node?.alias,
     nodes.map((n) => n.alias).join("_"),
     endpoint,
     identifier,
     updateInterval,
     isInvisible,
-    forceNotSend,
+    getExtraRequestData,
   ];
+
+  const getMessage = useCallback(
+    () =>
+      getPythonRequest({
+        node,
+        nodes,
+        identifier,
+        getExtraRequestData,
+        opt: { t, lang },
+      }).then((req) => ({ hash: hash!, ...req })),
+    [deps],
+  );
+
   const requestFn = useCallback(() => {
-    if (isInvisible || forceNotSend) return Promise.resolve();
-    const exportBox = new INodes(nodes).bbox;
-    const preprocess = beforeRequest ? beforeRequest() : Promise.resolve();
-    return preprocess
-      .then(() =>
-        getPythonRequest({
-          node,
-          nodes,
-          identifier,
-          getExtraRequestData,
-          opt: { t, lang, exportBox },
-        }),
-      )
-      .then((req) => Requests.postJson<IPythonResponse<R>>("_python", endpoint, req))
-      .then((res) => {
-        if (res.success) return onUseHttpPythonSuccess(res);
-        throw Error(res.message);
-      })
-      .catch((err) => {
-        if (onUseHttpPythonError) return onUseHttpPythonError(err);
-        Logger.error(err);
-      });
-  }, deps);
+    useWebSocketHook({
+      isInvisible,
+      hash,
+      getMessage,
+      onMessage,
+      onSocketError,
+      updateInterval,
+    });
+  }, [getMessage, onMessage, onSocketError]);
 
-  useEffect(() => {
-    let timer: any;
-    let shouldIgnore = false; // IMPORTANT!
-    function requestWithTimeout() {
-      if (isInvisible || shouldIgnore) return;
-      requestFn().then(() => (timer = setTimeout(requestWithTimeout, updateInterval)));
-    }
-    if (!updateInterval) requestFn();
-    else requestWithTimeout();
-
-    return () => {
-      shouldIgnore = true;
-      clearTimeout(timer);
-    };
-  }, deps);
+  requestFn();
 }
 
 export function useSyncPython() {
-  const getMessage = () => ({
-    identifier: "sync",
-    nodeData: {},
-    nodeDataList: [],
-    extraData: {},
-    isInternal: true,
-  });
-
-  useWebSocket<IPythonStore>({
-    getMessage,
-    onMessage: async ({ success, message, data: { status, data } }) => {
-      if (!success) {
-        Logger.warn(`sync python settings failed: ${message}`);
-        return { newMessage: getMessage };
-      }
+  const hash = "0";
+  const getMessage = useCallback(
+    (): Promise<IPythonSocketRequest> =>
+      Promise.resolve({
+        hash,
+        userId: userStore.userId,
+        identifier: "sync",
+        nodeData: {},
+        nodeDataList: [],
+        extraData: {},
+        isInternal: true,
+      }),
+    [],
+  );
+  const onMessage = useCallback<IPythonOnSocketMessage<IPythonStore>>(
+    async ({ status, total, pending, message, data: { progress, final } }) => {
       if (status !== "finished") {
-        Logger.warn(`sync in progress: ${JSON.stringify(data)}`);
+        if (status === "pending") {
+          Logger.warn(`sync pending: ${pending} / ${total}`);
+        } else if (status === "working") {
+          // Logger.warn(`sync in progress: ${progress}`);
+        } else {
+          Logger.warn(`sync failed: ${message}`);
+          return { newMessage: getMessage };
+        }
+        return {};
       } else {
-        if (updatePythonStore(data)) {
-          Logger.log(`sync successfully: ${JSON.stringify(data)}, rerendering`);
+        if (!final) {
+          Logger.warn("sync data not found");
+          return { newMessage: getMessage };
         }
-        return { newMessage: getMessage };
+        if (updatePythonStore(final)) {
+          Logger.log(`sync successfully: ${JSON.stringify(final)}, rerendering`);
+        }
+        return debugStore.pollSync ? { newMessage: getMessage } : {};
       }
     },
-  });
+    [],
+  );
+
+  useWebSocketHook<IPythonStore>({ isInvisible: false, hash, getMessage, onMessage });
 }
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/add.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/download.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/plugins.ts`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   allAvailablePlugins,
   allAvailablePythonPlugins,
   AvailablePluginsAndPythonPlugins,
 } from "@/schema/plugins";
 
 const _pluginsLangRecords: Record<Lang, Record<AvailablePluginsAndPythonPlugins, string>> = {
   zh: {
+    meta: "元数据",
     settings: "设置",
     project: "项目",
     add: "添加",
     arrange: "智能整理",
     undo: "撤销",
     redo: "重做",
     download: "下载",
@@ -19,19 +20,20 @@
     wiki: "文档",
     github: "Github",
     email: "邮件",
     textEditor: "编辑文本",
     groupEditor: "编辑组",
     multiEditor: "编辑多节点",
     brush: "画笔",
-    "_python.httpTextArea": "Python 文本框",
-    "_python.httpQA": "Python 问答",
-    "_python.httpFields": "Python 插件",
+    "_python.textArea": "Python 文本框",
+    "_python.QA": "Python 问答",
+    "_python.fields": "Python 插件",
   },
   en: {
+    meta: "Meta",
     settings: "Settings",
     project: "Project",
     add: "Add",
     arrange: "Auto Arrange",
     undo: "Undo",
     redo: "Redo",
     download: "Download",
@@ -39,17 +41,17 @@
     wiki: "Wiki",
     github: "Github",
     email: "Email",
     textEditor: "Edit Text",
     groupEditor: "Edit Group",
     multiEditor: "Edit Multi Nodes",
     brush: "Brush",
-    "_python.httpTextArea": "Python TextArea",
-    "_python.httpQA": "Python Q & A",
-    "_python.httpFields": "Python Plugin",
+    "_python.textArea": "Python TextArea",
+    "_python.QA": "Python Q & A",
+    "_python.fields": "Python Plugin",
   },
 };
 
 export const Plugins_Words: Record<AvailablePluginsAndPythonPlugins, string> = {} as any;
 export const pluginsLangRecords: Dictionary<Dictionary<string>> = {};
 
 function injectScope(scope: string, data: Dictionary<string>) {
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/lang/toast.ts`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,18 @@
   "downloading-project-message" = "downloading-project-message",
   "importing-local-project-message" = "importing-local-project-message",
   "import-local-project-success-message" = "import-local-project-success-message",
   "import-local-project-error-message" = "import-local-project-error-message",
   "add-text-success-message" = "add-text-success-message",
   "add-text-error-message" = "add-text-error-message",
   "auto-arrange-no-need-message" = "auto-arrange-no-need-message",
+  "submit-task-busy-message" = "submit-task-busy-message",
   "submit-task-success-message" = "submit-task-success-message",
   "submit-task-error-message" = "submit-task-error-message",
+  "submit-task-finished-message" = "submit-task-finished-message",
   "downloading-nodes-message" = "downloading-nodes-message",
   "export-blob-error-message" = "export-blob-error-message",
   "enter-brush-mode-message" = "enter-brush-mode-message",
   "exit-brush-mode-message" = "exit-brush-mode-message",
 }
 
 export const toastLangRecords: Record<Lang, Record<Toast_Words, string>> = {
@@ -53,16 +55,18 @@
     [Toast_Words["downloading-project-message"]]: "下载项目中",
     [Toast_Words["importing-local-project-message"]]: "导入中",
     [Toast_Words["import-local-project-success-message"]]: "导入成功",
     [Toast_Words["import-local-project-error-message"]]: "导入失败",
     [Toast_Words["add-text-success-message"]]: "添加文字成功",
     [Toast_Words["add-text-error-message"]]: "添加文字时出了些问题",
     [Toast_Words["auto-arrange-no-need-message"]]: "当前节点无需整理",
+    [Toast_Words["submit-task-busy-message"]]: "当前任务正在执行中，请稍候...",
     [Toast_Words["submit-task-success-message"]]: "任务提交成功",
     [Toast_Words["submit-task-error-message"]]: "执行任务时出了些问题",
+    [Toast_Words["submit-task-finished-message"]]: "任务已执行完成",
     [Toast_Words["downloading-nodes-message"]]: "下载中",
     [Toast_Words["export-blob-error-message"]]: "导出节点时出了些问题",
     [Toast_Words["enter-brush-mode-message"]]: "已进入涂鸦模式",
     [Toast_Words["exit-brush-mode-message"]]: "已退出涂鸦模式",
   },
   en: {
     [Toast_Words["dropping-message"]]: "Detecting",
@@ -84,15 +88,18 @@
     [Toast_Words["downloading-project-message"]]: "Downloading",
     [Toast_Words["importing-local-project-message"]]: "Importing",
     [Toast_Words["import-local-project-success-message"]]: "Imported successfully!",
     [Toast_Words["import-local-project-error-message"]]: "Import failed",
     [Toast_Words["add-text-success-message"]]: "Text added successfully",
     [Toast_Words["add-text-error-message"]]: "Something is wrong when adding Text Node",
     [Toast_Words["auto-arrange-no-need-message"]]: "There is no need to arrange the Nodes",
+    [Toast_Words["submit-task-busy-message"]]:
+      "Current task is being executed, please wait for a while...",
     [Toast_Words["submit-task-success-message"]]: "Task submitted successfully!",
     [Toast_Words["submit-task-error-message"]]: "Something is wrong when executing the task",
+    [Toast_Words["submit-task-finished-message"]]: "Task has been executed successfully",
     [Toast_Words["downloading-nodes-message"]]: "Downloading",
     [Toast_Words["export-blob-error-message"]]: "Something is wrong when exporting Node",
     [Toast_Words["enter-brush-mode-message"]]: "Entered sketch mode",
     [Toast_Words["exit-brush-mode-message"]]: "Exited sketch mode",
   },
 };
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/AddPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/AddPlugin.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 import { loadLocalProject, saveProject } from "@/actions/manageProjects";
 import { getNewProject } from "@/stores/projects";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import CFImageUploader from "@/components/CFImageUploader";
 import { drawboardPluginFactory } from "./utils/factory";
-import { floatingControlEvent, floatingEvent } from "./components/Floating";
+import { floatingEvent } from "./components/Floating";
 import Render from "./components/Render";
+import { useClosePanel } from "./components/hooks";
 
 const AddPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `add_${getRandomHash()}`, []);
   const t = useToast();
   const lang = langStore.tgt;
 
-  const closePanel = () => floatingControlEvent.emit({ id, expand: false });
+  const closePanel = useClosePanel(id);
   const onNewProject = () => {
     toast(t, "info", translate(Toast_Words["adding-project-message"], lang));
     saveProject(
       t,
       lang,
       async () =>
         loadLocalProject(
@@ -70,10 +71,8 @@
           {translate(Add_Words["add-text-button"], lang)}
         </CFButton>
       </Flex>
     </Render>
   );
 };
 
-const _ = observer(AddPlugin);
-drawboardPluginFactory.register("add")(_);
-export default _;
+drawboardPluginFactory.register("add", true)(observer(AddPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ArrangePlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/ArrangePlugin.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     <Render
       id={id}
       onFloatingButtonClick={async () => onArrange(t, lang, { type: "multiple", nodes })}
       {...props}
     />
   );
 };
-drawboardPluginFactory.register("arrange")(observer(ArrangePlugin));
+drawboardPluginFactory.register("arrange", true)(observer(ArrangePlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/BrushPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/BrushPlugin.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -137,8 +137,8 @@
           switchBrushMode();
         }}>
         {translate(Brush_Words["finish-brush-message"], lang)}
       </CFButton>
     </Render>
   );
 };
-drawboardPluginFactory.register("brush")(observer(BrushPlugin));
+drawboardPluginFactory.register("brush", true)(observer(BrushPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DeletePlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/DeletePlugin.tsx`

 * *Files 13% similar despite different names*

```diff
@@ -14,10 +14,8 @@
   if (type === "none") return null;
   function onDelete(): void {
     useSafeExecute("remove", null, true)(nodes.map((node) => node.alias));
   }
   return <Render id={id} onFloatingButtonClick={async () => onDelete()} {...props} />;
 };
 
-const _ = observer(DeletePlugin);
-drawboardPluginFactory.register("delete")(_);
-export default _;
+drawboardPluginFactory.register("delete", true)(observer(DeletePlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DownloadPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/DownloadPlugin.tsx`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import { downloadNodes } from "@/actions/download";
 import CFSelect, { CFSrollableSelect } from "@/components/CFSelect";
 import CFText from "@/components/CFText";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "./utils/factory";
-import { floatingControlEvent } from "./components/Floating";
 import Render from "./components/Render";
+import { useClosePanel } from "./components/hooks";
 
 const DownloadPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `download_${getRandomHash()}`, []);
   const t = useToast();
   const lang = langStore.tgt;
   const { type, nodes } = useSelecting("raw");
   const { w, h, imgWH } = useSelecting("basic")({ fixed: 0 }) ?? {};
@@ -41,15 +41,15 @@
   const getWord = (keepOriginal: string) =>
     translate(
       keepOriginal === "true"
         ? Download_Words["download-image-size-original"]
         : Download_Words["download-image-size-drawboard"],
       lang,
     );
-  const closePanel = () => floatingControlEvent.emit({ id, expand: false });
+  const closePanel = useClosePanel(id);
   const onDownload = () => {
     downloadNodes(t, lang, nodes, format, keepOriginal);
     closePanel();
   };
 
   return (
     <Render id={id} {...props}>
@@ -83,10 +83,8 @@
           {translate(Download_Words["download-button"], lang)}
         </CFButton>
       </Flex>
     </Render>
   );
 };
 
-const _ = observer(DownloadPlugin);
-drawboardPluginFactory.register("download")(_);
-export default _;
+drawboardPluginFactory.register("download", true)(observer(DownloadPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/GroupPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/GroupPlugin.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -14,9 +14,10 @@
   return <Render id={id} onFloatingButtonClick={async () => unGroup?.()} {...props} />;
 };
 const MultiEditorPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `multiEditor_${getRandomHash()}`, []);
   const { setGroup } = useSelecting("multiple") ?? {};
   return <Render id={id} onFloatingButtonClick={async () => setGroup?.()} {...props} />;
 };
-drawboardPluginFactory.register("groupEditor")(observer(GroupEditorPlugin));
-drawboardPluginFactory.register("multiEditor")(observer(MultiEditorPlugin));
+
+drawboardPluginFactory.register("groupEditor", true)(observer(GroupEditorPlugin));
+drawboardPluginFactory.register("multiEditor", true)(observer(MultiEditorPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/LinksPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/LinksPlugin.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -15,10 +15,11 @@
   const id = useMemo(() => `emailLink_${getRandomHash()}`, []);
   return <Link id={id} href="mailto: syameimaru.saki@gmail.com" {...props} />;
 };
 const GitHubPlugin = (props: IPlugin) => {
   const id = useMemo(() => `githubLink_${getRandomHash()}`, []);
   return <Link id={id} url="https://github.com/carefree0910/carefree-drawboard" {...props} />;
 };
-drawboardPluginFactory.register("wiki")(observer(WikiPlugin));
-drawboardPluginFactory.register("email")(observer(EmailPlugin));
-drawboardPluginFactory.register("github")(observer(GitHubPlugin));
+
+drawboardPluginFactory.register("wiki", true)(observer(WikiPlugin));
+drawboardPluginFactory.register("email", true)(observer(EmailPlugin));
+drawboardPluginFactory.register("github", true)(observer(GitHubPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ProjectPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/ProjectPlugin.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 import { setCurrentProjectName, useCurrentProject } from "@/stores/projects";
 import {
   ILoadedProject,
   fetchAllProjects,
   loadProject,
   saveProject,
 } from "@/actions/manageProjects";
+import { downloadCurrentFullProject } from "@/actions/download";
 import CFText from "@/components/CFText";
 import CFInput from "@/components/CFInput";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { CFSrollableSelect } from "@/components/CFSelect";
 import { drawboardPluginFactory } from "./utils/factory";
 import Render from "./components/Render";
-import { floatingControlEvent, floatingEvent, floatingRenderEvent } from "./components/Floating";
-import { downloadCurrentFullProject } from "@/actions/download";
+import { floatingEvent, floatingRenderEvent } from "./components/Floating";
+import { useClosePanel } from "./components/hooks";
 
 type IImportLocal = ILoadedProject | INodePack[];
 const ProjectPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `project_${getRandomHash()}`, []);
   const t = useToast();
   const lang = langStore.tgt;
   const { uid, name } = useCurrentProject();
@@ -68,15 +69,15 @@
 
     return () => {
       floatingDispose();
       floatingRenderDispose();
     };
   }, [id]);
 
-  const closePanel = () => floatingControlEvent.emit({ id, expand: false });
+  const closePanel = useClosePanel(id);
   function updateProjectStates(uid: string, name: string) {
     setSelectedUid(uid);
     setUserInputName(name);
   }
 
   function onRenameProject() {
     setCurrentProjectName(userInputName);
@@ -168,10 +169,8 @@
           </CFButton>
         </Upload>
       </Flex>
     </Render>
   );
 };
 
-const _ = observer(ProjectPlugin);
-drawboardPluginFactory.register("project")(_);
-export default _;
+drawboardPluginFactory.register("project", true)(observer(ProjectPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/SettingsPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/SettingsPlugin.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import { uiStore } from "@/stores/ui";
 import { usePythonPluginSettings } from "@/stores/_python";
 import {
   pluginIsVisible,
   pythonPluginIsVisible,
   setPythonPluginVisible,
   setPluginVisible,
-} from "@/stores/plugins";
+} from "@/stores/pluginVisible";
 import { hideAllPlugins, showAllPlugins } from "@/actions/managePlugins";
 import CFButton from "@/components/CFButton";
 import CFSelect from "@/components/CFSelect";
 import CFSlider from "@/components/CFSlider";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "./utils/factory";
@@ -118,10 +118,8 @@
           </Flex>
         </Box>
       </Flex>
     </Render>
   );
 };
 
-const _ = observer(SettingsPlugin);
-drawboardPluginFactory.register("settings")(_);
-export default _;
+drawboardPluginFactory.register("settings", true)(observer(SettingsPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/TextEditorPlugin.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,8 @@
           }}
           onBlur={() => editContent({ trace: true })(content)}
         />
       </Flex>
     </Render>
   );
 };
-drawboardPluginFactory.register("textEditor")(observer(TextEditorPlugin));
+drawboardPluginFactory.register("textEditor", true)(observer(TextEditorPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-import { useMemo } from "react";
+import { useEffect, useMemo } from "react";
 import { observer } from "mobx-react-lite";
 
 import { getRandomHash } from "@carefree0910/core";
-import { safeRedo, safeUndo } from "@carefree0910/business";
+import { safeRedo, safeUndo, useUndoRedoSteps } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
+import { setPluginVisible } from "@/stores/pluginVisible";
 import { drawboardPluginFactory } from "./utils/factory";
 import Render from "./components/Render";
 
 const UndoPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `undo_${getRandomHash()}`, []);
+  const { undoSteps } = useUndoRedoSteps();
+  useEffect(() => setPluginVisible("undo", undoSteps > 0), [undoSteps]);
+
   return <Render id={id} onFloatingButtonClick={async () => safeUndo()} {...props} />;
 };
 const RedoPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `redo_${getRandomHash()}`, []);
+  const { redoSteps } = useUndoRedoSteps();
+  useEffect(() => setPluginVisible("redo", redoSteps > 0), [redoSteps]);
+
   return <Render id={id} onFloatingButtonClick={async () => safeRedo()} {...props} />;
 };
-drawboardPluginFactory.register("undo")(observer(UndoPlugin));
-drawboardPluginFactory.register("redo")(observer(RedoPlugin));
+
+drawboardPluginFactory.register("undo", true)(observer(UndoPlugin));
+drawboardPluginFactory.register("redo", true)(observer(RedoPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,109 @@
-import { useMemo, useCallback } from "react";
+import { useCallback } from "react";
 import { observer } from "mobx-react-lite";
 import { CloseIcon } from "@chakra-ui/icons";
 import { Flex, Spacer, useToast } from "@chakra-ui/react";
 
-import { Dictionary, getRandomHash } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
-import type { IMeta, IPythonHttpFieldsResponse } from "@/schema/meta";
-import type { IPythonHttpFieldsPlugin, IPythonResponse } from "@/schema/_python";
+import type { IPythonResults } from "@/schema/meta";
+import type { IPythonFieldsPlugin, IPythonOnSocketMessage } from "@/schema/_python";
 import { UI_Words } from "@/lang/ui";
 import { Toast_Words } from "@/lang/toast";
 import { toast } from "@/utils/toast";
 import { titleCaseWord } from "@/utils/misc";
+import { removeSocketHook, socketLog } from "@/stores/socket";
+import { getPluginIds, removePluginMessage, updatePluginMessage } from "@/stores/plugins";
 import { importMeta } from "@/actions/importMeta";
-import { getMetaField } from "@/stores/meta";
-import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import CFHeading from "@/components/CFHeading";
-import { useDefinitions } from "../components/Fields";
-import { floatingControlEvent } from "../components/Floating";
-import { useIdentifierId } from "./hooks";
-import PythonHttpPluginWithSubmit from "./HttpPluginWithSubmit";
-
-const PythonHttpFieldsPlugin = ({ pluginInfo, ...props }: IPythonHttpFieldsPlugin) => {
-  const identifierId = useIdentifierId(pluginInfo.identifier);
-  const id = useMemo(() => `${identifierId}_${getRandomHash()}`, [identifierId]);
+import { drawboardPluginFactory } from "@/plugins/utils/factory";
+import { useClosePanel } from "../components/hooks";
+import { useCurrentMeta, useDefinitionsRequestDataFn } from "./hooks";
+import PythonPluginWithSubmit, { socketFinishedEvent } from "./PluginWithSubmit";
+import DefinitionFields from "./DefinitionFields";
+
+const PythonFieldsPlugin = ({ pluginInfo, ...props }: IPythonFieldsPlugin) => {
+  const { id, pureIdentifier } = getPluginIds(pluginInfo.identifier);
   const t = useToast();
   const lang = langStore.tgt;
   const definitions = pluginInfo.definitions;
-  const getExtraRequestData = useMemo(
-    () => () => {
-      const data: Dictionary<any> = {};
-      Object.keys(definitions).forEach((field) => {
-        data[field] = getMetaField(field);
-      });
-      return data;
+  const getExtraRequestData = useDefinitionsRequestDataFn(definitions);
+  const currentMeta = useCurrentMeta(pluginInfo.node);
+  const emitClose = useClosePanel(id);
+
+  const onMessage = useCallback<IPythonOnSocketMessage<IPythonResults>>(
+    async (message) => {
+      const {
+        hash,
+        status,
+        data: { final },
+      } = message;
+      switch (status) {
+        case "pending": {
+          updatePluginMessage(id, message);
+          break;
+        }
+        case "working": {
+          updatePluginMessage(id, message);
+          break;
+        }
+        case "finished": {
+          removePluginMessage(id);
+          socketFinishedEvent.emit({ id });
+          if (!final) {
+            toast(
+              t,
+              "success",
+              `${translate(Toast_Words["submit-task-finished-message"], lang)} (${pureIdentifier})`,
+            );
+          } else {
+            const { _duration, ...response } = final;
+            importMeta({
+              t,
+              lang,
+              type: "python.fields",
+              metaData: {
+                identifier: pureIdentifier,
+                parameters: getExtraRequestData(),
+                response,
+                duration: _duration,
+                from: currentMeta,
+              },
+            });
+          }
+          socketLog(`> remove hook (${hash})`);
+          removeSocketHook(hash);
+          break;
+        }
+      }
+      return {};
+    },
+    [id, lang, pureIdentifier, currentMeta, getExtraRequestData],
+  );
+  const onSocketError = useCallback(
+    async (err: any) => {
+      toast(t, "error", `${translate(Toast_Words["submit-task-error-message"], lang)} - ${err}`);
     },
-    [definitions],
+    [t, lang],
   );
-  const currentMeta = useMemo(() => {
-    const node = pluginInfo.node;
-    let currentMeta: IMeta | undefined;
-    if (node && node.type !== "group") {
-      currentMeta = node.params.meta as IMeta;
-    }
-    return currentMeta;
-  }, [pluginInfo.node]);
-  const emitClose = useCallback(() => floatingControlEvent.emit({ id, expand: false }), [id]);
-
-  async function onUseHttpPythonSuccess({
-    data: { _duration, ...response },
-  }: IPythonResponse<IPythonHttpFieldsResponse>) {
-    importMeta({
-      t,
-      lang,
-      type: "python.httpFields",
-      metaData: {
-        identifier: identifierId,
-        parameters: getExtraRequestData(),
-        response,
-        duration: _duration,
-        from: currentMeta,
-      },
-    });
-  }
-  async function onUseHttpPythonError(err: any) {
-    toast(t, "error", `${translate(Toast_Words["submit-task-error-message"], lang)} - ${err}`);
-  }
 
-  const header = pluginInfo.header ?? titleCaseWord(identifierId);
+  const header = pluginInfo.header ?? titleCaseWord(pureIdentifier);
   return (
-    <PythonHttpPluginWithSubmit
+    <PythonPluginWithSubmit
       id={id}
       buttonText={translate(UI_Words["submit-task"], lang)}
       getExtraRequestData={getExtraRequestData}
-      onUseHttpPythonSuccess={onUseHttpPythonSuccess}
-      onUseHttpPythonError={onUseHttpPythonError}
+      onMessage={onMessage}
+      onSocketError={onSocketError}
       pluginInfo={pluginInfo}
       {...props}>
       <Flex>
         <CFHeading>{header}</CFHeading>
         <Spacer />
         <CloseIcon w="12px" cursor="pointer" onClick={emitClose} />
       </Flex>
-      {Object.keys(definitions).length > 0 && (
-        <Flex p="12px" gap="12px" flexWrap="wrap" alignItems="center" justifyContent="space-around">
-          {useDefinitions(definitions, pluginInfo.numColumns)}
-        </Flex>
-      )}
-    </PythonHttpPluginWithSubmit>
+      <DefinitionFields definitions={definitions} numColumns={pluginInfo.numColumns} />
+    </PythonPluginWithSubmit>
   );
 };
 
-const _ = observer(PythonHttpFieldsPlugin);
-drawboardPluginFactory.registerPython("_python.httpFields", true)(_);
-export default _;
+drawboardPluginFactory.registerPython("_python.fields", true)(observer(PythonFieldsPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,101 @@
-import { useState } from "react";
+import { useCallback, useEffect, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { useToast } from "@chakra-ui/react";
 
+import { getRandomHash } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
-import type { IPythonHttpPluginWithSubmit } from "@/schema/_python";
+import type { IPythonSocketPluginWithSubmit } from "@/schema/_python";
+import { Event } from "@/utils/event";
 import { toast } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
-import { useHttpPython } from "@/hooks/usePython";
-import CFButton from "@/components/CFButton";
+import { userStore } from "@/stores/user";
+import { getPluginHash } from "@/stores/plugins";
+import { useSocketPython } from "@/hooks/usePython";
+import { CFButtonWithBusyTooltip } from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import Render from "../components/Render";
 import { floatingControlEvent } from "../components/Floating";
 
-const PythonHttpPluginWithSubmit = ({
+export const socketFinishedEvent = new Event<{ id: string }>();
+function PythonPluginWithSubmit<R>({
   id,
   pluginInfo: {
     node,
     nodes,
     endpoint,
     identifier,
     updateInterval,
     closeOnSubmit = true,
     toastOnSubmit = true,
-    submitToastMessage,
+    toastMessageOnSubmit,
   },
   buttonText,
-  onUseHttpPythonError,
-  onUseHttpPythonSuccess,
-  beforeRequest,
+  onMessage,
+  onSocketError,
   getExtraRequestData,
   children,
   ...props
-}: IPythonHttpPluginWithSubmit<any>) => {
+}: IPythonSocketPluginWithSubmit<R>) {
   const t = useToast();
   const lang = langStore.tgt;
-  const [send, setSend] = useState(false);
+  const [hash, setHash] = useState<string | undefined>(undefined);
+  const [busy, setBusy] = useState(false);
+  const onClick = useCallback(() => {
+    if (busy) return;
+    if (!userStore.canAlwaysSubmit) {
+      setBusy(true);
+    }
+    setHash(getPluginHash(id));
+    if (closeOnSubmit) {
+      floatingControlEvent.emit({ id, expand: false });
+    }
+    if (toastOnSubmit) {
+      toastMessageOnSubmit ??= translate(Toast_Words["submit-task-success-message"], lang);
+      toast(t, "info", toastMessageOnSubmit);
+    }
+  }, [id, t, lang, closeOnSubmit, toastOnSubmit, toastMessageOnSubmit, busy]);
 
-  useHttpPython<{ text: string }>({
+  useSocketPython<R>({
     t,
     lang,
+    hash,
     node,
     nodes,
     endpoint,
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
     updateInterval,
-    forceNotSend: !send,
-    onUseHttpPythonError,
-    onUseHttpPythonSuccess,
-    beforeRequest: async () => {
-      setSend(false);
-      beforeRequest && (await beforeRequest());
-    },
+    onMessage,
+    onSocketError,
     getExtraRequestData,
   });
 
-  function onClick() {
-    setSend(true);
-    if (closeOnSubmit) {
-      floatingControlEvent.emit({ id, expand: false });
-    }
-    if (toastOnSubmit) {
-      submitToastMessage ??= translate(Toast_Words["submit-task-success-message"], lang);
-      toast(t, "info", submitToastMessage);
-    }
-  }
+  useEffect(() => {
+    const { dispose } = socketFinishedEvent.on(({ id: incomingId }) => {
+      if (incomingId === id) {
+        setBusy(false);
+        setHash(undefined);
+      }
+    });
+
+    return () => {
+      dispose();
+    };
+  }, [id, setBusy, setHash]);
 
   return (
     <Render id={id} {...props}>
       {children}
       <CFDivider />
-      <CFButton onClick={onClick}>{buttonText}</CFButton>
+      <CFButtonWithBusyTooltip
+        busy={busy}
+        tooltip={translate(Toast_Words["submit-task-busy-message"], lang)}
+        onClick={onClick}>
+        {buttonText}
+      </CFButtonWithBusyTooltip>
     </Render>
   );
-};
+}
 
-export default observer(PythonHttpPluginWithSubmit);
+export default observer(PythonPluginWithSubmit);
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/QAPlugin.tsx`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-import { useMemo, useState } from "react";
+import { useCallback, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { Textarea } from "@chakra-ui/react";
 
-import { getRandomHash } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
-import type { IPythonHttpQAPlugin, IPythonResponse } from "@/schema/_python";
+import type { IPythonOnSocketMessage, IPythonQAPlugin } from "@/schema/_python";
 import { UI_Words } from "@/lang/ui";
+import { getPluginIds } from "@/stores/plugins";
 import CFInput from "@/components/CFInput";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
-import { useIdentifierId } from "./hooks";
-import PythonHttpPluginWithSubmit from "./HttpPluginWithSubmit";
+import PythonPluginWithSubmit from "./PluginWithSubmit";
 
-const PythonHttpQAPlugin = ({ pluginInfo, ...props }: IPythonHttpQAPlugin) => {
-  const identifierId = useIdentifierId(pluginInfo.identifier);
-  const id = useMemo(() => `${identifierId}_QA_${getRandomHash()}`, []);
+const PythonQAPlugin = ({ pluginInfo, ...props }: IPythonQAPlugin) => {
+  const { id } = getPluginIds(`QA_${pluginInfo.identifier}`);
   const [userInput, setUserInput] = useState("");
   const [serverText, setServerText] = useState(pluginInfo.initialText);
   const lang = langStore.tgt;
-
-  function getExtraRequestData() {
-    return { text: userInput };
-  }
-  async function onUseHttpPythonSuccess(res: IPythonResponse<{ text: string }>) {
-    setServerText(res.data.text);
-  }
+  const getExtraRequestData = useCallback(() => ({ text: userInput }), [userInput]);
+  const onMessage = useCallback<IPythonOnSocketMessage<{ text: string }>>(
+    async ({ status, data }) => {
+      if (status === "finished") {
+        setServerText(data.final?.text ?? "");
+      } else {
+        setServerText("Thinking...");
+      }
+      return {};
+    },
+    [setServerText],
+  );
 
   return (
-    <PythonHttpPluginWithSubmit
+    <PythonPluginWithSubmit
       id={id}
       buttonText={translate(UI_Words["submit-task"], lang)}
       getExtraRequestData={getExtraRequestData}
-      onUseHttpPythonSuccess={onUseHttpPythonSuccess}
+      onMessage={onMessage}
       pluginInfo={pluginInfo}
       {...props}>
       <Textarea w="100%" h="40%" minH="0px" value={serverText} readOnly />
       <CFInput
         w="100%"
         h="30%"
         mt="16px"
         value={userInput}
         onChange={(event) => setUserInput(event.target.value)}
         placeholder={translate(UI_Words["qa-field-placeholder"], langStore.tgt)}
       />
-    </PythonHttpPluginWithSubmit>
+    </PythonPluginWithSubmit>
   );
 };
 
-const _ = observer(PythonHttpQAPlugin);
-drawboardPluginFactory.registerPython("_python.httpQA", true)(_);
-export default _;
+drawboardPluginFactory.registerPython("_python.QA", true)(observer(PythonQAPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,55 @@
-import { useMemo, useState } from "react";
+import { useCallback, useMemo, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { Textarea, useToast } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
 import { langStore } from "@carefree0910/business";
 
-import type { IPythonHttpTextAreaPlugin } from "@/schema/_python";
-import { useHttpPython } from "@/hooks/usePython";
+import type { IPythonTextAreaPlugin, IPythonOnSocketMessage } from "@/schema/_python";
+import { getPluginIds } from "@/stores/plugins";
+import { useSocketPython } from "@/hooks/usePython";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import Render from "@/plugins/components/Render";
-import { useIdentifierId } from "./hooks";
 
-const PythonHttpTextAreaPlugin = ({
+const PythonTextAreaPlugin = ({
   pluginInfo: { node, nodes, endpoint, identifier, updateInterval, noLoading, textAlign },
   ...props
-}: IPythonHttpTextAreaPlugin) => {
+}: IPythonTextAreaPlugin) => {
   const t = useToast();
   const lang = langStore.tgt;
-  const identifierId = useIdentifierId(identifier);
-  const id = useMemo(() => `${identifierId}_textArea_${getRandomHash()}`, []);
+  const id = getPluginIds(`textArea_${identifier}`);
+  const hash = useMemo(() => getRandomHash().toString(), [id]);
   const [value, setValue] = useState("");
+  const onMessage = useCallback<IPythonOnSocketMessage<{ text: string }>>(
+    async ({ status, data }) => {
+      if (status === "finished") {
+        setValue(data.final?.text ?? "");
+      } else if (!noLoading) {
+        setValue("Loading...");
+      }
+      return {};
+    },
+    [setValue],
+  );
 
-  useHttpPython<{ text: string }>({
+  useSocketPython({
     t,
     lang,
+    hash,
     node,
     nodes,
     endpoint,
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
     updateInterval,
-    onUseHttpPythonSuccess: async (res) => setValue(res.data.text),
-    beforeRequest: noLoading ? undefined : async () => setValue("Loading..."),
+    onMessage,
   });
 
   return (
     <Render id={id} {...props}>
       <Textarea w="100%" h="100%" minH="0px" value={value} textAlign={textAlign} readOnly />
     </Render>
   );
 };
 
-const _ = observer(PythonHttpTextAreaPlugin);
-drawboardPluginFactory.registerPython("_python.httpTextArea", true)(_);
-export default _;
+drawboardPluginFactory.registerPython("_python.textArea", true)(observer(PythonTextAreaPlugin));
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/utils.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Fields/utils.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files 22% similar despite different names*

```diff
@@ -1,260 +1,205 @@
+import type { ChakraComponent } from "@chakra-ui/react";
+import { useLayoutEffect, useMemo } from "react";
 import { observer } from "mobx-react-lite";
-import { useState, useMemo, useLayoutEffect, forwardRef } from "react";
-import { Box, BoxProps, Flex, FlexProps, Image, Portal } from "@chakra-ui/react";
 
-import { Coordinate, Dictionary, isUndefined } from "@carefree0910/core";
+import { Coordinate, getRandomHash, INodes, PivotType, shallowCopy } from "@carefree0910/core";
 import {
+  boardBBoxToDom,
+  injectNodeTransformEventCallback,
+  removeNodeTransformEventCallback,
   useBoardContainerLeftTop,
   useBoardContainerWH,
   useIsReady,
+  useSelectHooks,
   useSelecting,
 } from "@carefree0910/business";
 
-import type { IFloating, IPositionInfo } from "@/schema/plugins";
-import { Event } from "@/utils/event";
-import { DEFAULT_PLUGIN_SETTINGS, VISIBILITY_TRANSITION } from "@/utils/constants";
-import { themeStore } from "@/stores/theme";
+import type { IRender } from "@/schema/plugins";
+import { DEFAULT_PLUGIN_SETTINGS } from "@/utils/constants";
+import { getNodeFilter } from "../utils/renderFilters";
+import Floating, {
+  floatingRenderEvent,
+  getExpandId,
+  getExpandPosition,
+  IFloatingRenderEvent,
+} from "./Floating";
+
+let DEBUG_PREFIX: string | undefined;
+
+const Render = (({ id, nodeConstraint, renderInfo, containerRef, children, ...props }: IRender) => {
+  const _id = useMemo(() => id ?? `plugin_${getRandomHash()}`, [id]);
+  let { w, h, iconW, iconH, pivot, follow, offsetX, offsetY, expandOffsetX, expandOffsetY } =
+    renderInfo;
+  iconW ??= DEFAULT_PLUGIN_SETTINGS.iconW;
+  iconH ??= DEFAULT_PLUGIN_SETTINGS.iconH;
+  pivot ??= DEFAULT_PLUGIN_SETTINGS.pivot as PivotType;
+  follow ??= DEFAULT_PLUGIN_SETTINGS.follow;
+  expandOffsetX ??=
+    renderInfo.useModal || ["top", "center", "bottom"].includes(pivot)
+      ? 0
+      : ["lt", "left", "lb"].includes(pivot) === follow
+      ? -DEFAULT_PLUGIN_SETTINGS.expandOffsetX
+      : DEFAULT_PLUGIN_SETTINGS.expandOffsetX;
+  expandOffsetY ??=
+    renderInfo.useModal || ["left", "right", "lt", "rt", "lb", "rb"].includes(pivot)
+      ? 0
+      : pivot === "center"
+      ? DEFAULT_PLUGIN_SETTINGS.expandOffsetY
+      : (pivot === "top") === follow
+      ? -DEFAULT_PLUGIN_SETTINGS.expandOffsetY
+      : DEFAULT_PLUGIN_SETTINGS.expandOffsetY;
 
-export function getExpandId(id: string): string {
-  return `${id}_expand`;
-}
-export function getExpandPosition(
-  isModal: boolean,
-  {
-    x,
-    y,
+  const updatedRenderInfo = {
+    ...renderInfo,
     w,
     h,
     iconW,
     iconH,
     pivot,
     follow,
     expandOffsetX,
     expandOffsetY,
-  }: { x: number; y: number } & IPositionInfo,
-): Coordinate {
-  if (isModal) {
-    pivot = "center";
-    const { w: bw, h: bh } = useBoardContainerWH();
-    const { x: left, y: top } = useBoardContainerLeftTop();
-    x = left + 0.5 * (bw - iconW);
-    y = top + 0.5 * (bh - h) - iconH;
-  }
-  // x
-  if (["top", "center", "bottom"].includes(pivot)) {
-    x += 0.5 * (iconW - w) + expandOffsetX;
-  } else if (["rt", "right", "rb"].includes(pivot)) {
-    if (follow) {
-      x += iconW + expandOffsetX;
-    } else {
-      x += expandOffsetX - w;
-    }
-  } else {
-    if (follow) {
-      x += expandOffsetX - w;
-    } else {
-      x += iconW + expandOffsetX;
-    }
-  }
-  // y
-  if (["left", "right"].includes(pivot)) {
-    y += 0.5 * (iconH - h) + expandOffsetY;
-  } else if (pivot === "center") {
-    y += iconH + expandOffsetY;
-  } else {
-    if (!follow) {
-      if (["lb", "bottom", "rb"].includes(pivot)) {
-        y += expandOffsetY - h;
-      } else if (["lt", "top", "rt"].includes(pivot)) {
-        y += iconH + expandOffsetY;
-      }
-    } else {
-      if (pivot === "bottom") {
-        y += iconH + expandOffsetY;
-      } else if (pivot === "top") {
-        y += expandOffsetY - h;
-      } else if (["lb", "rb"].includes(pivot)) {
-        y += expandOffsetY + iconH - h;
-      } else if (["lt", "rt"].includes(pivot)) {
-        y += expandOffsetY;
-      }
-    }
-  }
-  // return
-  return new Coordinate(x, y);
-}
-
-export interface IFloatingEvent {
-  type: string;
-  data: Dictionary<any>;
-}
-export interface IFloatingRenderEvent {
-  id: string;
-  expand: boolean;
-  needRender: boolean;
-  noExpand?: boolean;
-}
-export interface IFloatingControlEvent {
-  id?: string;
-  expand?: boolean;
-  ignoreId?: boolean;
-  forceCheckIds?: string[];
-}
-export const floatingEvent = new Event<IFloatingEvent>();
-export const floatingRenderEvent = new Event<IFloatingRenderEvent>();
-export const floatingControlEvent = new Event<IFloatingControlEvent>();
-
-const Floating = forwardRef(function (
-  {
-    id,
-    w: _w, // will not take effect
-    h: _h, // will not take effect
-    renderInfo: {
-      w,
-      h,
-      iconW,
-      iconH,
-      pivot,
-      follow,
-      expandOffsetX,
-      expandOffsetY,
-      src,
-      bgOpacity,
-      renderFilter,
-      useModal,
-      modalOpacity,
-      expandProps,
-      isInvisible,
-    },
-    noExpand,
-    onFloatingButtonClick,
-    children,
-    ...props
-  }: IFloating,
-  ref,
-) {
-  const needRender = useIsReady() && (!renderFilter || renderFilter(useSelecting("raw")));
-  const { panelBg } = themeStore.styles;
-  bgOpacity ??= DEFAULT_PLUGIN_SETTINGS.bgOpacity;
-  const bgOpacityHex = Math.round(bgOpacity * 255).toString(16);
-  const commonProps: BoxProps = {
-    p: "12px",
-    bg: `${panelBg}${bgOpacityHex}`,
-    position: "absolute",
-    boxShadow: "2px 2px 4px rgba(0, 0, 0, 0.25)",
-    borderRadius: "4px",
+    renderFilter: getNodeFilter(nodeConstraint),
   };
-  Object.keys(props).forEach((key) => {
-    const commonV = commonProps[key as keyof BoxProps];
-    (props as any)[key] ??= commonV;
-  });
-  const parsedExpandProps: FlexProps = {};
-  Object.entries(expandProps ?? {}).forEach(([key, value]) => {
-    if (!isUndefined(value) && value !== null) {
-      parsedExpandProps[key as keyof FlexProps] = value;
-    }
-  });
-  const [expand, setExpand] = useState(false);
-  const [transform, setTransform] = useState<string | undefined>(undefined);
-  const expandId = useMemo(() => getExpandId(id), [id]);
-  // convert float to hex
-  modalOpacity ??= DEFAULT_PLUGIN_SETTINGS.modalOpacity;
-  const modalOpacityHex = Math.round(modalOpacity * 255).toString(16);
-  const expandBg = useMemo(
-    () => (useModal ? `${panelBg}${modalOpacityHex}` : commonProps.bg),
-    [useModal],
-  );
+
+  // This effect handles callbacks that dynamically render the plugin's position
   useLayoutEffect(() => {
-    const { dispose: disposeRender } = floatingRenderEvent.on(
-      ({ id: incomingId, expand: incomingExpand }) => {
-        if (id !== incomingId && incomingExpand && expand) {
-          setExpand(false);
+    const updateFloating = async (e: any) => {
+      const _iconW = iconW!;
+      const _iconH = iconH!;
+      const _pivot = pivot!;
+      const _follow = follow!;
+      const _offsetX =
+        offsetX ??
+        (["top", "center", "bottom"].includes(_pivot)
+          ? 0
+          : ["lt", "left", "lb"].includes(_pivot) === _follow
+          ? -DEFAULT_PLUGIN_SETTINGS.offsetX
+          : DEFAULT_PLUGIN_SETTINGS.offsetX);
+      const _offsetY =
+        offsetY ??
+        (["left", "center", "right"].includes(_pivot)
+          ? 0
+          : ["lt", "top", "rt"].includes(_pivot) === _follow
+          ? -DEFAULT_PLUGIN_SETTINGS.offsetY
+          : DEFAULT_PLUGIN_SETTINGS.offsetY);
+      // adjust floating
+      const domFloating = document.querySelector<HTMLDivElement>(`#${_id}`);
+      if (!domFloating) return;
+      let x, y;
+      if (!_follow) {
+        const { x: left, y: top } = useBoardContainerLeftTop();
+        const { w: bw, h: bh } = useBoardContainerWH();
+        // x
+        if (["lt", "left", "lb"].includes(_pivot)) {
+          x = left + _offsetX;
+        } else if (["rt", "right", "rb"].includes(_pivot)) {
+          x = left + bw - _iconW + _offsetX;
+        } else {
+          x = left + 0.5 * (bw - _iconW) + _offsetX;
+        }
+        // y
+        if (["lt", "top", "rt"].includes(_pivot)) {
+          y = top + _offsetY;
+        } else if (["lb", "bottom", "rb"].includes(_pivot)) {
+          y = top + bh - _iconH + _offsetY;
+        } else {
+          y = top + 0.5 * (bh - _iconH) + _offsetY;
+        }
+      } else {
+        const info = useSelecting("raw");
+        if (DEBUG_PREFIX && _id.startsWith(DEBUG_PREFIX)) {
+          console.log("> e", e);
+          console.log("> info", _id, shallowCopy(info));
+        }
+        if (!info || (updatedRenderInfo.renderFilter && !updatedRenderInfo.renderFilter(info))) {
+          return;
+        }
+        const bounding = info.displayNode
+          ? info.displayNode.bbox.bounding
+          : new INodes(info.nodes).bbox;
+        const domPivot = boardBBoxToDom(bounding).pivot(_pivot);
+        let offsetX, offsetY;
+        // x
+        if (["lt", "left", "lb"].includes(_pivot)) {
+          offsetX = -_iconW + _offsetX;
+        } else if (["rt", "right", "rb"].includes(_pivot)) {
+          offsetX = _offsetX;
+        } else {
+          offsetX = -0.5 * _iconW + _offsetX;
         }
-      },
-    );
-    const { dispose: disposeControl } = floatingControlEvent.on(
-      ({ id: incomingId, expand: incomingExpand, ignoreId, forceCheckIds }) => {
-        if (
-          !isUndefined(incomingExpand) &&
-          (id === incomingId ||
-            (ignoreId &&
-              (!forceCheckIds ||
-                forceCheckIds.every((forcedId) => id !== forcedId && !id.startsWith(forcedId)))))
-        ) {
-          setExpand(incomingExpand);
+        // y
+        if (["lt", "top", "rt"].includes(_pivot)) {
+          offsetY = -_iconH + _offsetY;
+        } else if (["lb", "bottom", "rb"].includes(_pivot)) {
+          offsetY = _offsetY;
+        } else {
+          offsetY = -0.5 * _iconH + _offsetY;
         }
-      },
-    );
-    floatingRenderEvent.emit({ id, expand, needRender, noExpand });
+        ({ x, y } = domPivot.add(new Coordinate(offsetX, offsetY)));
+      }
+      domFloating.dataset.x = x.toString();
+      domFloating.dataset.y = y.toString();
+      domFloating.style.transform = `matrix(1,0,0,1,${x},${y})`;
+      // adjust expand of the floating
+      const domFloatingExpand = document.querySelector<HTMLDivElement>(`#${getExpandId(_id)}`);
+      if (!domFloatingExpand) return;
+      const { x: ex, y: ey } = getExpandPosition(updatedRenderInfo.useModal ?? false, {
+        x,
+        y,
+        w,
+        h,
+        iconW: _iconW,
+        iconH: _iconH,
+        pivot: _pivot,
+        follow: _follow,
+        expandOffsetX: expandOffsetX!,
+        expandOffsetY: expandOffsetY!,
+      });
+      domFloatingExpand.style.transform = `matrix(1,0,0,1,${ex},${ey})`;
+    };
+    const onFloatingReRender = ({ id: renderedId, needRender }: IFloatingRenderEvent) => {
+      if (_id === renderedId && needRender) {
+        updateFloating({ event: "rerender", needRender });
+      }
+    };
+    const { dispose } = floatingRenderEvent.on(onFloatingReRender);
+    injectNodeTransformEventCallback(_id, updateFloating);
+    useSelectHooks().register({ key: _id, after: updateFloating });
+    window.addEventListener("resize", updateFloating);
+    if (useIsReady()) {
+      updateFloating({ event: "init" });
+    }
 
     return () => {
-      disposeRender();
-      disposeControl();
+      if (DEBUG_PREFIX && _id.startsWith(DEBUG_PREFIX)) {
+        console.log(">>>>> clean up");
+      }
+      dispose();
+      removeNodeTransformEventCallback(_id);
+      useSelectHooks().remove(_id);
+      window.removeEventListener("resize", updateFloating);
     };
-  }, [id, expand, needRender, noExpand]);
-
-  if (!needRender) return null;
+  }, [
+    _id,
+    iconW,
+    iconH,
+    nodeConstraint,
+    pivot,
+    follow,
+    offsetX,
+    offsetY,
+    expandOffsetX,
+    expandOffsetY,
+    JSON.stringify(props),
+    useIsReady(),
+  ]);
 
   return (
-    <>
-      <Box
-        as="button"
-        id={id}
-        w={`${iconW}px`}
-        h={`${iconH}px`}
-        onClick={() => {
-          const self = document.querySelector<HTMLDivElement>(`#${id}`);
-          if (self && self.dataset.x && self.dataset.y) {
-            let x = parseFloat(self.dataset.x);
-            let y = parseFloat(self.dataset.y);
-            ({ x, y } = getExpandPosition(useModal ?? false, {
-              x,
-              y,
-              w,
-              h,
-              iconW,
-              iconH,
-              pivot,
-              follow,
-              expandOffsetX,
-              expandOffsetY,
-            }));
-            setTransform(`matrix(1,0,0,1,${x},${y})`);
-          }
-          if (!noExpand) {
-            setExpand(!expand);
-          }
-          onFloatingButtonClick?.();
-        }}
-        opacity={isInvisible ? 0 : 1}
-        visibility={isInvisible ? "hidden" : "visible"}
-        transition={VISIBILITY_TRANSITION}
-        {...commonProps}
-        {...props}>
-        <Image src={src} draggable={false} />
-      </Box>
-      {!noExpand && (
-        <Portal containerRef={ref as any}>
-          <Flex
-            id={expandId}
-            w={`${w}px`}
-            h={`${h}px`}
-            overflowY="auto"
-            overflowX="hidden"
-            direction="column"
-            transform={transform}
-            opacity={expand ? 1 : 0}
-            visibility={expand ? "visible" : "hidden"}
-            transition={VISIBILITY_TRANSITION}
-            {...commonProps}
-            bg={expandBg}
-            {...parsedExpandProps}>
-            {children}
-          </Flex>
-        </Portal>
-      )}
-    </>
+    <Floating id={_id} ref={containerRef} renderInfo={updatedRenderInfo} {...props}>
+      {children}
+    </Floating>
   );
-});
+}) as ChakraComponent<"div", {}>;
 
-export default observer(Floating);
+export default observer(Render);
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/index.tsx` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/index.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import { Logger, shallowCopy } from "@carefree0910/core";
 import { useSelecting } from "@carefree0910/business";
 
 import type { AvailablePluginsAndPythonPlugins, IMakePlugin } from "@/schema/plugins";
-import { pluginIsVisible, pythonPluginIsVisible } from "@/stores/plugins";
+import { pluginIsVisible, pythonPluginIsVisible } from "@/stores/pluginVisible";
 import { drawboardPluginFactory } from "./utils/factory";
 import { getNodeFilter } from "./utils/renderFilters";
 
 // these lines are needed to make sure the plugins are registered
+export * from "./MetaPlugin";
 export * from "./SettingsPlugin";
 export * from "./ProjectPlugin";
 export * from "./AddPlugin";
 export * from "./ArrangePlugin";
 export * from "./UndoRedoPlugin";
 export * from "./DownloadPlugin";
 export * from "./DeletePlugin";
 export * from "./TextEditorPlugin";
 export * from "./GroupPlugin";
 export * from "./LinksPlugin";
 export * from "./BrushPlugin";
-export * from "./_python/HttpTextAreaPlugin";
-export * from "./_python/HttpQAPlugin";
-export * from "./_python/HttpFieldsPlugin";
+export * from "./_python/TextAreaPlugin";
+export * from "./_python/QAPlugin";
+export * from "./_python/FieldsPlugin";
 
 export function makePlugin<T extends AvailablePluginsAndPythonPlugins>({
   key,
   type,
   containerRef,
   props: { renderInfo, pluginInfo, ...props },
 }: IMakePlugin<T> & { key: string }) {
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/meta.ts`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import type { Dictionary, Lang } from "@carefree0910/core";
 
 import type { IToast } from "./misc";
 
 // general
 
-export const allMetaTypes = ["upload", "python.httpFields", "add.text", "add.sketch.path"] as const;
-export type MetaType = typeof allMetaTypes[number];
+export const allMetaTypes = ["upload", "add.text", "add.sketch.path", "python.fields"] as const;
+export type MetaType = (typeof allMetaTypes)[number];
 export interface ICommonMetaData<T extends _IMetaData = _IMetaData> {
+  alias?: string;
   timestamp?: number;
   duration?: number;
   from?: IMeta<T>;
 }
 type _IMetaData = ICommonMetaData & Dictionary<any>;
 export interface IMeta<T extends _IMetaData = _IMetaData> {
   type: MetaType;
@@ -21,29 +22,29 @@
 
 interface IUploadMetaData extends ICommonMetaData {
   w: number;
   h: number;
   url: string;
   isDrag: boolean;
 }
-export type IPythonHttpFieldsResponse = { _duration?: number } & (
+export type IPythonResults = { _duration?: number } & (
   | { type: "text"; value: string[] }
   | { type: "image"; value: { w: number; h: number; url: string }[] }
 );
-export type IPythonHttpFieldsMetaData = ICommonMetaData & {
+export type IPythonFieldsMetaData = ICommonMetaData & {
   identifier: string;
   parameters: Dictionary<any>;
-  response: IPythonHttpFieldsResponse;
+  response: IPythonResults;
 };
 
 export interface IMetaData {
   upload: IUploadMetaData;
   "add.text": ICommonMetaData;
   "add.sketch.path": ICommonMetaData;
-  "python.httpFields": IPythonHttpFieldsMetaData;
+  "python.fields": IPythonFieldsMetaData;
 }
 
 export interface IImportMeta<T extends MetaType> {
   t: IToast;
   lang: Lang;
   type: T;
   metaData: IMetaData[T];
@@ -54,7 +55,11 @@
 export function checkMeta(meta: any): meta is IMeta {
   return allMetaTypes.includes(meta?.type);
 }
 export function getOriginMeta(meta: any): IMeta | undefined {
   if (!checkMeta(meta)) return;
   return getOriginMeta(meta.data.from);
 }
+export function getMetaTrace(meta: IMeta): IMeta[] {
+  if (!checkMeta(meta)) return [];
+  return [meta, ...(meta.data.from ? getMetaTrace(meta.data.from) : [])];
+}
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/metaFields.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/metaFields.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/plugins.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import type { RefObject } from "react";
 import type { FlexProps } from "@chakra-ui/react";
 
 import type { INode, NodeType, PivotType } from "@carefree0910/core";
 import type { IResponse } from "@carefree0910/business";
 
 import type { IFieldDefinition, _IFieldDefinition } from "./metaFields";
-import type {
-  IPythonHttpFieldsPlugin,
-  IPythonHttpQAPlugin,
-  IPythonHttpTextAreaPlugin,
-} from "./_python";
+import type { IPythonFieldsPlugin, IPythonQAPlugin, IPythonTextAreaPlugin } from "./_python";
 
 // general
 
 export type NodeConstraints = NodeType | "none" | "anyNode" | "singleNode" | "multiNode";
-export interface IPositionInfo {
+export interface IExpandPositionInfo {
   w: number;
   h: number;
   iconW: number;
   iconH: number;
   pivot: PivotType;
   follow: boolean;
   expandOffsetX: number;
   expandOffsetY: number;
 }
-export interface IRenderInfo extends IPositionInfo {
+export interface IRenderInfo extends IExpandPositionInfo {
   src?: string;
+  offsetX?: number;
+  offsetY?: number;
   bgOpacity?: number;
   renderFilter?: (info?: IResponse) => boolean;
   useModal?: boolean;
   modalOpacity?: number;
   expandProps?: FlexProps;
   isInvisible?: boolean;
 }
@@ -37,16 +35,14 @@
   id: string;
   renderInfo: IRenderInfo;
   noExpand?: boolean;
   onFloatingButtonClick?: () => Promise<void>;
 }
 export interface IRender extends Omit<IFloating, "id" | "renderInfo"> {
   id?: string;
-  offsetX?: number;
-  offsetY?: number;
   nodeConstraint: NodeConstraints;
   renderInfo: Partial<IRenderInfo> & { w: number; h: number };
   containerRef?: RefObject<HTMLDivElement>;
 }
 export interface IPluginInfo {
   node: INode | null;
   nodes: INode[];
@@ -61,14 +57,15 @@
   field: string;
   definition: IFieldDefinition<T>;
 }
 
 // factory
 
 export const allAvailablePlugins = [
+  "meta",
   "settings",
   "project",
   "add",
   "arrange",
   "undo",
   "redo",
   "download",
@@ -78,20 +75,20 @@
   "email",
   "textEditor",
   "groupEditor",
   "multiEditor",
   "brush",
 ] as const;
 export const allAvailablePythonPlugins = [
-  "_python.httpTextArea",
-  "_python.httpQA",
-  "_python.httpFields",
+  "_python.textArea",
+  "_python.QA",
+  "_python.fields",
 ] as const;
-export type AvailablePlugins = typeof allAvailablePlugins[number];
-export type AvailablePythonPlugins = typeof allAvailablePythonPlugins[number];
+export type AvailablePlugins = (typeof allAvailablePlugins)[number];
+export type AvailablePythonPlugins = (typeof allAvailablePythonPlugins)[number];
 export type AvailablePluginsAndPythonPlugins = AvailablePlugins | AvailablePythonPlugins;
 
 export interface IPluginProps {
   // react plugins
   meta: IPlugin;
   settings: IPlugin;
   project: IPlugin;
@@ -105,17 +102,17 @@
   github: IPlugin;
   email: IPlugin;
   textEditor: IPlugin;
   groupEditor: IPlugin;
   multiEditor: IPlugin;
   brush: IPlugin;
   // python plugins
-  "_python.httpTextArea": IPythonHttpTextAreaPlugin;
-  "_python.httpQA": IPythonHttpQAPlugin;
-  "_python.httpFields": IPythonHttpFieldsPlugin;
+  "_python.textArea": IPythonTextAreaPlugin;
+  "_python.QA": IPythonQAPlugin;
+  "_python.fields": IPythonFieldsPlugin;
 }
 
 export interface IMakePlugin<T extends AvailablePluginsAndPythonPlugins> {
   type: T;
   props: Omit<IPluginProps[T], "containerRef" | "pluginInfo"> & {
     pluginInfo: Omit<IPluginProps[T]["pluginInfo"], "node" | "nodes">;
   };
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/_python.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/_python.ts`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 import { ABCStore } from "@carefree0910/business";
 
 import type { AvailablePythonPlugins, IMakePlugin } from "@/schema/plugins";
 
 interface IGlobalSettings {
   timeout?: number;
   useStrictMode?: boolean;
-  sockenEndpoint?: string;
+  socketEndpoint?: string;
 }
 export interface IPythonStore {
   pluginSettings: IMakePlugin<AvailablePythonPlugins>[];
-  globalSettings: IGlobalSettings;
+  globalSettings?: IGlobalSettings;
 }
 class PythonStore extends ABCStore<IPythonStore> implements IPythonStore {
   hash: string = "";
   pluginSettings: IMakePlugin<AvailablePythonPlugins>[] = [];
-  globalSettings: IGlobalSettings = {};
+  globalSettings?: IGlobalSettings;
 
   constructor() {
     super();
     makeObservable(this, {
       hash: observable,
       pluginSettings: observable,
       globalSettings: observable,
@@ -37,11 +37,14 @@
 export const usePythonPluginSettings = () => pythonStore.pluginSettings;
 export const updatePythonStore = (data: IPythonStore): boolean => {
   const incomingHash = getHash(JSON.stringify(data)).toString();
   if (pythonStore.hash === incomingHash) return false;
   runInAction(() => {
     pythonStore.hash = incomingHash;
     pythonStore.pluginSettings = data.pluginSettings;
-    pythonStore.globalSettings = data.globalSettings;
+    // `globalSettings` should only be updated once.
+    if (!pythonStore.globalSettings) {
+      pythonStore.globalSettings = data.globalSettings;
+    }
   });
   return true;
 };
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/gridLines.ts`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 }
 class GridLinesStore extends ABCStore<IGridLinesStore> implements IGridLinesStore {
   enable = true;
   lineWidth = 1;
   lineColor = "208,208,208";
   maxOpacity = 0.8;
   maxGridSize = 250;
-  span = 5;
+  span = 4;
   startSubGridsFraction = 0.45;
 
   constructor() {
     super();
     makeObservable(this, {
       enable: observable,
       lineWidth: observable,
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/meta.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/plugins.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/pluginVisible.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/theme.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/theme.ts`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,23 @@
   // styles for the `CFSwitch` component
   switchColors: {
     checkedBgColor: string;
     uncheckedBgColor: string;
   };
   // styles for the `brush`
   defaultBrushStyles: Partial<IPathOptions>;
+  // styles for the `CFCircularProgress` component
+  circularProgressColors: {
+    pendingColor: string;
+    workingColor: string;
+  };
+  // styles for the `Floating` component
+  floatingColors: {
+    busyColor: string;
+  };
 };
 
 export const allThemes: Record<ThemeType, ThemeStyles> = {
   light: {
     boardBg: "#f7f7f7",
     panelBg: "#f9f9f9",
     textColor: "#333333",
@@ -64,14 +73,21 @@
       uncheckedBgColor: "#dddddd",
     },
     defaultBrushStyles: {
       stroke: "rgba(96, 120, 244, 0.6)",
       fill: "rgba(96, 120, 244, 0.4)",
       width: 3,
     },
+    circularProgressColors: {
+      pendingColor: "#5e7fd8",
+      workingColor: "#3fc9a8",
+    },
+    floatingColors: {
+      busyColor: "#999999",
+    },
   },
   // currently dark mode is just a placeholder
   dark: {
     boardBg: "#242424",
     panelBg: "#f9f9f9",
     textColor: "#333333",
     captionColor: "#888888",
@@ -94,14 +110,21 @@
       uncheckedBgColor: "#dddddd",
     },
     defaultBrushStyles: {
       stroke: "rgba(96, 120, 244, 0.7)",
       fill: "rgba(96, 120, 244, 0.7)",
       width: 3,
     },
+    circularProgressColors: {
+      pendingColor: "#5e7fd8",
+      workingColor: "#3fc9a8",
+    },
+    floatingColors: {
+      busyColor: "#999999",
+    },
   },
 };
 
 export interface IThemeStore {
   theme: ThemeType;
 }
 class ThemeStore extends ABCStore<IThemeStore> implements IThemeStore {
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/stores/ui.ts`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import type { AvailablePlugins } from "@/schema/plugins";
 import { reactPluginSettings } from "@/_settings";
 import {
   pluginIsVisible,
   pythonPluginIsVisible,
   setPluginVisible,
   setPythonPluginVisible,
-} from "./plugins";
+} from "./pluginVisible";
 import { usePythonPluginSettings } from "./_python";
 
 export interface IUIStore {
   disablePluginSettings: boolean;
 }
 class UIStore extends ABCStore<IUIStore> implements IUIStore {
   disablePluginSettings: boolean = false;
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/misc.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 // {identifier}.{hash}
 export function stripHashFromIdentifier(identifierWithHash: string): string {
-  return identifierWithHash.split(".").slice(0, -1).join(".");
+  return identifierWithHash.includes(".")
+    ? identifierWithHash.split(".").slice(0, -1).join(".")
+    : identifierWithHash;
 }
 
 export function isDate(time: Date | number) {
   return time instanceof Date;
 }
 export function formatTime(time: Date | number, pattern = "YYYY-MM-DD HH:mm:ss") {
   const dateTime: Date = !isDate(time) ? new Date(time) : (time as Date);
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/toast.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/src/utils/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.0a7/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/vite.config.ts` & `carefree-drawboard-0.0.0a7/cfdraw/.web/vite.config.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.0a7/cfdraw/.web/yarn.lock`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/app/app.py` & `carefree-drawboard-0.0.0a7/cfdraw/app/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,98 +1,106 @@
 from typing import Dict
 from typing import List
+from typing import AsyncGenerator
 from aiohttp import ClientSession
 from fastapi import FastAPI
+from contextlib import asynccontextmanager
 from cftool.misc import print_info
 from cftool.misc import random_hash
 from fastapi.middleware import cors
 
 from cfdraw import constants
 from cfdraw.config import get_config
 from cfdraw.app.schema import IApp
 from cfdraw.app.endpoints import *
-from cfdraw.schema.plugins import IPlugin
+from cfdraw.plugins.factory import Plugins
 from cfdraw.plugins.factory import PluginFactory
 
 
 async def ping() -> str:
     return "pong"
 
 
 class App(IApp):
     def __init__(self) -> None:
+        # FastAPI lifspan
+
+        @asynccontextmanager
+        async def lifespan(api: FastAPI) -> AsyncGenerator:
+            # startup
+
+            def info(msg: str) -> None:
+                print_info(msg)
+
+            self.hash = random_hash()
+            info(f"🚀 Starting Backend Server at {self.config.api_url} ...")
+            info("🔨 Compiling Plugins & Endpoints...")
+            for plugin_type in self.plugins.values():
+                plugin_type.hash = self.hash
+                plugin_type.http_session = self.http_session
+            for endpoint in self.endpoints:
+                await endpoint.on_startup()
+            upload_root_path = self.config.upload_root_path
+            info(f"🔔 Your files will be saved to '{upload_root_path}'")
+            info("🎉 Backend Server is Ready!")
+
+            yield
+
+            # shutdown
+
+            await self.http_session.close()
+            for plugin_type in self.plugins.values():
+                plugin_type.http_session = None
+            for endpoint in self.endpoints:
+                await endpoint.on_shutdown()
+            self.http_session = None
+
         # config
         self.config = get_config()
         # clients
         self.http_session = ClientSession()
+        # queue
+        self.request_queue = RequestQueue()
         # fastapi
-        self.api = FastAPI()
+        self.api = FastAPI(lifespan=lifespan)
         self.add_cors()
         self.add_default_endpoints()
-        self.add_events()
         self.endpoints: List[IEndpoint] = [
             UploadEndpoint(self),
             ProjectEndpoint(self),
-            PluginsEndpoint(self),
             WebsocketEndpoint(self),
         ]
+        if self.config.use_unified:
+            self.endpoints.append(AssetsEndpoint(self))
         for endpoint in self.endpoints:
             endpoint.register()
         self.hash = random_hash()
 
     def __str__(self) -> str:
         return "<App />"
 
     __repr__ = __str__
 
     @property
-    def plugins(self) -> Dict[str, IPlugin]:
+    def plugins(self) -> Plugins:
         return PluginFactory.plugins
 
     @property
-    def internal_plugins(self) -> Dict[str, IPlugin]:
+    def internal_plugins(self) -> Plugins:
         return PluginFactory.internal_plugins
 
     def add_cors(self) -> None:
         self.api.add_middleware(
             cors.CORSMiddleware,
             allow_credentials=True,
             allow_methods=["*"],
             allow_headers=["*"],
             allow_origins=["*"],
         )
 
-    def add_events(self) -> None:
-        @self.api.on_event("startup")
-        async def startup() -> None:
-            def info(msg: str) -> None:
-                if not self.config.use_tornado:
-                    print_info(msg)
-
-            self.hash = random_hash()
-            info(f"🚀 Starting Backend Server at {self.config.api_url} ...")
-            info("🔨 Compiling Plugins & Endpoints...")
-            for plugin in self.plugins.values():
-                plugin.hash = self.hash
-                plugin.http_session = self.http_session
-            for endpoint in self.endpoints:
-                await endpoint.on_startup()
-            upload_root_path = self.config.upload_root_path
-            info(f"🔔 Your files will be saved to '{upload_root_path}'")
-            info("🎉 Backend Server is Ready!")
-
-        @self.api.on_event("shutdown")
-        async def shutdown() -> None:
-            await self.http_session.close()
-            for plugin in self.plugins.values():
-                plugin.http_session = None
-            for endpoint in self.endpoints:
-                await endpoint.on_shutdown()
-            self.http_session = None
-
     def add_default_endpoints(self) -> None:
         self.api.get(str(constants.Endpoint.PING))(ping)
 
 
 __all__ = [
     "App",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/plugins.py` & `carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/upload.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,73 @@
-from cftool.misc import print_info
+from io import BytesIO
+from PIL import Image
+from typing import Optional
+from fastapi import File
+from fastapi import Response
+from fastapi import UploadFile
+from pydantic import BaseModel
 
+from cfdraw import constants
+from cfdraw.utils import server
 from cfdraw.app.schema import IApp
 from cfdraw.utils.server import get_err_msg
 from cfdraw.utils.server import get_responses
-from cfdraw.schema.plugins import IPluginRequest
-from cfdraw.schema.plugins import IPluginResponse
-from cfdraw.plugins.base import IHttpPlugin
-from cfdraw.plugins.base import ISocketPlugin
+from cfdraw.utils.server import get_image_response_kwargs
 from cfdraw.app.endpoints.base import IEndpoint
 
 
-def add_plugins(app: IApp) -> None:
-    for identifier, plugin in app.plugins.items():
-        if not isinstance(plugin, IHttpPlugin):
-            continue
-        endpoint = f"/{identifier}"
-        if not app.config.prod:
-            print_info(f"registering endpoint '{endpoint}'")
-
-        def _register(_id: str, _p: IHttpPlugin) -> None:
-            @app.api.post(
-                endpoint,
-                name=endpoint[1:].replace("/", "_"),
-                responses=get_responses(IPluginResponse),
-            )
-            async def fn(data: IPluginRequest) -> IPluginResponse:
-                if _p.hash_identifier(_id) != data.identifier:
-                    return IPluginResponse(
-                        success=False,
-                        message=(
-                            f"internal error occurred: identifier mismatch, "
-                            f"current hash is {_p.hash_identifier(_id)} "
-                            f"but incoming identifier is {data.identifier}"
-                        ),
-                        data={},
-                    )
-                try:
-                    return await _p(data)
-                except Exception as err:
-                    err_msg = get_err_msg(err)
-                    return IPluginResponse(success=False, message=err_msg, data={})
+class ImageDataModel(BaseModel):
+    w: int
+    h: int
+    url: str
+
+
+class UploadImageResponse(BaseModel):
+    success: bool
+    message: str
+    data: Optional[ImageDataModel]
+
+
+class FetchImageModel(BaseModel):
+    url: str
+    jpeg: bool
+
+
+def add_upload_image(app: IApp) -> None:
+    @app.api.post("/upload_image", responses=get_responses(UploadImageResponse))
+    def upload_image(image: UploadFile = File(...)) -> UploadImageResponse:
+        try:
+            contents = image.file.read()
+            loaded_image = Image.open(BytesIO(contents))
+            res = server.upload_image(loaded_image)
+        except Exception as err:
+            err_msg = get_err_msg(err)
+            return UploadImageResponse(success=False, message=err_msg, data=None)
+        finally:
+            image.file.close()
+        return UploadImageResponse(
+            success=True,
+            message="",
+            data=ImageDataModel(**res),
+        )
+
+    @app.api.post("/fetch_image", **get_image_response_kwargs())
+    async def fetch_image(data: FetchImageModel) -> Response:
+        file = data.url.split(constants.UPLOAD_IMAGE_FOLDER_NAME)[1][1:]  # remove '/'
+        return server.get_image_response(file, data.jpeg)
+
+    @app.api.get(
+        f"/{constants.UPLOAD_IMAGE_FOLDER_NAME}/{{file}}/",
+        **get_image_response_kwargs(),
+    )
+    async def get_image(file: str, jpeg: bool = False) -> Response:
+        return server.get_image_response(file, jpeg)
 
-        _register(identifier, plugin)
 
-
-class PluginsEndpoint(IEndpoint):
+class UploadEndpoint(IEndpoint):
     def register(self) -> None:
-        add_plugins(self.app)
+        add_upload_image(self.app)
 
 
 __all__ = [
-    "PluginsEndpoint",
+    "UploadEndpoint",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.0a7/cfdraw/app/endpoints/project.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.0a7/cfdraw/plugins/middlewares/fields.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,30 @@
-from io import BytesIO
-from PIL import Image
-from typing import Optional
-from fastapi import File
-from fastapi import Response
-from fastapi import UploadFile
-from pydantic import BaseModel
-
-from cfdraw import constants
-from cfdraw.utils import server
-from cfdraw.app.schema import IApp
-from cfdraw.utils.server import get_err_msg
-from cfdraw.utils.server import get_responses
-from cfdraw.utils.server import get_image_response_kwargs
-from cfdraw.app.endpoints.base import IEndpoint
-
-
-class ImageDataModel(BaseModel):
-    w: int
-    h: int
-    url: str
-
-
-class UploadImageResponse(BaseModel):
-    success: bool
-    message: str
-    data: Optional[ImageDataModel]
-
-
-def add_upload_image(app: IApp) -> None:
-    @app.api.post("/upload_image", responses=get_responses(UploadImageResponse))
-    def upload_image(image: UploadFile = File(...)) -> UploadImageResponse:
-        try:
-            contents = image.file.read()
-            loaded_image = Image.open(BytesIO(contents))
-            res = server.upload_image(loaded_image)
-        except Exception as err:
-            err_msg = get_err_msg(err)
-            return UploadImageResponse(success=False, message=err_msg, data=None)
-        finally:
-            image.file.close()
-        return UploadImageResponse(
-            success=True,
-            message="",
-            data=ImageDataModel(**res),
-        )
-
-    @app.api.get(
-        f"/{constants.UPLOAD_IMAGE_FOLDER_NAME}/{{file}}/",
-        **get_image_response_kwargs(),
-    )
-    async def fetch_image(file: str, jpeg: bool = False) -> Response:
-        return server.get_image_response(file, jpeg)
-
-
-class UploadEndpoint(IEndpoint):
-    def register(self) -> None:
-        add_upload_image(self.app)
+from typing import List
+from typing import Union
+from PIL.Image import Image
+
+from cfdraw.utils.server import upload_image
+from cfdraw.schema.plugins import PluginType
+from cfdraw.schema.plugins import IMiddleWare
+from cfdraw.schema.plugins import ISocketMessage
+
+
+class FieldsMiddleWare(IMiddleWare):
+    @property
+    def subscriptions(self) -> List[PluginType]:
+        return [PluginType.FIELDS]
+
+    async def process(
+        self,
+        response: Union[str, List[str], Image, List[Image]],
+    ) -> ISocketMessage:
+        if not isinstance(response, list):
+            response = [response]
+        if isinstance(response[0], str):
+            return self.make_success(dict(type="text", value=response))
+        urls = [upload_image(image) for image in response]
+        return self.make_success(dict(type="image", value=urls))
 
 
 __all__ = [
-    "UploadEndpoint",
+    "FieldsMiddleWare",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/cli.py` & `carefree-drawboard-0.0.0a7/cfdraw/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,55 +23,53 @@
     no_frontend: bool = typer.Option(False, help="Whether not to run the frontend."),
     no_backend: bool = typer.Option(False, help="Whether not to run the backend."),
     log_level: constants.LogLevel = typer.Option(
         constants.LogLevel.ERROR,
         help="The log level to use.",
     ),
     prod: bool = typer.Option(False, help="Whether to run in production mode."),
-    tornado: bool = typer.Option(False, help="Whether use tornado to unify servers."),
+    unified: bool = typer.Option(False, help="Whether use unified servers."),
+    host: bool = typer.Option(False, help="Whether use `--host` in development mode."),
 ) -> None:
     sys.path.insert(0, os.getcwd())
-    if tornado:
+    if unified:
         if not prod:
             console.print(
-                "[bold orange1]Tornado is only available in production mode, "
+                "[bold orange1]`--unified` is only available in production mode, "
                 "so `--prod` flag will be forced."
             )
             prod = True
     constants.set_env(constants.Env.PROD if prod else constants.Env.DEV)
-    constants.set_tornado(tornado)
+    constants.set_unified(unified)
     # fetch config
     config = get_config()
     # fetch module
     if module is None:
         module = constants.DEFAULT_MODULE
     if module.endswith(".py"):
         module = module[:-3]
     path_prefix = f".{os.path.sep}"
     if module.startswith(path_prefix):
         module = module[len(path_prefix) :]
     console.rule(f"[bold green]Running {module}")
     # execute
     frontend_port = config.frontend_port
     backend_port = config.backend_port
-    tornado_port = config.tornado_port
     if not no_frontend and processes.is_process_on_port(frontend_port):
         frontend_port = processes.change_or_terminate_port(frontend_port, "frontend")
     if not no_backend and processes.is_process_on_port(backend_port):
         backend_port = processes.change_or_terminate_port(backend_port, "backend")
-    if tornado and not no_backend and processes.is_process_on_port(tornado_port):
-        tornado_port = processes.change_or_terminate_port(tornado_port, "tornado")
     config.frontend_port = frontend_port
     config.backend_port = backend_port
-    config.tornado_port = tornado_port
     if not prod:
-        frontend_fn, backend_fn = exec.run_frontend, exec.run_backend
+        frontend_fn = lambda: exec.run_frontend(host)
+        backend_fn = exec.run_backend
     else:
         frontend_fn = exec.run_frontend_prod
-        backend_fn = exec.run_tornado if tornado else exec.run_backend
+        backend_fn = exec.run_backend_prod  # type: ignore
     try:
         if not no_frontend:
             frontend_fn()
         if not no_backend:
             backend_fn(module, log_level=log_level)
     finally:
         console.rule("[bold]Shutting down")
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/config.py` & `carefree-drawboard-0.0.0a7/cfdraw/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,46 +13,49 @@
 class Config:
     # app
     entry: str = constants.DEFAULT_ENTRY
     # frontend
     frontend_port: str = constants.FRONTEND_PORT
     # api
     backend_port: str = constants.BACKEND_PORT
-    tornado_port: str = constants.TORNADO_PORT
     backend_hosting_url: Optional[str] = None  # this must be provided for hosting
     # upload
     upload_root: str = str(constants.UPLOAD_ROOT)
     # misc
     use_react_strict_mode: bool = False
 
     @property
     def prod(self) -> bool:
         return constants.get_env() == constants.Env.PROD
 
     @property
-    def use_tornado(self) -> bool:
-        return constants.use_tornado()
+    def use_unified(self) -> bool:
+        return constants.use_unified()
 
     @property
     def api_port(self) -> str:
-        return self.tornado_port if self.use_tornado else self.backend_port
+        return self.backend_port
 
     @property
     def api_url(self) -> str:
         if self.backend_hosting_url is not None:
             api_url = self.backend_hosting_url
         else:
             env_api_url = os.environ.get(constants.API_URL_KEY)
             if env_api_url is not None:
                 api_url = env_api_url
             else:
                 api_url = f"http://localhost:{self.api_port}"
         return api_url.rstrip("/").rstrip("\\")
 
     @property
+    def frontend_url(self) -> str:
+        return f"http://localhost:{self.frontend_port}"
+
+    @property
     def upload_root_path(self) -> Path:
         return Path(self.upload_root).absolute()
 
     @property
     def upload_image_folder(self) -> Path:
         folder = self.upload_root_path / constants.UPLOAD_IMAGE_FOLDER_NAME
         folder.mkdir(parents=True, exist_ok=True)
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/constants.py` & `carefree-drawboard-0.0.0a7/cfdraw/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 # frontend
 FRONTEND_PORT = "5123"
 
 # api
 ERR_CODE = 406
 BACKEND_PORT = "8123"
-TORNADO_PORT = "8234"
 DEV_BACKEND_HOST = "0.0.0.0"
 API_URL_KEY = "CFDRAW_API_URL"
 
 
 class Endpoint(Enum):
     PING = "ping"
     WEBSOCKET = "ws"
@@ -29,15 +28,15 @@
         return f"/{self.value}"
 
     __repr__ = __str__
 
 
 # misc
 ENV_KEY = "CFDRAW_ENV"
-TORNADO_KEY = "CFDRAW_TORNADO"
+UNIFIED_KEY = "CFDRAW_UNIFIED"
 
 
 class Env(str, Enum):
     DEV = "development"
     PROD = "production"
 
 
@@ -45,20 +44,20 @@
     return os.environ.get(ENV_KEY, Env.DEV)  # type: ignore
 
 
 def set_env(env: Env) -> None:
     os.environ[ENV_KEY] = env.value
 
 
-def use_tornado() -> bool:
-    return os.environ.get(TORNADO_KEY, None) == "enabled"
+def use_unified() -> bool:
+    return os.environ.get(UNIFIED_KEY, None) == "enabled"
 
 
-def set_tornado(enable: bool) -> None:
-    os.environ[TORNADO_KEY] = "enabled" if enable else "disabled"
+def set_unified(enable: bool) -> None:
+    os.environ[UNIFIED_KEY] = "enabled" if enable else "disabled"
 
 
 class LogLevel(str, Enum):
     DEBUG = "debug"
     INFO = "info"
     WARNING = "warning"
     ERROR = "error"
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.0a7/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/parsers/noli.py` & `carefree-drawboard-0.0.0a7/cfdraw/parsers/noli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import math
 
+import numpy as np
+
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 from typing import Optional
 from typing import Generator
 from pydantic import BaseModel
+from dataclasses import dataclass
 
 
 class PivotType(str, Enum):
     LT = "lt"
     TOP = "top"
     RT = "rt"
     LEFT = "left"
@@ -45,22 +48,40 @@
     SINGLE_NODE = "singleNode"
     MULTI_NODE = "multiNode"
 
 
 # data structures
 
 
+@dataclass
+class Point:
+    x: float
+    y: float
+
+    @property
+    def tuple(self) -> Tuple[float, float]:
+        return self.x, self.y
+
+    def __rmatmul__(self, other: "Matrix2D") -> "Point":
+        a, b, c, d, e, f = [pair[1] for pair in other]
+        x, y = self.x, self.y
+        return Point(x=a * x + c * y + e, y=b * x + d * y + f)
+
+
 class Matrix2D(BaseModel):
     a: float
     b: float
     c: float
     d: float
     e: float
     f: float
 
+    def __matmul__(self, other: Point) -> Point:
+        return other.__rmatmul__(self)
+
     @property
     def w(self) -> float:
         return math.sqrt(self.a**2 + self.b**2)
 
     @property
     def h(self) -> float:
         return (self.a * self.d - self.b * self.c) / max(self.w, 1.0e-12)
@@ -90,14 +111,18 @@
             "theta": self.theta,
             "skew_x": math.atan2(a * c + b * d, w**2),
             "skew_y": 0.0,
             "w": w,
             "h": h,
         }
 
+    @property
+    def matrix(self) -> np.ndarray:
+        return np.array([[self.a, self.c, self.e], [self.b, self.d, self.f]])
+
 
 class SingleNodeType(str, Enum):
     POLYGON = "polygon"
     ELLIPSE = "ellipse"
     RECTANGLE = "rectangle"
     STAR = "star"
     LINE = "line"
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/plugins/base.py` & `carefree-drawboard-0.0.0a7/cfdraw/plugins/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from io import BytesIO
 from abc import abstractmethod
 from abc import ABCMeta
 from PIL import Image
 from typing import Any
 from typing import Dict
 from typing import List
-from typing import Callable
-from typing import Coroutine
+from typing import Optional
 
 from cfdraw import constants
 from cfdraw.utils import server
+from cfdraw.utils.misc import deprecated
+from cfdraw.utils.misc import offload_run
 from cfdraw.schema.plugins import *
 from cfdraw.plugins.middlewares import *
 from cfdraw.parsers.noli import SingleNodeType
 from cfdraw.parsers.noli import NodeConstraints
 from cfdraw.parsers.chakra import IChakra
 
 
-class IBasePlugin(IPlugin, metaclass=ABCMeta):
+class ISocketPlugin(IPlugin, metaclass=ABCMeta):
     @abstractmethod
-    async def process(self, data: IPluginRequest) -> Any:
+    async def process(self, data: ISocketRequest) -> Any:
         pass
 
+    # internal APIs
+
     @property
     def middlewares(self) -> List[IMiddleWare]:
-        return []
+        common_middlewares: List[IMiddleWare] = [
+            TextAreaMiddleWare(self.send_message),
+            FieldsMiddleWare(self.send_message),
+            TimerMiddleWare(self.send_message),
+        ]
+        send_message_middleware = SendSocketMessageMiddleWare(self.send_message)
+        return common_middlewares + [send_message_middleware]
 
-    async def __call__(self, data: IPluginRequest) -> IPluginResponse:
+    async def __call__(self, data: ISocketRequest) -> ISocketMessage:
         middlewares = self.middlewares
         for middleware in middlewares:
             await middleware.before(data)
         response = await self.process(data)
         for middleware in middlewares:
             response = await middleware(self, response)
         return response
@@ -41,16 +50,14 @@
     def to_plugin_settings(self) -> Dict[str, Any]:
         d = self.settings.dict()
         plugin_info = d.pop("pluginInfo")
         # `identifier` has hashed into `{identifier}.{hash}`
         plugin_info["endpoint"] = f"/{self.identifier}"
         plugin_info["identifier"] = self.hash_identifier(self.identifier)
         plugin_type = f"_python.{self.type}"
-        offset_x = d.pop("offsetX")
-        offset_y = d.pop("offsetY")
         node_constraint = d.pop("nodeConstraint")
         chakra_props = {}
         for field in IChakra.__fields__:
             chakra_value = d.pop(field)
             if chakra_value is not None:
                 chakra_props[field] = chakra_value
         for k, v in list(d.items()):
@@ -58,45 +65,37 @@
                 d.pop(k)
         props = dict(
             nodeConstraint=node_constraint,
             pluginInfo=plugin_info,
             renderInfo=d,
             **chakra_props,
         )
-        if offset_x is not None:
-            props["offsetX"] = offset_x
-        if offset_y is not None:
-            props["offsetY"] = offset_y
         return dict(type=plugin_type, props=props)
 
+    # helper methods
+
     def filter(self, nodes: List[INodeData], target: SingleNodeType) -> List[INodeData]:
         return list(filter(lambda node: node.type == target, nodes))
 
     async def load_image(self, src: str) -> Image.Image:
         # check whether the incoming url refers to a local image
         # if so, load it from the local file system directly
         if src.startswith("http://") and constants.UPLOAD_IMAGE_FOLDER_NAME in src:
             file = src.split(constants.UPLOAD_IMAGE_FOLDER_NAME)[1][1:]  # remove '/'
             return server.get_image(file)
         async with self.http_session.get(src) as res:
             return Image.open(BytesIO(await res.read()))
 
-
-class IHttpPlugin(IBasePlugin, metaclass=ABCMeta):
-    @property
-    def middlewares(self) -> List[IMiddleWare]:
-        return [TextAreaMiddleWare(), FieldsMiddleWare(), TimerMiddleWare()]
-
-
-class ISocketPlugin(IBasePlugin, metaclass=ABCMeta):
-    send_text: Callable[[ISocketMessage], Coroutine[Any, Any, None]]
-
-    @abstractmethod
-    async def process(self, data: IPluginRequest) -> ISocketMessage:
-        pass
+    def send_progress(
+        self,
+        progress: float,
+        intermediate: Optional[ISocketIntermediate] = None,
+    ) -> None:
+        message = ISocketMessage.make_progress(self.task_hash, progress, intermediate)
+        offload_run(self.send_message(message))
 
 
 class IInternalSocketPlugin(ISocketPlugin, metaclass=ABCMeta):
     @property
     def type(self) -> PluginType:
         return PluginType._INTERNAL
 
@@ -104,33 +103,60 @@
     def settings(self) -> IPluginSettings:
         return IPluginSettings(w=1, h=1, nodeConstraint=NodeConstraints.NONE)
 
 
 # bindings
 
 
-class IHttpTextAreaPlugin(IHttpPlugin):
+class ITextAreaPlugin(ISocketPlugin):
     @property
     def type(self) -> PluginType:
-        return PluginType.HTTP_TEXT_AREA
+        return PluginType.TEXT_AREA
 
 
-class IHttpQAPlugin(IHttpPlugin):
+class IQAPlugin(ISocketPlugin):
     @property
     def type(self) -> PluginType:
-        return PluginType.HTTP_QA
+        return PluginType.QA
 
 
-class IHttpFieldsPlugin(IHttpPlugin):
+class IFieldsPlugin(ISocketPlugin):
     @property
     def type(self) -> PluginType:
-        return PluginType.HTTP_FIELDS
+        return PluginType.FIELDS
+
+
+## deprecated
+
+
+@deprecated("please use `ISocketPlugin` instead")
+class IHttpPlugin(ISocketPlugin, metaclass=ABCMeta):
+    pass
+
+
+@deprecated("please use `ITextAreaPlugin` instead")
+class IHttpTextAreaPlugin(ITextAreaPlugin):
+    pass
+
+
+@deprecated("please use `IQAPlugin` instead")
+class IHttpQAPlugin(IQAPlugin):
+    pass
+
+
+@deprecated("please use `IFieldsPlugin` instead")
+class IHttpFieldsPlugin(IFieldsPlugin):
+    pass
 
 
 __all__ = [
-    "IHttpPlugin",
     "ISocketPlugin",
     "IInternalSocketPlugin",
+    "ITextAreaPlugin",
+    "IQAPlugin",
+    "IFieldsPlugin",
+    # deprecated
+    "IHttpPlugin",
     "IHttpTextAreaPlugin",
     "IHttpQAPlugin",
     "IHttpFieldsPlugin",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.0a7/cfdraw/plugins/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from typing import Dict
 from typing import Type
 from typing import Callable
 from typing import NamedTuple
 
+from cfdraw.utils.data_structures import Types
 from cfdraw.schema.plugins import IPlugin
 from cfdraw.schema.plugins import IPluginSettings
 
+
 TPlugin = Type[IPlugin]
 
 
+class Plugins(Types[IPlugin]):
+    pass
+
+
 class PluginInfo(NamedTuple):
     name: str
     settings: IPluginSettings
     plugin_type: Type[IPlugin]
 
 
 class PluginFactory:
@@ -22,31 +28,27 @@
     > `recorded` stores all plugins that are recorded, and can be accessed via `available`
     >> You can record a plugin by using the `record` decorator
     >> After which you can decide which plugins to use with the `register` method!
     > Notice that we don't need to guarantee that the plugin's name is identical to the plugin's identifier
     >> `plugins` use 'identifier' as the key, and `recorded` use 'name' as the key
     """
 
-    plugins: Dict[str, IPlugin] = {}
-    recorded: Dict[str, IPlugin] = {}
-    internal_plugins: Dict[str, IPlugin] = {}
+    plugins = Plugins()
+    recorded = Plugins()
+    internal_plugins = Plugins()
 
     @classmethod
-    def _register(
-        cls,
-        d: Dict[str, IPlugin],
-        identifier: str,
-    ) -> Callable[[TPlugin], TPlugin]:
+    def _register(cls, d: Plugins, identifier: str) -> Callable[[TPlugin], TPlugin]:
         if identifier in d:
             raise ValueError(f"plugin {identifier} already exists")
 
-        def _fn(plugin: TPlugin) -> TPlugin:
-            plugin.identifier = identifier
-            d[identifier] = plugin()
-            return plugin
+        def _fn(plugin_type: TPlugin) -> TPlugin:
+            plugin_type.identifier = identifier
+            d[identifier] = plugin_type
+            return plugin_type
 
         return _fn
 
     @classmethod
     def register(cls, identifier: str) -> Callable[[TPlugin], TPlugin]:
         return cls._register(cls.plugins, identifier)
 
@@ -55,25 +57,26 @@
         return cls._register(cls.internal_plugins, identifier)
 
     @classmethod
     def record(cls, name: str) -> Callable[[TPlugin], TPlugin]:
         if name in cls.recorded:
             raise ValueError(f"plugin {name} already recorded")
 
-        def _record(plugin: TPlugin) -> TPlugin:
-            cls.recorded[name] = plugin()
-            return plugin
+        def _record(plugin_type: TPlugin) -> TPlugin:
+            cls.recorded[name] = plugin_type
+            return plugin_type
 
         return _record
 
     @classmethod
     def available(cls) -> Dict[str, PluginInfo]:
         return {
-            name: PluginInfo(name, plugin.settings, plugin.__class__)
-            for name, plugin in cls.recorded.items()
+            name: PluginInfo(name, plugin_type().settings, plugin_type)
+            for name, plugin_type in cls.recorded.items()
         }
 
 
 __all__ = [
+    "Plugins",
     "PluginInfo",
     "PluginFactory",
 ]
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/plugins/sync.py` & `carefree-drawboard-0.0.0a7/cfdraw/plugins/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,26 @@
 from cfdraw.schema.plugins import *
 from cfdraw.plugins.base import *
 from cfdraw.plugins.factory import PluginFactory
 
 
 @PluginFactory.register_internal("sync")
 class SyncSocketPlugin(IInternalSocketPlugin):
-    async def process(self, data: IPluginRequest) -> ISocketMessage:
+    async def process(self, data: ISocketRequest) -> ISocketMessage:
         config = get_config()
-        return ISocketMessage(
-            success=True,
-            message="",
-            data=ISocketData(
-                status=SocketStatus.FINISHED,
-                pending=0,
-                data=dict(
-                    pluginSettings=[
-                        plugin.to_plugin_settings()
-                        for plugin in PluginFactory.plugins.values()
-                    ],
-                    globalSettings=dict(
-                        useStrictMode=config.use_react_strict_mode,
-                        sockenEndpoint=str(constants.Endpoint.WEBSOCKET),
-                    ),
+        return ISocketMessage.make_success(
+            data.hash,
+            dict(
+                pluginSettings=[
+                    plugin_type().to_plugin_settings()
+                    for plugin_type in PluginFactory.plugins.values()
+                ],
+                globalSettings=dict(
+                    useStrictMode=config.use_react_strict_mode,
+                    sockenEndpoint=str(constants.Endpoint.WEBSOCKET),
                 ),
             ),
         )
 
 
 __all__ = [
     "SyncSocketPlugin",
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.0a7/cfdraw/schema/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.0a7/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/console.py` & `carefree-drawboard-0.0.0a7/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.0a7/cfdraw/utils/exec.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 
 from cftool.misc import print_info
 
 from cfdraw import constants
 from cfdraw.utils import console
 from cfdraw.utils import prerequisites
 from cfdraw.config import get_config
-from cfdraw.config import Config
-from cfdraw.server import launch_server
 
 
 def setup_frontend() -> None:
     config = get_config()
     prerequisites.install_frontend_packages()
     console.rule("[bold green]Launching App")
     os.environ["CFDRAW_FE_PORT"] = config.frontend_port
     os.environ["CFDRAW_BE_PORT"] = config.api_port
     if config.backend_hosting_url is not None:
         os.environ[constants.API_URL_KEY] = config.api_url
 
 
-def run_frontend() -> None:
+def run_frontend(host: bool) -> None:
     setup_frontend()
+    cmd = [prerequisites.get_yarn(), "dev", "--force"]
+    if host:
+        cmd.append("--host")
     subprocess.Popen(
-        [prerequisites.get_yarn(), "dev", "--force"],
+        cmd,
         cwd=constants.WEB_ROOT,
         env=os.environ,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.STDOUT,
     )
-    frontend_url = f"http://localhost:{get_config().frontend_port}"
-    print_info(f"👌 Your app will be ready at {frontend_url} soon...")
+    print_info(f"👌 Your app will be ready at {get_config().frontend_url} soon...")
 
 
 def run_frontend_prod() -> None:
     setup_frontend()
     config = get_config()
-    if config.use_tornado:
+    if config.use_unified:
         print_info(f"👀 Your app codes are being compiled, please wait for a while...")
         subprocess.run(
             [prerequisites.get_yarn(), "build"],
             cwd=constants.WEB_ROOT,
             env=os.environ,
         )
     else:
@@ -53,34 +53,33 @@
         )
         print_info(
             f"👀 Your app codes are being compiled, "
             "please wait until a bunch of urls appear..."
         )
 
 
-def run_backend(module: str, *, log_level: constants.LogLevel) -> None:
-    console.rule("[bold green]Launching Backend")
+def run_backend(
+    module: str,
+    *,
+    log_level: constants.LogLevel,
+    verbose: bool = True,
+) -> None:
+    if verbose:
+        console.rule("[bold green]Launching Backend")
     config = get_config()
     # I'm not familiar with production stuffs of `uvicorn`, so currently
     # only the `reload` flag is different.
     uvicorn.run(
         f"{module}:{config.entry}.{constants.API_VAR}",
         host=constants.DEV_BACKEND_HOST,
         port=int(config.backend_port),
         log_level=log_level,
         reload=not config.prod,
     )
 
 
-def run_tornado(module: str, *, log_level: constants.LogLevel) -> None:
-    def before_launch(config: Config) -> None:
-        cmd = [
-            "uvicorn",
-            f"{module}:{config.entry}.{constants.API_VAR}",
-            f"--host={constants.DEV_BACKEND_HOST}",
-            f"--port={config.backend_port}",
-            f"--log-level={log_level}",
-        ]
-        subprocess.Popen(cmd)
-
-    console.rule("[bold green]Launching Tornado Backend")
-    launch_server(before_launch)
+def run_backend_prod(module: str, *, log_level: constants.LogLevel) -> None:
+    console.rule("[bold green]Launching Production Backend")
+    config = get_config()
+    if config.use_unified:
+        print_info(f"👌 Your app will be ready at {config.api_url} soon...")
+    run_backend(module, log_level=log_level, verbose=False)
```

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.0a7/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.0a7/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/server.py` & `carefree-drawboard-0.0.0a7/cfdraw/utils/server.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a4/cfdraw/utils/template.py` & `carefree-drawboard-0.0.0a7/cfdraw/utils/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,44 +8,43 @@
 
 IMAGE_APP_TEMPLATE = f"""
 from PIL import Image
 from PIL import ImageFilter
 from cfdraw import *
 
 # This will perform a Gaussian blur on the image
-class Plugin(IHttpFieldsPlugin):
+class Plugin(IFieldsPlugin):
     @property
     def settings(self) -> IPluginSettings:
         return IPluginSettings(
             w=300,
             h=180,
             nodeConstraint=NodeConstraints.IMAGE,
             pivot=PivotType.RT,
             follow=True,
-            pluginInfo=IHttpFieldsPluginInfo(
+            pluginInfo=IFieldsPluginInfo(
                 definitions=dict(
                     size=INumberField(
                         default=3,
                         min=1,
                         max=10,
                         step=1,
                         isInt=True,
                         label="Size",
                     )
                 ),
             ),
         )
 
-    async def process(self, data: IPluginRequest) -> Image.Image:
+    async def process(self, data: ISocketRequest) -> Image.Image:
         image = await self.load_image(data.nodeData.src)
         return image.filter(ImageFilter.GaussianBlur(data.extraData["size"]))
 
 
 register_plugin("blur")(Plugin)
-register_all_available_plugins()
 {constants.DEFAULT_ENTRY} = App()
 """
 
 CONFIG_TEMPLATE = f"""
 from cfdraw.config import Config
 
 {constants.DEFAULT_CONFIG_ENTRY} = Config(
```

### Comparing `carefree-drawboard-0.0.0a4/setup.py` & `carefree-drawboard-0.0.0a7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.0-alpha.4"
+VERSION = "0.0.0-alpha.7"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
@@ -12,26 +12,26 @@
     version=VERSION,
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     entry_points={"console_scripts": ["cfdraw = cfdraw.cli:cli"]},
     install_requires=[
         "rich",
         "typer",
-        "fastapi",
+        "fastapi>=0.95.1",
         "gunicorn",
         "pydantic",
         "uvicorn",
         "websockets",
         "watchdog",
         "python-multipart",
         "carefree-toolkit>=0.3.4",
         "pillow",
         "aiohttp",
         "charset-normalizer==2.1.0",
-        "tornado",
+        "aiofiles",
     ],
     author="carefree0910",
     author_email="syameimaru.saki@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="python carefree-learn drawboard",
```


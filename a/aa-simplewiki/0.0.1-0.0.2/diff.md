# Comparing `tmp/aa-simplewiki-0.0.1.tar.gz` & `tmp/aa-simplewiki-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-simplewiki-0.0.1.tar", last modified: Mon Apr 24 14:25:20 2023, max compression
+gzip compressed data, was "aa-simplewiki-0.0.2.tar", last modified: Mon Apr 24 15:48:46 2023, max compression
```

## Comparing `aa-simplewiki-0.0.1.tar` & `aa-simplewiki-0.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/LICENSE
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/MANIFEST.in
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5412 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4379 2023-04-23 21:25:01.000000 aa-simplewiki-0.0.1/README.md
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.357612 aa-simplewiki-0.0.1/aa_simplewiki.egg-info/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5412 2023-04-24 14:25:20.000000 aa-simplewiki-0.0.1/aa_simplewiki.egg-info/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-04-24 14:25:20.000000 aa-simplewiki-0.0.1/aa_simplewiki.egg-info/SOURCES.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-24 14:25:20.000000 aa-simplewiki-0.0.1/aa_simplewiki.egg-info/dependency_links.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-24 14:24:55.000000 aa-simplewiki-0.0.1/aa_simplewiki.egg-info/not-zip-safe
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       13 2023-04-24 14:25:20.000000 aa-simplewiki-0.0.1/aa_simplewiki.egg-info/requires.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-04-24 14:25:20.000000 aa-simplewiki-0.0.1/aa_simplewiki.egg-info/top_level.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/pyproject.toml
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/setup.cfg
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1182 2023-04-24 14:22:44.000000 aa-simplewiki-0.0.1/setup.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.357612 aa-simplewiki-0.0.1/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       48 2023-04-24 14:21:11.000000 aa-simplewiki-0.0.1/simplewiki/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-04-23 21:25:21.000000 aa-simplewiki-0.0.1/simplewiki/admin.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11864 2023-04-22 07:13:33.000000 aa-simplewiki-0.0.1/simplewiki/admin_helper_menus.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-04-22 07:13:40.000000 aa-simplewiki-0.0.1/simplewiki/admin_helper_sections.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/app_settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/apps.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/auth_hooks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/simplewiki/migrations/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0001_initial.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0002_pageitem_page_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0003_menuitem_icon.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0010_rename_path_menuitem_name.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0011_rename_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0012_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0013_alter_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0018_rename_group_menuitem_groups.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0019_alter_general_options.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/0020_menuitem_parent.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/migrations/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-04-21 10:07:09.000000 aa-simplewiki-0.0.1/simplewiki/models.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.357612 aa-simplewiki-0.0.1/simplewiki/static/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/simplewiki/static/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/static/simplewiki/.gitkeep
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/static/simplewiki/custom.css
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/tasks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.357612 aa-simplewiki-0.0.1/simplewiki/templates/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-04-23 09:54:06.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/base.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-23 21:22:31.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/dynamic_page.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6552 2023-04-23 09:56:49.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/editor_menus.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-04-23 18:31:44.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/editor_sections.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/partials/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2311 2023-04-21 16:05:35.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2345 2023-04-21 16:06:22.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/error.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/index.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-04-22 13:52:24.000000 aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/search.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/simplewiki/templatetags/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2121 2023-04-23 21:22:45.000000 aa-simplewiki-0.0.1/simplewiki/templatetags/custom_filters.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/templatetags/markdown_filters.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/simplewiki/tests/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/tests/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/simplewiki/tests/test_example.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-04-21 10:07:44.000000 aa-simplewiki-0.0.1/simplewiki/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12689 2023-04-22 13:58:33.000000 aa-simplewiki-0.0.1/simplewiki/views.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 14:25:20.361613 aa-simplewiki-0.0.1/testauth/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/testauth/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/testauth/celery.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/testauth/settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/testauth/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.1/testauth/wsgi.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/LICENSE
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/MANIFEST.in
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5500 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4467 2023-04-24 15:47:03.000000 aa-simplewiki-0.0.2/README.md
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.102739 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5500 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-24 14:24:55.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/not-zip-safe
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       24 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/requires.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/top_level.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/pyproject.toml
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/setup.cfg
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1200 2023-04-24 14:46:01.000000 aa-simplewiki-0.0.2/setup.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.102739 aa-simplewiki-0.0.2/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       48 2023-04-24 15:48:37.000000 aa-simplewiki-0.0.2/simplewiki/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-04-23 21:25:21.000000 aa-simplewiki-0.0.2/simplewiki/admin.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11877 2023-04-24 14:48:20.000000 aa-simplewiki-0.0.2/simplewiki/admin_helper_menus.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-04-22 07:13:40.000000 aa-simplewiki-0.0.2/simplewiki/admin_helper_sections.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/app_settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/apps.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/auth_hooks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/migrations/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0001_initial.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0002_pageitem_page_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0003_menuitem_icon.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0010_rename_path_menuitem_name.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0011_rename_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0012_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0013_alter_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0018_rename_group_menuitem_groups.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0019_alter_general_options.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0020_menuitem_parent.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-04-21 10:07:09.000000 aa-simplewiki-0.0.2/simplewiki/models.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.102739 aa-simplewiki-0.0.2/simplewiki/static/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/static/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/static/simplewiki/.gitkeep
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/static/simplewiki/custom.css
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/tasks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.102739 aa-simplewiki-0.0.2/simplewiki/templates/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-04-23 09:54:06.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/base.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-23 21:22:31.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/dynamic_page.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6552 2023-04-23 09:56:49.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/editor_menus.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-04-23 18:31:44.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/editor_sections.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2311 2023-04-21 16:05:35.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2345 2023-04-21 16:06:22.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/error.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/index.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-04-22 13:52:24.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/search.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/templatetags/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2121 2023-04-23 21:22:45.000000 aa-simplewiki-0.0.2/simplewiki/templatetags/custom_filters.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/templatetags/markdown_filters.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/tests/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/tests/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/tests/test_example.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-04-21 10:07:44.000000 aa-simplewiki-0.0.2/simplewiki/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12689 2023-04-22 13:58:33.000000 aa-simplewiki-0.0.2/simplewiki/views.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/testauth/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/celery.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/wsgi.py
```

### Comparing `aa-simplewiki-0.0.1/LICENSE` & `aa-simplewiki-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/PKG-INFO` & `aa-simplewiki-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
@@ -51,21 +51,28 @@
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
-* Add repo to PyPi
 * Quality-of-life updates
 * Improve code documentation
 * Clean-up code
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
+* Add translations for 
+  * German
+  * Spanish
+  * Chinese
+  * Russian
+  * Korean 
+  * French
+  * Italian
 
 ### Active devs:
 * [Meowosaurus](https://github.com/meowosaurus)
 
 ## Screenshots
 ![Showcase](https://i.imgur.com/vST5An1.png)
 
@@ -80,24 +87,24 @@
 ![Section Edit](https://i.imgur.com/3LrysW7.png)
 
 ## Installation
 
 ### Alliance Auth Production
 
 #### Non-Docker Version
-1.) Install the pip package via `pip install git+https://github.com/meowosaurus/aa-simplewiki`
+1.) Install the pip package via `pip install aa-simplewiki`
 
 2.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 3.) Make migrations and migrate, then restart your server
 
 #### Docker Version
 1.) Please make sure you followed the custom docker-image tutorial [here](https://gitlab.com/allianceauth/allianceauth/-/tree/master/docker#using-a-custom-docker-image): 
 
-2.) Edit your `conf/requirements` and add the following lines `git+https://github.com/meowosaurus/aa-simplewiki`
+2.) Edit your `conf/requirements` and add the following line `aa-simplewiki` (Check https://pypi.org/project/aa-simplewiki/ for different versions!)
 
 3.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 4.) Start your server `docker compose --env-file=.env up -d`
 
 5.) Run `docker compose exec allianceauth bash`
```

### Comparing `aa-simplewiki-0.0.1/README.md` & `aa-simplewiki-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,28 @@
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
-* Add repo to PyPi
 * Quality-of-life updates
 * Improve code documentation
 * Clean-up code
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
+* Add translations for 
+  * German
+  * Spanish
+  * Chinese
+  * Russian
+  * Korean 
+  * French
+  * Italian
 
 ### Active devs:
 * [Meowosaurus](https://github.com/meowosaurus)
 
 ## Screenshots
 ![Showcase](https://i.imgur.com/vST5An1.png)
 
@@ -54,24 +61,24 @@
 ![Section Edit](https://i.imgur.com/3LrysW7.png)
 
 ## Installation
 
 ### Alliance Auth Production
 
 #### Non-Docker Version
-1.) Install the pip package via `pip install git+https://github.com/meowosaurus/aa-simplewiki`
+1.) Install the pip package via `pip install aa-simplewiki`
 
 2.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 3.) Make migrations and migrate, then restart your server
 
 #### Docker Version
 1.) Please make sure you followed the custom docker-image tutorial [here](https://gitlab.com/allianceauth/allianceauth/-/tree/master/docker#using-a-custom-docker-image): 
 
-2.) Edit your `conf/requirements` and add the following lines `git+https://github.com/meowosaurus/aa-simplewiki`
+2.) Edit your `conf/requirements` and add the following line `aa-simplewiki` (Check https://pypi.org/project/aa-simplewiki/ for different versions!)
 
 3.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 4.) Start your server `docker compose --env-file=.env up -d`
 
 5.) Run `docker compose exec allianceauth bash`
```

### Comparing `aa-simplewiki-0.0.1/aa_simplewiki.egg-info/PKG-INFO` & `aa-simplewiki-0.0.2/aa_simplewiki.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
@@ -51,21 +51,28 @@
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
-* Add repo to PyPi
 * Quality-of-life updates
 * Improve code documentation
 * Clean-up code
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
+* Add translations for 
+  * German
+  * Spanish
+  * Chinese
+  * Russian
+  * Korean 
+  * French
+  * Italian
 
 ### Active devs:
 * [Meowosaurus](https://github.com/meowosaurus)
 
 ## Screenshots
 ![Showcase](https://i.imgur.com/vST5An1.png)
 
@@ -80,24 +87,24 @@
 ![Section Edit](https://i.imgur.com/3LrysW7.png)
 
 ## Installation
 
 ### Alliance Auth Production
 
 #### Non-Docker Version
-1.) Install the pip package via `pip install git+https://github.com/meowosaurus/aa-simplewiki`
+1.) Install the pip package via `pip install aa-simplewiki`
 
 2.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 3.) Make migrations and migrate, then restart your server
 
 #### Docker Version
 1.) Please make sure you followed the custom docker-image tutorial [here](https://gitlab.com/allianceauth/allianceauth/-/tree/master/docker#using-a-custom-docker-image): 
 
-2.) Edit your `conf/requirements` and add the following lines `git+https://github.com/meowosaurus/aa-simplewiki`
+2.) Edit your `conf/requirements` and add the following line `aa-simplewiki` (Check https://pypi.org/project/aa-simplewiki/ for different versions!)
 
 3.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 4.) Start your server `docker compose --env-file=.env up -d`
 
 5.) Run `docker compose exec allianceauth bash`
```

### Comparing `aa-simplewiki-0.0.1/aa_simplewiki.egg-info/SOURCES.txt` & `aa-simplewiki-0.0.2/aa_simplewiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/setup.cfg` & `aa-simplewiki-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/setup.py` & `aa-simplewiki-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 install_requires = [
+    'commonmark',
     'allianceauth',
 ]
 
 setup(
     name='aa-simplewiki',
     version=__version__,
     packages=find_packages(),
```

### Comparing `aa-simplewiki-0.0.1/simplewiki/admin_helper_menus.py` & `aa-simplewiki-0.0.2/simplewiki/admin_helper_menus.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
                 return render(request, 'simplewiki/error.html', context)
             except Exception as e:
                 return render(request, 'simplewiki/error.html', gen_error_context(context, '#1003', e))
 
         # Take all inputs from the group multiple select and put them in a string, seperated by a comma
         group_string = ""
         try:
+            
             groups = request.POST.getlist('group_select')
 
             for group_item in groups:
                 group_string += group_item
                 group_string += ","
             group_string = group_string[:-1]
         except Exception as e:
```

### Comparing `aa-simplewiki-0.0.1/simplewiki/admin_helper_sections.py` & `aa-simplewiki-0.0.2/simplewiki/admin_helper_sections.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/auth_hooks.py` & `aa-simplewiki-0.0.2/simplewiki/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0001_initial.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0012_menuitem_group.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0012_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0013_alter_menuitem_group.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0013_alter_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/migrations/0020_menuitem_parent.py` & `aa-simplewiki-0.0.2/simplewiki/migrations/0020_menuitem_parent.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/models.py` & `aa-simplewiki-0.0.2/simplewiki/models.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/base.html` & `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/base.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/dynamic_page.html` & `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/dynamic_page.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/editor_menus.html` & `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/editor_menus.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/editor_sections.html` & `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/editor_sections.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/partials/_create_menu.html` & `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/_create_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html` & `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/error.html` & `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/error.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templates/simplewiki/search.html` & `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/search.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/templatetags/custom_filters.py` & `aa-simplewiki-0.0.2/simplewiki/templatetags/custom_filters.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/simplewiki/views.py` & `aa-simplewiki-0.0.2/simplewiki/views.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/testauth/celery.py` & `aa-simplewiki-0.0.2/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.1/testauth/settings.py` & `aa-simplewiki-0.0.2/testauth/settings.py`

 * *Files identical despite different names*


# Comparing `tmp/govuk_frontend_django-0.1.2.tar.gz` & `tmp/govuk_frontend_django-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk_frontend_django-0.1.2.tar", max compression
+gzip compressed data, was "govuk_frontend_django-0.1.3.tar", max compression
```

## Comparing `govuk_frontend_django-0.1.2.tar` & `govuk_frontend_django-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.1.2/LICENSE
--rw-r--r--   0        0        0     1017 2023-04-20 16:48:35.945315 govuk_frontend_django-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.1.2/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.1.2/govuk_frontend_django/components/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-20 12:42:14.586043 govuk_frontend_django-0.1.2/govuk_frontend_django/components/accordion.py
--rw-r--r--   0        0        0      939 2023-04-20 12:42:14.581422 govuk_frontend_django-0.1.2/govuk_frontend_django/components/back_link.py
--rw-r--r--   0        0        0     3767 2023-04-18 16:00:56.573577 govuk_frontend_django-0.1.2/govuk_frontend_django/components/base.py
--rw-r--r--   0        0        0     1170 2023-04-20 12:42:14.592265 govuk_frontend_django-0.1.2/govuk_frontend_django/components/breadcrumbs.py
--rw-r--r--   0        0        0     1221 2023-04-20 12:42:14.589664 govuk_frontend_django-0.1.2/govuk_frontend_django/components/button.py
--rw-r--r--   0        0        0     1838 2023-04-20 12:42:14.598186 govuk_frontend_django-0.1.2/govuk_frontend_django/components/character_count.py
--rw-r--r--   0        0        0     1892 2023-04-20 12:42:14.600823 govuk_frontend_django-0.1.2/govuk_frontend_django/components/checkboxes.py
--rw-r--r--   0        0        0     1723 2023-04-20 12:42:14.599909 govuk_frontend_django-0.1.2/govuk_frontend_django/components/cookie_banner.py
--rw-r--r--   0        0        0     1598 2023-04-20 12:42:14.602359 govuk_frontend_django-0.1.2/govuk_frontend_django/components/date_input.py
--rw-r--r--   0        0        0     1053 2023-04-20 12:42:14.597544 govuk_frontend_django-0.1.2/govuk_frontend_django/components/details.py
--rw-r--r--   0        0        0     1023 2023-04-20 12:42:14.607348 govuk_frontend_django-0.1.2/govuk_frontend_django/components/error_message.py
--rw-r--r--   0        0        0     1349 2023-04-20 12:42:14.613252 govuk_frontend_django-0.1.2/govuk_frontend_django/components/error_summary.py
--rw-r--r--   0        0        0     1024 2023-04-20 12:42:14.605229 govuk_frontend_django-0.1.2/govuk_frontend_django/components/fieldset.py
--rw-r--r--   0        0        0     1251 2023-04-20 12:42:14.606408 govuk_frontend_django-0.1.2/govuk_frontend_django/components/file_upload.py
--rw-r--r--   0        0        0     2007 2023-04-20 12:42:14.627934 govuk_frontend_django-0.1.2/govuk_frontend_django/components/footer.py
--rw-r--r--   0        0        0     1552 2023-04-20 12:42:14.613758 govuk_frontend_django-0.1.2/govuk_frontend_django/components/header.py
--rw-r--r--   0        0        0      927 2023-04-20 12:42:14.610338 govuk_frontend_django-0.1.2/govuk_frontend_django/components/hint.py
--rw-r--r--   0        0        0     1890 2023-04-20 12:42:14.623920 govuk_frontend_django-0.1.2/govuk_frontend_django/components/input.py
--rw-r--r--   0        0        0      960 2023-04-20 12:42:14.615085 govuk_frontend_django-0.1.2/govuk_frontend_django/components/inset_text.py
--rw-r--r--   0        0        0     1024 2023-04-20 12:42:14.621898 govuk_frontend_django-0.1.2/govuk_frontend_django/components/label.py
--rw-r--r--   0        0        0     1241 2023-04-20 12:42:14.628819 govuk_frontend_django-0.1.2/govuk_frontend_django/components/notification_banner.py
--rw-r--r--   0        0        0     1729 2023-04-20 12:42:14.623896 govuk_frontend_django-0.1.2/govuk_frontend_django/components/pagination.py
--rw-r--r--   0        0        0     1015 2023-04-20 12:42:14.619587 govuk_frontend_django-0.1.2/govuk_frontend_django/components/panel.py
--rw-r--r--   0        0        0      980 2023-04-20 12:42:14.620287 govuk_frontend_django-0.1.2/govuk_frontend_django/components/phase_banner.py
--rw-r--r--   0        0        0     1753 2023-04-20 12:42:14.629631 govuk_frontend_django-0.1.2/govuk_frontend_django/components/radios.py
--rw-r--r--   0        0        0     1504 2023-04-20 12:42:14.633487 govuk_frontend_django-0.1.2/govuk_frontend_django/components/select.py
--rw-r--r--   0        0        0      956 2023-04-20 12:42:14.623517 govuk_frontend_django-0.1.2/govuk_frontend_django/components/skip_link.py
--rw-r--r--   0        0        0     1850 2023-04-20 12:42:14.630760 govuk_frontend_django-0.1.2/govuk_frontend_django/components/summary_list.py
--rw-r--r--   0        0        0     1653 2023-04-20 12:42:14.634408 govuk_frontend_django-0.1.2/govuk_frontend_django/components/table.py
--rw-r--r--   0        0        0     1171 2023-04-20 12:42:14.629681 govuk_frontend_django-0.1.2/govuk_frontend_django/components/tabs.py
--rw-r--r--   0        0        0      892 2023-04-20 12:42:14.627472 govuk_frontend_django-0.1.2/govuk_frontend_django/components/tag.py
--rw-r--r--   0        0        0     1344 2023-04-20 12:42:14.630308 govuk_frontend_django-0.1.2/govuk_frontend_django/components/textarea.py
--rw-r--r--   0        0        0      986 2023-04-20 12:42:14.633202 govuk_frontend_django-0.1.2/govuk_frontend_django/components/warning_text.py
--rw-r--r--   0        0        0     2584 2023-04-18 16:38:49.732120 govuk_frontend_django-0.1.2/govuk_frontend_django/templates/govuk_frontend_django/base.html
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/__init__.py
--rw-r--r--   0        0        0     6411 2023-04-18 16:20:36.488163 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0     1500 2023-04-18 16:43:36.564559 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
--rw-r--r--   0        0        0     1202 2023-04-18 16:39:43.479073 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
--rw-r--r--   0        0        0     2904 2023-04-18 16:39:52.639160 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
--rw-r--r--   0        0        0     2177 2023-04-18 16:39:58.841418 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
--rw-r--r--   0        0        0     1522 2023-04-18 16:40:02.398875 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
--rw-r--r--   0        0        0     5044 2023-04-18 16:40:08.273697 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
--rw-r--r--   0        0        0     1373 2023-04-18 16:40:12.508567 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
--rw-r--r--   0        0        0     2129 2023-04-18 16:40:15.259567 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
--rw-r--r--   0        0        0     1340 2023-04-18 16:40:19.370940 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
--rw-r--r--   0        0        0     6872 2023-04-18 16:40:25.682436 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
--rw-r--r--   0        0        0     1357 2023-04-18 16:40:28.276062 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
--rw-r--r--   0        0        0     1231 2023-04-18 16:40:33.574374 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
--rw-r--r--   0        0        0     1219 2023-04-21 08:44:08.300797 govuk_frontend_django-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 govuk_frontend_django-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1017 2023-04-20 16:48:35.945315 govuk_frontend_django-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.1.3/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.1.3/govuk_frontend_django/components/__init__.py
+-rw-r--r--   0        0        0     1252 2023-04-21 17:53:53.647717 govuk_frontend_django-0.1.3/govuk_frontend_django/components/accordion.py
+-rw-r--r--   0        0        0      939 2023-04-21 17:53:53.640544 govuk_frontend_django-0.1.3/govuk_frontend_django/components/back_link.py
+-rw-r--r--   0        0        0     3767 2023-04-18 16:00:56.573577 govuk_frontend_django-0.1.3/govuk_frontend_django/components/base.py
+-rw-r--r--   0        0        0     1170 2023-04-21 17:53:53.647358 govuk_frontend_django-0.1.3/govuk_frontend_django/components/breadcrumbs.py
+-rw-r--r--   0        0        0     1192 2023-04-21 17:53:53.652242 govuk_frontend_django-0.1.3/govuk_frontend_django/components/button.py
+-rw-r--r--   0        0        0     1743 2023-04-21 17:53:53.658844 govuk_frontend_django-0.1.3/govuk_frontend_django/components/character_count.py
+-rw-r--r--   0        0        0     1892 2023-04-21 17:53:53.661111 govuk_frontend_django-0.1.3/govuk_frontend_django/components/checkboxes.py
+-rw-r--r--   0        0        0     1723 2023-04-21 17:53:53.661217 govuk_frontend_django-0.1.3/govuk_frontend_django/components/cookie_banner.py
+-rw-r--r--   0        0        0     1598 2023-04-21 17:53:53.655825 govuk_frontend_django-0.1.3/govuk_frontend_django/components/date_input.py
+-rw-r--r--   0        0        0     1053 2023-04-21 17:53:53.652778 govuk_frontend_django-0.1.3/govuk_frontend_django/components/details.py
+-rw-r--r--   0        0        0     1023 2023-04-21 17:53:53.655383 govuk_frontend_django-0.1.3/govuk_frontend_django/components/error_message.py
+-rw-r--r--   0        0        0     1349 2023-04-21 17:53:53.658748 govuk_frontend_django-0.1.3/govuk_frontend_django/components/error_summary.py
+-rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.657118 govuk_frontend_django-0.1.3/govuk_frontend_django/components/fieldset.py
+-rw-r--r--   0        0        0     1215 2023-04-21 17:53:53.668678 govuk_frontend_django-0.1.3/govuk_frontend_django/components/file_upload.py
+-rw-r--r--   0        0        0     2007 2023-04-21 17:53:53.671128 govuk_frontend_django-0.1.3/govuk_frontend_django/components/footer.py
+-rw-r--r--   0        0        0     1552 2023-04-21 17:53:53.664873 govuk_frontend_django-0.1.3/govuk_frontend_django/components/header.py
+-rw-r--r--   0        0        0      927 2023-04-21 17:53:53.661696 govuk_frontend_django-0.1.3/govuk_frontend_django/components/hint.py
+-rw-r--r--   0        0        0     1854 2023-04-21 17:53:53.669769 govuk_frontend_django-0.1.3/govuk_frontend_django/components/input.py
+-rw-r--r--   0        0        0      960 2023-04-21 17:53:53.665398 govuk_frontend_django-0.1.3/govuk_frontend_django/components/inset_text.py
+-rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.666367 govuk_frontend_django-0.1.3/govuk_frontend_django/components/label.py
+-rw-r--r--   0        0        0     1241 2023-04-21 17:53:53.667052 govuk_frontend_django-0.1.3/govuk_frontend_django/components/notification_banner.py
+-rw-r--r--   0        0        0     1729 2023-04-21 17:53:53.670872 govuk_frontend_django-0.1.3/govuk_frontend_django/components/pagination.py
+-rw-r--r--   0        0        0     1015 2023-04-21 17:53:53.675594 govuk_frontend_django-0.1.3/govuk_frontend_django/components/panel.py
+-rw-r--r--   0        0        0      980 2023-04-21 17:53:53.668688 govuk_frontend_django-0.1.3/govuk_frontend_django/components/phase_banner.py
+-rw-r--r--   0        0        0     1753 2023-04-21 17:53:53.677427 govuk_frontend_django-0.1.3/govuk_frontend_django/components/radios.py
+-rw-r--r--   0        0        0     1468 2023-04-21 17:53:53.678377 govuk_frontend_django-0.1.3/govuk_frontend_django/components/select.py
+-rw-r--r--   0        0        0      956 2023-04-21 17:53:53.671708 govuk_frontend_django-0.1.3/govuk_frontend_django/components/skip_link.py
+-rw-r--r--   0        0        0     1850 2023-04-21 17:53:53.679515 govuk_frontend_django-0.1.3/govuk_frontend_django/components/summary_list.py
+-rw-r--r--   0        0        0     1653 2023-04-21 17:53:53.681216 govuk_frontend_django-0.1.3/govuk_frontend_django/components/table.py
+-rw-r--r--   0        0        0     1171 2023-04-21 17:53:53.675164 govuk_frontend_django-0.1.3/govuk_frontend_django/components/tabs.py
+-rw-r--r--   0        0        0      892 2023-04-21 17:53:53.675735 govuk_frontend_django-0.1.3/govuk_frontend_django/components/tag.py
+-rw-r--r--   0        0        0     1308 2023-04-21 17:53:53.678375 govuk_frontend_django-0.1.3/govuk_frontend_django/components/textarea.py
+-rw-r--r--   0        0        0      969 2023-04-21 17:53:53.676929 govuk_frontend_django-0.1.3/govuk_frontend_django/components/warning_text.py
+-rw-r--r--   0        0        0     2583 2023-04-24 16:19:58.566629 govuk_frontend_django-0.1.3/govuk_frontend_django/templates/govuk_frontend_django/base.html
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/__init__.py
+-rw-r--r--   0        0        0     6410 2023-04-24 16:19:56.027315 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0     1500 2023-04-18 16:43:36.564559 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
+-rw-r--r--   0        0        0     1202 2023-04-18 16:39:43.479073 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
+-rw-r--r--   0        0        0     2904 2023-04-18 16:39:52.639160 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
+-rw-r--r--   0        0        0     2177 2023-04-18 16:39:58.841418 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
+-rw-r--r--   0        0        0     1522 2023-04-18 16:40:02.398875 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
+-rw-r--r--   0        0        0     5044 2023-04-18 16:40:08.273697 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
+-rw-r--r--   0        0        0     1373 2023-04-18 16:40:12.508567 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
+-rw-r--r--   0        0        0     2129 2023-04-18 16:40:15.259567 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
+-rw-r--r--   0        0        0     1340 2023-04-18 16:40:19.370940 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
+-rw-r--r--   0        0        0     6872 2023-04-18 16:40:25.682436 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
+-rw-r--r--   0        0        0     1357 2023-04-18 16:40:28.276062 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
+-rw-r--r--   0        0        0     1231 2023-04-18 16:40:33.574374 govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
+-rw-r--r--   0        0        0     1218 2023-04-24 16:23:17.087317 govuk_frontend_django-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 govuk_frontend_django-0.1.3/PKG-INFO
```

### Comparing `govuk_frontend_django-0.1.2/LICENSE` & `govuk_frontend_django-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/README.md` & `govuk_frontend_django-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/accordion.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/accordion.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     """GOV.UK Accordion
 
     See: https://design-system.service.gov.uk/components/accordion/
     """
 
     id: str
     headingLevel: Optional[int] = None
-    rememberExpanded: Optional[bool] = None
     hideAllSectionsText: Optional[str] = None
     hideSectionText: Optional[str] = None
     hideSectionAriaLabelText: Optional[str] = None
     showAllSectionsText: Optional[str] = None
     showSectionText: Optional[str] = None
     showSectionAriaLabelText: Optional[str] = None
     items: List[govuk_frontend_base.AccordionItem]
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/back_link.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/back_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/base.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/base.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/breadcrumbs.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/button.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,13 @@
     name: Optional[str] = None
     type: Optional[str] = None
     value: Optional[str] = None
     disabled: Optional[bool] = None
     href: Optional[str] = None
     preventDoubleClick: Optional[bool] = None
     isStartButton: Optional[bool] = None
-    id: Optional[str] = None
 
     _jinja2_template = "govuk_frontend_jinja/components/button/macro.html"
     _macro_name = "govukButton"
 
 
 COMPONENT = GovUKButton
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/character_count.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/character_count.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,17 +35,15 @@
     errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
     formGroup: Optional[govuk_frontend_base.FormGroup] = None
     spellcheck: Optional[bool] = None
     countMessage: Optional[CharacterCountCountmessage] = None
     textareaDescriptionText: Optional[str] = None
     charactersUnderLimitText: Optional[Any] = None
     charactersAtLimitText: Optional[str] = None
-    charactersOverLimitText: Optional[Any] = None
     wordsUnderLimitText: Optional[Any] = None
     wordsAtLimitText: Optional[str] = None
-    wordsOverLimitText: Optional[Any] = None
 
     _jinja2_template = "govuk_frontend_jinja/components/character-count/macro.html"
     _macro_name = "govukCharacterCount"
 
 
 COMPONENT = GovUKCharacterCount
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/checkboxes.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/cookie_banner.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/date_input.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/date_input.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/details.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/details.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/error_message.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/error_message.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/error_summary.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/fieldset.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/fieldset.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/file_upload.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/tabs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from dataclasses import dataclass
-from typing import Optional
+from typing import List, Optional
 
 from govuk_frontend_django.components import base as govuk_frontend_base
 from govuk_frontend_django.components import (
     error_message as govuk_frontend_error_message,
 )
 from govuk_frontend_django.components import fieldset as govuk_frontend_fieldset
 from govuk_frontend_django.components import hint as govuk_frontend_hint
 from govuk_frontend_django.components import label as govuk_frontend_label
 from govuk_frontend_django.components import tag as govuk_frontend_tag
 
 
 @dataclass(kw_only=True)
-class GovUKFileUpload(govuk_frontend_base.GovUKComponent):
-    """GOV.UK File Upload
+class TabsItems:
+    id: str
+    label: govuk_frontend_label.GovUKLabel
+    attributes: Optional[govuk_frontend_base.Attributes] = None
+    panel: govuk_frontend_base.TextAndHtml
 
-    See: https://design-system.service.gov.uk/components/file-upload/
+
+@dataclass(kw_only=True)
+class GovUKTabs(govuk_frontend_base.GovUKComponent):
+    """GOV.UK Tabs
+
+    See: https://design-system.service.gov.uk/components/tabs/
     """
 
-    name: str
-    id: str
-    value: Optional[str] = None
-    disabled: Optional[bool] = None
-    describedBy: Optional[str] = None
-    label: govuk_frontend_label.GovUKLabel
-    hint: Optional[govuk_frontend_hint.GovUKHint] = None
-    errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
-    formGroup: Optional[govuk_frontend_base.FormGroup] = None
+    id: Optional[str] = None
+    idPrefix: Optional[str] = None
+    title: Optional[str] = None
+    items: List[TabsItems]
 
-    _jinja2_template = "govuk_frontend_jinja/components/file-upload/macro.html"
-    _macro_name = "govukFileUpload"
+    _jinja2_template = "govuk_frontend_jinja/components/tabs/macro.html"
+    _macro_name = "govukTabs"
 
 
-COMPONENT = GovUKFileUpload
+COMPONENT = GovUKTabs
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/footer.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/header.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/hint.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/hint.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/input.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     """
 
     id: str
     name: str
     type: Optional[str] = None
     inputmode: Optional[str] = None
     value: Optional[str] = None
-    disabled: Optional[bool] = None
     describedBy: Optional[str] = None
     label: govuk_frontend_label.GovUKLabel
     hint: Optional[govuk_frontend_hint.GovUKHint] = None
     errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
     prefix: Optional[InputPrefix] = None
     suffix: Optional[InputSuffix] = None
     formGroup: Optional[govuk_frontend_base.FormGroup] = None
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/inset_text.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/inset_text.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/label.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/label.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/notification_banner.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/notification_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/pagination.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/panel.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/panel.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/phase_banner.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/radios.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/radios.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/select.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     See: https://design-system.service.gov.uk/components/select/
     """
 
     id: str
     name: str
     items: List[SelectItems]
     value: Optional[str] = None
-    disabled: Optional[bool] = None
     describedBy: Optional[str] = None
     label: Optional[govuk_frontend_label.GovUKLabel] = None
     hint: Optional[govuk_frontend_hint.GovUKHint] = None
     errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
     formGroup: Optional[govuk_frontend_base.FormGroup] = None
 
     _jinja2_template = "govuk_frontend_jinja/components/select/macro.html"
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/skip_link.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/skip_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/summary_list.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/table.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/tabs.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/warning_text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import Optional
 
 from govuk_frontend_django.components import base as govuk_frontend_base
 from govuk_frontend_django.components import (
     error_message as govuk_frontend_error_message,
 )
 from govuk_frontend_django.components import fieldset as govuk_frontend_fieldset
 from govuk_frontend_django.components import hint as govuk_frontend_hint
 from govuk_frontend_django.components import label as govuk_frontend_label
 from govuk_frontend_django.components import tag as govuk_frontend_tag
 
 
 @dataclass(kw_only=True)
-class TabsItems:
-    id: str
-    label: govuk_frontend_label.GovUKLabel
-    attributes: Optional[govuk_frontend_base.Attributes] = None
-    panel: govuk_frontend_base.TextAndHtml
+class GovUKWarningText(govuk_frontend_base.GovUKComponent):
+    """GOV.UK Warning Text
 
-
-@dataclass(kw_only=True)
-class GovUKTabs(govuk_frontend_base.GovUKComponent):
-    """GOV.UK Tabs
-
-    See: https://design-system.service.gov.uk/components/tabs/
+    See: https://design-system.service.gov.uk/components/warning-text/
     """
 
-    id: Optional[str] = None
-    idPrefix: Optional[str] = None
-    title: Optional[str] = None
-    items: List[TabsItems]
+    text: Optional[str] = None
+    html: Optional[str] = None
+    iconFallbackText: str
 
-    _jinja2_template = "govuk_frontend_jinja/components/tabs/macro.html"
-    _macro_name = "govukTabs"
+    _jinja2_template = "govuk_frontend_jinja/components/warning-text/macro.html"
+    _macro_name = "govukWarningText"
 
 
-COMPONENT = GovUKTabs
+COMPONENT = GovUKWarningText
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/tag.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/tag.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/components/textarea.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/components/textarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     """
 
     id: str
     name: str
     spellcheck: Optional[bool] = None
     rows: Optional[str] = None
     value: Optional[str] = None
-    disabled: Optional[bool] = None
     describedBy: Optional[str] = None
     label: govuk_frontend_label.GovUKLabel
     hint: Optional[govuk_frontend_hint.GovUKHint] = None
     errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
     formGroup: Optional[govuk_frontend_base.FormGroup] = None
     autocomplete: Optional[str] = None
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templates/govuk_frontend_django/base.html` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templates/govuk_frontend_django/base.html`

 * *Files 5% similar despite different names*

```diff
@@ -27,30 +27,30 @@
         {% block body_start %}
         {% endblock body_start %}
 
         {% gds_component "skip-link" text="Skip to main content" href="#main-content" %}
 
         {% block header %}
             {% gds_header homepageUrl="/" serviceName="Service name" serviceUrl="/" containerClasses="govuk-width-container" %}
-            {% end_gds_header %}
+            {% endgds_header %}
         {% endblock header %}
 
         <div class="govuk-width-container ">
             <main class="govuk-main-wrapper " id="main-content" role="main">
                 {% block content %}
                     <h1 class="govuk-heading-xl">Default page template</h1>
                 {% endblock content %}
             </main>
         </div>
 
         {% block footer %}
             {% gds_footer %}
-            {% end_gds_footer %}
+            {% endgds_footer %}
         {% endblock footer %}
 
         {% block body_end %}
             <script src='{% static "govuk-frontend/all.js" %}''></script>
             <script>window.GOVUKFrontend.initAll()</script>
         {% endblock body_end %}
     </body>
 
-</html>
+</html>
```

#### html2text {}

```diff
@@ -8,16 +8,16 @@
 
 
  {% block head %}
  {% endblock head %}
  {% block body_start %} {% endblock body_start %} {% gds_component "skip-link"
 text="Skip to main content" href="#main-content" %} {% block header %} {%
 gds_header homepageUrl="/" serviceName="Service name" serviceUrl="/
-" containerClasses="govuk-width-container" %} {% end_gds_header %} {% endblock
+" containerClasses="govuk-width-container" %} {% endgds_header %} {% endblock
 header %}
  {% block content %}
 ****** Default page template ******
 {% endblock content %}
-{% block footer %} {% gds_footer %} {% end_gds_footer %} {% endblock footer %}
+{% block footer %} {% gds_footer %} {% endgds_footer %} {% endblock footer %}
 {% block body_end %}
 >
  {% endblock body_end %}
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         if has_end_tag:
             if not any(
                 [
                     end_if_not_contain in extra_context
                     for end_if_not_contain in end_if_not_contains
                 ]
             ):
-                nodelist = parser.parse((f"end_{name}",))
+                nodelist = parser.parse((f"end{name}",))
                 parser.delete_first_token()
 
         return node_cls(
             extra_context=extra_context,
             nodelist=nodelist,
         )
```

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/header.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/table.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py` & `govuk_frontend_django-0.1.3/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.2/pyproject.toml` & `govuk_frontend_django-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "govuk-frontend-django"
-version = "0.1.2"
+version = "0.1.3"
 description = "Django functionality to help when building a GOV.UK website."
 authors = [
     "DBT Live Service Team <live.services@digital.trade.gov.uk>",
     "Cam Lamb <cameron.lamb@digital.trade.gov.uk>",
     "Sam Dudley <samuel.dudley@digital.trade.gov.uk>",
 ]
 license = "MIT"
@@ -18,15 +18,15 @@
 documentation = "https://uktrade.github.io/govuk-frontend-django/"
 packages = [{include = "govuk_frontend_django"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Django = "^4.1.7"
 jinja2 = "^3.1.2"
-govuk-frontend-jinja = "^2.5.0"
+govuk-frontend-jinja = "2.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pyyaml = "^6.0"
 isort = "^5.12.0"
 autoflake = "^2.0.2"
```

### Comparing `govuk_frontend_django-0.1.2/PKG-INFO` & `govuk_frontend_django-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-django
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django functionality to help when building a GOV.UK website.
 Home-page: https://uktrade.github.io/govuk-frontend-django/
 License: MIT
 Author: DBT Live Service Team
 Author-email: live.services@digital.trade.gov.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=4.1.7,<5.0.0)
-Requires-Dist: govuk-frontend-jinja (>=2.5.0,<3.0.0)
+Requires-Dist: govuk-frontend-jinja (==2.5.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Project-URL: Documentation, https://uktrade.github.io/govuk-frontend-django/
 Project-URL: Repository, https://github.com/uktrade/govuk-frontend-django/
 Description-Content-Type: text/markdown
 
 # GOV.UK Frontend Django
```


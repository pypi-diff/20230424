# Comparing `tmp/badi_users-0.9.5.tar.gz` & `tmp/badi_users-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badi_users-0.9.5.tar", last modified: Tue Apr 18 06:30:18 2023, max compression
+gzip compressed data, was "badi_users-0.9.6.tar", last modified: Mon Apr 24 06:57:36 2023, max compression
```

## Comparing `badi_users-0.9.5.tar` & `badi_users-0.9.6.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.357362 badi_users-0.9.5/
--rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-0.9.5/LICENSE
--rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-0.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0      419 2023-04-18 06:30:18.356367 badi_users-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-0.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.430353 badi_users-0.9.5/badi_ticket/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/__init__.py
--rw-rw-rw-   0        0        0      143 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/admin.py
--rw-rw-rw-   0        0        0     9803 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/api.py
--rw-rw-rw-   0        0        0      129 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.362538 badi_users-0.9.5/badi_ticket/locale/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.362538 badi_users-0.9.5/badi_ticket/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.436305 badi_users-0.9.5/badi_ticket/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2781 2023-04-16 12:25:05.000000 badi_users-0.9.5/badi_ticket/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.437303 badi_users-0.9.5/badi_ticket/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.5/badi_ticket/migrations/__init__.py
--rw-rw-rw-   0        0        0     3657 2023-04-16 09:10:44.000000 badi_users-0.9.5/badi_ticket/models.py
--rw-rw-rw-   0        0        0      313 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/routers.py
--rw-rw-rw-   0        0        0     2082 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.363769 badi_users-0.9.5/badi_ticket/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.363769 badi_users-0.9.5/badi_ticket/static/ticket/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.446279 badi_users-0.9.5/badi_ticket/static/ticket/js/
--rw-rw-rw-   0        0        0     2448 2023-04-16 09:16:22.000000 badi_users-0.9.5/badi_ticket/static/ticket/js/chat.js
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.447276 badi_users-0.9.5/badi_ticket/templates/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.510636 badi_users-0.9.5/badi_ticket/templates/ticket/
--rw-rw-rw-   0        0        0     6358 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/templates/ticket/admin_tickets.html
--rw-rw-rw-   0        0        0     5265 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/templates/ticket/message_list.html
--rw-rw-rw-   0        0        0     9642 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/templates/ticket/my_tickets.html
--rw-rw-rw-   0        0        0     7097 2023-04-16 08:20:08.000000 badi_users-0.9.5/badi_ticket/templates/ticket/ticket_create.html
--rw-rw-rw-   0        0        0     1639 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/templates/ticket/ticket_update.html
--rw-rw-rw-   0        0        0       63 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/tests.py
--rw-rw-rw-   0        0        0      583 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/urls.py
--rw-rw-rw-   0        0        0     2057 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_ticket/views.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.542583 badi_users-0.9.5/badi_user/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.563462 badi_users-0.9.5/badi_user/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/api/__init__.py
--rw-rw-rw-   0        0        0    29106 2023-04-16 11:46:57.000000 badi_users-0.9.5/badi_user/api/api.py
--rw-rw-rw-   0        0        0      485 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/api/routers.py
--rw-rw-rw-   0        0        0     6013 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/api/serializers.py
--rw-rw-rw-   0        0        0      183 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/apps.py
--rw-rw-rw-   0        0        0     3428 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.365767 badi_users-0.9.5/badi_user/locale/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.365767 badi_users-0.9.5/badi_user/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.568448 badi_users-0.9.5/badi_user/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     4486 2023-04-16 12:25:06.000000 badi_users-0.9.5/badi_user/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.569413 badi_users-0.9.5/badi_user/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.5/badi_user/migrations/__init__.py
--rw-rw-rw-   0        0        0     6551 2023-04-17 07:59:44.000000 badi_users-0.9.5/badi_user/models.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.575398 badi_users-0.9.5/badi_user/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/__init__.py
--rw-rw-rw-   0        0        0       27 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/badi-user-test.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.603218 badi_users-0.9.5/badi_user/templates/group/
--rw-rw-rw-   0        0        0     8558 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/group/group_create.html
--rw-rw-rw-   0        0        0     5472 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/group/group_update.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.615545 badi_users-0.9.5/badi_user/templates/log/
--rw-rw-rw-   0        0        0     3987 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/log/log_list.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.628512 badi_users-0.9.5/badi_user/templates/login-theme/
--rw-rw-rw-   0        0        0     7336 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/login-theme/login-1.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.682500 badi_users-0.9.5/badi_user/templates/member/
--rw-rw-rw-   0        0        0     6863 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/member/member_create.html
--rw-rw-rw-   0        0        0    22635 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/member/member_list.html
--rw-rw-rw-   0        0        0     4783 2023-03-28 07:29:01.000000 badi_users-0.9.5/badi_user/templates/member/member_self_update.html
--rw-rw-rw-   0        0        0     6525 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/member/member_update.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.728458 badi_users-0.9.5/badi_user/templates/user/
--rw-rw-rw-   0        0        0     5056 2023-04-16 12:18:39.000000 badi_users-0.9.5/badi_user/templates/user/change_password.html
--rw-rw-rw-   0        0        0     5973 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/user/user_create.html
--rw-rw-rw-   0        0        0     4019 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/user/user_list.html
--rw-rw-rw-   0        0        0     5005 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templates/user/user_update.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.737436 badi_users-0.9.5/badi_user/templatetags/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templatetags/__init__.py
--rw-rw-rw-   0        0        0     5950 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/templatetags/appfilter.py
--rw-rw-rw-   0        0        0      500 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.783825 badi_users-0.9.5/badi_user/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/ui/__init__.py
--rw-rw-rw-   0        0        0     1484 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/ui/forms.py
--rw-rw-rw-   0        0        0      320 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/ui/log_views.py
--rw-rw-rw-   0        0        0     1706 2023-03-28 08:00:41.000000 badi_users-0.9.5/badi_user/ui/member_views.py
--rw-rw-rw-   0        0        0      672 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/ui/notification_views.py
--rw-rw-rw-   0        0        0      644 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/ui/roles_views.py
--rw-rw-rw-   0        0        0     1624 2023-04-16 08:12:22.000000 badi_users-0.9.5/badi_user/ui/urls.py
--rw-rw-rw-   0        0        0     2633 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_user/ui/views.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.801911 badi_users-0.9.5/badi_users.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-18 06:30:16.000000 badi_users-0.9.5/badi_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10750 2023-04-18 06:30:16.000000 badi_users-0.9.5/badi_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:30:16.000000 badi_users-0.9.5/badi_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-18 06:30:16.000000 badi_users-0.9.5/badi_users.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.888622 badi_users-0.9.5/badi_utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/__init__.py
--rw-rw-rw-   0        0        0     6835 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/date_calc.py
--rw-rw-rw-   0        0        0    28225 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/dynamic.py
--rw-rw-rw-   0        0        0    22478 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/dynamic_api.py
--rw-rw-rw-   0        0        0     3412 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/dynamic_models.py
--rw-rw-rw-   0        0        0     2990 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/email.py
--rw-rw-rw-   0        0        0      252 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/errors.py
--rw-rw-rw-   0        0        0     1509 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/logging.py
--rw-rw-rw-   0        0        0      947 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/responses.py
--rw-rw-rw-   0        0        0      904 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/rss.py
--rw-rw-rw-   0        0        0     1529 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/select2.py
--rw-rw-rw-   0        0        0     2956 2023-04-16 12:07:37.000000 badi_users-0.9.5/badi_utils/sms.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.369481 badi_users-0.9.5/badi_utils/static/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.370481 badi_users-0.9.5/badi_utils/static/badi_utils/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.894607 badi_users-0.9.5/badi_utils/static/badi_utils/css/
--rw-rw-rw-   0        0        0    40504 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/custom.css
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:17.283125 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/
--rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
--rw-rw-rw-   0        0        0    59532 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
--rw-rw-rw-   0        0        0    38401 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
--rw-rw-rw-   0        0        0    31304 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
--rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
--rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
--rw-rw-rw-   0        0        0    57268 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
--rw-rw-rw-   0        0        0    36069 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
--rw-rw-rw-   0        0        0    28856 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
--rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
--rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
--rw-rw-rw-   0        0        0    60584 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
--rw-rw-rw-   0        0        0    39557 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
--rw-rw-rw-   0        0        0    32344 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
--rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
--rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
--rw-rw-rw-   0        0        0    58192 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
--rw-rw-rw-   0        0        0    36145 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
--rw-rw-rw-   0        0        0    28912 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
--rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
--rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
--rw-rw-rw-   0        0        0    56352 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
--rw-rw-rw-   0        0        0    36913 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
--rw-rw-rw-   0        0        0    30072 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
--rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
--rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
--rw-rw-rw-   0        0        0    38473 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
--rw-rw-rw-   0        0        0    31320 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
--rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
--rw-rw-rw-   0        0        0    57760 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
--rw-rw-rw-   0        0        0    36629 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
--rw-rw-rw-   0        0        0    29688 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
--rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
--rw-rw-rw-   0        0        0    59968 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
--rw-rw-rw-   0        0        0    39693 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
--rw-rw-rw-   0        0        0    32420 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
--rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
--rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
--rw-rw-rw-   0        0        0    57544 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
--rw-rw-rw-   0        0        0    36141 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
--rw-rw-rw-   0        0        0    28916 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
--rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
--rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
--rw-rw-rw-   0        0        0    55640 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
--rw-rw-rw-   0        0        0    36945 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
--rw-rw-rw-   0        0        0    29840 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
--rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
--rw-rw-rw-   0        0        0    93376 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
--rw-rw-rw-   0        0        0    94304 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
--rw-rw-rw-   0        0        0    94740 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/Ray.ttf
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:17.541927 badi_users-0.9.5/badi_utils/static/badi_utils/js/
--rw-rw-rw-   0        0        0   478686 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/apexchart.js
--rw-rw-rw-   0        0        0    19110 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/api-login.js
--rw-rw-rw-   0        0        0    20445 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/api.js
--rw-rw-rw-   0        0        0    25944 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/base.js
--rw-rw-rw-   0        0        0     2149 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/chat.js
--rw-rw-rw-   0        0        0     3167 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/custom-vue.js
--rw-rw-rw-   0        0        0    18429 2023-04-16 15:34:42.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/datatable.js
--rw-rw-rw-   0        0        0     2470 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/image-field.js
--rw-rw-rw-   0        0        0    30541 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/main.js
--rw-rw-rw-   0        0        0      959 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/notification.js
--rw-rw-rw-   0        0        0     2213 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/pagination-vue.js
--rw-rw-rw-   0        0        0    20317 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/tableexport.js
--rw-rw-rw-   0        0        0      654 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/transaction.js
--rw-rw-rw-   0        0        0   354110 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/vue.js
--rw-rw-rw-   0        0        0   268386 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/static/badi_utils/js/xlsx.mini.min.js
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:17.549316 badi_users-0.9.5/badi_utils/templates/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:17.685159 badi_users-0.9.5/badi_utils/templates/component/
--rw-rw-rw-   0        0        0     1777 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/createModal.html
--rw-rw-rw-   0        0        0     1645 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/createTitle.html
--rw-rw-rw-   0        0        0     1054 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/filter-form.html
--rw-rw-rw-   0        0        0      729 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/form-errors.html
--rw-rw-rw-   0        0        0     1340 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/form-progressbar-js.html
--rw-rw-rw-   0        0        0      491 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/form-progressbar.html
--rw-rw-rw-   0        0        0      342 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/form.html
--rw-rw-rw-   0        0        0     1231 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/image-field.html
--rw-rw-rw-   0        0        0    34439 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/index-menu.html
--rw-rw-rw-   0        0        0     2346 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/input.html
--rw-rw-rw-   0        0        0       69 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/loader.html
--rw-rw-rw-   0        0        0      468 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/menu-item.html
--rw-rw-rw-   0        0        0      362 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/menu-list.html
--rw-rw-rw-   0        0        0      746 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/messages.html
--rw-rw-rw-   0        0        0     1134 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/pagination-vue.html
--rw-rw-rw-   0        0        0      361 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/profile_item.html
--rw-rw-rw-   0        0        0      204 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/space-between.html
--rw-rw-rw-   0        0        0      430 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/svg-button-with-text.html
--rw-rw-rw-   0        0        0      428 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/svg-button.html
--rw-rw-rw-   0        0        0     1411 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/table-item.html
--rw-rw-rw-   0        0        0     2114 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/user-card.html
--rw-rw-rw-   0        0        0      257 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/component/yesno.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.173853 badi_users-0.9.5/badi_utils/templates/svg/
--rw-rw-rw-   0        0        0     1949 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/Incoming-box.html
--rw-rw-rw-   0        0        0     1159 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/add-user.html
--rw-rw-rw-   0        0        0     1092 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/address-book.html
--rw-rw-rw-   0        0        0     1095 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/arrow-left.html
--rw-rw-rw-   0        0        0     1081 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/arrow-right.html
--rw-rw-rw-   0        0        0     2024 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/bitcoin.html
--rw-rw-rw-   0        0        0      697 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/box.html
--rw-rw-rw-   0        0        0     1378 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/calendar-day.html
--rw-rw-rw-   0        0        0     1489 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/calendar-gym.html
--rw-rw-rw-   0        0        0      925 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/calendar.html
--rw-rw-rw-   0        0        0     1223 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/call.html
--rw-rw-rw-   0        0        0     1385 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/category.html
--rw-rw-rw-   0        0        0     1270 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/chat.html
--rw-rw-rw-   0        0        0      938 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/check.html
--rw-rw-rw-   0        0        0      344 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/circle.html
--rw-rw-rw-   0        0        0     1686 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/city.html
--rw-rw-rw-   0        0        0     1430 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/clipboard-list.html
--rw-rw-rw-   0        0        0     2247 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/clock.html
--rw-rw-rw-   0        0        0      645 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/close.html
--rw-rw-rw-   0        0        0     2483 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/collection.html
--rw-rw-rw-   0        0        0     1046 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/comment.html
--rw-rw-rw-   0        0        0     1103 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/dashboard.html
--rw-rw-rw-   0        0        0      893 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/delete.html
--rw-rw-rw-   0        0        0     1505 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/download.html
--rw-rw-rw-   0        0        0      901 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/edit.html
--rw-rw-rw-   0        0        0     1361 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/file-check.html
--rw-rw-rw-   0        0        0      988 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/file.html
--rw-rw-rw-   0        0        0     2111 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/film.html
--rw-rw-rw-   0        0        0      681 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/fire.html
--rw-rw-rw-   0        0        0     1648 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/group-chat.html
--rw-rw-rw-   0        0        0     1213 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/group.html
--rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/half_star.html
--rw-rw-rw-   0        0        0      944 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/home.html
--rw-rw-rw-   0        0        0     1906 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/hourse.html
--rw-rw-rw-   0        0        0      631 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/image.html
--rw-rw-rw-   0        0        0      508 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/info.html
--rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/interview.html
--rw-rw-rw-   0        0        0     1389 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/key.html
--rw-rw-rw-   0        0        0     2472 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/logout.html
--rw-rw-rw-   0        0        0      940 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/mail.html
--rw-rw-rw-   0        0        0      731 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/map.html
--rw-rw-rw-   0        0        0     1601 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/message.html
--rw-rw-rw-   0        0        0     1607 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/messages.html
--rw-rw-rw-   0        0        0      683 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/notification.html
--rw-rw-rw-   0        0        0      708 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/plus.html
--rw-rw-rw-   0        0        0      753 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/puzzle.html
--rw-rw-rw-   0        0        0      882 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/question.html
--rw-rw-rw-   0        0        0     1174 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/refresh.html
--rw-rw-rw-   0        0        0     1416 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/safe.html
--rw-rw-rw-   0        0        0     1091 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/search.html
--rw-rw-rw-   0        0        0     1114 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/shield-protected.html
--rw-rw-rw-   0        0        0     1219 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/shield-user.html
--rw-rw-rw-   0        0        0      451 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/slide.html
--rw-rw-rw-   0        0        0     1587 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/timer.html
--rw-rw-rw-   0        0        0     1043 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/town.html
--rw-rw-rw-   0        0        0      804 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/user.html
--rw-rw-rw-   0        0        0      936 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/wallet.html
--rw-rw-rw-   0        0        0      933 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/svg/warning.html
--rw-rw-rw-   0        0        0       19 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templates/test.html
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.182829 badi_users-0.9.5/badi_utils/templatetags/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0      148 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/templatetags/badi_utils.py
--rw-rw-rw-   0        0        0     7102 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/utils.py
--rw-rw-rw-   0        0        0     1911 2023-04-11 07:22:40.000000 badi_users-0.9.5/badi_utils/validations.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.203773 badi_users-0.9.5/badi_visit/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.5/badi_visit/__init__.py
--rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-0.9.5/badi_visit/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.217736 badi_users-0.9.5/badi_visit/api/
--rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-0.9.5/badi_visit/api/__init__.py
--rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-0.9.5/badi_visit/api/api.py
--rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-0.9.5/badi_visit/api/routers.py
--rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-0.9.5/badi_visit/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.218734 badi_users-0.9.5/badi_visit/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.5/badi_visit/migrations/__init__.py
--rw-rw-rw-   0        0        0     1614 2022-11-10 16:59:20.000000 badi_users-0.9.5/badi_visit/models.py
--rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-0.9.5/badi_visit/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.251645 badi_users-0.9.5/badi_wallet/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/__init__.py
--rw-rw-rw-   0        0        0     8873 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/action.py
--rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.271591 badi_users-0.9.5/badi_wallet/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/api/__init__.py
--rw-rw-rw-   0        0        0      241 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/api/routers.py
--rw-rw-rw-   0        0        0      543 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/api/serializers.py
--rw-rw-rw-   0        0        0     8037 2023-03-29 08:19:18.000000 badi_users-0.9.5/badi_wallet/api/view_sets.py
--rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/apps.py
--rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-0.9.5/badi_wallet/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.373474 badi_users-0.9.5/badi_wallet/locale/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:16.373474 badi_users-0.9.5/badi_wallet/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.277576 badi_users-0.9.5/badi_wallet/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1633 2023-04-16 12:25:06.000000 badi_users-0.9.5/badi_wallet/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.278573 badi_users-0.9.5/badi_wallet/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.5/badi_wallet/migrations/__init__.py
--rw-rw-rw-   0        0        0     3146 2023-03-30 05:05:34.000000 badi_users-0.9.5/badi_wallet/models.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.279571 badi_users-0.9.5/badi_wallet/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.338413 badi_users-0.9.5/badi_wallet/templates/transaction/
--rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-0.9.5/badi_wallet/templates/transaction/all_transaction_list.html
--rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:20.000000 badi_users-0.9.5/badi_wallet/templates/transaction/all_transaction_report.html
--rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/templates/transaction/request-transaction.html
--rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-0.9.5/badi_wallet/templates/transaction/transaction_list.html
--rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/templates/transaction/transaction_result.html
--rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:30:18.354372 badi_users-0.9.5/badi_wallet/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.5/badi_wallet/ui/__init__.py
--rw-rw-rw-   0        0        0      577 2023-03-28 19:11:37.000000 badi_users-0.9.5/badi_wallet/ui/urls.py
--rw-rw-rw-   0        0        0     1449 2023-03-28 19:16:42.000000 badi_users-0.9.5/badi_wallet/ui/views.py
--rw-rw-rw-   0        0        0       42 2023-04-18 06:30:18.357362 badi_users-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-04-18 06:29:53.000000 badi_users-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:36.050414 badi_users-0.9.6/
+-rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-0.9.6/LICENSE
+-rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-0.9.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      419 2023-04-24 06:57:36.050414 badi_users-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-0.9.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.621911 badi_users-0.9.6/badi_ticket/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/admin.py
+-rw-rw-rw-   0        0        0     9803 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/api.py
+-rw-rw-rw-   0        0        0      129 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.527161 badi_users-0.9.6/badi_ticket/locale/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.527161 badi_users-0.9.6/badi_ticket/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.623904 badi_users-0.9.6/badi_ticket/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2781 2023-04-16 12:25:05.000000 badi_users-0.9.6/badi_ticket/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.625897 badi_users-0.9.6/badi_ticket/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.6/badi_ticket/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3657 2023-04-16 09:10:44.000000 badi_users-0.9.6/badi_ticket/models.py
+-rw-rw-rw-   0        0        0      313 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/routers.py
+-rw-rw-rw-   0        0        0     2082 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.529156 badi_users-0.9.6/badi_ticket/static/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.529156 badi_users-0.9.6/badi_ticket/static/ticket/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.635870 badi_users-0.9.6/badi_ticket/static/ticket/js/
+-rw-rw-rw-   0        0        0     2448 2023-04-16 09:16:22.000000 badi_users-0.9.6/badi_ticket/static/ticket/js/chat.js
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.637865 badi_users-0.9.6/badi_ticket/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.702695 badi_users-0.9.6/badi_ticket/templates/ticket/
+-rw-rw-rw-   0        0        0     6358 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/templates/ticket/admin_tickets.html
+-rw-rw-rw-   0        0        0     5265 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/templates/ticket/message_list.html
+-rw-rw-rw-   0        0        0     9642 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/templates/ticket/my_tickets.html
+-rw-rw-rw-   0        0        0     7097 2023-04-16 08:20:08.000000 badi_users-0.9.6/badi_ticket/templates/ticket/ticket_create.html
+-rw-rw-rw-   0        0        0     1639 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/templates/ticket/ticket_update.html
+-rw-rw-rw-   0        0        0       63 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/tests.py
+-rw-rw-rw-   0        0        0      583 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/urls.py
+-rw-rw-rw-   0        0        0     2057 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_ticket/views.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.709674 badi_users-0.9.6/badi_user/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.714660 badi_users-0.9.6/badi_user/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/api/__init__.py
+-rw-rw-rw-   0        0        0    29476 2023-04-24 05:00:36.000000 badi_users-0.9.6/badi_user/api/api.py
+-rw-rw-rw-   0        0        0      485 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/api/routers.py
+-rw-rw-rw-   0        0        0     6013 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/api/serializers.py
+-rw-rw-rw-   0        0        0      183 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/apps.py
+-rw-rw-rw-   0        0        0     3428 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.532148 badi_users-0.9.6/badi_user/locale/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.533145 badi_users-0.9.6/badi_user/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.716655 badi_users-0.9.6/badi_user/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     4486 2023-04-16 12:25:06.000000 badi_users-0.9.6/badi_user/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.717652 badi_users-0.9.6/badi_user/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.6/badi_user/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6975 2023-04-24 04:40:45.000000 badi_users-0.9.6/badi_user/models.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.719648 badi_users-0.9.6/badi_user/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/badi-user-test.html
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.721641 badi_users-0.9.6/badi_user/templates/group/
+-rw-rw-rw-   0        0        0     8558 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/group/group_create.html
+-rw-rw-rw-   0        0        0     5472 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/group/group_update.html
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.723636 badi_users-0.9.6/badi_user/templates/log/
+-rw-rw-rw-   0        0        0     3987 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/log/log_list.html
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.724633 badi_users-0.9.6/badi_user/templates/login-theme/
+-rw-rw-rw-   0        0        0     7336 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/login-theme/login-1.html
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.729620 badi_users-0.9.6/badi_user/templates/member/
+-rw-rw-rw-   0        0        0     6863 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/member/member_create.html
+-rw-rw-rw-   0        0        0    22635 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/member/member_list.html
+-rw-rw-rw-   0        0        0     4783 2023-03-28 07:29:01.000000 badi_users-0.9.6/badi_user/templates/member/member_self_update.html
+-rw-rw-rw-   0        0        0     6525 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/member/member_update.html
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.734607 badi_users-0.9.6/badi_user/templates/user/
+-rw-rw-rw-   0        0        0     5056 2023-04-16 12:18:39.000000 badi_users-0.9.6/badi_user/templates/user/change_password.html
+-rw-rw-rw-   0        0        0     6743 2023-04-24 04:38:27.000000 badi_users-0.9.6/badi_user/templates/user/user_create.html
+-rw-rw-rw-   0        0        0     4019 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/user/user_list.html
+-rw-rw-rw-   0        0        0     5005 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templates/user/user_update.html
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.737600 badi_users-0.9.6/badi_user/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     5950 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/templatetags/appfilter.py
+-rw-rw-rw-   0        0        0      500 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.748569 badi_users-0.9.6/badi_user/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/ui/__init__.py
+-rw-rw-rw-   0        0        0     1484 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/ui/forms.py
+-rw-rw-rw-   0        0        0      320 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/ui/log_views.py
+-rw-rw-rw-   0        0        0     1706 2023-03-28 08:00:41.000000 badi_users-0.9.6/badi_user/ui/member_views.py
+-rw-rw-rw-   0        0        0      672 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/ui/notification_views.py
+-rw-rw-rw-   0        0        0      644 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/ui/roles_views.py
+-rw-rw-rw-   0        0        0     1624 2023-04-16 08:12:22.000000 badi_users-0.9.6/badi_user/ui/urls.py
+-rw-rw-rw-   0        0        0     2633 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_user/ui/views.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.771509 badi_users-0.9.6/badi_users.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-24 06:57:33.000000 badi_users-0.9.6/badi_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10750 2023-04-24 06:57:33.000000 badi_users-0.9.6/badi_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:57:33.000000 badi_users-0.9.6/badi_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-24 06:57:33.000000 badi_users-0.9.6/badi_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.874234 badi_users-0.9.6/badi_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/__init__.py
+-rw-rw-rw-   0        0        0     6835 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/date_calc.py
+-rw-rw-rw-   0        0        0    28225 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/dynamic.py
+-rw-rw-rw-   0        0        0    22478 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/dynamic_api.py
+-rw-rw-rw-   0        0        0     3412 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/dynamic_models.py
+-rw-rw-rw-   0        0        0     2990 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/email.py
+-rw-rw-rw-   0        0        0      252 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/errors.py
+-rw-rw-rw-   0        0        0     1509 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/logging.py
+-rw-rw-rw-   0        0        0      947 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/responses.py
+-rw-rw-rw-   0        0        0      904 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/rss.py
+-rw-rw-rw-   0        0        0     1529 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/select2.py
+-rw-rw-rw-   0        0        0     2956 2023-04-16 12:07:37.000000 badi_users-0.9.6/badi_utils/sms.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.540128 badi_users-0.9.6/badi_utils/static/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.541124 badi_users-0.9.6/badi_utils/static/badi_utils/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.880216 badi_users-0.9.6/badi_utils/static/badi_utils/css/
+-rw-rw-rw-   0        0        0    40504 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/custom.css
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:34.367915 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/
+-rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
+-rw-rw-rw-   0        0        0    59532 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
+-rw-rw-rw-   0        0        0    38401 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
+-rw-rw-rw-   0        0        0    31304 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
+-rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
+-rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
+-rw-rw-rw-   0        0        0    57268 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
+-rw-rw-rw-   0        0        0    36069 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
+-rw-rw-rw-   0        0        0    28856 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
+-rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
+-rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
+-rw-rw-rw-   0        0        0    60584 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
+-rw-rw-rw-   0        0        0    39557 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
+-rw-rw-rw-   0        0        0    32344 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
+-rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
+-rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
+-rw-rw-rw-   0        0        0    58192 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
+-rw-rw-rw-   0        0        0    36145 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
+-rw-rw-rw-   0        0        0    28912 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
+-rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
+-rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
+-rw-rw-rw-   0        0        0    56352 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36913 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
+-rw-rw-rw-   0        0        0    30072 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
+-rw-rw-rw-   0        0        0    38473 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
+-rw-rw-rw-   0        0        0    31320 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
+-rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
+-rw-rw-rw-   0        0        0    57760 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
+-rw-rw-rw-   0        0        0    36629 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
+-rw-rw-rw-   0        0        0    29688 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
+-rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
+-rw-rw-rw-   0        0        0    59968 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
+-rw-rw-rw-   0        0        0    39693 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
+-rw-rw-rw-   0        0        0    32420 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
+-rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
+-rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
+-rw-rw-rw-   0        0        0    57544 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
+-rw-rw-rw-   0        0        0    36141 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
+-rw-rw-rw-   0        0        0    28916 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
+-rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
+-rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
+-rw-rw-rw-   0        0        0    55640 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36945 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
+-rw-rw-rw-   0        0        0    29840 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    93376 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
+-rw-rw-rw-   0        0        0    94304 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
+-rw-rw-rw-   0        0        0    94740 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/Ray.ttf
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:34.706009 badi_users-0.9.6/badi_utils/static/badi_utils/js/
+-rw-rw-rw-   0        0        0   478686 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/apexchart.js
+-rw-rw-rw-   0        0        0    19110 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/api-login.js
+-rw-rw-rw-   0        0        0    20445 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/api.js
+-rw-rw-rw-   0        0        0    25944 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/base.js
+-rw-rw-rw-   0        0        0     2149 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/chat.js
+-rw-rw-rw-   0        0        0     3167 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/custom-vue.js
+-rw-rw-rw-   0        0        0    18429 2023-04-16 15:34:42.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/datatable.js
+-rw-rw-rw-   0        0        0     2470 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/image-field.js
+-rw-rw-rw-   0        0        0    30541 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/main.js
+-rw-rw-rw-   0        0        0      959 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/notification.js
+-rw-rw-rw-   0        0        0     2213 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/pagination-vue.js
+-rw-rw-rw-   0        0        0    20317 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/tableexport.js
+-rw-rw-rw-   0        0        0      654 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/transaction.js
+-rw-rw-rw-   0        0        0   354110 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/vue.js
+-rw-rw-rw-   0        0        0   268386 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/static/badi_utils/js/xlsx.mini.min.js
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:34.714985 badi_users-0.9.6/badi_utils/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:34.869603 badi_users-0.9.6/badi_utils/templates/component/
+-rw-rw-rw-   0        0        0     1777 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/createModal.html
+-rw-rw-rw-   0        0        0     1645 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/createTitle.html
+-rw-rw-rw-   0        0        0     1054 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/filter-form.html
+-rw-rw-rw-   0        0        0      729 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/form-errors.html
+-rw-rw-rw-   0        0        0     1340 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/form-progressbar-js.html
+-rw-rw-rw-   0        0        0      491 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/form-progressbar.html
+-rw-rw-rw-   0        0        0      342 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/form.html
+-rw-rw-rw-   0        0        0     1231 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/image-field.html
+-rw-rw-rw-   0        0        0    34439 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/index-menu.html
+-rw-rw-rw-   0        0        0     2346 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/input.html
+-rw-rw-rw-   0        0        0       69 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/loader.html
+-rw-rw-rw-   0        0        0      468 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/menu-item.html
+-rw-rw-rw-   0        0        0      362 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/menu-list.html
+-rw-rw-rw-   0        0        0      746 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/messages.html
+-rw-rw-rw-   0        0        0     1134 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/pagination-vue.html
+-rw-rw-rw-   0        0        0      361 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/profile_item.html
+-rw-rw-rw-   0        0        0      204 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/space-between.html
+-rw-rw-rw-   0        0        0      430 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/svg-button-with-text.html
+-rw-rw-rw-   0        0        0      428 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/svg-button.html
+-rw-rw-rw-   0        0        0     1411 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/table-item.html
+-rw-rw-rw-   0        0        0     2114 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/user-card.html
+-rw-rw-rw-   0        0        0      257 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/component/yesno.html
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.602611 badi_users-0.9.6/badi_utils/templates/svg/
+-rw-rw-rw-   0        0        0     1949 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/Incoming-box.html
+-rw-rw-rw-   0        0        0     1159 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/add-user.html
+-rw-rw-rw-   0        0        0     1092 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/address-book.html
+-rw-rw-rw-   0        0        0     1095 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/arrow-left.html
+-rw-rw-rw-   0        0        0     1081 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/arrow-right.html
+-rw-rw-rw-   0        0        0     2024 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/bitcoin.html
+-rw-rw-rw-   0        0        0      697 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/box.html
+-rw-rw-rw-   0        0        0     1378 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/calendar-day.html
+-rw-rw-rw-   0        0        0     1489 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/calendar-gym.html
+-rw-rw-rw-   0        0        0      925 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/calendar.html
+-rw-rw-rw-   0        0        0     1223 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/call.html
+-rw-rw-rw-   0        0        0     1385 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/category.html
+-rw-rw-rw-   0        0        0     1270 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/chat.html
+-rw-rw-rw-   0        0        0      938 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/check.html
+-rw-rw-rw-   0        0        0      344 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/circle.html
+-rw-rw-rw-   0        0        0     1686 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/city.html
+-rw-rw-rw-   0        0        0     1430 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/clipboard-list.html
+-rw-rw-rw-   0        0        0     2247 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/clock.html
+-rw-rw-rw-   0        0        0      645 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/close.html
+-rw-rw-rw-   0        0        0     2483 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/collection.html
+-rw-rw-rw-   0        0        0     1046 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/comment.html
+-rw-rw-rw-   0        0        0     1103 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/dashboard.html
+-rw-rw-rw-   0        0        0      893 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/delete.html
+-rw-rw-rw-   0        0        0     1505 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/download.html
+-rw-rw-rw-   0        0        0      901 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/edit.html
+-rw-rw-rw-   0        0        0     1361 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/file-check.html
+-rw-rw-rw-   0        0        0      988 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/file.html
+-rw-rw-rw-   0        0        0     2111 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/film.html
+-rw-rw-rw-   0        0        0      681 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/fire.html
+-rw-rw-rw-   0        0        0     1648 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/group-chat.html
+-rw-rw-rw-   0        0        0     1213 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/group.html
+-rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/half_star.html
+-rw-rw-rw-   0        0        0      944 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/home.html
+-rw-rw-rw-   0        0        0     1906 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/hourse.html
+-rw-rw-rw-   0        0        0      631 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/image.html
+-rw-rw-rw-   0        0        0      508 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/info.html
+-rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/interview.html
+-rw-rw-rw-   0        0        0     1389 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/key.html
+-rw-rw-rw-   0        0        0     2472 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/logout.html
+-rw-rw-rw-   0        0        0      940 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/mail.html
+-rw-rw-rw-   0        0        0      731 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/map.html
+-rw-rw-rw-   0        0        0     1601 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/message.html
+-rw-rw-rw-   0        0        0     1607 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/messages.html
+-rw-rw-rw-   0        0        0      683 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/notification.html
+-rw-rw-rw-   0        0        0      708 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/plus.html
+-rw-rw-rw-   0        0        0      753 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/puzzle.html
+-rw-rw-rw-   0        0        0      882 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/question.html
+-rw-rw-rw-   0        0        0     1174 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/refresh.html
+-rw-rw-rw-   0        0        0     1416 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/safe.html
+-rw-rw-rw-   0        0        0     1091 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/search.html
+-rw-rw-rw-   0        0        0     1114 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/shield-protected.html
+-rw-rw-rw-   0        0        0     1219 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/shield-user.html
+-rw-rw-rw-   0        0        0      451 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/slide.html
+-rw-rw-rw-   0        0        0     1587 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/timer.html
+-rw-rw-rw-   0        0        0     1043 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/town.html
+-rw-rw-rw-   0        0        0      804 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/user.html
+-rw-rw-rw-   0        0        0      936 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/wallet.html
+-rw-rw-rw-   0        0        0      933 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/svg/warning.html
+-rw-rw-rw-   0        0        0       19 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templates/test.html
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.627544 badi_users-0.9.6/badi_utils/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/templatetags/badi_utils.py
+-rw-rw-rw-   0        0        0     7102 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/utils.py
+-rw-rw-rw-   0        0        0     1911 2023-04-11 07:22:40.000000 badi_users-0.9.6/badi_utils/validations.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.777145 badi_users-0.9.6/badi_visit/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.6/badi_visit/__init__.py
+-rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-0.9.6/badi_visit/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.802078 badi_users-0.9.6/badi_visit/api/
+-rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-0.9.6/badi_visit/api/__init__.py
+-rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-0.9.6/badi_visit/api/api.py
+-rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-0.9.6/badi_visit/api/routers.py
+-rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-0.9.6/badi_visit/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.804073 badi_users-0.9.6/badi_visit/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.6/badi_visit/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1614 2022-11-10 16:59:20.000000 badi_users-0.9.6/badi_visit/models.py
+-rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-0.9.6/badi_visit/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.874883 badi_users-0.9.6/badi_wallet/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/__init__.py
+-rw-rw-rw-   0        0        0     8873 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/action.py
+-rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.911784 badi_users-0.9.6/badi_wallet/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/api/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/api/routers.py
+-rw-rw-rw-   0        0        0      543 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/api/serializers.py
+-rw-rw-rw-   0        0        0     8037 2023-03-29 08:19:18.000000 badi_users-0.9.6/badi_wallet/api/view_sets.py
+-rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/apps.py
+-rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-0.9.6/badi_wallet/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.547108 badi_users-0.9.6/badi_wallet/locale/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:33.548107 badi_users-0.9.6/badi_wallet/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.917769 badi_users-0.9.6/badi_wallet/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1633 2023-04-16 12:25:06.000000 badi_users-0.9.6/badi_wallet/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.919764 badi_users-0.9.6/badi_wallet/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.6/badi_wallet/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3146 2023-03-30 05:05:34.000000 badi_users-0.9.6/badi_wallet/models.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:35.921758 badi_users-0.9.6/badi_wallet/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:36.006531 badi_users-0.9.6/badi_wallet/templates/transaction/
+-rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-0.9.6/badi_wallet/templates/transaction/all_transaction_list.html
+-rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:20.000000 badi_users-0.9.6/badi_wallet/templates/transaction/all_transaction_report.html
+-rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/templates/transaction/request-transaction.html
+-rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-0.9.6/badi_wallet/templates/transaction/transaction_list.html
+-rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/templates/transaction/transaction_result.html
+-rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:57:36.048418 badi_users-0.9.6/badi_wallet/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.6/badi_wallet/ui/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-03-28 19:11:37.000000 badi_users-0.9.6/badi_wallet/ui/urls.py
+-rw-rw-rw-   0        0        0     1449 2023-03-28 19:16:42.000000 badi_users-0.9.6/badi_wallet/ui/views.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:57:36.051411 badi_users-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-04-24 06:50:48.000000 badi_users-0.9.6/setup.py
```

### Comparing `badi_users-0.9.5/LICENSE` & `badi_users-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/MANIFEST.in` & `badi_users-0.9.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/api.py` & `badi_users-0.9.6/badi_ticket/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.6/badi_ticket/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/models.py` & `badi_users-0.9.6/badi_ticket/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/serializers.py` & `badi_users-0.9.6/badi_ticket/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/static/ticket/js/chat.js` & `badi_users-0.9.6/badi_ticket/static/ticket/js/chat.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/templates/ticket/admin_tickets.html` & `badi_users-0.9.6/badi_ticket/templates/ticket/admin_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/templates/ticket/message_list.html` & `badi_users-0.9.6/badi_ticket/templates/ticket/message_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/templates/ticket/my_tickets.html` & `badi_users-0.9.6/badi_ticket/templates/ticket/my_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/templates/ticket/ticket_create.html` & `badi_users-0.9.6/badi_ticket/templates/ticket/ticket_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/templates/ticket/ticket_update.html` & `badi_users-0.9.6/badi_ticket/templates/ticket/ticket_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/urls.py` & `badi_users-0.9.6/badi_ticket/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_ticket/views.py` & `badi_users-0.9.6/badi_ticket/views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/api/api.py` & `badi_users-0.9.6/badi_user/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from rest_framework import status, viewsets
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework.status import HTTP_400_BAD_REQUEST, HTTP_401_UNAUTHORIZED
 from rest_framework_simplejwt.exceptions import InvalidToken, TokenError
 from rest_framework_simplejwt.serializers import TokenObtainPairSerializer, TokenRefreshSerializer
 from rest_framework_simplejwt.tokens import RefreshToken
-from badi_utils.dynamic_api import DynamicModelApi, InCaseSensitiveTokenObtainPairSerializer
+from badi_utils.dynamic_api import DynamicModelApi, InCaseSensitiveTokenObtainPairSerializer, CustomValidation
 from badi_utils.logging import log
 from badi_utils.responses import ResponseOk, ResponseNotOk
 from badi_utils.utils import random_with_N_digits, permissions_json
 from rest_framework_simplejwt.views import TokenRefreshView
 from badi_user.api.serializers import UserSerializer, GroupSerializer, MemberSerializer, LogSerializer, \
     UserProfileSerializer, UserRegisterSerializer
 from badi_user.filter import UserListFilter, MemberListFilter, LogFilter
@@ -47,16 +47,16 @@
     queryset = User.objects.filter(is_admin=True)
     serializer_class = UserSerializer
     custom_perms = {
         'self': True
     }
     switches = {
         'is_active': {
-            'true': ' ',
-            'false': ' ',
+            'true': '/api/v1/user/change_state/0',
+            'false': '/api/v1/user/change_state/0',
         }
     }
 
     def create(self, request, *args, **kwargs):
         return super().create(request, *args, **kwargs)
 
     def filter_queryset(self, qs):
@@ -76,17 +76,20 @@
         instance = self.request.user
         serializer = self.get_serializer(instance)
         return Response(serializer.data)
 
     @action(methods=['put'], detail=False, url_path='change_state/(?P<pk>[^/.]+)')
     def change_state(self, request, pk, *args, **kwargs):
         user = User.objects.get(pk=pk)
+        if user.is_superuser or user == self.request.user:
+            raise CustomValidation('user', _('You are not allowed to disable this user!'))
         user.is_active = not user.is_active
         user.save()
-
+        log(self.request.user, 3, 4, True,
+            text=f'User {self.request.user.__str__()} {"Activated" if user.is_active else "Disabled"}!')
         return JsonResponse({
             'message': 'با موفقیت {0} شد'.format('فعال' if user.is_active else 'غیرفعال')
         })
 
 
 class LoginAuth:
     @staticmethod
```

### Comparing `badi_users-0.9.5/badi_user/api/serializers.py` & `badi_users-0.9.6/badi_user/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/filter.py` & `badi_users-0.9.6/badi_user/filter.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.6/badi_user/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/models.py` & `badi_users-0.9.6/badi_user/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,21 +77,27 @@
     @classmethod
     def get_form_fields(cls, action, *args):
         if action == 'member_create':
             return ['username', 'password', 'first_name', 'picture', 'last_name', 'is_admin', 'mobile_number']
         if action == 'member_update':
             return ['username', 'password', 'first_name', 'picture', 'last_name', 'is_admin', 'mobile_number']
         if action == 'member_self_update':
-            return ['username', 'password', 'first_name', 'picture', 'last_name', 'is_admin', 'mobile_number']
+            return ['username', 'password', 'first_name', 'picture', 'last_name', 'mobile_number']
+        if action == 'user_create':
+            return ['username', 'password', 'first_name', 'picture', 'last_name', 'is_admin', 'mobile_number', 'email']
+        if action == 'user_update':
+            return ['username', 'password', 'first_name', 'picture', 'last_name', 'is_admin', 'mobile_number', 'email']
         return ['first_name', 'last_name', 'mobile_number', 'picture']
 
     @classmethod
     def get_datatable_cols(cls, class_name, *args):
         if class_name == 'MemberListView':
             return ['#', _("Select"), "", _("Username"), _("FirstName"), _("LastName"), _("Amount")]
+        if class_name == 'UserListView':
+            return ['#', '', _("Mobile Number"), _("is admin"), _("active")]
         return [_("FirstName"), _("LastName"), _("Mobile Number"), _("Picture")]
 
     @staticmethod
     def get_api_url(view):
         if view == 'MemberListView':
             return '/api/v1/member/'
```

### Comparing `badi_users-0.9.5/badi_user/templates/group/group_create.html` & `badi_users-0.9.6/badi_user/templates/group/group_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/group/group_update.html` & `badi_users-0.9.6/badi_user/templates/group/group_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/log/log_list.html` & `badi_users-0.9.6/badi_user/templates/log/log_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/login-theme/login-1.html` & `badi_users-0.9.6/badi_user/templates/login-theme/login-1.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/member/member_create.html` & `badi_users-0.9.6/badi_user/templates/member/member_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/member/member_list.html` & `badi_users-0.9.6/badi_user/templates/member/member_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/member/member_self_update.html` & `badi_users-0.9.6/badi_user/templates/member/member_self_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/member/member_update.html` & `badi_users-0.9.6/badi_user/templates/member/member_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/user/change_password.html` & `badi_users-0.9.6/badi_user/templates/user/change_password.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/user/user_create.html` & `badi_users-0.9.6/badi_user/templates/user/user_create.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,173 +1,183 @@
 {% extends 'base.html' %}
 {% load widget_tweaks %}
 {% load i18n %}
 {% load badi_utils %}
 {% block body %}
-<div class="d-flex flex-column-fluid">
-	<!--begin::Container-->
-	<div class="container-fluid">
-		<div class="row">
-			<div class="col-md-12">
-				<!--begin::Card-->
-				<div class="card card-custom">
-					<div class="card-header">
-						<h3 class="card-title">
-							{% trans "Create" %}
-							{{ model_name }}
-						</h3>
-					</div>
-					<!--begin::Form-->
-					<form class="form" id="form" method="POST">
-						<div class="card-body">
-							<div class="row">
-								<div class="col-md-4">
-									<div class="form-group">
-										<label class="col-form-label">{{ form.username.label }}:</label>
-										{{ form.username }}
-									</div>
-								</div>
-								<div class="col-md-4">
-									<div class="form-group">
-										<label class="col-form-label">{{ form.password.label }}:</label>
-										{% render_field form.password type='password' %}
-									</div>
-								</div>
-								<div class="col-md-4">
-									<div class="form-group">
-										<label class="col-form-label">{% trans "Repeat Password" %}:</label>
-										{% render_field form.password type='password' name='repeat_password' id='id_repeat_password' %}
-									</div>
-								</div>
-								<div class="col-lg-3 col-md-6">
-									<div class="form-group">
-										<label class="col-form-label">{{ form.first_name.label }}</label>
-										{{ form.first_name }}
-									</div>
-								</div>
-								<div class="col-lg-3 col-md-6">
-									<div class="form-group">
-										<label class="col-form-label">{{ form.last_name.label }}</label>
-										{{ form.last_name }}
-									</div>
-								</div>
-								<div class="col-lg-3 col-md-6">
-									<div class="form-group">
-										<label class="col-form-label">{{ form.mobile_number.label }}</label>
-										{{ form.mobile_number }}
-									</div>
+	<div class="d-flex flex-column-fluid">
+		<!--begin::Container-->
+		<div class="container-fluid">
+			<div class="row">
+				<div class="col-md-12">
+					<!--begin::Card-->
+					<div class="card card-custom">
+						<div class="card-header">
+							<h3 class="card-title">
+								{% trans "Create" %}
+								{{ model_name }}
+							</h3>
+						</div>
+						<!--begin::Form-->
+						<form class="form" id="form" method="POST">
+							<div class="card-body">
+								<div class="row">
+									<div class="col-md-4">
+										<div class="form-group">
+											<label class="col-form-label">{{ form.username.label }}:</label>
+											{{ form.username }}
+										</div>
+									</div>
+									<div class="col-md-4">
+										<div class="form-group">
+											<label class="col-form-label">{{ form.password.label }}:</label>
+											{% render_field form.password type='password' %}
+										</div>
+									</div>
+									<div class="col-md-4">
+										<div class="form-group">
+											<label class="col-form-label">{% trans "Repeat Password" %}:</label>
+											{% render_field form.password type='password' name='repeat_password' id='id_repeat_password' %}
+										</div>
+									</div>
+									<div class="col-lg-3 col-md-6">
+										<div class="form-group">
+											<label class="col-form-label">{{ form.first_name.label }}</label>
+											{{ form.first_name }}
+										</div>
+									</div>
+									<div class="col-lg-3 col-md-6">
+										<div class="form-group">
+											<label class="col-form-label">{{ form.last_name.label }}</label>
+											{{ form.last_name }}
+										</div>
+									</div>
+									{% if form.mobile_number %}
+										<div class="col-lg-3 col-md-6">
+											<div class="form-group">
+												<label class="col-form-label">{{ form.mobile_number.label }}</label>
+												{{ form.mobile_number }}
+											</div>
+										</div>
+									{% endif %}
+									{% if form.email %}
+										<div class="col-lg-3 col-md-6">
+											<div class="form-group">
+												<label class="col-form-label">{{ form.email.label }}</label>
+												{{ form.email }}
+											</div>
+										</div>
+									{% endif %}
 								</div>
 							</div>
-						</div>
 
-						<div class="card-footer">
-							<a href="{{ back }}" class="btn ml-2 btn-secondary">{% trans "Back" %}</a>
-							<button type="submit" class="btn btn-primary">{% trans "Submit" %}</button>
-						</div>
-					</form>
-					<!--end::Form-->
+							<div class="card-footer">
+								<a href="{{ back }}" class="btn ml-2 btn-secondary">{% trans "Back" %}</a>
+								<button type="submit" class="btn btn-primary">{% trans "Submit" %}</button>
+							</div>
+						</form>
+						<!--end::Form-->
+					</div>
+					<!--end::Card-->
 				</div>
-				<!--end::Card-->
 			</div>
 		</div>
+		<!--end::Container-->
 	</div>
-	<!--end::Container-->
-</div>
 
 
 {% endblock %}
 {% block script %}
-<script>
-    const formV = FormValidation.formValidation(
-        document.getElementById('form'),
-        {
-            fields: {
-                first_name: {
-                    validators: {
-                        stringLength: {
-                            max: 20,
-                            min: 2,
-                            message:'{% trans "must be between 2 and 20 character" %}'
-                        },
-                        notEmpty: {
-                            message: '{% trans "This Field is required" %}'
-                        },
-                    }
-                },
-                last_name: {
-                    validators: {
-                        stringLength: {
-                            max: 20,
-                            min: 2,
-                            message: '{% trans "must be between 2 and 20 character" %}'
-                        },
-                        notEmpty: {
-                            message: '{% trans "This Field is required" %}'
-                        },
-                    }
-                },
-                password: {
-                    validators: {
-                        stringLength: {
-                            min: 6,
-                            max: 20,
-                            message: '{% trans "must be between 6 and 20 character" %}'
-                        },
-                        notEmpty: {
-                            message: '{% trans "This Field is required" %}'
-                        },
-                    }
-                },
-                repeat_password: {
-                    validators: {
-                        notEmpty: {
-                            message: '{% trans "This Field is required" %}'
-                        },
-                        callback: {
-                            message: '{% trans "Repeat Password and New Password are not equal" %}',
-                            callback: function (input) {
-                                return input.value === document.querySelector('#id_password').value
-                            }
+	<script>
+        const formV = FormValidation.formValidation(
+            document.getElementById('form'),
+            {
+                fields: {
+                    first_name: {
+                        validators: {
+                            stringLength: {
+                                max: 20,
+                                min: 2,
+                                message: '{% trans "must be between 2 and 20 character" %}'
+                            },
+                            notEmpty: {
+                                message: '{% trans "This Field is required" %}'
+                            },
+                        }
+                    },
+                    last_name: {
+                        validators: {
+                            stringLength: {
+                                max: 20,
+                                min: 2,
+                                message: '{% trans "must be between 2 and 20 character" %}'
+                            },
+                            notEmpty: {
+                                message: '{% trans "This Field is required" %}'
+                            },
+                        }
+                    },
+                    password: {
+                        validators: {
+                            stringLength: {
+                                min: 6,
+                                max: 20,
+                                message: '{% trans "must be between 6 and 20 character" %}'
+                            },
+                            notEmpty: {
+                                message: '{% trans "This Field is required" %}'
+                            },
+                        }
+                    },
+                    repeat_password: {
+                        validators: {
+                            notEmpty: {
+                                message: '{% trans "This Field is required" %}'
+                            },
+                            callback: {
+                                message: '{% trans "Repeat Password and New Password are not equal" %}',
+                                callback: function (input) {
+                                    return input.value === document.querySelector('#id_password').value
+                                }
 
+                            }
                         }
-                    }
+                    },
+                },
+                plugins: {
+                    trigger: new FormValidation.plugins.Trigger(),
+                    bootstrap: new FormValidation.plugins.Bootstrap()
                 },
-            },
-            plugins: {
-                trigger: new FormValidation.plugins.Trigger(),
-                bootstrap: new FormValidation.plugins.Bootstrap()
-            },
 
-        }
-    );
-    $('#form').on('submit', function (e) {
-        e.preventDefault()
-        const button = document.querySelector('#form button[type="submit"]');
-        formV.validate().then(function (status) {
-            if (status === 'Valid') {
-                ApiAjax({
-                    success_url: 'list',
-                    url: '{{ api_url }}',
-                    form: '#form',
-                    method: 'POST',
-                    button: button,
-                    success_message: '{% trans "" %}',
-                    check: function (data) {
-                        return data
-                    }
-                })
-            } else {
-                Swal.fire({
-                    text: '{% trans "Seems some error exists" %}',
-                    icon: "error",
-                    confirmButtonText: '{% trans "Got it" %}',
-                    customClass: {
-                        confirmButton: "btn font-weight-bold btn-secondary"
-                    }
-                }).then(function () {
-                    KTUtil.scrollTop();
-                });
             }
+        );
+        $('#form').on('submit', function (e) {
+            e.preventDefault()
+            const button = document.querySelector('#form button[type="submit"]');
+            formV.validate().then(function (status) {
+                if (status === 'Valid') {
+                    ApiAjax({
+                        success_url: 'list',
+                        url: '{{ api_url }}',
+                        form: '#form',
+                        method: 'POST',
+                        button: button,
+                        success_message: '{% trans "" %}',
+                        check: function (data) {
+                            return data
+                        }
+                    })
+                } else {
+                    Swal.fire({
+                        text: '{% trans "Seems some error exists" %}',
+                        icon: "error",
+                        confirmButtonText: '{% trans "Got it" %}',
+                        customClass: {
+                            confirmButton: "btn font-weight-bold btn-secondary"
+                        }
+                    }).then(function () {
+                        KTUtil.scrollTop();
+                    });
+                }
+            });
         });
-    });
-</script>
+	</script>
 {% endblock %}
```

### Comparing `badi_users-0.9.5/badi_user/templates/user/user_list.html` & `badi_users-0.9.6/badi_user/templates/user/user_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templates/user/user_update.html` & `badi_users-0.9.6/badi_user/templates/user/user_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/templatetags/appfilter.py` & `badi_users-0.9.6/badi_user/templatetags/appfilter.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/ui/forms.py` & `badi_users-0.9.6/badi_user/ui/forms.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/ui/member_views.py` & `badi_users-0.9.6/badi_user/ui/member_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/ui/notification_views.py` & `badi_users-0.9.6/badi_user/ui/notification_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/ui/roles_views.py` & `badi_users-0.9.6/badi_user/ui/roles_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/ui/urls.py` & `badi_users-0.9.6/badi_user/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_user/ui/views.py` & `badi_users-0.9.6/badi_user/ui/views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_users.egg-info/SOURCES.txt` & `badi_users-0.9.6/badi_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/date_calc.py` & `badi_users-0.9.6/badi_utils/date_calc.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/dynamic.py` & `badi_users-0.9.6/badi_utils/dynamic.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/dynamic_api.py` & `badi_users-0.9.6/badi_utils/dynamic_api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/dynamic_models.py` & `badi_users-0.9.6/badi_utils/dynamic_models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/email.py` & `badi_users-0.9.6/badi_utils/email.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/logging.py` & `badi_users-0.9.6/badi_utils/logging.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/responses.py` & `badi_users-0.9.6/badi_utils/responses.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/rss.py` & `badi_users-0.9.6/badi_utils/rss.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/select2.py` & `badi_users-0.9.6/badi_utils/select2.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/sms.py` & `badi_users-0.9.6/badi_utils/sms.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/custom.css` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/custom.css`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/css/fonts/Ray.ttf` & `badi_users-0.9.6/badi_utils/static/badi_utils/css/fonts/Ray.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/apexchart.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/apexchart.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/api-login.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/api-login.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/api.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/api.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/base.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/base.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/chat.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/chat.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/custom-vue.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/custom-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/datatable.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/datatable.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/image-field.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/image-field.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/main.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/main.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/notification.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/notification.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/pagination-vue.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/pagination-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/tableexport.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/tableexport.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/transaction.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/transaction.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/vue.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/static/badi_utils/js/xlsx.mini.min.js` & `badi_users-0.9.6/badi_utils/static/badi_utils/js/xlsx.mini.min.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/createModal.html` & `badi_users-0.9.6/badi_utils/templates/component/createModal.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/createTitle.html` & `badi_users-0.9.6/badi_utils/templates/component/createTitle.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/filter-form.html` & `badi_users-0.9.6/badi_utils/templates/component/filter-form.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/form-errors.html` & `badi_users-0.9.6/badi_utils/templates/component/form-errors.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/form-progressbar-js.html` & `badi_users-0.9.6/badi_utils/templates/component/form-progressbar-js.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/image-field.html` & `badi_users-0.9.6/badi_utils/templates/component/image-field.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/index-menu.html` & `badi_users-0.9.6/badi_utils/templates/component/index-menu.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/input.html` & `badi_users-0.9.6/badi_utils/templates/component/input.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/messages.html` & `badi_users-0.9.6/badi_utils/templates/component/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/pagination-vue.html` & `badi_users-0.9.6/badi_utils/templates/component/pagination-vue.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/table-item.html` & `badi_users-0.9.6/badi_utils/templates/component/table-item.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/component/user-card.html` & `badi_users-0.9.6/badi_utils/templates/component/user-card.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/Incoming-box.html` & `badi_users-0.9.6/badi_utils/templates/svg/Incoming-box.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/add-user.html` & `badi_users-0.9.6/badi_utils/templates/svg/add-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/address-book.html` & `badi_users-0.9.6/badi_utils/templates/svg/address-book.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/arrow-left.html` & `badi_users-0.9.6/badi_utils/templates/svg/arrow-left.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/arrow-right.html` & `badi_users-0.9.6/badi_utils/templates/svg/arrow-right.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/bitcoin.html` & `badi_users-0.9.6/badi_utils/templates/svg/bitcoin.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/box.html` & `badi_users-0.9.6/badi_utils/templates/svg/box.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/calendar-day.html` & `badi_users-0.9.6/badi_utils/templates/svg/calendar-day.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/calendar-gym.html` & `badi_users-0.9.6/badi_utils/templates/svg/calendar-gym.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/calendar.html` & `badi_users-0.9.6/badi_utils/templates/svg/calendar.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/call.html` & `badi_users-0.9.6/badi_utils/templates/svg/call.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/category.html` & `badi_users-0.9.6/badi_utils/templates/svg/category.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/chat.html` & `badi_users-0.9.6/badi_utils/templates/svg/chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/check.html` & `badi_users-0.9.6/badi_utils/templates/svg/check.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/city.html` & `badi_users-0.9.6/badi_utils/templates/svg/city.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/clipboard-list.html` & `badi_users-0.9.6/badi_utils/templates/svg/clipboard-list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/clock.html` & `badi_users-0.9.6/badi_utils/templates/svg/clock.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/close.html` & `badi_users-0.9.6/badi_utils/templates/svg/close.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/collection.html` & `badi_users-0.9.6/badi_utils/templates/svg/collection.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/comment.html` & `badi_users-0.9.6/badi_utils/templates/svg/comment.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/dashboard.html` & `badi_users-0.9.6/badi_utils/templates/svg/dashboard.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/delete.html` & `badi_users-0.9.6/badi_utils/templates/svg/delete.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/download.html` & `badi_users-0.9.6/badi_utils/templates/svg/download.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/edit.html` & `badi_users-0.9.6/badi_utils/templates/svg/edit.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/file-check.html` & `badi_users-0.9.6/badi_utils/templates/svg/file-check.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/file.html` & `badi_users-0.9.6/badi_utils/templates/svg/file.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/film.html` & `badi_users-0.9.6/badi_utils/templates/svg/film.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/fire.html` & `badi_users-0.9.6/badi_utils/templates/svg/fire.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/group-chat.html` & `badi_users-0.9.6/badi_utils/templates/svg/group-chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/group.html` & `badi_users-0.9.6/badi_utils/templates/svg/group.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/half_star.html` & `badi_users-0.9.6/badi_utils/templates/svg/half_star.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/home.html` & `badi_users-0.9.6/badi_utils/templates/svg/home.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/hourse.html` & `badi_users-0.9.6/badi_utils/templates/svg/hourse.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/image.html` & `badi_users-0.9.6/badi_utils/templates/svg/image.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/interview.html` & `badi_users-0.9.6/badi_utils/templates/svg/interview.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/key.html` & `badi_users-0.9.6/badi_utils/templates/svg/key.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/logout.html` & `badi_users-0.9.6/badi_utils/templates/svg/logout.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/mail.html` & `badi_users-0.9.6/badi_utils/templates/svg/mail.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/map.html` & `badi_users-0.9.6/badi_utils/templates/svg/map.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/message.html` & `badi_users-0.9.6/badi_utils/templates/svg/message.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/messages.html` & `badi_users-0.9.6/badi_utils/templates/svg/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/notification.html` & `badi_users-0.9.6/badi_utils/templates/svg/notification.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/plus.html` & `badi_users-0.9.6/badi_utils/templates/svg/plus.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/puzzle.html` & `badi_users-0.9.6/badi_utils/templates/svg/puzzle.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/question.html` & `badi_users-0.9.6/badi_utils/templates/svg/question.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/refresh.html` & `badi_users-0.9.6/badi_utils/templates/svg/refresh.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/safe.html` & `badi_users-0.9.6/badi_utils/templates/svg/safe.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/search.html` & `badi_users-0.9.6/badi_utils/templates/svg/search.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/shield-protected.html` & `badi_users-0.9.6/badi_utils/templates/svg/shield-protected.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/shield-user.html` & `badi_users-0.9.6/badi_utils/templates/svg/shield-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/timer.html` & `badi_users-0.9.6/badi_utils/templates/svg/timer.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/town.html` & `badi_users-0.9.6/badi_utils/templates/svg/town.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/user.html` & `badi_users-0.9.6/badi_utils/templates/svg/user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/wallet.html` & `badi_users-0.9.6/badi_utils/templates/svg/wallet.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/templates/svg/warning.html` & `badi_users-0.9.6/badi_utils/templates/svg/warning.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/utils.py` & `badi_users-0.9.6/badi_utils/utils.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_utils/validations.py` & `badi_users-0.9.6/badi_utils/validations.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_visit/api/api.py` & `badi_users-0.9.6/badi_visit/api/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_visit/models.py` & `badi_users-0.9.6/badi_visit/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/action.py` & `badi_users-0.9.6/badi_wallet/action.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/api/serializers.py` & `badi_users-0.9.6/badi_wallet/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/api/view_sets.py` & `badi_users-0.9.6/badi_wallet/api/view_sets.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.6/badi_wallet/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/models.py` & `badi_users-0.9.6/badi_wallet/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/templates/transaction/all_transaction_list.html` & `badi_users-0.9.6/badi_wallet/templates/transaction/all_transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/templates/transaction/all_transaction_report.html` & `badi_users-0.9.6/badi_wallet/templates/transaction/all_transaction_report.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/templates/transaction/request-transaction.html` & `badi_users-0.9.6/badi_wallet/templates/transaction/request-transaction.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/templates/transaction/transaction_list.html` & `badi_users-0.9.6/badi_wallet/templates/transaction/transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/templates/transaction/transaction_result.html` & `badi_users-0.9.6/badi_wallet/templates/transaction/transaction_result.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/ui/urls.py` & `badi_users-0.9.6/badi_wallet/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.5/badi_wallet/ui/views.py` & `badi_users-0.9.6/badi_wallet/ui/views.py`

 * *Files identical despite different names*


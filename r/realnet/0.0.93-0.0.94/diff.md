# Comparing `tmp/realnet-0.0.93.tar.gz` & `tmp/realnet-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realnet-0.0.93.tar", last modified: Mon Apr 24 01:51:28 2023, max compression
+gzip compressed data, was "realnet-0.0.94.tar", last modified: Mon Apr 24 02:12:28 2023, max compression
```

## Comparing `realnet-0.0.93.tar` & `realnet-0.0.94.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.869871 realnet-0.0.93/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 01:48:06.000000 realnet-0.0.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 01:51:28.865871 realnet-0.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-24 01:48:06.000000 realnet-0.0.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.849870 realnet-0.0.93/realnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.849870 realnet-0.0.93/realnet/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/cmd/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/cmd/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/cmd/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/cmd/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/cmd/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.849870 realnet-0.0.93/realnet/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/core/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/core/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/core/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.849870 realnet-0.0.93/realnet/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.849870 realnet-0.0.93/realnet/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/aws/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.849870 realnet-0.0.93/realnet/provider/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/generic/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/generic/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/provider/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/provider/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/org.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/orgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/provider/sql/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/postgres/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/provider/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/sql/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/provider/xml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/provider/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/provider/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/realnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/accounts/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/attributes/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/auths/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/auths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/auths/auths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/chatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/chatgpt/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/clients/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/ctrls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/ctrls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/ctrls/ctrls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/endpoints/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.853870 realnet-0.0.93/realnet/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/files/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/forms/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/gltf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/gltf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/gltf/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/gltf/gltf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/groups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/groups/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35333 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/items/items.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/public/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/public/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/roles/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/resource/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/resource/views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/runner/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/runner/http/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.845870 realnet-0.0.93/realnet/runner/http/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.857870 realnet-0.0.93/realnet/runner/http/static/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.861871 realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.845870 realnet-0.0.93/realnet/runner/http/static/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.865871 realnet-0.0.93/realnet/runner/http/static/scripts/ace/
--rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/ace.js
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/ext-beautify.js
--rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/ext-language_tools.js
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-css.js
--rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-html.js
--rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-javascript.js
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-json.js
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-python.js
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/http/static/scripts/ace/theme-monokai.js
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.865871 realnet-0.0.93/realnet/runner/sqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/runner/sqs/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.865871 realnet-0.0.93/realnet/shell/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/shell/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/shell/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/shell/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/shell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.865871 realnet-0.0.93/realnet/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.865871 realnet-0.0.93/realnet/static/initialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/initialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/initialization/access.json
--rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/initialization/apps.json
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/initialization/controls.json
--rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/initialization/core.json
--rw-r--r--   0 runner    (1001) docker     (123)   115082 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/initialization/forms.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/initialization/geometry.json
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/static/initialization/views.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.865871 realnet-0.0.93/realnet/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/control.html
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/register.html
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/register_org.html
--rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-24 01:48:06.000000 realnet-0.0.93/realnet/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:51:28.849870 realnet-0.0.93/realnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 01:51:28.000000 realnet-0.0.93/realnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 01:51:28.000000 realnet-0.0.93/realnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:51:28.000000 realnet-0.0.93/realnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 01:51:28.000000 realnet-0.0.93/realnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 01:51:28.000000 realnet-0.0.93/realnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 01:51:28.000000 realnet-0.0.93/realnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 01:51:28.869871 realnet-0.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 01:48:10.000000 realnet-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.699375 realnet-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 02:09:45.000000 realnet-0.0.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 02:12:28.699375 realnet-0.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-24 02:09:45.000000 realnet-0.0.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/cmd/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/cmd/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/cmd/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/cmd/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/cmd/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/core/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/core/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/core/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/aws/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet/provider/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/generic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/generic/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/generic/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/provider/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/provider/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/orgs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/provider/sql/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/postgres/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/provider/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/sql/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/provider/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/provider/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/provider/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/realnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/accounts/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/attributes/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/auths/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/auths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/auths/auths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/chatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/chatgpt/chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/clients/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/ctrls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/ctrls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/ctrls/ctrls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/endpoints/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/files/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/forms/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/gltf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/gltf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/gltf/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/gltf/gltf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/groups/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35333 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/items/items.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/public/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/public/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.691374 realnet-0.0.94/realnet/resource/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.695374 realnet-0.0.94/realnet/resource/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/roles/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.695374 realnet-0.0.94/realnet/resource/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.695374 realnet-0.0.94/realnet/resource/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/resource/views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.695374 realnet-0.0.94/realnet/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.695374 realnet-0.0.94/realnet/runner/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.695374 realnet-0.0.94/realnet/runner/http/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet/runner/http/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.695374 realnet-0.0.94/realnet/runner/http/static/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.695374 realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet/runner/http/static/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.699375 realnet-0.0.94/realnet/runner/http/static/scripts/ace/
+-rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/ace.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/ext-beautify.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/ext-language_tools.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-css.js
+-rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-html.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-javascript.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-json.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-python.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/http/static/scripts/ace/theme-monokai.js
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.699375 realnet-0.0.94/realnet/runner/sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/runner/sqs/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.699375 realnet-0.0.94/realnet/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/shell/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/shell/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/shell/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/shell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.699375 realnet-0.0.94/realnet/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.699375 realnet-0.0.94/realnet/static/initialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/initialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/initialization/access.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/initialization/apps.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/initialization/controls.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/initialization/core.json
+-rw-r--r--   0 runner    (1001) docker     (123)   115082 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/initialization/forms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/initialization/geometry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/static/initialization/views.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.699375 realnet-0.0.94/realnet/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/control.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/register.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/register_org.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-24 02:09:45.000000 realnet-0.0.94/realnet/templates/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:12:28.687374 realnet-0.0.94/realnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 02:12:28.000000 realnet-0.0.94/realnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 02:12:28.000000 realnet-0.0.94/realnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 02:12:28.000000 realnet-0.0.94/realnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 02:12:28.000000 realnet-0.0.94/realnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 02:12:28.000000 realnet-0.0.94/realnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 02:12:28.000000 realnet-0.0.94/realnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 02:12:28.699375 realnet-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 02:09:47.000000 realnet-0.0.94/setup.py
```

### Comparing `realnet-0.0.93/LICENSE` & `realnet-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/PKG-INFO` & `realnet-0.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realnet
-Version: 0.0.93
+Version: 0.0.94
 Summary: Realnet command line interface
 Home-page: https://github.com/virtual-space/realnet
 Author: Marko Laban
 Author-email: marko.laban@l33tsystems.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `realnet-0.0.93/README.md` & `realnet-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/cmd/server.py` & `realnet-0.0.94/realnet/cmd/server.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/core/config.py` & `realnet-0.0.94/realnet/core/config.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/core/hierarchy.py` & `realnet-0.0.94/realnet/core/hierarchy.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/core/provider.py` & `realnet-0.0.94/realnet/core/provider.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/core/type.py` & `realnet-0.0.94/realnet/core/type.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/aws/data.py` & `realnet-0.0.94/realnet/provider/aws/data.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/generic/endpoint.py` & `realnet-0.0.94/realnet/provider/generic/endpoint.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/generic/resource.py` & `realnet-0.0.94/realnet/provider/generic/resource.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/client.py` & `realnet-0.0.94/realnet/provider/sql/client.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/init.py` & `realnet-0.0.94/realnet/provider/sql/init.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/models.py` & `realnet-0.0.94/realnet/provider/sql/models.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/org.py` & `realnet-0.0.94/realnet/provider/sql/org.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/orgs.py` & `realnet-0.0.94/realnet/provider/sql/orgs.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/postgres/item.py` & `realnet-0.0.94/realnet/provider/sql/postgres/item.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/roles.py` & `realnet-0.0.94/realnet/provider/sql/roles.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/type.py` & `realnet-0.0.94/realnet/provider/sql/type.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/provider/sql/utility.py` & `realnet-0.0.94/realnet/provider/sql/utility.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/accounts/accounts.py` & `realnet-0.0.94/realnet/resource/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/apps/apps.py` & `realnet-0.0.94/realnet/resource/apps/apps.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/auths/auths.py` & `realnet-0.0.94/realnet/resource/auths/auths.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/chatgpt/chatgpt.py` & `realnet-0.0.94/realnet/resource/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/clients/clients.py` & `realnet-0.0.94/realnet/resource/clients/clients.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/ctrls/ctrls.py` & `realnet-0.0.94/realnet/resource/ctrls/ctrls.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/files/files.py` & `realnet-0.0.94/realnet/resource/files/files.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/gltf/export.py` & `realnet-0.0.94/realnet/resource/gltf/export.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/gltf/gltf.py` & `realnet-0.0.94/realnet/resource/gltf/gltf.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/groups/groups.py` & `realnet-0.0.94/realnet/resource/groups/groups.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/items/items.py` & `realnet-0.0.94/realnet/resource/items/items.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/login/login.py` & `realnet-0.0.94/realnet/resource/login/login.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/roles/roles.py` & `realnet-0.0.94/realnet/resource/roles/roles.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/types/types.py` & `realnet-0.0.94/realnet/resource/types/types.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/resource/views/views.py` & `realnet-0.0.94/realnet/resource/views/views.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/app.py` & `realnet-0.0.94/realnet/runner/http/app.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/auth.py` & `realnet-0.0.94/realnet/runner/http/auth.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/router.py` & `realnet-0.0.94/realnet/runner/http/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 try:
     import urlparse
 except ImportError:
     import urllib.parse as urlparse
 
 from authlib.common.urls import url_encode
 
+import logging
+logger = logging.getLogger()
+logger.setLevel(logging.INFO)
+
 router_bp = Blueprint('router_bp',__name__)
 
 def current_user(contextProvider):
     if 'id' in session:
         uid = session['id']
         return contextProvider.get_account_by_id(uid)
     return None
@@ -94,14 +98,17 @@
                     if not password:
                         password = request.args.get('password')
                     if not password and request.is_json:
                         password = request.json.get('password')
                     if password:
                         account = contextProvider.check_password(org.id, username, password)
                         if account:
+                            logger.info('*** request scheme: ' + request.scheme)
+                            logger.info('*** request base url: ' + request.base_url)
+                            logger.info('*** request query string: ' + request.bquery_string)
                             return authorization.create_token_response()
                             # return authorization.create_authorization_response(grant_user=account)
             else:
                 if name == None:
                     oauths = [{'name': n['name'],
                                'url': '/{0}/login/{1}?client_id={2}&response_type={3}'.format(id, n['name'], client_id, response_type)} for n in
                               [q.to_dict() for q in contextProvider.get_org_authenticators(org.id)]]
```

### Comparing `realnet-0.0.93/realnet/runner/http/static/font-awesome/css/font-awesome.css` & `realnet-0.0.94/realnet/runner/http/static/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/font-awesome/css/font-awesome.min.css` & `realnet-0.0.94/realnet/runner/http/static/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf` & `realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot` & `realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg` & `realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf` & `realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff` & `realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2` & `realnet-0.0.94/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/ace.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/ace.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/ext-beautify.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/ext-beautify.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/ext-language_tools.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-css.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-css.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-html.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-html.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-javascript.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-javascript.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-json.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-json.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/mode-python.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/runner/http/static/scripts/ace/theme-monokai.js` & `realnet-0.0.94/realnet/runner/http/static/scripts/ace/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/shell/cmd.py` & `realnet-0.0.94/realnet/shell/cmd.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/shell/proto.py` & `realnet-0.0.94/realnet/shell/proto.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/shell/shell.py` & `realnet-0.0.94/realnet/shell/shell.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/static/initialization/access.json` & `realnet-0.0.94/realnet/static/initialization/access.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/static/initialization/apps.json` & `realnet-0.0.94/realnet/static/initialization/apps.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/static/initialization/controls.json` & `realnet-0.0.94/realnet/static/initialization/controls.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/static/initialization/core.json` & `realnet-0.0.94/realnet/static/initialization/core.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/static/initialization/forms.json` & `realnet-0.0.94/realnet/static/initialization/forms.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/static/initialization/geometry.json` & `realnet-0.0.94/realnet/static/initialization/geometry.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/static/initialization/views.json` & `realnet-0.0.94/realnet/static/initialization/views.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/control.html` & `realnet-0.0.94/realnet/templates/control.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/form.html` & `realnet-0.0.94/realnet/templates/form.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/item.html` & `realnet-0.0.94/realnet/templates/item.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/login.html` & `realnet-0.0.94/realnet/templates/login.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/main.html` & `realnet-0.0.94/realnet/templates/main.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/nav.html` & `realnet-0.0.94/realnet/templates/nav.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/register.html` & `realnet-0.0.94/realnet/templates/register.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/register_org.html` & `realnet-0.0.94/realnet/templates/register_org.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet/templates/view.html` & `realnet-0.0.94/realnet/templates/view.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/realnet.egg-info/PKG-INFO` & `realnet-0.0.94/realnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realnet
-Version: 0.0.93
+Version: 0.0.94
 Summary: Realnet command line interface
 Home-page: https://github.com/virtual-space/realnet
 Author: Marko Laban
 Author-email: marko.laban@l33tsystems.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `realnet-0.0.93/realnet.egg-info/SOURCES.txt` & `realnet-0.0.94/realnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `realnet-0.0.93/setup.py` & `realnet-0.0.94/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="realnet",
-    version="0.0.93",
+    version="0.0.94",
     description="Realnet command line interface",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/virtual-space/realnet",
     author="Marko Laban",
     author_email="marko.laban@l33tsystems.com",
     license="BSD",
```


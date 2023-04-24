# Comparing `tmp/realnet-0.0.95.tar.gz` & `tmp/realnet-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realnet-0.0.95.tar", last modified: Mon Apr 24 02:24:57 2023, max compression
+gzip compressed data, was "realnet-0.0.96.tar", last modified: Mon Apr 24 02:47:39 2023, max compression
```

## Comparing `realnet-0.0.95.tar` & `realnet-0.0.96.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.704586 realnet-0.0.95/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 02:21:14.000000 realnet-0.0.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 02:24:57.704586 realnet-0.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-24 02:21:14.000000 realnet-0.0.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.688586 realnet-0.0.95/realnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.688586 realnet-0.0.95/realnet/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/cmd/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/cmd/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/cmd/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/cmd/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/cmd/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.688586 realnet-0.0.95/realnet/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/core/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/core/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/core/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.688586 realnet-0.0.95/realnet/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.688586 realnet-0.0.95/realnet/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/aws/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/provider/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/generic/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/generic/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/provider/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/provider/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/org.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/orgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/provider/sql/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/postgres/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/provider/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/sql/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/provider/xml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/provider/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/provider/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/realnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/accounts/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/attributes/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/auths/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/auths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/auths/auths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/chatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/chatgpt/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/clients/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/ctrls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/ctrls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/ctrls/ctrls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/endpoints/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/files/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/forms/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/gltf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/gltf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/gltf/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/gltf/gltf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.692586 realnet-0.0.95/realnet/resource/groups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/groups/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/resource/items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35333 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/items/items.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/resource/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/resource/public/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/public/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/resource/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/resource/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/roles/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/resource/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/resource/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/resource/views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/runner/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/runner/http/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.688586 realnet-0.0.95/realnet/runner/http/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.696586 realnet-0.0.95/realnet/runner/http/static/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.700586 realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.688586 realnet-0.0.95/realnet/runner/http/static/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.700586 realnet-0.0.95/realnet/runner/http/static/scripts/ace/
--rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/ace.js
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/ext-beautify.js
--rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/ext-language_tools.js
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-css.js
--rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-html.js
--rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-javascript.js
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-json.js
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-python.js
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/http/static/scripts/ace/theme-monokai.js
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.700586 realnet-0.0.95/realnet/runner/sqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/runner/sqs/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.700586 realnet-0.0.95/realnet/shell/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/shell/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/shell/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/shell/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/shell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.700586 realnet-0.0.95/realnet/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.700586 realnet-0.0.95/realnet/static/initialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/initialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/initialization/access.json
--rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/initialization/apps.json
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/initialization/controls.json
--rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/initialization/core.json
--rw-r--r--   0 runner    (1001) docker     (123)   115082 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/initialization/forms.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/initialization/geometry.json
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/static/initialization/views.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.704586 realnet-0.0.95/realnet/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/control.html
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/register.html
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/register_org.html
--rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-24 02:21:14.000000 realnet-0.0.95/realnet/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:24:57.688586 realnet-0.0.95/realnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 02:24:57.000000 realnet-0.0.95/realnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 02:24:57.000000 realnet-0.0.95/realnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 02:24:57.000000 realnet-0.0.95/realnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 02:24:57.000000 realnet-0.0.95/realnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 02:24:57.000000 realnet-0.0.95/realnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 02:24:57.000000 realnet-0.0.95/realnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 02:24:57.704586 realnet-0.0.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 02:21:25.000000 realnet-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.591259 realnet-0.0.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 02:44:15.000000 realnet-0.0.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 02:47:39.591259 realnet-0.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-24 02:44:15.000000 realnet-0.0.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.575259 realnet-0.0.96/realnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.575259 realnet-0.0.96/realnet/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/cmd/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/cmd/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/cmd/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/cmd/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/cmd/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/core/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/core/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/core/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/aws/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/generic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/generic/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/generic/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/orgs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/sql/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/postgres/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/sql/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/provider/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/provider/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/realnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/resource/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/accounts/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/resource/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/attributes/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/resource/auths/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/auths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/auths/auths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/resource/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/chatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/chatgpt/chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.579259 realnet-0.0.96/realnet/resource/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/clients/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/ctrls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/ctrls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/ctrls/ctrls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/endpoints/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/files/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/forms/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/gltf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/gltf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/gltf/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/gltf/gltf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/groups/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35333 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/items/items.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/public/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/public/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/roles/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/resource/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/resource/views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/runner/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/runner/http/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.575259 realnet-0.0.96/realnet/runner/http/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.583259 realnet-0.0.96/realnet/runner/http/static/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.587259 realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.575259 realnet-0.0.96/realnet/runner/http/static/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.587259 realnet-0.0.96/realnet/runner/http/static/scripts/ace/
+-rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/ace.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/ext-beautify.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/ext-language_tools.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-css.js
+-rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-html.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-javascript.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-json.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-python.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/http/static/scripts/ace/theme-monokai.js
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.587259 realnet-0.0.96/realnet/runner/sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/runner/sqs/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.591259 realnet-0.0.96/realnet/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/shell/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/shell/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/shell/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/shell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.591259 realnet-0.0.96/realnet/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.591259 realnet-0.0.96/realnet/static/initialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/initialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/initialization/access.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/initialization/apps.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/initialization/controls.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/initialization/core.json
+-rw-r--r--   0 runner    (1001) docker     (123)   115082 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/initialization/forms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/initialization/geometry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/static/initialization/views.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.591259 realnet-0.0.96/realnet/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/control.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/register.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/register_org.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-24 02:44:15.000000 realnet-0.0.96/realnet/templates/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:47:39.575259 realnet-0.0.96/realnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-24 02:47:39.000000 realnet-0.0.96/realnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 02:47:39.000000 realnet-0.0.96/realnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 02:47:39.000000 realnet-0.0.96/realnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 02:47:39.000000 realnet-0.0.96/realnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 02:47:39.000000 realnet-0.0.96/realnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 02:47:39.000000 realnet-0.0.96/realnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 02:47:39.591259 realnet-0.0.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 02:44:23.000000 realnet-0.0.96/setup.py
```

### Comparing `realnet-0.0.95/LICENSE` & `realnet-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/PKG-INFO` & `realnet-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realnet
-Version: 0.0.95
+Version: 0.0.96
 Summary: Realnet command line interface
 Home-page: https://github.com/virtual-space/realnet
 Author: Marko Laban
 Author-email: marko.laban@l33tsystems.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `realnet-0.0.95/README.md` & `realnet-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/cmd/server.py` & `realnet-0.0.96/realnet/cmd/server.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/core/config.py` & `realnet-0.0.96/realnet/core/config.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/core/hierarchy.py` & `realnet-0.0.96/realnet/core/hierarchy.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/core/provider.py` & `realnet-0.0.96/realnet/core/provider.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/core/type.py` & `realnet-0.0.96/realnet/core/type.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/aws/data.py` & `realnet-0.0.96/realnet/provider/aws/data.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/generic/endpoint.py` & `realnet-0.0.96/realnet/provider/generic/endpoint.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/generic/resource.py` & `realnet-0.0.96/realnet/provider/generic/resource.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/client.py` & `realnet-0.0.96/realnet/provider/sql/client.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/init.py` & `realnet-0.0.96/realnet/provider/sql/init.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/models.py` & `realnet-0.0.96/realnet/provider/sql/models.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/org.py` & `realnet-0.0.96/realnet/provider/sql/org.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/orgs.py` & `realnet-0.0.96/realnet/provider/sql/orgs.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/postgres/item.py` & `realnet-0.0.96/realnet/provider/sql/postgres/item.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/roles.py` & `realnet-0.0.96/realnet/provider/sql/roles.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/type.py` & `realnet-0.0.96/realnet/provider/sql/type.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/provider/sql/utility.py` & `realnet-0.0.96/realnet/provider/sql/utility.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/accounts/accounts.py` & `realnet-0.0.96/realnet/resource/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/apps/apps.py` & `realnet-0.0.96/realnet/resource/apps/apps.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/auths/auths.py` & `realnet-0.0.96/realnet/resource/auths/auths.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/chatgpt/chatgpt.py` & `realnet-0.0.96/realnet/resource/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/clients/clients.py` & `realnet-0.0.96/realnet/resource/clients/clients.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/ctrls/ctrls.py` & `realnet-0.0.96/realnet/resource/ctrls/ctrls.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/files/files.py` & `realnet-0.0.96/realnet/resource/files/files.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/gltf/export.py` & `realnet-0.0.96/realnet/resource/gltf/export.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/gltf/gltf.py` & `realnet-0.0.96/realnet/resource/gltf/gltf.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/groups/groups.py` & `realnet-0.0.96/realnet/resource/groups/groups.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/items/items.py` & `realnet-0.0.96/realnet/resource/items/items.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/login/login.py` & `realnet-0.0.96/realnet/resource/login/login.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/roles/roles.py` & `realnet-0.0.96/realnet/resource/roles/roles.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/types/types.py` & `realnet-0.0.96/realnet/resource/types/types.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/resource/views/views.py` & `realnet-0.0.96/realnet/resource/views/views.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/app.py` & `realnet-0.0.96/realnet/runner/http/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from flask import Flask, Response, redirect, render_template, render_template_string, request, jsonify, Blueprint, send_file, session
 from flask_cors import CORS
 from flask_bootstrap import Bootstrap
 
 from werkzeug.middleware.proxy_fix import ProxyFix
 
+import os
 import json
 import jinja2
 
 import logging
 
 from realnet.core.config import Config
 from .auth import config_oauth
@@ -15,14 +16,17 @@
 
 
 def create_app(contextProvider):
     logging.basicConfig(level=logging.DEBUG)
 
     cfg = Config()
 
+    # TODO make sure this is properly set unless we are behind a proxy
+    os.environ['AUTHLIB_INSECURE_TRANSPORT'] = '1'
+
     app = Flask(__name__)
     CORS(app)
     # import realnet_server.wsgi
 
     
 
     app.secret_key = cfg.get_app_secret()
```

### Comparing `realnet-0.0.95/realnet/runner/http/auth.py` & `realnet-0.0.96/realnet/runner/http/auth.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/router.py` & `realnet-0.0.96/realnet/runner/http/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,17 +98,17 @@
                     if not password:
                         password = request.args.get('password')
                     if not password and request.is_json:
                         password = request.json.get('password')
                     if password:
                         account = contextProvider.check_password(org.id, username, password)
                         if account:
-                            logger.info('*** request scheme: ' + request.scheme)
-                            logger.info('*** request base url: ' + request.base_url)
-                            logger.info('*** request query string: ' + to_unicode(request.query_string))
+                            # logger.info('*** request scheme: ' + request.scheme)
+                            # logger.info('*** request base url: ' + request.base_url)
+                            # logger.info('*** request query string: ' + to_unicode(request.query_string))
                             return authorization.create_token_response()
                             # return authorization.create_authorization_response(grant_user=account)
             else:
                 if name == None:
                     oauths = [{'name': n['name'],
                                'url': '/{0}/login/{1}?client_id={2}&response_type={3}'.format(id, n['name'], client_id, response_type)} for n in
                               [q.to_dict() for q in contextProvider.get_org_authenticators(org.id)]]
```

### Comparing `realnet-0.0.95/realnet/runner/http/static/font-awesome/css/font-awesome.css` & `realnet-0.0.96/realnet/runner/http/static/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/font-awesome/css/font-awesome.min.css` & `realnet-0.0.96/realnet/runner/http/static/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf` & `realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot` & `realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg` & `realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf` & `realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff` & `realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2` & `realnet-0.0.96/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/ace.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/ace.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/ext-beautify.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/ext-beautify.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/ext-language_tools.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-css.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-css.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-html.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-html.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-javascript.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-javascript.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-json.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-json.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/mode-python.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/runner/http/static/scripts/ace/theme-monokai.js` & `realnet-0.0.96/realnet/runner/http/static/scripts/ace/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/shell/cmd.py` & `realnet-0.0.96/realnet/shell/cmd.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/shell/proto.py` & `realnet-0.0.96/realnet/shell/proto.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/shell/shell.py` & `realnet-0.0.96/realnet/shell/shell.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/static/initialization/access.json` & `realnet-0.0.96/realnet/static/initialization/access.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/static/initialization/apps.json` & `realnet-0.0.96/realnet/static/initialization/apps.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/static/initialization/controls.json` & `realnet-0.0.96/realnet/static/initialization/controls.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/static/initialization/core.json` & `realnet-0.0.96/realnet/static/initialization/core.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/static/initialization/forms.json` & `realnet-0.0.96/realnet/static/initialization/forms.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/static/initialization/geometry.json` & `realnet-0.0.96/realnet/static/initialization/geometry.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/static/initialization/views.json` & `realnet-0.0.96/realnet/static/initialization/views.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/control.html` & `realnet-0.0.96/realnet/templates/control.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/form.html` & `realnet-0.0.96/realnet/templates/form.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/item.html` & `realnet-0.0.96/realnet/templates/item.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/login.html` & `realnet-0.0.96/realnet/templates/login.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/main.html` & `realnet-0.0.96/realnet/templates/main.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/nav.html` & `realnet-0.0.96/realnet/templates/nav.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/register.html` & `realnet-0.0.96/realnet/templates/register.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/register_org.html` & `realnet-0.0.96/realnet/templates/register_org.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet/templates/view.html` & `realnet-0.0.96/realnet/templates/view.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/realnet.egg-info/PKG-INFO` & `realnet-0.0.96/realnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realnet
-Version: 0.0.95
+Version: 0.0.96
 Summary: Realnet command line interface
 Home-page: https://github.com/virtual-space/realnet
 Author: Marko Laban
 Author-email: marko.laban@l33tsystems.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `realnet-0.0.95/realnet.egg-info/SOURCES.txt` & `realnet-0.0.96/realnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `realnet-0.0.95/setup.py` & `realnet-0.0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="realnet",
-    version="0.0.95",
+    version="0.0.96",
     description="Realnet command line interface",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/virtual-space/realnet",
     author="Marko Laban",
     author_email="marko.laban@l33tsystems.com",
     license="BSD",
```


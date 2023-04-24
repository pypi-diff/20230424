# Comparing `tmp/investing_algorithm_framework-0.9.tar.gz` & `tmp/investing_algorithm_framework-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-0.9.tar", last modified: Wed Oct 20 15:06:39 2021, max compression
+gzip compressed data, was "investing_algorithm_framework-1.0.tar", last modified: Mon Apr 24 15:39:32 2023, max compression
```

## Comparing `investing_algorithm_framework-0.9.tar` & `investing_algorithm_framework-1.0.tar`

### file list

```diff
@@ -1,225 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11343 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8376 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6326 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.462071 investing_algorithm_framework-0.9/investing_algorithm_framework/
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      907 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/__pycache__/globals.cpython-39.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/app/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/app/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/app/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     5381 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/app/__pycache__/app.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     5704 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      819 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      992 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/__pycache__/constants.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     5900 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     4342 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/__pycache__/setup.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/__pycache__/validator.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      894 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4727 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5919 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/context/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/context/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/context/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      663 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/context/__pycache__/singleton.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      345 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/context/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/__pycache__/identifier.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/__pycache__/market_identifier.cpython-39.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/context/
--rw-r--r--   0 runner    (1001) docker     (121)      684 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/context/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      982 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/context/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)    15021 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/context/__pycache__/algorithm_context.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/context/__pycache__/algorithm_context_configuration.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)    21920 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/context/algorithm_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/context/algorithm_context_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      589 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/__pycache__/binance_data_provider.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/__pycache__/data_provider.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/binance_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/data_providers/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/events/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/events/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/events/observer.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      598 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     6313 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/__pycache__/binance_market_service.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      804 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/__pycache__/market_service.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     6654 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/binance_market_service.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/market_services/market_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/__pycache__/binance_api_secret_key_specifier.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/binance_api_secret_key_specifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/data_providers/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/data_providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/data_providers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/data_providers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/data_providers/__pycache__/binance.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/data_providers/binance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/order_executors/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/order_executors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/order_executors/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/order_executors/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/order_executors/__pycache__/binance.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/order_executors/binance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/portfolio_managers/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/portfolio_managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/portfolio_managers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/portfolio_managers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/portfolio_managers/__pycache__/binance.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/mixins/portfolio_managers/binance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.470071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/model_extension.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     9171 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/order.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/order_side.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/order_status.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      953 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/order_type.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     6777 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/portfolio.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/position.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      967 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/__pycache__/time_unit.cpython-39.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/__pycache__/order_book.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/__pycache__/ticker.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/__pycache__/trading_data_types.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/order_book.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/ticker.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/trading_data_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/model_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)    12008 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/order.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/order_side.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/order_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     8683 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/position.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/time_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      930 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/__pycache__/binance.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/__pycache__/order_executor.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      517 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/binance.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_executors/order_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/__pycache__/default_order_validator.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/__pycache__/order_validation_factory.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/__pycache__/order_validator.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/default_order_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/order_validation_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3416 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/order_validators/order_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/__pycache__/binance.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      804 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     4300 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/__pycache__/portfolio_manager.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/binance.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     4791 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/portfolio_managers/portfolio_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/workers/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/workers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/core/workers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/workers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/workers/__pycache__/scheduler.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/core/workers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/exchanges/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5674 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/exchanges/binance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/exchanges/exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.474071 investing_algorithm_framework-0.9/investing_algorithm_framework/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/investing_algorithm_framework/extensions/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/extensions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/extensions/__pycache__/scheduler.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/extensions/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)      320 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      517 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/__pycache__/order.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/__pycache__/portfolio.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      937 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/__pycache__/position.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      908 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/order.py
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/schemas/position.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      740 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/__pycache__/random.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/__pycache__/stoppable_thread.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/__pycache__/synchronized.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-10-20 15:06:38.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/__pycache__/version.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/signatures.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/synchronized.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/investing_algorithm_framework/views/
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/investing_algorithm_framework/views/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      717 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/__pycache__/operational_views.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/__pycache__/order_views.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/__pycache__/portfolio_views.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/__pycache__/position_views.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/operational_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/order_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/portfolio_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/position_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/investing_algorithm_framework/views/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-20 15:06:39.466071 investing_algorithm_framework-0.9/investing_algorithm_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8376 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11938 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-10-20 15:06:39.000000 investing_algorithm_framework-0.9/investing_algorithm_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-20 15:06:39.478071 investing_algorithm_framework-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-10-20 15:06:19.000000 investing_algorithm_framework-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/run_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/dependency_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/asset_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/synchronized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/model_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/order/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/order/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/position/position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/services/market_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/investing_algorithm_framework/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/market_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/order_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/portfolio_configuration_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/portfolio_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/setup_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/tests/test_create_app.py
```

### Comparing `investing_algorithm_framework-0.9/LICENSE` & `investing_algorithm_framework-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-0.9/PKG-INFO` & `investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,166 +1,159 @@
 Metadata-Version: 2.1
-Name: investing_algorithm_framework
-Version: 0.9
+Name: investing-algorithm-framework
+Version: 1.0
 Summary: A framework for creating an investment algorithm
 Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
+Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
 Author: coding kitties
 License: Apache License 2.0
-Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
-Description: [![Build](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml)
-        [![Tests](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml)
-        [![Downloads](https://pepy.tech/badge/investing-algorithm-framework)](https://pepy.tech/badge/investing-algorithm-framework)
-        [![Current Version](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)
-        
-        # Investing Algorithm Framework
-        
-        > :warning: **Documentation outdated**: We are working hard on releasing v1.0.0. After 
-        > this release we will update the documentation at the website.
-        
-        The Investing Algorithm Framework is a python framework for building
-        investment algorithms. It encourages rapid development and clean, pragmatic code design.
-        
-        The framework provides you with an all the components you need to create an 
-        investing algorithm (data providing, portfolio management, order execution, etc..). 
-        Also, the algorithm can be controlled with a REST Api that will run in the background.
-        
-        
-        ## Example Algorithm for Binance
-        ```python
-        import os
-        
-        from investing_algorithm_framework import App, TimeUnit, AlgorithmContext, \
-            TradingDataTypes
-        from investing_algorithm_framework.configuration.constants import BINANCE, \
-            BINANCE_API_KEY, BINANCE_SECRET_KEY, TRADING_SYMBOL
-        
-        BTC_SYMBOL = "BTC"
-        
-        # Our trading symbol (e.g. dot/usdt, sol/usdt)
-        USDT_SYMBOL = "USDT"
-        
-        # Make the parent dir your resources directory (database, csv storage)
-        dir_path = os.path.abspath(os.path.join(os.path.realpath(__file__), os.pardir))
-        
-        # Create an application (setups your algorithm, database, rest api, etc...)
-        app = App(
-            resources_directory=dir_path,
-            config={
-                BINANCE_API_KEY: "<BINANCE_API_KEY>",
-                BINANCE_SECRET_KEY: "<BINANCE_SECRET_KEY>",
-                TRADING_SYMBOL: USDT_SYMBOL,
-            }
-        )
-        
-        
-        # Algorithm strategy that runs every 5 minutes
-        @app.algorithm.schedule(time_unit=TimeUnit.MINUTE, interval=5)
-        def perform_strategy(context: AlgorithmContext):
-            # Get ticker data from binance
-            ticker = context.get_data(
-                BINANCE,
-                trading_data_type=TradingDataTypes.TICKER,
-                target_symbol=BTC_SYMBOL,
-            )
-        
-            if ticker.ask_price > 50000:
-                # Execute a market order on binance
-                context.create_market_buy_order(
-                    BINANCE, BTC_SYMBOL, amount_trading_symbol=10, execute=True
-                )
-        
-        
-        if __name__ == "__main__":
-            app.start()
-        ```
-        The goal of the framework is to provide you with a set of components for 
-        your algorithm that takes care of a wide variety of operational processes 
-        out of the box.
-        
-        * Data providing
-        * Order execution
-        * Portfolio management
-        * Performance tracking
-        * Strategy scheduling
-        * Resource management
-        * Model snapshots
-        * Order status management
-        * Clients (Rest API)
-        
-        However, we aim to also provide a modular framework where you can write your
-        own components or use third party plugins for the framework.
-        
-        Further information and the complete documentation can be found at the [webstie](https://investing-algorithm-framework.com)
-        
-        
-        ## Download
-        You can download the framework with pypi.
-        
-        ```bash
-        pip install investing-algorithm-framework
-        ```
-        
-        #### Disclaimer
-        If you use this framework for your investments, do not risk money 
-        which you are afraid to lose, until you have clear understanding how 
-        the framework works. We can't stress this enough:
-        
-        BEFORE YOU START USING MONEY WITH THE FRAMEWORK, MAKE SURE THAT YOU TESTED 
-        YOUR COMPONENTS THOROUGHLY. USE THE SOFTWARE AT YOUR OWN RISK. 
-        THE AUTHORS AND ALL AFFILIATES ASSUME NO RESPONSIBILITY FOR YOUR INVESTMENT RESULTS.
-        
-        Also, make sure that you read the source code of any plugin you use or 
-        implementation of an algorithm made with this framework.
-        
-        For further information regarding usage and licensing we recommend going 
-        to the licensing page at the website.
-        
-        ## Documentation
-        
-        All the documentation can be found online at the [documentation webstie](https://investing-algorithm-framework.com)
-        
-        In most cases, you'll probably never have to change code on this repo directly 
-        if you are building your algorithm/bot. But if you do, check out the 
-        contributing page at the website.
-        
-        If you'd like to chat with investing-algorithm-framework users 
-        and developers, [join us on Slack](https://inv-algo-framework.slack.com) or [join us on reddit](https://www.reddit.com/r/InvestingAlgorithms/)
-        
-        ## Acknowledgements
-        We want to thank all contributors to this project. A full list of all 
-        the people that contributed to the project can be
-        found [here](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/docs/AUTHORS.md)
-        
-        ### Help / Slack
-        
-        For any questions not covered by the documentation or for further
-        information about the framework, we encourage you to join our slack channel.
-        
-        [join us on Slack](https://inv-algo-framework.slack.com)
-        
-        ### [Bugs / Issues](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
-        
-        If you discover a bug in the framework, please [search our issue tracker](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
-        first. If it hasn't been reported, please [create a new issue](https://github.com/investing-algorithms/investing-algorithm-framework/issues/new).
-        
-        Feel like the framework is missing a feature? We welcome your pull requests!
-        
-        Please read our [Contributing document](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/docs/CONTRIBUTING.md)
-        to understand the requirements before sending your pull-requests.
-        
-        **Note** before starting any major new feature work, *please open an issue describing what you are planning to do* or talk to us on [Slack](https://join.slack.com/t/investingbots/shared_invite/enQtODgwNTg3MzA2MjYyLTdiZjczZDRlNWJjNDdmYThiMGE0MzFhOTg4Y2E0NzQ2OTgxYjA1NzU3ZWJiY2JhOTE1ZGJlZGFiNDU3OTAzMDg).
-        This will ensure that interested parties can give valuable feedback on the feature, and let others know that you are working on it.
-        
-        **Important:** Always create your feature or hotfix against the `develop` branch, not `master`.
-        
-Keywords: INVESTING,BOT,ALGORITHM,FRAMEWORK
-Platform: UNKNOWN
+Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+<a href=https://investing-algorithm-framework.com><img src="https://img.shields.io/badge/docs-website-brightgreen"></a>
+[![Build](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml)
+[![Tests](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml)
+[![Downloads](https://pepy.tech/badge/investing-algorithm-framework)](https://pepy.tech/badge/investing-algorithm-framework)
+[![Current Version](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)
+<a href="https://www.reddit.com/r/InvestingBots/"><img src="https://img.shields.io/reddit/subreddit-subscribers/investingbots?style=social"></a>
+###### Sponsors
+<p align="left">
+<a href="https://logicfunds.io">
+  <img alt="logicfunds" src="https://logicfunds-web-app-images.s3.eu-central-1.amazonaws.com/logicfunds-logo.png" width="200px" />
+</a>
+</p>
+
+# Investing Algorithm Framework
+The Investing Algorithm Framework is a python framework for building
+investment algorithms. It encourages rapid development and clean, pragmatic code design.
+
+The framework provides you with all the components you need to create an 
+investing algorithm (data providing, portfolio management, order execution, etc..). Also,
+it has various deployment options, such as web server, stateless, etc..
+
+## Example
+The following algorithm connects to binance and buys BTC every 5 seconds. 
+It also exposes an REST API that allows you to interact with the algorithm.
+```python
+import pathlib
+from datetime import datetime, timedelta
+
+from investing_algorithm_framework import create_app, PortfolioConfiguration, \
+    RESOURCE_DIRECTORY, TimeUnit, TradingTimeFrame, TradingDataType, OrderSide
+
+app = create_app({RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()})
+app.add_portfolio_configuration(
+    PortfolioConfiguration(
+        market="binance",
+        api_key="xxxxxx",
+        secret_key="xxxxxx",
+        trading_symbol="USDT"
+    )
+)
+
+
+@app.strategy(
+    time_unit=TimeUnit.SECOND, # Algorithm will be executed every 5 seconds
+    interval=5,
+    market="binance", # Will retrieve trading data from binance
+    symbols=["BTC/USDT", "ETH/USDT", ["DOT/USDT"]], # Symbols must be in the format of TARGET/TRADE symbol (e.g. BTC/USDT)
+    trading_data_types=[TradingDataType.OHLCV, TradingDataType.TICKER, TradingDataType.ORDER_BOOK],
+    trading_time_frame_start_date=datetime.utcnow() - timedelta(days=1), # Will retrieve data from the last 24 hours
+    trading_time_frame=TradingTimeFrame.ONE_MINUTE # Will retrieve data on 1m interval (OHLCV)
+)
+def perform_strategy(algorithm, market_data):
+    print(algorithm.get_allocated())
+    print(algorithm.get_unallocated())
+    print(market_data)
+    algorithm.create_limit_order(
+        target_symbol="BTC", 
+        side=OrderSide.BUY,
+        price=market_data["TICKER"]["BTC/USDT"]["BID"], 
+        amount_target_symbol=0.00001
+    )
+
+
+if __name__ == "__main__":
+    app.run()
+```
+
+> You can find more examples [here](./examples) folder.
+
+## Broker/Exchange configuration
+The framework has by default support for [ccxt](https://github.com/ccxt/ccxt).
+This should allow you to connect to a lot of brokers/exchanges.
+
+```python
+from investing_algorithm_framework import App, PortfolioConfiguration
+app = App()
+app.add_portfolio_configuration(
+    PortfolioConfiguration(
+        market="bitvavo", 
+        api_key="xxxx", 
+        secret_key="xxxx", 
+        track_from="01/01/2022",
+        trading_symbol="EUR"
+    )
+)
+```
+
+## Download
+You can download the framework with pypi.
+
+```bash
+pip install investing-algorithm-framework
+```
+
+## Disclaimer
+If you use this framework for your investments, do not risk money 
+which you are afraid to lose, until you have clear understanding how 
+the framework works. We can't stress this enough:
+
+BEFORE YOU START USING MONEY WITH THE FRAMEWORK, MAKE SURE THAT YOU TESTED 
+YOUR COMPONENTS THOROUGHLY. USE THE SOFTWARE AT YOUR OWN RISK. 
+THE AUTHORS AND ALL AFFILIATES ASSUME NO RESPONSIBILITY FOR YOUR INVESTMENT RESULTS.
+
+Also, make sure that you read the source code of any plugin you use or 
+implementation of an algorithm made with this framework.
+
+For further information regarding usage and licensing we recommend going 
+to the licensing page at the website.
+
+## Documentation
+
+All the documentation can be found online 
+at the [documentation webstie](https://investing-algorithm-framework.com)
+
+In most cases, you'll probably never have to change code on this repo directly 
+if you are building your algorithm/bot. But if you do, check out the 
+contributing page at the website.
+
+If you'd like to chat with investing-algorithm-framework users 
+and developers, [join us on Slack](https://inv-algo-framework.slack.com) or [join us on reddit](https://www.reddit.com/r/InvestingBots/)
+
+## Acknowledgements
+We want to thank all contributors to this project. A full list of all 
+the people that contributed to the project can be
+found [here](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/AUTHORS.md)
+
+### [Bugs / Issues](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
+
+If you discover a bug in the framework, please [search our issue tracker](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
+first. If it hasn't been reported, please [create a new issue](https://github.com/investing-algorithms/investing-algorithm-framework/issues/new).
+
+Feel like the framework is missing a feature? We welcome your pull requests!
+
+**Note** before starting any major new feature work, *please open an issue describing what you are planning to do*.
+This will ensure that interested parties can give valuable feedback on the feature, and let others know that you are working on it.
+
+**Important:** Always create your feature or hotfix against the `develop` branch, not `master`.
```

### Comparing `investing_algorithm_framework-0.9/README.md` & `investing_algorithm_framework-1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,102 @@
+<a href=https://investing-algorithm-framework.com><img src="https://img.shields.io/badge/docs-website-brightgreen"></a>
 [![Build](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml)
-[![Tests](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml)
+[![Tests](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml)
 [![Downloads](https://pepy.tech/badge/investing-algorithm-framework)](https://pepy.tech/badge/investing-algorithm-framework)
 [![Current Version](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)
+<a href="https://www.reddit.com/r/InvestingBots/"><img src="https://img.shields.io/reddit/subreddit-subscribers/investingbots?style=social"></a>
+###### Sponsors
+<p align="left">
+<a href="https://logicfunds.io">
+  <img alt="logicfunds" src="https://logicfunds-web-app-images.s3.eu-central-1.amazonaws.com/logicfunds-logo.png" width="200px" />
+</a>
+</p>
 
 # Investing Algorithm Framework
-
-> :warning: **Documentation outdated**: We are working hard on releasing v1.0.0. After 
-> this release we will update the documentation at the website.
-
 The Investing Algorithm Framework is a python framework for building
 investment algorithms. It encourages rapid development and clean, pragmatic code design.
 
-The framework provides you with an all the components you need to create an 
-investing algorithm (data providing, portfolio management, order execution, etc..). 
-Also, the algorithm can be controlled with a REST Api that will run in the background.
-
-
-## Example Algorithm for Binance
+The framework provides you with all the components you need to create an 
+investing algorithm (data providing, portfolio management, order execution, etc..). Also,
+it has various deployment options, such as web server, stateless, etc..
+
+## Example
+The following algorithm connects to binance and buys BTC every 5 seconds. 
+It also exposes an REST API that allows you to interact with the algorithm.
 ```python
-import os
+import pathlib
+from datetime import datetime, timedelta
 
-from investing_algorithm_framework import App, TimeUnit, AlgorithmContext, \
-    TradingDataTypes
-from investing_algorithm_framework.configuration.constants import BINANCE, \
-    BINANCE_API_KEY, BINANCE_SECRET_KEY, TRADING_SYMBOL
-
-BTC_SYMBOL = "BTC"
-
-# Our trading symbol (e.g. dot/usdt, sol/usdt)
-USDT_SYMBOL = "USDT"
-
-# Make the parent dir your resources directory (database, csv storage)
-dir_path = os.path.abspath(os.path.join(os.path.realpath(__file__), os.pardir))
-
-# Create an application (setups your algorithm, database, rest api, etc...)
-app = App(
-    resources_directory=dir_path,
-    config={
-        BINANCE_API_KEY: "<BINANCE_API_KEY>",
-        BINANCE_SECRET_KEY: "<BINANCE_SECRET_KEY>",
-        TRADING_SYMBOL: USDT_SYMBOL,
-    }
+from investing_algorithm_framework import create_app, PortfolioConfiguration, \
+    RESOURCE_DIRECTORY, TimeUnit, TradingTimeFrame, TradingDataType, OrderSide
+
+app = create_app({RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()})
+app.add_portfolio_configuration(
+    PortfolioConfiguration(
+        market="binance",
+        api_key="xxxxxx",
+        secret_key="xxxxxx",
+        trading_symbol="USDT"
+    )
 )
 
 
-# Algorithm strategy that runs every 5 minutes
-@app.algorithm.schedule(time_unit=TimeUnit.MINUTE, interval=5)
-def perform_strategy(context: AlgorithmContext):
-    # Get ticker data from binance
-    ticker = context.get_data(
-        BINANCE,
-        trading_data_type=TradingDataTypes.TICKER,
-        target_symbol=BTC_SYMBOL,
+@app.strategy(
+    time_unit=TimeUnit.SECOND, # Algorithm will be executed every 5 seconds
+    interval=5,
+    market="binance", # Will retrieve trading data from binance
+    symbols=["BTC/USDT", "ETH/USDT", ["DOT/USDT"]], # Symbols must be in the format of TARGET/TRADE symbol (e.g. BTC/USDT)
+    trading_data_types=[TradingDataType.OHLCV, TradingDataType.TICKER, TradingDataType.ORDER_BOOK],
+    trading_time_frame_start_date=datetime.utcnow() - timedelta(days=1), # Will retrieve data from the last 24 hours
+    trading_time_frame=TradingTimeFrame.ONE_MINUTE # Will retrieve data on 1m interval (OHLCV)
+)
+def perform_strategy(algorithm, market_data):
+    print(algorithm.get_allocated())
+    print(algorithm.get_unallocated())
+    print(market_data)
+    algorithm.create_limit_order(
+        target_symbol="BTC", 
+        side=OrderSide.BUY,
+        price=market_data["TICKER"]["BTC/USDT"]["BID"], 
+        amount_target_symbol=0.00001
     )
 
-    if ticker.ask_price > 50000:
-        # Execute a market order on binance
-        context.create_market_buy_order(
-            BINANCE, BTC_SYMBOL, amount_trading_symbol=10, execute=True
-        )
-
 
 if __name__ == "__main__":
-    app.start()
+    app.run()
 ```
-The goal of the framework is to provide you with a set of components for 
-your algorithm that takes care of a wide variety of operational processes 
-out of the box.
-
-* Data providing
-* Order execution
-* Portfolio management
-* Performance tracking
-* Strategy scheduling
-* Resource management
-* Model snapshots
-* Order status management
-* Clients (Rest API)
 
-However, we aim to also provide a modular framework where you can write your
-own components or use third party plugins for the framework.
+> You can find more examples [here](./examples) folder.
 
-Further information and the complete documentation can be found at the [webstie](https://investing-algorithm-framework.com)
+## Broker/Exchange configuration
+The framework has by default support for [ccxt](https://github.com/ccxt/ccxt).
+This should allow you to connect to a lot of brokers/exchanges.
 
+```python
+from investing_algorithm_framework import App, PortfolioConfiguration
+app = App()
+app.add_portfolio_configuration(
+    PortfolioConfiguration(
+        market="bitvavo", 
+        api_key="xxxx", 
+        secret_key="xxxx", 
+        track_from="01/01/2022",
+        trading_symbol="EUR"
+    )
+)
+```
 
 ## Download
 You can download the framework with pypi.
 
 ```bash
 pip install investing-algorithm-framework
 ```
 
-#### Disclaimer
+## Disclaimer
 If you use this framework for your investments, do not risk money 
 which you are afraid to lose, until you have clear understanding how 
 the framework works. We can't stress this enough:
 
 BEFORE YOU START USING MONEY WITH THE FRAMEWORK, MAKE SURE THAT YOU TESTED 
 YOUR COMPONENTS THOROUGHLY. USE THE SOFTWARE AT YOUR OWN RISK. 
 THE AUTHORS AND ALL AFFILIATES ASSUME NO RESPONSIBILITY FOR YOUR INVESTMENT RESULTS.
@@ -104,42 +105,33 @@
 implementation of an algorithm made with this framework.
 
 For further information regarding usage and licensing we recommend going 
 to the licensing page at the website.
 
 ## Documentation
 
-All the documentation can be found online at the [documentation webstie](https://investing-algorithm-framework.com)
+All the documentation can be found online 
+at the [documentation webstie](https://investing-algorithm-framework.com)
 
 In most cases, you'll probably never have to change code on this repo directly 
 if you are building your algorithm/bot. But if you do, check out the 
 contributing page at the website.
 
 If you'd like to chat with investing-algorithm-framework users 
-and developers, [join us on Slack](https://inv-algo-framework.slack.com) or [join us on reddit](https://www.reddit.com/r/InvestingAlgorithms/)
+and developers, [join us on Slack](https://inv-algo-framework.slack.com) or [join us on reddit](https://www.reddit.com/r/InvestingBots/)
 
 ## Acknowledgements
 We want to thank all contributors to this project. A full list of all 
 the people that contributed to the project can be
-found [here](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/docs/AUTHORS.md)
-
-### Help / Slack
-
-For any questions not covered by the documentation or for further
-information about the framework, we encourage you to join our slack channel.
-
-[join us on Slack](https://inv-algo-framework.slack.com)
+found [here](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/AUTHORS.md)
 
 ### [Bugs / Issues](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
 
 If you discover a bug in the framework, please [search our issue tracker](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
 first. If it hasn't been reported, please [create a new issue](https://github.com/investing-algorithms/investing-algorithm-framework/issues/new).
 
 Feel like the framework is missing a feature? We welcome your pull requests!
 
-Please read our [Contributing document](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/docs/CONTRIBUTING.md)
-to understand the requirements before sending your pull-requests.
-
-**Note** before starting any major new feature work, *please open an issue describing what you are planning to do* or talk to us on [Slack](https://join.slack.com/t/investingbots/shared_invite/enQtODgwNTg3MzA2MjYyLTdiZjczZDRlNWJjNDdmYThiMGE0MzFhOTg4Y2E0NzQ2OTgxYjA1NzU3ZWJiY2JhOTE1ZGJlZGFiNDU3OTAzMDg).
+**Note** before starting any major new feature work, *please open an issue describing what you are planning to do*.
 This will ensure that interested parties can give valuable feedback on the feature, and let others know that you are working on it.
 
 **Important:** Always create your feature or hotfix against the `develop` branch, not `master`.
```

### Comparing `investing_algorithm_framework-0.9/investing_algorithm_framework/configuration/settings.py` & `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
+import logging
 import os
-
 from enum import Enum
-import logging
 
-from investing_algorithm_framework.core import OperationalException
-from investing_algorithm_framework.configuration.constants import \
-    DATABASE_NAME, DATABASE_DIRECTORY_PATH, RESOURCES_DIRECTORY
+from .constants import RESOURCE_DIRECTORY
+from .exceptions import OperationalException
 
 logger = logging.getLogger(__name__)
 
 
 class Environment(Enum):
     """
     Class TimeUnit: Enum for data_provider base type
@@ -51,16 +49,16 @@
             except OperationalException:
                 pass
 
             return other == self.value
 
 
 class Config(dict):
-    ENV = "DEV"
-    LOG_LEVEL = 'INFO'
+    ENVIRONMENT = Environment.PROD.value
+    LOG_LEVEL = 'DEBUG'
     APP_DIR = os.path.abspath(os.path.dirname(__file__))
     PROJECT_ROOT = os.path.abspath(os.path.join(APP_DIR, os.pardir))
     DEBUG_TB_INTERCEPT_REDIRECTS = False
     SQLALCHEMY_TRACK_MODIFICATIONS = False
     CACHE_TYPE = 'simple'  # Can be "memcached", "redis", etc.
     CORS_ORIGIN_WHITELIST = [
         'http://0.0.0.0:4100',
@@ -68,25 +66,26 @@
         'http://0.0.0.0:8000',
         'http://localhost:8000',
         'http://0.0.0.0:4200',
         'http://localhost:4200',
         'http://0.0.0.0:4000',
         'http://localhost:4000',
     ]
-    RESOURCES_DIRECTORY = os.getenv(RESOURCES_DIRECTORY)
-    DATABASE_CONFIG = {
-        DATABASE_NAME: os.getenv(DATABASE_NAME, "database"),
-        DATABASE_DIRECTORY_PATH: os.getenv(DATABASE_DIRECTORY_PATH)
-    }
+    RESOURCE_DIRECTORY = os.getenv(RESOURCE_DIRECTORY)
     SCHEDULER_API_ENABLED = True
     CHECK_PENDING_ORDERS = True
+    SQLITE_ENABLED = True
+    SQLITE_INITIALIZED = False
 
-    def __init__(self):
+    def __init__(self, resource_directory=None):
         super().__init__()
 
+        if resource_directory is not None:
+            self.RESOURCE_DIRECTORY = resource_directory
+
         for attribute_key in dir(Config):
 
             if attribute_key.isupper():
                 self[attribute_key] = getattr(self, attribute_key)
 
     def __setitem__(self, key, item):
         self.__dict__[key] = item
@@ -174,19 +173,17 @@
             if attribute_key:
                 config.set(attribute_key, dictionary[attribute_key])
                 config[attribute_key] = dictionary[attribute_key]
         return config
 
 
 class TestConfig(Config):
-    ENV = Environment.TEST.value
+    ENVIRONMENT = Environment.TEST.value
     TESTING = True
-    DATABASE_CONFIG = {
-        'DATABASE_NAME': "test",
-    }
+    DATABASE_CONFIG = {'DATABASE_NAME': "test"}
+    LOG_LEVEL = "INFO"
 
 
 class DevConfig(Config):
-    ENV = Environment.DEV.value
-    DATABASE_CONFIG = {
-        'DATABASE_NAME': "dev",
-    }
+    ENVIRONMENT = Environment.DEV.value
+    DATABASE_CONFIG = {'DATABASE_NAME': "dev"}
+    LOG_LEVEL = "INFO"
```

### Comparing `investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/data_provider/trading_data_types.py` & `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 from enum import Enum
 
 
-class TradingDataTypes(Enum):
+class TradingDataType(Enum):
     TICKER = 'TICKER'
     ORDER_BOOK = 'ORDER_BOOK'
-    UN_SPECIFIED = "UN_SPECIFIED"
+    OHLCV = "OHLCV"
+
+    @staticmethod
+    def from_value(value):
+
+        if isinstance(value, TradingDataType):
+            for trading_data_type in TradingDataType:
+
+                if value == trading_data_type:
+                    return trading_data_type
+
+        elif isinstance(value, str):
+            return TradingDataType.from_string(value)
+
+        raise ValueError(
+            "Could not convert value to trading data type"
+        )
 
     @staticmethod
     def from_string(value: str):
 
         if isinstance(value, str):
-            for order_type in TradingDataTypes:
+            for order_type in TradingDataType:
 
                 if value.upper() == order_type.value:
                     return order_type
 
         raise ValueError(
-            "Could not convert value to data_provider provider "
-            "data_provider type"
+            "Could not convert value to trading data type"
         )
 
     def equals(self, other):
 
         if other is None:
             return False
 
         if isinstance(other, Enum):
             return self.value == other.value
 
         else:
-            return TradingDataTypes.from_string(other) == self
+            return TradingDataType.from_string(other) == self
```

### Comparing `investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/order.py` & `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/services/market_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,411 +1,420 @@
 import logging
 from datetime import datetime
-from random import randint
+from time import sleep
+import pandas as pd
+from dateutil.parser import parse
+import ccxt
 
-from sqlalchemy.ext.hybrid import hybrid_property
-from sqlalchemy.orm import validates
-from sqlalchemy.orm.base import NO_VALUE
-from sqlalchemy import event
-
-from investing_algorithm_framework.core.exceptions import OperationalException
-from investing_algorithm_framework.core.models import db, OrderType, \
-    OrderStatus
-from investing_algorithm_framework.core.models.model_extension \
-    import ModelExtension
-from .order_side import OrderSide
+from investing_algorithm_framework.domain import OperationalException, \
+    OHLCV, AssetPrice, Order
 
 logger = logging.getLogger(__name__)
 
 
-def random_id():
-    """
-    Function to create a random ID. This function checks first if
-    the generated ID is not already taken.
-    Returns: random integer that can be used as an ID
-    """
-    minimal = 100
-    maximal = 1000000000000000000
-    rand = randint(minimal, maximal)
-
-    while Order.query.filter_by(id=rand).first() is not None:
-        rand = randint(minimal, maximal)
-
-    return rand
-
-
-class Order(db.Model, ModelExtension):
-    """
-        Class AlgorithmOrder: a database model for an AlgorithmOrder instance.
-
-        Attributes:
-        An AlgorithmOrder instance consists out of the following attributes:
-
-        - id: unique identification also used externally
-        - target_symbol: the target asset symbol of the order
-        - trading_symbol: the asset that is traded for the target symbol
-        - order side: the side of the order, e.g. BUY or SELL
-        - order type: the order type, e.g LIMIT.
-
-        The following attributes are OPTIONAL:
-
-        - price: the price of the target symbol (in trading symbol currency)
-        - amount: the amount of the target symbol
-
-        Updated post-execution:
-
-        for all child orders
-        - completed_at: DateTime the order was marked as completed
-
-        Relations:
-
-        - position: relation to the AlgorithmPosition instances
-        of users subscribed to the algorithm
-        """
-
-    __tablename__ = "orders"
-
-    # Integer id for the Order as the primary key
-    id = db.Column(
-        db.Integer,
-        primary_key=True,
-        unique=True,
-        default=random_id
-    )
-    order_reference = db.Column(db.Integer)
-    target_symbol = db.Column(db.String)
-    trading_symbol = db.Column(db.String)
-
-    order_side = db.Column(
-        db.String,
-        nullable=False,
-        default=OrderSide.BUY.value
-    )
-    order_type = db.Column(
-        db.String,
-        nullable=False,
-        default=OrderType.LIMIT.value
-    )
-
-    # The price and amount of the asset
-    price = db.Column(db.Float)
-    closing_price = db.Column(db.Float)
-    amount = db.Column(db.Float)
-    amount_trading_symbol = db.Column(db.Float)
-    status = db.Column(db.String)
-
-    position_id = db.Column(
-        db.Integer, db.ForeignKey('positions.id')
-    )
-    position = db.relationship("Position", back_populates="orders")
-
-    # Standard date time attributes
-    created_at = db.Column(db.DateTime, default=datetime.utcnow)
-    updated_at = db.Column(
-        db.DateTime,
-        default=datetime.utcnow,
-        onupdate=datetime.utcnow
-    )
-
-    # Post execution
-    executed_at = db.Column(db.DateTime)
-
-    def __init__(
-            self,
-            order_side,
-            order_type,
-            target_symbol,
-            trading_symbol,
-            price,
-            amount=None,
-            amount_trading_symbol=None,
-            **kwargs
-    ):
-        self.order_side = OrderSide.from_string(order_side).value
-        self.order_type = OrderType.from_string(order_type).value
-        self.target_symbol = target_symbol
-        self.trading_symbol = trading_symbol
-        self.price = price
-        self.amount = amount
-        self.amount_trading_symbol = amount_trading_symbol
-        self.open = True
-        self.status = None
-
-        super(Order, self).__init__(**kwargs)
-
-    @validates(
-        'id',
-        'target_symbol',
-        'trading_symbol',
-        'order_side',
-        'order_type',
-        'price',
-    )
-    def _write_once(self, key, value):
-        existing = getattr(self, key)
+class MarketService:
+    exchange = None
+    _market = None
+    api_key = None,
+    secret_key = None
+    exchange_class = None
+    msec = 1000
+    minute = 60 * msec
+
+    @property
+    def market(self):
+        return self._market
 
-        if existing is not None:
-            raise ValueError("{} is write-once".format(key))
+    @market.setter
+    def market(self, value):
 
-        return value
+        if not isinstance(value, str):
+            raise OperationalException("Market must be a string")
 
-    @property
-    def current_price(self):
-        from investing_algorithm_framework import current_app
-        market_service = current_app.algorithm \
-            .get_market_service(self.position.portfolio.market)
+        self._market = value.lower()
+
+        if not hasattr(ccxt, self._market):
+            raise OperationalException(
+                f"No market service found for market id {self._market}"
+            )
 
-        current_price = self.price
+        self.exchange_class = getattr(ccxt, self._market)
+        self.exchange = self.exchange_class()
+
+    def initialize(self, portfolio_configuration):
+        self.api_key = portfolio_configuration.api_key
+        self.secret_key = portfolio_configuration.secret_key
+        self._market = portfolio_configuration.market
+
+        if not hasattr(ccxt, self.market):
+            raise OperationalException(
+                f"No market service found for market id {self.market}"
+            )
+
+        self.exchange_class = getattr(ccxt, self.market)
+
+        if self.exchange_class is None:
+            raise OperationalException(
+                f"No market service found for market id {self.market}"
+            )
+
+        if self.api_key is not None or self.secret_key is not None:
+            self.exchange = self.exchange_class({
+                'apiKey': self.api_key,
+                'secret': self.secret_key,
+            })
+        else:
+            self.exchange = self.exchange_class({})
+
+    def pair_exists(self, target_symbol: str, trading_symbol: str):
+
+        if not self.exchange.has['fetchTicker']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality pair_exists"
+            )
 
         try:
-            if OrderSide.SELL.equals(self.order_side):
-                current_price = market_service.get_price(
-                    self.trading_symbol, self.target_symbol
-                )
-            else:
-                current_price = market_service.get_price(
-                    self.target_symbol, self.trading_symbol
-                )
+            data = self.get_ticker(f"{target_symbol}/{trading_symbol}")
+            return "symbol" in data
+        except OperationalException:
+            return False
+
+    def get_ticker(self, symbol):
+
+        if not self.exchange.has['fetchTicker']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_ticker"
+            )
+
+        try:
+            return self.exchange.fetchTicker(symbol)
         except Exception as e:
-            logger.error(e)
-            return current_price
+            logger.exception(e)
+            raise OperationalException(
+                f"Could not retrieve ticker for symbol {symbol}"
+            )
 
-        return current_price
+    def get_tickers(self, symbols):
 
-    @hybrid_property
-    def delta(self):
+        if not self.exchange.has['fetchTickers']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_tickers"
+            )
 
-        # Delta is 0 if it is a sell order
-        if OrderSide.SELL.equals(self.order_side):
-            return 0
+        try:
+            return self.exchange.fetchTickers(symbols)
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException(
+                "Could not retrieve selection of tickers"
+            )
 
-        if self.closing_price:
-            return (self.closing_price * self.amount) - \
-                   (self.price * self.amount)
+    def get_order_book(self, symbol):
 
-        if not OrderStatus.SUCCESS.equals(self.status):
-            return 0
+        if not self.exchange.has['fetchOrderBook']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_order_book"
+            )
+
+        try:
+            return self.exchange.fetchOrderBook(symbol)
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not retrieve order book")
+
+    def get_order_books(self, symbols):
+        data = {}
+
+        for symbol in symbols:
+            try:
+                entry = self.get_order_book(symbol)
+                del entry['symbol']
+                data[symbol] = entry
+            except Exception as e:
+                logger.exception(e)
+
+        return data
+
+    def get_order(self, order):
+        symbol = f"{order.target_symbol.upper()}/" \
+                 f"{order.trading_symbol.upper()}"
+
+        if not self.exchange.has['fetchOrder']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_order"
+            )
+
+        try:
+            order = self.exchange.fetchOrder(order.external_id, symbol)
+            return Order.from_ccxt_order(order)
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not retrieve order")
 
-        price = self.current_price
+    def get_orders(self, symbol, since: datetime = None):
 
-        # With no price data_provider return 0
-        if price == -1:
-            return 0
+        if not self.exchange.has['fetchOrders']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_orders"
+            )
 
-        return (price * self.amount) - (self.price * self.amount)
+        if since is not None:
+            since = self.exchange.parse8601(
+                since.strftime(":%Y-%m-%d %H:%M:%S")
+            )
 
-    @hybrid_property
-    def percentage(self):
+            try:
+                ccxt_orders = self.exchange.fetchOrders(symbol, since=since)
+                return [Order.from_ccxt_order(order) for order in ccxt_orders]
+            except Exception as e:
+                logger.exception(e)
+                raise OperationalException("Could not retrieve orders")
+        else:
+            try:
+                ccxt_orders = self.exchange.fetchOrders(symbol)
+                return [Order.from_ccxt_order(order) for order in ccxt_orders]
+            except Exception as e:
+                logger.exception(e)
+                raise OperationalException("Could not retrieve orders")
 
-        if OrderSide.SELL.equals(self.order_side):
-            return 0
+    def get_balance(self):
 
-        if not OrderStatus.SUCCESS.equals(self.status):
-            return 0
+        if not self.exchange.has['fetchBalance']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_balance"
+            )
 
-        portfolio = self.position.portfolio
+        try:
+            return self.exchange.fetchBalance()
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not retrieve balance")
 
-        return (
-                       self.current_value /
-                       (portfolio.allocated + portfolio.unallocated)
-               ) * 100
+    def create_limit_buy_order(
+        self,
+        target_symbol: str,
+        trading_symbol: str,
+        amount: float,
+        price: float
+    ):
 
-    @hybrid_property
-    def percentage_position(self):
+        if not self.exchange.has['createLimitBuyOrder']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality create_limit_buy_order"
+            )
 
-        if OrderSide.SELL.equals(self.order_side):
-            return 0
+        symbol = f"{target_symbol.upper()}/{trading_symbol.upper()}"
 
-        if not OrderStatus.SUCCESS.equals(self.status):
-            return 0
+        try:
+            order = self.exchange.createLimitBuyOrder(
+                symbol, amount, price
+            )
+            return Order.from_ccxt_order(order)
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not create limit buy order")
 
-        return self.amount / self.position.amount * 100
+    def create_limit_sell_order(
+        self,
+        target_symbol: str,
+        trading_symbol: str,
+        amount: float,
+        price: float
+    ):
 
-    @hybrid_property
-    def percentage_realized(self):
+        if not self.exchange.has['createLimitSellOrder']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality create_limit_sell_order"
+            )
 
-        if OrderSide.SELL.equals(self.order_side):
-            return 0
+        symbol = f"{target_symbol.upper()}/{trading_symbol.upper()}"
 
-        if not OrderStatus.CLOSED.equals(self.status):
-            return 0
+        try:
+            order = self.exchange.createLimitSellOrder(
+                symbol, amount, price
+            )
+            return Order.from_ccxt_order(order)
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not create limit sell order")
 
-        portfolio = self.position.portfolio
+    def create_market_sell_order(
+        self,
+        target_symbol: str,
+        trading_symbol: str,
+        amount: float,
+    ):
 
-        return (self.amount * self.closing_price) / portfolio.realized * 100
+        if not self.exchange.has['createMarketSellOrder']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality create_market_sell_order"
+            )
 
-    @hybrid_property
-    def current_value(self):
+        symbol = f"{target_symbol.upper()}/{trading_symbol.upper()}"
 
-        # Current value is 0 if it is a sell order
-        if OrderSide.SELL.equals(self.order_side):
-            return 0
+        try:
+            order = self.exchange.createMarketSellOrder(symbol, amount)
+            return Order.from_ccxt_order(order)
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not create market sell order")
 
-        if self.status is None:
-            return self.price * self.amount
+    def cancel_order(self, order):
 
-        if OrderStatus.PENDING.equals(self.status):
-            return self.price * self.amount
+        if not self.exchange.has['cancelOrder']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality cancel_order"
+            )
 
-        if not OrderStatus.SUCCESS.equals(self.status):
-            return 0
+        self.exchange.cancelOrder(
+            order.get_order_reference(),
+            f"{order.get_target_symbol()}/{order.get_trading_symbol()}")
 
-        price = self.current_price
-        return price * self.amount
+    def get_open_orders(
+        self, target_symbol: str = None, trading_symbol: str = None
+    ):
 
-    def set_executed(self):
+        if not self.exchange.has['fetchOpenOrders']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_open_orders"
+            )
 
-        if not OrderStatus.PENDING.equals(self.status) and \
-                self.status is not None:
+        try:
+            if target_symbol is None or trading_symbol is None:
+                return self.exchange.fetchOpenOrders()
 
-            return
+            symbol = f"{target_symbol.upper()}/{trading_symbol.upper()}"
+            ccxt_orders = self.exchange.fetchOpenOrders(symbol)
+            return [Order.from_ccxt_order(order) for order in ccxt_orders]
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not retrieve open orders")
 
-        if OrderSide.BUY.equals(self.order_side):
-            self.status = OrderStatus.SUCCESS.value
-            self.executed_at = datetime.utcnow()
+    def get_closed_orders(
+        self, target_symbol: str = None, trading_symbol: str = None
+    ):
 
-            self.position.cost += self.amount * self.price
-            self.position.amount += self.amount
+        if not self.exchange.has['fetchClosedOrders']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_closed_orders"
+            )
 
-            if OrderType.MARKET.equals(self.order_type):
-                self.position.portfolio.unallocated -= \
-                    self.amount_trading_symbol
+        try:
+            if target_symbol is None or trading_symbol is None:
+                return self.exchange.fetchClosedOrders()
 
-        else:
-            self.status = OrderStatus.SUCCESS.value
-            self.executed_at = datetime.utcnow()
-            self.position.amount -= self.amount
-
-        db.session.commit()
-
-    def set_closed(self, sell_order):
-        self.status = OrderStatus.CLOSED.value
-        self.closing_price = sell_order.price
-        db.session.commit()
-
-    def set_pending(self):
-        self.status = OrderStatus.PENDING.value
-        db.session.commit()
-
-    def update(self, db, data, commit=True, **kwargs):
-        self.updated_at = datetime.utcnow()
-        super(Order, self).update(db, data, commit, **kwargs)
-
-    def copy(self, amount=None):
-
-        if amount is None:
-            amount = self.amount
-
-        order = Order(
-            amount=amount,
-            price=self.price,
-            order_side=self.order_side,
-            order_type=self.order_type,
-            target_symbol=self.target_symbol,
-            trading_symbol=self.trading_symbol
-        )
+            symbol = f"{target_symbol.upper()}/{trading_symbol.upper()}"
+            ccxt_orders = self.exchange.fetchClosedOrders(symbol)
+            return [Order.from_ccxt_order(order) for order in ccxt_orders]
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not retrieve closed orders")
 
-        order.order_reference = self.order_reference
-        order.status = self.status
-        order.amount_trading_symbol = order.amount_trading_symbol
-        order.executed_at = self.executed_at
-        order.updated_at = self.updated_at
-        order.created_at = self.created_at
-        order.closing_price = self.closing_price
+    def get_prices(self, symbols):
+        asset_prices = []
 
-        return order
+        try:
+            tickers = self.exchange.fetchTickers(symbols)
+            for ticker in tickers:
+                asset_prices.append(
+                    AssetPrice(
+                        tickers[ticker]["symbol"],
+                        tickers[ticker]["ask"],
+                        tickers[ticker]["datetime"]
+                    )
+                )
 
-    def split(self, amount):
+            return asset_prices
+        except Exception as e:
+            logger.exception(e)
+            raise OperationalException("Could not retrieve prices")
 
-        if not OrderSide.BUY.equals(self.order_side):
-            raise OperationalException("Sell order can't be split")
+    def get_ohclv(self, symbol, time_unit, since):
 
-        if not OrderStatus.SUCCESS.equals(self.status):
-            raise OperationalException("Order can't be split")
+        if not self.exchange.has['fetchOHLCV']:
+            raise OperationalException(
+                f"Market service {self.market} does not support "
+                f"functionality get_ohclvs"
+            )
 
-        if amount <= 0 or amount >= self.amount:
-            raise OperationalException("Split amount has a wrong value")
+        from_timestamp = self.exchange.parse8601(
+            since.strftime(":%Y-%m-%d %H:%M:%S")
+        )
+        now = self.exchange.milliseconds()
+        data = []
 
-        algorithm_order = self.copy(amount=amount)
-        self.amount = self.amount - amount
-        self.position.orders.append(algorithm_order)
-        db.session.commit()
+        while from_timestamp < now:
+            ohlcv = self.exchange.fetch_ohlcv(
+                symbol, time_unit, from_timestamp
+            )
+            sleep(self.exchange.rateLimit / 1000)
+            from_timestamp = \
+                ohlcv[-1][0] + self.exchange.parse_timeframe(time_unit) * 1000
+            ohlcv = [[self.exchange.iso8601(candle[0])] + candle[1:] for candle
+                     in ohlcv]
+            data += ohlcv
 
-        return self, algorithm_order
+        return OHLCV.from_dict({"symbol": symbol, "data": data})
 
-    def save(self, db, commit=True):
+    def get_ohclvs(self, symbols, time_frame, from_timestamp):
 
-        if self.position is None:
+        if not self.exchange.has['fetchOHLCV']:
             raise OperationalException(
-                "Can't save order that is not linked to an position"
+                f"Market service {self.market} does not support "
+                f"functionality get_ohclvs"
             )
 
-        super(Order, self).save(db, commit)
+        now = self.exchange.milliseconds()
+        ohlcvs = {}
 
-    def __repr__(self):
-        return self.repr(
-            id=self.id,
-            status=self.status,
-            order_side=self.order_side,
-            target_symbol=self.target_symbol,
-            trading_symbol=self.trading_symbol,
-            amount=self.amount,
-            amount_trading_symbol=self.amount_trading_symbol,
-            price=self.price,
-            created_at=self.created_at,
-        )
+        for symbol in symbols:
+
+            try:
+                time_stamp = self.exchange.parse8601(
+                    from_timestamp.strftime(":%Y-%m-%d %H:%M:%S")
+                )
+                dfs = []
+
+                while time_stamp < now:
 
+                    ohlcv = self.exchange.fetch_ohlcv(
+                        symbol, time_frame.to_ccxt_string(), time_stamp
+                    )
+                    sleep(self.exchange.rateLimit / 1000)
+                    time_stamp = \
+                        ohlcv[-1][0] + \
+                        self.exchange.parse_timeframe(
+                            time_frame.to_ccxt_string()
+                        ) * 1000
+
+                    ohlcv = [[self.exchange.iso8601(candle[0])]
+                             + candle[1:] for candle in ohlcv]
+                    df = pd.DataFrame(ohlcv,
+                                      columns=['timestamp', 'open', 'high',
+                                               'low', 'close', 'volume'])
+                    df['timestamp'] = df['timestamp'].apply(lambda x: parse(x))
+                    df['timestamp'] = pd.to_datetime(
+                        df['timestamp'], unit='ms'
+                    )
+                    df.set_index('timestamp', inplace=True)
+                    dfs.append(df)
+
+                combined_df = pd.concat(dfs, axis=0)
+                ohlcvs[symbol] = combined_df
+            except Exception as e:
+                logger.exception(e)
+                logger.error(f"Could not retrieve ohclv data for {symbol}")
 
-@event.listens_for(Order.status, "set")
-def sync_portfolio_and_position(target, value, old_value, initiator):
-    if old_value is NO_VALUE:
-        return
-
-    if OrderSide.SELL.equals(target.order_side):
-
-        if (old_value is None or OrderStatus.PENDING.equals(old_value)) and \
-                OrderStatus.SUCCESS.equals(value):
-
-            sell_amount = target.amount
-
-            # Close open buy orders
-            buy_orders = target.position.orders \
-                .filter_by(order_side=OrderSide.BUY.value) \
-                .filter_by(status=OrderStatus.SUCCESS.value) \
-                .order_by(Order.created_at) \
-                .all()
-
-            closed_orders = []
-            index = 0
-
-            while sell_amount != 0:
-                buy_order = buy_orders[index]
-
-                if buy_order.amount <= sell_amount:
-                    sell_amount -= buy_order.amount
-                    buy_order.set_closed(target)
-                    closed_orders.append(buy_order)
-                else:
-                    remainder = buy_order.amount - sell_amount
-                    og, split = buy_order.split(remainder)
-                    og.set_closed(target)
-                    closed_orders.append(og)
-                    sell_amount = 0
-
-                index += 1
-
-            portfolio = target.position.portfolio
-            position = target.position
-
-            unallocated = 0
-            realized = 0
-            cost = 0
-
-            for closed_order in closed_orders:
-                unallocated += closed_order.current_value
-                realized += closed_order.delta
-                cost += closed_order.amount * closed_order.price
-
-            position.cost -= cost
-            portfolio.unallocated += unallocated
-            portfolio.realized += realized
-            db.session.commit()
+        return ohlcvs
```

### Comparing `investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/order_side.py` & `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,26 @@
 
         if isinstance(value, str):
             for order_type in OrderSide:
 
                 if value.upper() == order_type.value:
                     return order_type
 
-        raise ValueError("Could not convert value to OrderSide")
+        raise ValueError(f"Could not convert value {value} to OrderSide")
+
+    @staticmethod
+    def from_value(value):
+
+        if isinstance(value, OrderSide):
+            for order_side in OrderSide:
+
+                if value == order_side:
+                    return order_side
+
+        return OrderSide.from_string(value)
 
     def equals(self, other):
 
         if isinstance(other, Enum):
             return self.value == other.value
 
         else:
```

### Comparing `investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/order_type.py` & `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from enum import Enum
 
 
 class OrderType(Enum):
     LIMIT = 'LIMIT'
     MARKET = 'MARKET'
+    STOP_LOSS_LIMIT = "STOP_LOSS_LIMIT"
 
     @staticmethod
     def from_string(value: str):
 
         if isinstance(value, str):
             for order_type in OrderType:
 
                 if value.upper() == order_type.value:
                     return order_type
 
         raise ValueError("Could not convert value to OrderType")
 
-    def equals(self, other):
+    @staticmethod
+    def from_value(value):
 
-        if isinstance(other, Enum):
-            return self.value == other.value
+        if isinstance(value, OrderType):
+            for order_type in OrderType:
 
-        else:
-            return OrderType.from_string(other) == self
+                if value == order_type:
+                    return order_type
+
+        return OrderType.from_string(value)
+
+    def equals(self, other):
+        return OrderType.from_value(other) == self
```

### Comparing `investing_algorithm_framework-0.9/investing_algorithm_framework/core/models/time_unit.py` & `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 from enum import Enum
 
 
 class TimeUnit(Enum):
-    SECONDS = "SECONDS"
+    SECOND = "SECOND"
     MINUTE = "MINUTE"
     HOUR = "HOUR"
 
     @staticmethod
     def from_string(value: str):
 
         if isinstance(value, str):
 
             for entry in TimeUnit:
 
                 if value.upper() == entry.value:
                     return entry
 
         raise ValueError(
-            "Could not convert value to time unit"
+            f"Could not convert value {value} to time unit"
         )
 
     def equals(self, other):
 
         if isinstance(other, Enum):
             return self.value == other.value
         else:
             return TimeUnit.from_string(other) == self
+
+    @staticmethod
+    def from_value(value):
+
+        if isinstance(value, TimeUnit):
+
+            for entry in TimeUnit:
+
+                if entry == value:
+                    return entry
+
+        return TimeUnit.from_string(value)
```

### Comparing `investing_algorithm_framework-0.9/investing_algorithm_framework/utils/csv.py` & `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import csv
 import shutil
 import tempfile
 from typing import Dict, List
 
-from investing_algorithm_framework.core.exceptions import OperationalException
+from ..exceptions import OperationalException
 
 
 # Function to add column headers to csv
 def add_column_headers_to_csv(file_name: str, column_names: List[str]) -> None:
 
     # Open file in append mode
     with open(file_name, 'a+', newline='') as write_obj:
```

### Comparing `investing_algorithm_framework-0.9/investing_algorithm_framework.egg-info/PKG-INFO` & `investing_algorithm_framework-1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,159 @@
 Metadata-Version: 2.1
-Name: investing-algorithm-framework
-Version: 0.9
+Name: investing_algorithm_framework
+Version: 1.0
 Summary: A framework for creating an investment algorithm
 Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
+Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
 Author: coding kitties
 License: Apache License 2.0
-Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
-Description: [![Build](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml)
-        [![Tests](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml)
-        [![Downloads](https://pepy.tech/badge/investing-algorithm-framework)](https://pepy.tech/badge/investing-algorithm-framework)
-        [![Current Version](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)
-        
-        # Investing Algorithm Framework
-        
-        > :warning: **Documentation outdated**: We are working hard on releasing v1.0.0. After 
-        > this release we will update the documentation at the website.
-        
-        The Investing Algorithm Framework is a python framework for building
-        investment algorithms. It encourages rapid development and clean, pragmatic code design.
-        
-        The framework provides you with an all the components you need to create an 
-        investing algorithm (data providing, portfolio management, order execution, etc..). 
-        Also, the algorithm can be controlled with a REST Api that will run in the background.
-        
-        
-        ## Example Algorithm for Binance
-        ```python
-        import os
-        
-        from investing_algorithm_framework import App, TimeUnit, AlgorithmContext, \
-            TradingDataTypes
-        from investing_algorithm_framework.configuration.constants import BINANCE, \
-            BINANCE_API_KEY, BINANCE_SECRET_KEY, TRADING_SYMBOL
-        
-        BTC_SYMBOL = "BTC"
-        
-        # Our trading symbol (e.g. dot/usdt, sol/usdt)
-        USDT_SYMBOL = "USDT"
-        
-        # Make the parent dir your resources directory (database, csv storage)
-        dir_path = os.path.abspath(os.path.join(os.path.realpath(__file__), os.pardir))
-        
-        # Create an application (setups your algorithm, database, rest api, etc...)
-        app = App(
-            resources_directory=dir_path,
-            config={
-                BINANCE_API_KEY: "<BINANCE_API_KEY>",
-                BINANCE_SECRET_KEY: "<BINANCE_SECRET_KEY>",
-                TRADING_SYMBOL: USDT_SYMBOL,
-            }
-        )
-        
-        
-        # Algorithm strategy that runs every 5 minutes
-        @app.algorithm.schedule(time_unit=TimeUnit.MINUTE, interval=5)
-        def perform_strategy(context: AlgorithmContext):
-            # Get ticker data from binance
-            ticker = context.get_data(
-                BINANCE,
-                trading_data_type=TradingDataTypes.TICKER,
-                target_symbol=BTC_SYMBOL,
-            )
-        
-            if ticker.ask_price > 50000:
-                # Execute a market order on binance
-                context.create_market_buy_order(
-                    BINANCE, BTC_SYMBOL, amount_trading_symbol=10, execute=True
-                )
-        
-        
-        if __name__ == "__main__":
-            app.start()
-        ```
-        The goal of the framework is to provide you with a set of components for 
-        your algorithm that takes care of a wide variety of operational processes 
-        out of the box.
-        
-        * Data providing
-        * Order execution
-        * Portfolio management
-        * Performance tracking
-        * Strategy scheduling
-        * Resource management
-        * Model snapshots
-        * Order status management
-        * Clients (Rest API)
-        
-        However, we aim to also provide a modular framework where you can write your
-        own components or use third party plugins for the framework.
-        
-        Further information and the complete documentation can be found at the [webstie](https://investing-algorithm-framework.com)
-        
-        
-        ## Download
-        You can download the framework with pypi.
-        
-        ```bash
-        pip install investing-algorithm-framework
-        ```
-        
-        #### Disclaimer
-        If you use this framework for your investments, do not risk money 
-        which you are afraid to lose, until you have clear understanding how 
-        the framework works. We can't stress this enough:
-        
-        BEFORE YOU START USING MONEY WITH THE FRAMEWORK, MAKE SURE THAT YOU TESTED 
-        YOUR COMPONENTS THOROUGHLY. USE THE SOFTWARE AT YOUR OWN RISK. 
-        THE AUTHORS AND ALL AFFILIATES ASSUME NO RESPONSIBILITY FOR YOUR INVESTMENT RESULTS.
-        
-        Also, make sure that you read the source code of any plugin you use or 
-        implementation of an algorithm made with this framework.
-        
-        For further information regarding usage and licensing we recommend going 
-        to the licensing page at the website.
-        
-        ## Documentation
-        
-        All the documentation can be found online at the [documentation webstie](https://investing-algorithm-framework.com)
-        
-        In most cases, you'll probably never have to change code on this repo directly 
-        if you are building your algorithm/bot. But if you do, check out the 
-        contributing page at the website.
-        
-        If you'd like to chat with investing-algorithm-framework users 
-        and developers, [join us on Slack](https://inv-algo-framework.slack.com) or [join us on reddit](https://www.reddit.com/r/InvestingAlgorithms/)
-        
-        ## Acknowledgements
-        We want to thank all contributors to this project. A full list of all 
-        the people that contributed to the project can be
-        found [here](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/docs/AUTHORS.md)
-        
-        ### Help / Slack
-        
-        For any questions not covered by the documentation or for further
-        information about the framework, we encourage you to join our slack channel.
-        
-        [join us on Slack](https://inv-algo-framework.slack.com)
-        
-        ### [Bugs / Issues](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
-        
-        If you discover a bug in the framework, please [search our issue tracker](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
-        first. If it hasn't been reported, please [create a new issue](https://github.com/investing-algorithms/investing-algorithm-framework/issues/new).
-        
-        Feel like the framework is missing a feature? We welcome your pull requests!
-        
-        Please read our [Contributing document](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/docs/CONTRIBUTING.md)
-        to understand the requirements before sending your pull-requests.
-        
-        **Note** before starting any major new feature work, *please open an issue describing what you are planning to do* or talk to us on [Slack](https://join.slack.com/t/investingbots/shared_invite/enQtODgwNTg3MzA2MjYyLTdiZjczZDRlNWJjNDdmYThiMGE0MzFhOTg4Y2E0NzQ2OTgxYjA1NzU3ZWJiY2JhOTE1ZGJlZGFiNDU3OTAzMDg).
-        This will ensure that interested parties can give valuable feedback on the feature, and let others know that you are working on it.
-        
-        **Important:** Always create your feature or hotfix against the `develop` branch, not `master`.
-        
-Keywords: INVESTING,BOT,ALGORITHM,FRAMEWORK
-Platform: UNKNOWN
+Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+<a href=https://investing-algorithm-framework.com><img src="https://img.shields.io/badge/docs-website-brightgreen"></a>
+[![Build](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml)
+[![Tests](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml)
+[![Downloads](https://pepy.tech/badge/investing-algorithm-framework)](https://pepy.tech/badge/investing-algorithm-framework)
+[![Current Version](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)
+<a href="https://www.reddit.com/r/InvestingBots/"><img src="https://img.shields.io/reddit/subreddit-subscribers/investingbots?style=social"></a>
+###### Sponsors
+<p align="left">
+<a href="https://logicfunds.io">
+  <img alt="logicfunds" src="https://logicfunds-web-app-images.s3.eu-central-1.amazonaws.com/logicfunds-logo.png" width="200px" />
+</a>
+</p>
+
+# Investing Algorithm Framework
+The Investing Algorithm Framework is a python framework for building
+investment algorithms. It encourages rapid development and clean, pragmatic code design.
+
+The framework provides you with all the components you need to create an 
+investing algorithm (data providing, portfolio management, order execution, etc..). Also,
+it has various deployment options, such as web server, stateless, etc..
+
+## Example
+The following algorithm connects to binance and buys BTC every 5 seconds. 
+It also exposes an REST API that allows you to interact with the algorithm.
+```python
+import pathlib
+from datetime import datetime, timedelta
+
+from investing_algorithm_framework import create_app, PortfolioConfiguration, \
+    RESOURCE_DIRECTORY, TimeUnit, TradingTimeFrame, TradingDataType, OrderSide
+
+app = create_app({RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()})
+app.add_portfolio_configuration(
+    PortfolioConfiguration(
+        market="binance",
+        api_key="xxxxxx",
+        secret_key="xxxxxx",
+        trading_symbol="USDT"
+    )
+)
+
+
+@app.strategy(
+    time_unit=TimeUnit.SECOND, # Algorithm will be executed every 5 seconds
+    interval=5,
+    market="binance", # Will retrieve trading data from binance
+    symbols=["BTC/USDT", "ETH/USDT", ["DOT/USDT"]], # Symbols must be in the format of TARGET/TRADE symbol (e.g. BTC/USDT)
+    trading_data_types=[TradingDataType.OHLCV, TradingDataType.TICKER, TradingDataType.ORDER_BOOK],
+    trading_time_frame_start_date=datetime.utcnow() - timedelta(days=1), # Will retrieve data from the last 24 hours
+    trading_time_frame=TradingTimeFrame.ONE_MINUTE # Will retrieve data on 1m interval (OHLCV)
+)
+def perform_strategy(algorithm, market_data):
+    print(algorithm.get_allocated())
+    print(algorithm.get_unallocated())
+    print(market_data)
+    algorithm.create_limit_order(
+        target_symbol="BTC", 
+        side=OrderSide.BUY,
+        price=market_data["TICKER"]["BTC/USDT"]["BID"], 
+        amount_target_symbol=0.00001
+    )
+
+
+if __name__ == "__main__":
+    app.run()
+```
+
+> You can find more examples [here](./examples) folder.
+
+## Broker/Exchange configuration
+The framework has by default support for [ccxt](https://github.com/ccxt/ccxt).
+This should allow you to connect to a lot of brokers/exchanges.
+
+```python
+from investing_algorithm_framework import App, PortfolioConfiguration
+app = App()
+app.add_portfolio_configuration(
+    PortfolioConfiguration(
+        market="bitvavo", 
+        api_key="xxxx", 
+        secret_key="xxxx", 
+        track_from="01/01/2022",
+        trading_symbol="EUR"
+    )
+)
+```
+
+## Download
+You can download the framework with pypi.
+
+```bash
+pip install investing-algorithm-framework
+```
+
+## Disclaimer
+If you use this framework for your investments, do not risk money 
+which you are afraid to lose, until you have clear understanding how 
+the framework works. We can't stress this enough:
+
+BEFORE YOU START USING MONEY WITH THE FRAMEWORK, MAKE SURE THAT YOU TESTED 
+YOUR COMPONENTS THOROUGHLY. USE THE SOFTWARE AT YOUR OWN RISK. 
+THE AUTHORS AND ALL AFFILIATES ASSUME NO RESPONSIBILITY FOR YOUR INVESTMENT RESULTS.
+
+Also, make sure that you read the source code of any plugin you use or 
+implementation of an algorithm made with this framework.
+
+For further information regarding usage and licensing we recommend going 
+to the licensing page at the website.
+
+## Documentation
+
+All the documentation can be found online 
+at the [documentation webstie](https://investing-algorithm-framework.com)
+
+In most cases, you'll probably never have to change code on this repo directly 
+if you are building your algorithm/bot. But if you do, check out the 
+contributing page at the website.
+
+If you'd like to chat with investing-algorithm-framework users 
+and developers, [join us on Slack](https://inv-algo-framework.slack.com) or [join us on reddit](https://www.reddit.com/r/InvestingBots/)
+
+## Acknowledgements
+We want to thank all contributors to this project. A full list of all 
+the people that contributed to the project can be
+found [here](https://github.com/investing-algorithms/investing-algorithm-framework/blob/master/AUTHORS.md)
+
+### [Bugs / Issues](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
+
+If you discover a bug in the framework, please [search our issue tracker](https://github.com/investing-algorithms/investing-algorithm-framework/issues?q=is%3Aissue)
+first. If it hasn't been reported, please [create a new issue](https://github.com/investing-algorithms/investing-algorithm-framework/issues/new).
+
+Feel like the framework is missing a feature? We welcome your pull requests!
+
+**Note** before starting any major new feature work, *please open an issue describing what you are planning to do*.
+This will ensure that interested parties can give valuable feedback on the feature, and let others know that you are working on it.
+
+**Important:** Always create your feature or hotfix against the `develop` branch, not `master`.
```

### Comparing `investing_algorithm_framework-0.9/setup.py` & `investing_algorithm_framework-1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-from investing_algorithm_framework import get_version
+from version import get_version
 
 VERSION = get_version()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open('requirements.txt') as f:
@@ -15,16 +15,18 @@
     license='Apache License 2.0',
     author="coding kitties",
     description="A framework for creating an investment algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/coding-kitties/investing-algorithm-framework.git",
     download_url='https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz',
-    packages=setuptools.find_packages(exclude=['tests', 'tests.*']),
-    keywords=['INVESTING', 'BOT', 'ALGORITHM', 'FRAMEWORK'],
+    packages=setuptools.find_packages(
+        exclude=['tests', 'tests.*', 'examples', 'examples.*']
+    ),
+    keywords=['TRADING', 'INVESTING', 'BOT', 'ALGORITHM', 'FRAMEWORK'],
     classifiers=[
         "Intended Audience :: Developers",
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         "Topic :: Software Development",
```


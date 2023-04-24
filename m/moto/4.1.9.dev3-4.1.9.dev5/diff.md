# Comparing `tmp/moto-4.1.9.dev3.tar.gz` & `tmp/moto-4.1.9.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moto-4.1.9.dev3.tar", last modified: Mon Apr 24 13:32:01 2023, max compression
+gzip compressed data, was "moto-4.1.9.dev5.tar", last modified: Mon Apr 24 13:34:35 2023, max compression
```

## Comparing `moto-4.1.9.dev3.tar` & `moto-4.1.9.dev5.tar`

### file list

```diff
@@ -1,2078 +1,2078 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:01.000597 moto-4.1.9.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-24 13:32:01.000597 moto-4.1.9.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.528596 moto-4.1.9.dev3/moto/
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-24 13:31:53.000000 moto-4.1.9.dev3/moto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.532596 moto-4.1.9.dev3/moto/acm/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acm/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acm/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acm/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.532596 moto-4.1.9.dev3/moto/acmpca/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acmpca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acmpca/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acmpca/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acmpca/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/acmpca/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.536596 moto-4.1.9.dev3/moto/amp/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/amp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/amp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/amp/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/amp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/amp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.536596 moto-4.1.9.dev3/moto/apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.536596 moto-4.1.9.dev3/moto/apigateway/integration_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/integration_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/integration_parsers/aws_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/integration_parsers/http_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/integration_parsers/unknown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    91751 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigateway/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.536596 moto-4.1.9.dev3/moto/apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigatewayv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    64715 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigatewayv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    36307 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigatewayv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/apigatewayv2/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.540596 moto-4.1.9.dev3/moto/applicationautoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/applicationautoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/applicationautoscaling/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/applicationautoscaling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/applicationautoscaling/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/applicationautoscaling/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/applicationautoscaling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.540596 moto-4.1.9.dev3/moto/appsync/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/appsync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/appsync/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/appsync/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/appsync/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.540596 moto-4.1.9.dev3/moto/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/athena/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/athena/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/athena/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/athena/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.544596 moto-4.1.9.dev3/moto/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/autoscaling/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    61357 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/autoscaling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    65472 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/autoscaling/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/autoscaling/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.544596 moto-4.1.9.dev3/moto/awslambda/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/awslambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/awslambda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    74928 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/awslambda/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/awslambda/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/awslambda/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/awslambda/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/awslambda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/backend_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.548596 moto-4.1.9.dev3/moto/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    69404 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.548596 moto-4.1.9.dev3/moto/batch_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch_simple/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch_simple/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/batch_simple/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.548596 moto-4.1.9.dev3/moto/budgets/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/budgets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/budgets/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/budgets/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/budgets/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.548596 moto-4.1.9.dev3/moto/ce/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ce/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ce/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ce/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ce/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.552596 moto-4.1.9.dev3/moto/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudformation/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudformation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudformation/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    37709 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudformation/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    53038 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudformation/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudformation/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudformation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.552596 moto-4.1.9.dev3/moto/cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudfront/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudfront/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudfront/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudfront/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.552596 moto-4.1.9.dev3/moto/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudtrail/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudtrail/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudtrail/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudtrail/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.556596 moto-4.1.9.dev3/moto/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudwatch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33739 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudwatch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudwatch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudwatch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cloudwatch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.556596 moto-4.1.9.dev3/moto/codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codebuild/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codebuild/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codebuild/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codebuild/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.556596 moto-4.1.9.dev3/moto/codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codecommit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codecommit/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codecommit/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codecommit/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.556596 moto-4.1.9.dev3/moto/codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codepipeline/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codepipeline/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codepipeline/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/codepipeline/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.560596 moto-4.1.9.dev3/moto/cognitoidentity/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidentity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidentity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidentity/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidentity/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidentity/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidentity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.560596 moto-4.1.9.dev3/moto/cognitoidp/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    83922 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.560596 moto-4.1.9.dev3/moto/cognitoidp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidp/resources/jwks-private.json
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidp/resources/jwks-public.json
--rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidp/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/cognitoidp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.560596 moto-4.1.9.dev3/moto/comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/comprehend/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/comprehend/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/comprehend/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/comprehend/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.560596 moto-4.1.9.dev3/moto/config/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    81665 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/config/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.564596 moto-4.1.9.dev3/moto/config/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   117575 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/config/resources/aws_managed_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/config/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/config/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.564596 moto-4.1.9.dev3/moto/core/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/botocore_stubber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/common_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/custom_responses_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/model_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40468 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/responses_custom_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.564596 moto-4.1.9.dev3/moto/databrew/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/databrew/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25372 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/databrew/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19227 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/databrew/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/databrew/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.568596 moto-4.1.9.dev3/moto/datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datapipeline/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datapipeline/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datapipeline/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datapipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.568596 moto-4.1.9.dev3/moto/datasync/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datasync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datasync/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datasync/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/datasync/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.568596 moto-4.1.9.dev3/moto/dax/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dax/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dax/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dax/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dax/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.572596 moto-4.1.9.dev3/moto/dms/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dms/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dms/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.572596 moto-4.1.9.dev3/moto/ds/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ds/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ds/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ds/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ds/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ds/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ds/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.576596 moto-4.1.9.dev3/moto/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42639 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/limits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.576596 moto-4.1.9.dev3/moto/dynamodb/models/
--rw-r--r--   0 runner    (1001) docker     (123)    33457 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17443 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/models/dynamo_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    39809 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/models/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/models/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.580596 moto-4.1.9.dev3/moto/dynamodb/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/ast_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    34656 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/key_condition_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/partiql.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/reserved_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/reserved_keywords.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/parsing/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    45017 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.580596 moto-4.1.9.dev3/moto/dynamodb_v20111205/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb_v20111205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb_v20111205/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb_v20111205/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb_v20111205/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodb_v20111205/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.580596 moto-4.1.9.dev3/moto/dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodbstreams/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodbstreams/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/dynamodbstreams/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.584596 moto-4.1.9.dev3/moto/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ebs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ebs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ebs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.584596 moto-4.1.9.dev3/moto/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.596596 moto-4.1.9.dev3/moto/ec2/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/amis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/iam_instance_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/managed_prefixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/nat_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/spot_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/transit_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/transit_gateway_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/transit_gateway_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/vpc_peering_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/vpn_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/models/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.596596 moto-4.1.9.dev3/moto/ec2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/amis.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.492596 moto-4.1.9.dev3/moto/ec2/resources/ecs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.612596 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/
--rw-r--r--   0 runner    (1001) docker     (123)   110385 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   184754 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   205924 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    76970 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   233439 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   224300 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   204442 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   236846 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   196475 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   151250 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   205418 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   205543 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   170773 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   216660 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   244124 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   219056 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   243613 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.496596 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.624596 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/
--rw-r--r--   0 runner    (1001) docker     (123)    40620 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    38329 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   112314 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    79281 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    42533 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    73186 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   100264 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   100490 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    31415 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    64924 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   102387 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23689 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    51746 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   121670 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    71490 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    58608 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    65537 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   200128 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   112258 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   147926 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.636596 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/
--rw-r--r--   0 runner    (1001) docker     (123)    38820 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37177 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   102960 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    72651 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    38975 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    69946 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    91900 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    92102 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    28787 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    60279 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    95067 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    50561 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    49457 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   118040 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    69350 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    56856 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    36936 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    63575 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   194154 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   108910 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    47322 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   143512 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.644596 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    40058 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    36191 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    34296 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    35491 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    40817 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    41887 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37998 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    41546 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/us-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)  1306310 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/instance_types.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.652596 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/resources/latest_amis/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.664596 moto-4.1.9.dev3/moto/ec2/responses/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/account_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/egress_only_internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/iam_instance_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/nat_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/reserved_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/spot_fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/spot_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/transit_gateway_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/transit_gateway_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/transit_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/virtual_private_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/vpc_peering_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    39221 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/responses/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    28837 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.664596 moto-4.1.9.dev3/moto/ec2instanceconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2instanceconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2instanceconnect/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2instanceconnect/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ec2instanceconnect/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.664596 moto-4.1.9.dev3/moto/ecr/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecr/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecr/policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecr/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecr/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.668596 moto-4.1.9.dev3/moto/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    86640 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ecs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.668596 moto-4.1.9.dev3/moto/efs/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/efs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26760 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/efs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/efs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/efs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.668596 moto-4.1.9.dev3/moto/eks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/eks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30391 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/eks/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/eks/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/eks/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/eks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.672596 moto-4.1.9.dev3/moto/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticache/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticache/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticache/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.672596 moto-4.1.9.dev3/moto/elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticbeanstalk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticbeanstalk/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    57275 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticbeanstalk/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticbeanstalk/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elasticbeanstalk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.672596 moto-4.1.9.dev3/moto/elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elastictranscoder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elastictranscoder/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elastictranscoder/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.676596 moto-4.1.9.dev3/moto/elb/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elb/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.676596 moto-4.1.9.dev3/moto/elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elbv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    70076 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elbv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    68565 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elbv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elbv2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/elbv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.676596 moto-4.1.9.dev3/moto/emr/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emr/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    65244 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emr/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emr/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.680596 moto-4.1.9.dev3/moto/emrcontainers/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrcontainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrcontainers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrcontainers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrcontainers/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrcontainers/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrcontainers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.680596 moto-4.1.9.dev3/moto/emrserverless/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrserverless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrserverless/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrserverless/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrserverless/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/emrserverless/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.680596 moto-4.1.9.dev3/moto/es/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/es/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/es/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/es/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/es/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.684596 moto-4.1.9.dev3/moto/events/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    66807 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/events/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/events/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/events/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.684596 moto-4.1.9.dev3/moto/firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/firehose/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29565 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/firehose/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/firehose/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/firehose/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.684596 moto-4.1.9.dev3/moto/forecast/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/forecast/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/forecast/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/forecast/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/forecast/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.688596 moto-4.1.9.dev3/moto/glacier/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glacier/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glacier/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glacier/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glacier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.688596 moto-4.1.9.dev3/moto/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glue/glue_schema_registry_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glue/glue_schema_registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glue/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22412 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glue/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/glue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.692596 moto-4.1.9.dev3/moto/greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/greengrass/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    54499 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/greengrass/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30895 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/greengrass/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/greengrass/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.692596 moto-4.1.9.dev3/moto/guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/guardduty/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/guardduty/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/guardduty/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/guardduty/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.696596 moto-4.1.9.dev3/moto/iam/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)  1599363 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/aws_managed_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   118618 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)   107097 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.696596 moto-4.1.9.dev3/moto/identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/identitystore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/identitystore/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/identitystore/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/identitystore/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.700596 moto-4.1.9.dev3/moto/instance_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/instance_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/instance_metadata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/instance_metadata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/instance_metadata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.700596 moto-4.1.9.dev3/moto/iot/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    70619 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iot/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iot/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.700596 moto-4.1.9.dev3/moto/iotdata/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iotdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iotdata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iotdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iotdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/iotdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.704596 moto-4.1.9.dev3/moto/kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37257 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesis/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesis/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesis/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.704596 moto-4.1.9.dev3/moto/kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideo/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideo/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.704596 moto-4.1.9.dev3/moto/kinesisvideoarchivedmedia/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideoarchivedmedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideoarchivedmedia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideoarchivedmedia/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideoarchivedmedia/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kinesisvideoarchivedmedia/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.708596 moto-4.1.9.dev3/moto/kms/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24852 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kms/policy_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kms/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kms/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/kms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.708596 moto-4.1.9.dev3/moto/lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/lakeformation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/lakeformation/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/lakeformation/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/lakeformation/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.708596 moto-4.1.9.dev3/moto/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/logs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/logs/metric_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/logs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/logs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/logs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/logs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.712596 moto-4.1.9.dev3/moto/managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/managedblockchain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37565 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/managedblockchain/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/managedblockchain/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/managedblockchain/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/managedblockchain/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.712596 moto-4.1.9.dev3/moto/mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediaconnect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediaconnect/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediaconnect/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediaconnect/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.712596 moto-4.1.9.dev3/moto/medialive/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/medialive/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/medialive/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/medialive/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/medialive/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.712596 moto-4.1.9.dev3/moto/mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediapackage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediapackage/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediapackage/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediapackage/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.716596 moto-4.1.9.dev3/moto/mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastore/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastore/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastore/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.716596 moto-4.1.9.dev3/moto/mediastoredata/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastoredata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastoredata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastoredata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastoredata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mediastoredata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.716596 moto-4.1.9.dev3/moto/meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/meteringmarketplace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/meteringmarketplace/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/meteringmarketplace/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/meteringmarketplace/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.716596 moto-4.1.9.dev3/moto/moto_api/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.716596 moto-4.1.9.dev3/moto/moto_api/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/managed_state_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/moto_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.716596 moto-4.1.9.dev3/moto/moto_api/_internal/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/recorder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/recorder/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_api/_internal/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.716596 moto-4.1.9.dev3/moto/moto_server/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.716596 moto-4.1.9.dev3/moto/moto_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_server/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_server/threaded_moto_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_server/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/moto_server/werkzeug_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.720596 moto-4.1.9.dev3/moto/mq/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19975 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mq/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mq/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/mq/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.720596 moto-4.1.9.dev3/moto/neptune/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/neptune/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/neptune/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/neptune/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/neptune/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.720596 moto-4.1.9.dev3/moto/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opensearch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opensearch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opensearch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opensearch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opensearch/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.720596 moto-4.1.9.dev3/moto/opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opsworks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24989 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opsworks/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opsworks/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/opsworks/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.724596 moto-4.1.9.dev3/moto/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/organizations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/organizations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/organizations/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/organizations/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/organizations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.724596 moto-4.1.9.dev3/moto/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.724596 moto-4.1.9.dev3/moto/packages/boto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/boto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.724596 moto-4.1.9.dev3/moto/packages/boto/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/boto/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/boto/ec2/blockdevicemapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/boto/ec2/ec2object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/boto/ec2/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/boto/ec2/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/boto/ec2/instancetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/boto/ec2/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.724596 moto-4.1.9.dev3/moto/packages/cfnresponse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/cfnresponse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/packages/cfnresponse/cfnresponse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.724596 moto-4.1.9.dev3/moto/personalize/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/personalize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/personalize/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/personalize/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/personalize/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.724596 moto-4.1.9.dev3/moto/pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/pinpoint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/pinpoint/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/pinpoint/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/pinpoint/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.728596 moto-4.1.9.dev3/moto/polly/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/polly/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/polly/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/polly/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/polly/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/polly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.728596 moto-4.1.9.dev3/moto/quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/quicksight/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/quicksight/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/quicksight/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/quicksight/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.728596 moto-4.1.9.dev3/moto/ram/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ram/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ram/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ram/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ram/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.728596 moto-4.1.9.dev3/moto/rds/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rds/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   182267 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rds/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.504596 moto-4.1.9.dev3/moto/rds/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.732596 moto-4.1.9.dev3/moto/rds/resources/cluster_options/
--rw-r--r--   0 runner    (1001) docker     (123)   480836 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rds/resources/cluster_options/aurora-postgresql.json
--rw-r--r--   0 runner    (1001) docker     (123)   133645 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rds/resources/cluster_options/neptune.json
--rw-r--r--   0 runner    (1001) docker     (123)    64354 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rds/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rds/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rds/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.732596 moto-4.1.9.dev3/moto/rdsdata/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rdsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rdsdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rdsdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rdsdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.732596 moto-4.1.9.dev3/moto/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshift/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42945 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshift/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29591 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshift/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshift/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.732596 moto-4.1.9.dev3/moto/redshiftdata/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshiftdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshiftdata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshiftdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshiftdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/redshiftdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.736596 moto-4.1.9.dev3/moto/rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rekognition/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rekognition/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/rekognition/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.736596 moto-4.1.9.dev3/moto/resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroups/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroups/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroups/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroups/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.736596 moto-4.1.9.dev3/moto/resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28011 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroupstaggingapi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroupstaggingapi/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/resourcegroupstaggingapi/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.736596 moto-4.1.9.dev3/moto/route53/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37075 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    35235 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.740596 moto-4.1.9.dev3/moto/route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53resolver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37251 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53resolver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53resolver/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53resolver/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53resolver/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/route53resolver/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.744596 moto-4.1.9.dev3/moto/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/cloud_formation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    90986 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)   119897 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/select_object_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.744596 moto-4.1.9.dev3/moto/s3bucket_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3bucket_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3bucket_path/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.744596 moto-4.1.9.dev3/moto/s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3control/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3control/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3control/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3control/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/s3control/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.748596 moto-4.1.9.dev3/moto/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sagemaker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    99020 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sagemaker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29641 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sagemaker/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sagemaker/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sagemaker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sagemaker/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.748596 moto-4.1.9.dev3/moto/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/scheduler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/scheduler/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/scheduler/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/scheduler/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.748596 moto-4.1.9.dev3/moto/sdb/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sdb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sdb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sdb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sdb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.752596 moto-4.1.9.dev3/moto/secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/secretsmanager/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.752596 moto-4.1.9.dev3/moto/secretsmanager/list_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/secretsmanager/list_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/secretsmanager/list_secrets/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    32283 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/secretsmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/secretsmanager/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/secretsmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/secretsmanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.752596 moto-4.1.9.dev3/moto/servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicediscovery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicediscovery/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicediscovery/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicediscovery/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.752596 moto-4.1.9.dev3/moto/servicequotas/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicequotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicequotas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicequotas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.756596 moto-4.1.9.dev3/moto/servicequotas/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicequotas/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.756596 moto-4.1.9.dev3/moto/servicequotas/resources/default_quotas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicequotas/resources/default_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicequotas/resources/default_quotas/vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicequotas/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/servicequotas/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.756596 moto-4.1.9.dev3/moto/ses/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ses/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ses/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    21690 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ses/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    31667 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ses/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ses/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ses/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.756596 moto-4.1.9.dev3/moto/signer/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/signer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/signer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/signer/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/signer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.760596 moto-4.1.9.dev3/moto/sns/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sns/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    38878 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sns/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    46551 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sns/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sns/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sns/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.764596 moto-4.1.9.dev3/moto/sqs/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sqs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sqs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41436 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sqs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sqs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sqs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sqs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.764596 moto-4.1.9.dev3/moto/ssm/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    76048 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.768597 moto-4.1.9.dev3/moto/ssm/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.776596 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.508596 moto-4.1.9.dev3/moto/ssm/resources/ecs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.800597 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/
--rw-r--r--   0 runner    (1001) docker     (123)   416937 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   688021 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   738181 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   360357 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   798560 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    85325 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   778515 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   239300 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   734929 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   806032 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    84904 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   717425 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   618637 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    99223 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   737073 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   737391 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   164329 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   659463 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   761741 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   823629 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   767008 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   820874 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/us-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)  1745761 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/regions.json
--rw-r--r--   0 runner    (1001) docker     (123)  1824341 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/resources/services.json
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.800597 moto-4.1.9.dev3/moto/ssoadmin/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssoadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssoadmin/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssoadmin/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssoadmin/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssoadmin/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/ssoadmin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.804597 moto-4.1.9.dev3/moto/stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/stepfunctions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21993 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/stepfunctions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/stepfunctions/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/stepfunctions/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/stepfunctions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.804597 moto-4.1.9.dev3/moto/sts/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sts/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sts/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sts/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/sts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.804597 moto-4.1.9.dev3/moto/support/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/support/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/support/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.804597 moto-4.1.9.dev3/moto/support/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   172189 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/support/resources/describe_trusted_advisor_checks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/support/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/support/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.808596 moto-4.1.9.dev3/moto/swf/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.812596 moto-4.1.9.dev3/moto/swf/models/
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/activity_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/activity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/decision_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/generic_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/history_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30491 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/workflow_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/models/workflow_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    21829 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/swf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.812596 moto-4.1.9.dev3/moto/textract/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/textract/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/textract/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/textract/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/textract/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.812596 moto-4.1.9.dev3/moto/timestreamwrite/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/timestreamwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/timestreamwrite/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/timestreamwrite/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/timestreamwrite/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/timestreamwrite/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.812596 moto-4.1.9.dev3/moto/transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/transcribe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/transcribe/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/transcribe/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/transcribe/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.816597 moto-4.1.9.dev3/moto/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/utilities/aws_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/utilities/distutils_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/utilities/docker_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/utilities/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/utilities/tagging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/utilities/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.816597 moto-4.1.9.dev3/moto/wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/wafv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/wafv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/wafv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/wafv2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/wafv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.816597 moto-4.1.9.dev3/moto/xray/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/xray/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/xray/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/xray/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/xray/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/moto/xray/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.532596 moto-4.1.9.dev3/moto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-24 13:32:00.000000 moto-4.1.9.dev3/moto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66096 2023-04-24 13:32:00.000000 moto-4.1.9.dev3/moto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:32:00.000000 moto-4.1.9.dev3/moto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 13:32:00.000000 moto-4.1.9.dev3/moto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-24 13:32:00.000000 moto-4.1.9.dev3/moto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 13:32:00.000000 moto-4.1.9.dev3/moto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-24 13:32:01.000597 moto-4.1.9.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.820597 moto-4.1.9.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.820597 moto-4.1.9.dev3/tests/test_acm/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.820597 moto-4.1.9.dev3/tests/test_acm/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/ca.key
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/ca.srl
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/star_moto_com-bad.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/star_moto_com.csr
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/star_moto_com.key
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/resources/star_moto_com.pem
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acm/test_acm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.820597 moto-4.1.9.dev3/tests/test_acmpca/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acmpca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_acmpca/test_acmpca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.820597 moto-4.1.9.dev3/tests/test_amp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_amp/test_amp_logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_amp/test_amp_rulegroupnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_amp/test_amp_workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.824597 moto-4.1.9.dev3/tests/test_apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.828596 moto-4.1.9.dev3/tests/test_apigateway/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/resources/petstore-swagger-v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/resources/test_api.json
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/resources/test_api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/resources/test_api_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/resources/test_api_invalid_version.json
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/resources/test_deep_api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    91558 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_gatewayresponses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_importrestapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_putrestapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_vpclink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigateway/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.828596 moto-4.1.9.dev3/tests/test_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_reimport.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_apigatewayv2/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.832597 moto-4.1.9.dev3/tests/test_applicationautoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_applicationautoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_applicationautoscaling/test_applicationautoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_applicationautoscaling/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.832597 moto-4.1.9.dev3/tests/test_appsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_appsync/test_appsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_appsync/test_appsync_apikeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_appsync/test_appsync_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_appsync/test_appsync_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_appsync/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.832597 moto-4.1.9.dev3/tests/test_athena/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_athena/test_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_athena/test_athena_server_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.836597 moto-4.1.9.dev3/tests/test_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48170 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_scheduledactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_elb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_launch_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_autoscaling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.840597 moto-4.1.9.dev3/tests/test_awslambda/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_awslambda_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda_eventsourcemapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda_function_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda_invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_lambda_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_awslambda/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.840597 moto-4.1.9.dev3/tests/test_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_compute_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    34446 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_tags_job_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_tags_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_tags_scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_batch_task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.844596 moto-4.1.9.dev3/tests/test_batch_simple/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch_simple/test_batch_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch_simple/test_batch_compute_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_batch_simple/test_batch_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.844596 moto-4.1.9.dev3/tests/test_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_budgets/test_budgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_budgets/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_budgets/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.844596 moto-4.1.9.dev3/tests/test_ce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ce/test_ce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ce/test_ce_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.848597 moto-4.1.9.dev3/tests/test_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.848597 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/custom_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/ec2_classic_eip.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/fn_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/kms_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/route53_health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/route53_roundrobin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/vpc_eip.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/vpc_eni.py
--rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_custom_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_depends_on.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_multi_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_nested_stacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    85564 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    69300 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_stack_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_stack_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_import_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_stack_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudformation/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.852597 moto-4.1.9.dev3/tests/test_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudfront/cloudfront_test_scaffolding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudfront/test_cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudfront/test_cloudfront_dist_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    28631 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudfront/test_cloudfront_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudfront/test_cloudfront_invalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudfront/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.852597 moto-4.1.9.dev3/tests/test_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudtrail/test_cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudtrail/test_cloudtrail_eventselectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudtrail/test_cloudtrail_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudtrail/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.856597 moto-4.1.9.dev3/tests/test_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudwatch/test_cloudwatch_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    54006 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudwatch/test_cloudwatch_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudwatch/test_cloudwatch_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cloudwatch/test_cloudwatch_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.856597 moto-4.1.9.dev3/tests/test_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_codebuild/test_codebuild.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.856597 moto-4.1.9.dev3/tests/test_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_codecommit/test_codecommit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.856597 moto-4.1.9.dev3/tests/test_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_codepipeline/test_codepipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.856597 moto-4.1.9.dev3/tests/test_cognitoidentity/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cognitoidentity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cognitoidentity/test_cognitoidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cognitoidentity/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.856597 moto-4.1.9.dev3/tests/test_cognitoidp/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cognitoidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161791 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cognitoidp/test_cognitoidp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cognitoidp/test_cognitoidp_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cognitoidp/test_cognitoidp_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_cognitoidp/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.856597 moto-4.1.9.dev3/tests/test_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_comprehend/test_comprehend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.860597 moto-4.1.9.dev3/tests/test_config/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83099 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_config/test_config_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_config/test_config_rules_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_config/test_config_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.864597 moto-4.1.9.dev3/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_account_id_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_backenddict.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_decorator_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_environ_patching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_importorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_instance_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_mock_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_mock_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_moto_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_request_mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_responses_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_url_base_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_url_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.864597 moto-4.1.9.dev3/tests/test_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_databrew/test_databrew_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_databrew/test_databrew_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_databrew/test_databrew_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_databrew/test_databrew_rulesets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.864597 moto-4.1.9.dev3/tests/test_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_datapipeline/test_datapipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_datapipeline/test_datapipeline_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_datapipeline/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.868597 moto-4.1.9.dev3/tests/test_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_datasync/test_datasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.868597 moto-4.1.9.dev3/tests/test_dax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dax/test_dax.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dax/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.868597 moto-4.1.9.dev3/tests/test_dms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dms/test_dms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.868597 moto-4.1.9.dev3/tests/test_ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ds/test_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ds/test_ds_ad_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ds/test_ds_microsoft_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ds/test_ds_simple_ad_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ds/test_ds_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.872597 moto-4.1.9.dev3/tests/test_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.872597 moto-4.1.9.dev3/tests/test_dynamodb/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/exceptions/test_key_length_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.872597 moto-4.1.9.dev3/tests/test_dynamodb/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/models/test_key_condition_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   205697 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_batch_get_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_condition_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_consumedcapacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_create_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    39804 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_table_with_range_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_table_without_range_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_update_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_update_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.876597 moto-4.1.9.dev3/tests/test_dynamodb_v20111205/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb_v20111205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43145 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb_v20111205/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodb_v20111205/test_servermode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.876597 moto-4.1.9.dev3/tests/test_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_dynamodbstreams/test_dynamodbstreams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.876597 moto-4.1.9.dev3/tests/test_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ebs/test_ebs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.888597 moto-4.1.9.dev3/tests/test_ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_account_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_amazon_dev_pay.py
--rw-r--r--   0 runner    (1001) docker     (123)    44698 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_ec2_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_ec2_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_ec2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_egress_only_igw.py
--rw-r--r--   0 runner    (1001) docker     (123)    42808 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    41728 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24744 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_flow_logs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_iam_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_instance_type_offerings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    98932 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_nat_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_placement_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_prefix_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_reserved_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40328 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    65961 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_security_groups_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_spot_fleet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_spot_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_transit_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_transit_gateway_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_transit_gateway_peering_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_virtual_private_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_vm_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_vm_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_vpc_endpoint_services_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_vpc_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    45725 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2/test_windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.888597 moto-4.1.9.dev3/tests/test_ec2instanceconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.892597 moto-4.1.9.dev3/tests/test_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92826 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecr/test_ecr_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecr/test_ecr_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecr/test_ecr_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecr/test_ecr_policy_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.892597 moto-4.1.9.dev3/tests/test_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecs/test_ecs_account_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)   122563 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecs/test_ecs_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecs/test_ecs_capacity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecs/test_ecs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecs/test_ecs_efs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecs/test_ecs_task_def_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ecs/test_ecs_tasksets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.896597 moto-4.1.9.dev3/tests/test_efs/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/junk_drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/test_access_point_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/test_access_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/test_filesystem_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/test_lifecycle_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/test_mount_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/test_mount_target_security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_efs/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.896597 moto-4.1.9.dev3/tests/test_eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52255 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_eks/test_eks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_eks/test_eks_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_eks/test_eks_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_eks/test_eks_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_eks/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.896597 moto-4.1.9.dev3/tests/test_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elasticache/test_elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elasticache/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.896597 moto-4.1.9.dev3/tests/test_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elasticbeanstalk/test_eb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.896597 moto-4.1.9.dev3/tests/test_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elastictranscoder/__init__
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elastictranscoder/test_elastictranscoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elastictranscoder/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.900597 moto-4.1.9.dev3/tests/test_elb/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41073 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elb/test_elb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elb/test_elb_availabilityzones.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elb/test_elb_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elb/test_elb_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elb/test_elb_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.900597 moto-4.1.9.dev3/tests/test_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66616 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_listener_rule_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_listener_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_listener_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_set_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_target_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_elbv2/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.904597 moto-4.1.9.dev3/tests/test_emr/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emr/test_emr_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emr/test_emr_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emr/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.904597 moto-4.1.9.dev3/tests/test_emrcontainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emrcontainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emrcontainers/test_emrcontainers.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emrcontainers/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.904597 moto-4.1.9.dev3/tests/test_emrserverless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emrserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emrserverless/test_emrserverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_emrserverless/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.908597 moto-4.1.9.dev3/tests/test_es/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_es/test_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_es/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.908597 moto-4.1.9.dev3/tests/test_events/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_events/test_event_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    81682 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_events/test_events_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_events/test_events_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_events/test_events_lambdatriggers_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.912597 moto-4.1.9.dev3/tests/test_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_firehose/test_firehose.py
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_firehose/test_firehose_destination_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_firehose/test_firehose_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_firehose/test_firehose_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_firehose/test_firehose_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_firehose/test_http_destinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.912597 moto-4.1.9.dev3/tests/test_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_forecast/test_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.912597 moto-4.1.9.dev3/tests/test_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glacier/test.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glacier/test_glacier_archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glacier/test_glacier_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glacier/test_glacier_vaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glacier/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.916597 moto-4.1.9.dev3/tests/test_glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.916597 moto-4.1.9.dev3/tests/test_glue/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/fixtures/datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/fixtures/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    48038 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/test_datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/test_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/test_glue_job_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/test_partition_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    47112 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_glue/test_schema_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.920597 moto-4.1.9.dev3/tests/test_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.920597 moto-4.1.9.dev3/tests/test_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_guardduty/test_guardduty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_guardduty/test_guardduty_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_guardduty/test_guardduty_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_guardduty/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.924597 moto-4.1.9.dev3/tests/test_iam/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   167646 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam_access_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam_account_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)    51772 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam_password_last_used.py
--rw-r--r--   0 runner    (1001) docker     (123)    51265 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_iam_server_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iam/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.924597 moto-4.1.9.dev3/tests/test_identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_identitystore/test_identitystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.928597 moto-4.1.9.dev3/tests/test_iot/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_ca_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_deprecate_thing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_domain_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_job_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    28056 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_thing_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_thing_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_things.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_iot_topic_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iot/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.928597 moto-4.1.9.dev3/tests/test_iotdata/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iotdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iotdata/test_iotdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_iotdata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.928597 moto-4.1.9.dev3/tests/test_kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31019 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/test_kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_stream_consumers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_stream_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesis/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.932597 moto-4.1.9.dev3/tests/test_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesisvideo/test_kinesisvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesisvideo/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.932597 moto-4.1.9.dev3/tests/test_kinesisvideoarchivedmedia/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesisvideoarchivedmedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kinesisvideoarchivedmedia/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.932597 moto-4.1.9.dev3/tests/test_kms/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kms/test_kms_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kms/test_kms_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kms/test_kms_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kms/test_kms_policy_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kms/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kms/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_kms/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.932597 moto-4.1.9.dev3/tests/test_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_lakeformation/test_lakeformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.936597 moto-4.1.9.dev3/tests/test_logs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_logs/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    47011 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_logs/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_logs/test_logs_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_logs/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.936597 moto-4.1.9.dev3/tests/test_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_managedblockchain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_proposals.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.936597 moto-4.1.9.dev3/tests/test_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediaconnect/test_mediaconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediaconnect/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.936597 moto-4.1.9.dev3/tests/test_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_medialive/test_medialive.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_medialive/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.936597 moto-4.1.9.dev3/tests/test_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediapackage/test_mediapackage.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediapackage/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.940597 moto-4.1.9.dev3/tests/test_mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediastore/test_mediastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediastore/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.940597 moto-4.1.9.dev3/tests/test_mediastoredata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediastoredata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediastoredata/test_mediastoredata.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mediastoredata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.940597 moto-4.1.9.dev3/tests/test_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_meteringmarketplace/test_meteringmarketplace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.940597 moto-4.1.9.dev3/tests/test_moto_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.940597 moto-4.1.9.dev3/tests/test_moto_api/mock_random/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/mock_random/test_mock_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.940597 moto-4.1.9.dev3/tests/test_moto_api/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/recorder/test_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.940597 moto-4.1.9.dev3/tests/test_moto_api/state_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/state_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.940597 moto-4.1.9.dev3/tests/test_moto_api/state_manager/servermode/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/state_manager/servermode/test_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/state_manager/test_batch_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/state_manager/test_managed_state_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_moto_api/state_manager/test_state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.944597 moto-4.1.9.dev3/tests/test_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mq/test_mq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mq/test_mq_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mq/test_mq_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mq/test_mq_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_mq/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.944597 moto-4.1.9.dev3/tests/test_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_neptune/test_cluster_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_neptune/test_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_neptune/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_neptune/test_global_clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.944597 moto-4.1.9.dev3/tests/test_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_opensearch/test_domain_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_opensearch/test_opensearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.944597 moto-4.1.9.dev3/tests/test_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_opsworks/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_opsworks/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_opsworks/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_opsworks/test_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.948597 moto-4.1.9.dev3/tests/test_organizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_organizations/organizations_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    85363 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_organizations/test_organizations_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.948597 moto-4.1.9.dev3/tests/test_personalize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_personalize/test_personalize_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.948597 moto-4.1.9.dev3/tests/test_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_pinpoint/test_pinpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_pinpoint/test_pinpoint_application_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_pinpoint/test_pinpoint_event_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.948597 moto-4.1.9.dev3/tests/test_polly/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_polly/test_polly.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_polly/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.948597 moto-4.1.9.dev3/tests/test_quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_quicksight/test_quicksight_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_quicksight/test_quicksight_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_quicksight/test_quicksight_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.948597 moto-4.1.9.dev3/tests/test_ram/
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ram/test_ram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.952597 moto-4.1.9.dev3/tests/test_rds/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_db_cluster_param_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_db_cluster_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_global_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)    91218 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_rds_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_rds_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_rds_clusters_with_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_rds_event_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_rds_export_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rds/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.952597 moto-4.1.9.dev3/tests/test_rdsdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rdsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rdsdata/test_rdsdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.956597 moto-4.1.9.dev3/tests/test_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73309 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_redshift/test_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_redshift/test_redshift_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_redshift/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.956597 moto-4.1.9.dev3/tests/test_redshiftdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_redshiftdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_redshiftdata/test_redshiftdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_redshiftdata/test_redshiftdata_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_redshiftdata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.956597 moto-4.1.9.dev3/tests/test_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_rekognition/test_rekognition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.956597 moto-4.1.9.dev3/tests/test_resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_resourcegroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_resourcegroups/test_resourcegroups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.956597 moto-4.1.9.dev3/tests/test_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_resourcegroupstaggingapi/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.960597 moto-4.1.9.dev3/tests/test_route53/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/test_change_set_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52862 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/test_route53.py
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/test_route53_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/test_route53_delegationsets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/test_route53_healthchecks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/test_route53_query_logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/test_route53_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.960597 moto-4.1.9.dev3/tests/test_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40356 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53resolver/test_route53resolver_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53resolver/test_route53resolver_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53resolver/test_route53resolver_rule_associations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_route53resolver/test_route53resolver_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.968597 moto-4.1.9.dev3/tests/test_s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_multiple_accounts_server.py
--rw-r--r--   0 runner    (1001) docker     (123)   115875 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_classdecorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18825 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_copyobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_custom_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_file_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_lambda_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    31026 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_object_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_ownership.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_storageclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.968597 moto-4.1.9.dev3/tests/test_s3bucket_path/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3bucket_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3bucket_path/test_s3bucket_path_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3bucket_path/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.968597 moto-4.1.9.dev3/tests/test_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3control/test_s3control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3control/test_s3control_access_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3control/test_s3control_accesspoint_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3control/test_s3control_config_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_s3control/test_s3control_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.972597 moto-4.1.9.dev3/tests/test_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/cloudformation_test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20469 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24758 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_trial_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.972597 moto-4.1.9.dev3/tests/test_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_scheduler/test_schedule_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_scheduler/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_scheduler/test_scheduler_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_scheduler/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.972597 moto-4.1.9.dev3/tests/test_sdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sdb/test_sdb_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sdb/test_sdb_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sdb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.976597 moto-4.1.9.dev3/tests/test_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_secretsmanager/test_list_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_secretsmanager/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    57270 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_secretsmanager/test_secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    33302 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_secretsmanager/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.976597 moto-4.1.9.dev3/tests/test_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_servicediscovery/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_servicediscovery/test_servicediscovery_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_servicediscovery/test_servicediscovery_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_servicediscovery/test_servicediscovery_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.976597 moto-4.1.9.dev3/tests/test_servicequotas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_servicequotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_servicequotas/test_servicequotas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.976597 moto-4.1.9.dev3/tests/test_ses/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ses/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    52328 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ses/test_ses_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ses/test_ses_sns_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ses/test_ses_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ses/test_templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.980597 moto-4.1.9.dev3/tests/test_signer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_signer/test_signing_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_signer/test_signing_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.980597 moto-4.1.9.dev3/tests/test_sns/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sns/test_application_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sns/test_publish_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    42805 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sns/test_publishing_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sns/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sns/test_sns_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19367 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sns/test_subscriptions_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sns/test_topics_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.980597 moto-4.1.9.dev3/tests/test_special_cases/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_special_cases/test_custom_amis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.980597 moto-4.1.9.dev3/tests/test_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sqs/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)   110801 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sqs/test_sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sqs/test_sqs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sqs/test_sqs_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sqs/test_sqs_multiaccount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.984597 moto-4.1.9.dev3/tests/test_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72169 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_default_amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_doc_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28425 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_ec2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_ecs_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_maintenance_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_parameterstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_ssm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.984597 moto-4.1.9.dev3/tests/test_ssm/test_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssm/test_templates/good.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.984597 moto-4.1.9.dev3/tests/test_ssoadmin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssoadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssoadmin/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_ssoadmin/test_ssoadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.988597 moto-4.1.9.dev3/tests/test_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_stepfunctions/test_stepfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_stepfunctions/test_stepfunctions_cloudformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.988597 moto-4.1.9.dev3/tests/test_sts/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sts/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sts/test_sts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_sts/test_sts_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.988597 moto-4.1.9.dev3/tests/test_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_support/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_support/test_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.988597 moto-4.1.9.dev3/tests/test_swf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.992597 moto-4.1.9.dev3/tests/test_swf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/test_activity_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/test_decision_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/test_generic_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/test_history_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/models/test_workflow_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.992597 moto-4.1.9.dev3/tests/test_swf/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/responses/test_activity_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/responses/test_activity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21702 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/responses/test_decision_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/responses/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/responses/test_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/responses/test_workflow_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/responses/test_workflow_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_swf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.992597 moto-4.1.9.dev3/tests/test_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_textract/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_textract/test_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.996597 moto-4.1.9.dev3/tests/test_timestreamwrite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_timestreamwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_timestreamwrite/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_timestreamwrite/test_timestreamwrite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_timestreamwrite/test_timestreamwrite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_timestreamwrite/test_timestreamwrite_tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.996597 moto-4.1.9.dev3/tests/test_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_transcribe/test_transcribe_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.996597 moto-4.1.9.dev3/tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_utilities/test_docker_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_utilities/test_paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_utilities/test_tagging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_utilities/test_threaded_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:00.996597 moto-4.1.9.dev3/tests/test_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_wafv2/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_wafv2/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_wafv2/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_wafv2/test_wafv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_wafv2/test_wafv2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_wafv2/test_wafv2_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_wafv2/test_wafv2_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:32:01.000597 moto-4.1.9.dev3/tests/test_xray/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_xray/test_xray_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-24 13:31:50.000000 moto-4.1.9.dev3/tests/test_xray/test_xray_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto/
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-24 13:34:27.000000 moto-4.1.9.dev5/moto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto/acmpca/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/apigateway/integration_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/integration_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/integration_parsers/aws_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/integration_parsers/http_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/integration_parsers/unknown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91751 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64715 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36307 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/applicationautoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61357 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65472 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/awslambda/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74928 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/backend_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69404 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/batch_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch_simple/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch_simple/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch_simple/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37709 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53038 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33739 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/cognitoidentity/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/cognitoidp/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83922 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/cognitoidp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/resources/jwks-private.json
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/resources/jwks-public.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81665 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/config/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   117575 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/resources/aws_managed_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/botocore_stubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/common_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/custom_responses_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/model_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40468 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/responses_custom_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25372 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19227 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/dax/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/dms/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42639 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/limits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/dynamodb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    33457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17443 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/models/dynamo_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39809 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/models/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/dynamodb/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/ast_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34656 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/key_condition_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/partiql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/reserved_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/reserved_keywords.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45017 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/dynamodb_v20111205/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodbstreams/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodbstreams/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodbstreams/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ebs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ebs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ebs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.064038 moto-4.1.9.dev5/moto/ec2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/iam_instance_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/managed_prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/spot_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/transit_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/transit_gateway_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/transit_gateway_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpc_peering_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpn_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.068038 moto-4.1.9.dev5/moto/ec2/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/amis.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.008033 moto-4.1.9.dev5/moto/ec2/resources/ecs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.076039 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)   110385 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   184754 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205924 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    76970 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224300 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   204442 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   236846 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   196475 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   151250 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205418 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205543 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   170773 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   216660 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   244124 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219056 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243613 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.008033 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.080039 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    40620 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38329 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   112314 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79281 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42533 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    73186 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100264 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31415 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64924 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   102387 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23689 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51746 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121670 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58608 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65537 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   200128 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   112258 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147926 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.088040 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/
+-rw-r--r--   0 runner    (1001) docker     (123)    38820 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37177 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   102960 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72651 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38975 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    69946 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91900 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    92102 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28787 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60279 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    95067 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50561 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   118040 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    69350 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56856 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36936 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63575 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   194154 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   108910 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47322 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   143512 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.092040 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40058 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34296 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35491 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40817 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41887 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37998 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41546 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1306310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_types.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.096041 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.100041 moto-4.1.9.dev5/moto/ec2/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/account_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/egress_only_internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/iam_instance_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/reserved_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/spot_fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/spot_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/transit_gateway_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/transit_gateway_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/transit_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/virtual_private_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/vpc_peering_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28837 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.100041 moto-4.1.9.dev5/moto/ec2instanceconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2instanceconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2instanceconnect/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2instanceconnect/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2instanceconnect/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.100041 moto-4.1.9.dev5/moto/ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86640 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/efs/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26760 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30391 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57275 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elastictranscoder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elastictranscoder/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elastictranscoder/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70076 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68565 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65244 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/emrcontainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/emrserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66807 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29565 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.116043 moto-4.1.9.dev5/moto/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/glue_schema_registry_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/glue_schema_registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22412 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.116043 moto-4.1.9.dev5/moto/greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54499 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30895 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.116043 moto-4.1.9.dev5/moto/guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.120043 moto-4.1.9.dev5/moto/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1599363 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/aws_managed_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118618 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107097 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.120043 moto-4.1.9.dev5/moto/identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.120043 moto-4.1.9.dev5/moto/instance_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/instance_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/instance_metadata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/instance_metadata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/instance_metadata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.120043 moto-4.1.9.dev5/moto/iot/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70619 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/iotdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37257 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/kms/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24852 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/policy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/metric_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37565 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/mediastoredata/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/moto_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/moto_api/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/managed_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/moto_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/moto_api/_internal/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/recorder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/recorder/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/moto_server/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/moto_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_server/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_server/threaded_moto_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_server/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_server/werkzeug_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19975 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/packages/boto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/packages/boto/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/blockdevicemapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/ec2object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/instancetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/packages/cfnresponse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/cfnresponse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/cfnresponse/cfnresponse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/polly/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182267 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.016033 moto-4.1.9.dev5/moto/rds/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/rds/resources/cluster_options/
+-rw-r--r--   0 runner    (1001) docker     (123)   480836 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/resources/cluster_options/aurora-postgresql.json
+-rw-r--r--   0 runner    (1001) docker     (123)   133645 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/resources/cluster_options/neptune.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64354 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/rdsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rdsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rdsdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rdsdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rdsdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42945 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29591 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/redshiftdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rekognition/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rekognition/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rekognition/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28011 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37075 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35235 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37251 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/cloud_formation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90986 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119897 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/select_object_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/s3bucket_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3bucket_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3bucket_path/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99020 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29641 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/secretsmanager/list_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/list_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/list_secrets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32283 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/servicequotas/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/servicequotas/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/servicequotas/resources/default_quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/resources/default_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/resources/default_quotas/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/ses/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21690 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31667 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/signer/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/sns/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42303 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46479 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.164047 moto-4.1.9.dev5/moto/sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41436 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.164047 moto-4.1.9.dev5/moto/ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80116 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.164047 moto-4.1.9.dev5/moto/ssm/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.172048 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.016033 moto-4.1.9.dev5/moto/ssm/resources/ecs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.192050 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)   416937 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   688021 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   738181 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   360357 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   798560 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85325 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   778515 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   239300 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   734929 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   806032 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    84904 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   717425 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   618637 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    99223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   737073 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   737391 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   164329 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659463 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   761741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   823629 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   767008 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   820874 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1745761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1824341 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/services.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.192050 moto-4.1.9.dev5/moto/ssoadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.192050 moto-4.1.9.dev5/moto/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21993 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/support/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/support/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   172189 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/resources/describe_trusted_advisor_checks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/swf/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/swf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/activity_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/decision_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/generic_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/history_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30491 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/workflow_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/workflow_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21829 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/textract/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/timestreamwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/aws_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/distutils_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/docker_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/tagging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/xray/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66096 2023-04-24 13:34:35.000000 moto-4.1.9.dev5/moto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-24 13:34:35.320062 moto-4.1.9.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_acm/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/ca.key
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/ca.srl
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com-bad.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.csr
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/test_acm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_acmpca/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acmpca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acmpca/test_acmpca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_amp/test_amp_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_amp/test_amp_rulegroupnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_amp/test_amp_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_apigateway/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/petstore-swagger-v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_api_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_api_invalid_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_deep_api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    91558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_gatewayresponses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_importrestapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_putrestapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_vpclink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_reimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_applicationautoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_applicationautoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_applicationautoscaling/test_applicationautoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_applicationautoscaling/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_appsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_appsync_apikeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_appsync_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_appsync_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_athena/test_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_athena/test_athena_server_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.212052 moto-4.1.9.dev5/tests/test_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_scheduledactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_launch_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.212052 moto-4.1.9.dev5/tests/test_awslambda/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_awslambda_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_eventsourcemapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_function_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_compute_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34446 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_tags_job_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_tags_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_tags_scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_batch_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch_simple/test_batch_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch_simple/test_batch_compute_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch_simple/test_batch_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_budgets/test_budgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_budgets/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_budgets/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ce/test_ce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ce/test_ce_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.220052 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/custom_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/ec2_classic_eip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/fn_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/kms_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_roundrobin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_eip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_eni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_custom_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_depends_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_multi_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_nested_stacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85564 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69300 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_import_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_stack_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.220052 moto-4.1.9.dev5/tests/test_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/cloudfront_test_scaffolding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_dist_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28631 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.220052 moto-4.1.9.dev5/tests/test_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail_eventselectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.220052 moto-4.1.9.dev5/tests/test_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54006 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_codebuild/test_codebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_codecommit/test_codecommit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_codepipeline/test_codepipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_cognitoidentity/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidentity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidentity/test_cognitoidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidentity/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_cognitoidp/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161791 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_comprehend/test_comprehend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83099 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/test_config_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/test_config_rules_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/test_config_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_account_id_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_backenddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_decorator_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_environ_patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_importorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_instance_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_mock_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_mock_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_moto_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_request_mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_responses_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_url_base_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_url_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/test_databrew_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/test_databrew_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/test_databrew_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/test_databrew_rulesets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datapipeline/test_datapipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datapipeline/test_datapipeline_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datapipeline/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datasync/test_datasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dax/test_dax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dax/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dms/test_dms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.232054 moto-4.1.9.dev5/tests/test_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds_ad_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds_microsoft_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds_simple_ad_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.232054 moto-4.1.9.dev5/tests/test_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_dynamodb/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/exceptions/test_key_length_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_dynamodb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/models/test_key_condition_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   205697 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_batch_get_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_condition_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_consumedcapacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39804 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_table_with_range_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_table_without_range_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_update_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_update_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_dynamodb_v20111205/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb_v20111205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43145 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb_v20111205/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb_v20111205/test_servermode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodbstreams/test_dynamodbstreams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ebs/test_ebs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.244055 moto-4.1.9.dev5/tests/test_ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_account_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_amazon_dev_pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44698 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_ec2_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_ec2_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_ec2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_egress_only_igw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42808 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41728 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24744 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_flow_logs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_iam_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_instance_type_offerings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98932 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_nat_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_placement_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_prefix_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_reserved_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40328 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65961 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_security_groups_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_spot_fleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_spot_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway_peering_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_virtual_private_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vm_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vm_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpc_endpoint_services_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpc_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45725 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.244055 moto-4.1.9.dev5/tests/test_ec2instanceconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.244055 moto-4.1.9.dev5/tests/test_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92826 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/test_ecr_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/test_ecr_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/test_ecr_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/test_ecr_policy_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_account_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122563 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_capacity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_task_def_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_tasksets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/junk_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_access_point_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_access_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_filesystem_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_lifecycle_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_mount_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_mount_target_security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52255 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_eks_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_eks_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_eks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elasticache/test_elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elasticache/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elasticbeanstalk/test_eb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elastictranscoder/__init__
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elastictranscoder/test_elastictranscoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elastictranscoder/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41073 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb_availabilityzones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66616 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_rule_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_set_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_target_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/test_emr_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/test_emr_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_emrcontainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrcontainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrcontainers/test_emrcontainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrcontainers/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_emrserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrserverless/test_emrserverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrserverless/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_es/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_es/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_es/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_events/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_event_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81682 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_events_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_events_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_events_lambdatriggers_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose_destination_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_http_destinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_forecast/test_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test_glacier_archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test_glacier_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test_glacier_vaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.260056 moto-4.1.9.dev5/tests/test_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.260056 moto-4.1.9.dev5/tests/test_glue/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/fixtures/datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/fixtures/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48038 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_glue_job_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_partition_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47112 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_schema_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.260056 moto-4.1.9.dev5/tests/test_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.260056 moto-4.1.9.dev5/tests/test_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/test_guardduty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/test_guardduty_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/test_guardduty_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.264057 moto-4.1.9.dev5/tests/test_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167646 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_access_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_account_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51772 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_password_last_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51265 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_server_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.264057 moto-4.1.9.dev5/tests/test_identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_identitystore/test_identitystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.264057 moto-4.1.9.dev5/tests/test_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_ca_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_deprecate_thing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_domain_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_job_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28056 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_thing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_thing_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_topic_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.264057 moto-4.1.9.dev5/tests/test_iotdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iotdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iotdata/test_iotdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iotdata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31019 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_stream_consumers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_stream_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideo/test_kinesisvideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideo/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_kms_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_kms_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_kms_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_kms_policy_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_lakeformation/test_lakeformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47011 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/test_logs_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_proposals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediaconnect/test_mediaconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediaconnect/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_medialive/test_medialive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_medialive/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediapackage/test_mediapackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediapackage/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastore/test_mediastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastore/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_mediastoredata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastoredata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastoredata/test_mediastoredata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastoredata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_meteringmarketplace/test_meteringmarketplace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_moto_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_moto_api/mock_random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/mock_random/test_mock_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_moto_api/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/recorder/test_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_moto_api/state_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/test_state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_batch_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_managed_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_mq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_mq_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_mq_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_mq_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/test_cluster_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/test_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/test_global_clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opensearch/test_domain_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opensearch/test_opensearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/test_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_organizations/organizations_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85363 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_organizations/test_organizations_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_personalize/test_personalize_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint_application_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint_event_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_polly/test_polly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_polly/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ram/test_ram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_rds/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_db_cluster_param_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_db_cluster_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_global_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91218 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_clusters_with_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_event_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_export_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_rdsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rdsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rdsdata/test_rdsdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73309 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshift/test_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshift/test_redshift_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshift/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_redshiftdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshiftdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshiftdata/test_redshiftdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshiftdata/test_redshiftdata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshiftdata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rekognition/test_rekognition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroups/test_resourcegroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.292059 moto-4.1.9.dev5/tests/test_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_change_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52862 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_delegationsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_healthchecks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_query_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.292059 moto-4.1.9.dev5/tests/test_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40356 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_rule_associations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.296059 moto-4.1.9.dev5/tests/test_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_multiple_accounts_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115875 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_classdecorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18825 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_copyobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_custom_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_file_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_lambda_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31026 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_object_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_storageclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.296059 moto-4.1.9.dev5/tests/test_s3bucket_path/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3bucket_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3bucket_path/test_s3bucket_path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3bucket_path/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.296059 moto-4.1.9.dev5/tests/test_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control_access_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control_accesspoint_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control_config_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/cloudformation_test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20469 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24758 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_trial_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/test_schedule_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/test_scheduler_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sdb/test_sdb_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sdb/test_sdb_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sdb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/test_list_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57270 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/test_secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33302 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_servicequotas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicequotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicequotas/test_servicequotas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52328 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_ses_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_ses_sns_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_ses_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_signer/test_signing_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_signer/test_signing_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_application_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_publish_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42807 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_publishing_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_sns_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_subscriptions_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_topics_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_special_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_special_cases/test_custom_amis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110801 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_sqs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_sqs_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_sqs_multiaccount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72442 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_default_amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_doc_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28425 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_ec2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_ecs_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_maintenance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_parameterstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_ssm/test_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_templates/good.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_ssoadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssoadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssoadmin/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssoadmin/test_ssoadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_stepfunctions/test_stepfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_stepfunctions/test_stepfunctions_cloudformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_sts/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sts/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sts/test_sts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sts/test_sts_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_support/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_support/test_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.312061 moto-4.1.9.dev5/tests/test_swf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.312061 moto-4.1.9.dev5/tests/test_swf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_activity_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_decision_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_generic_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_history_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_workflow_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.312061 moto-4.1.9.dev5/tests/test_swf/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_activity_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_activity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21702 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_decision_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_workflow_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_workflow_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.312061 moto-4.1.9.dev5/tests/test_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_textract/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_textract/test_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_timestreamwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_transcribe/test_transcribe_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_utilities/test_docker_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_utilities/test_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_utilities/test_tagging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_utilities/test_threaded_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_wafv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_xray/test_xray_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_xray/test_xray_client.py
```

### Comparing `moto-4.1.9.dev3/AUTHORS.md` & `moto-4.1.9.dev5/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/LICENSE` & `moto-4.1.9.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/MANIFEST.in` & `moto-4.1.9.dev5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/PKG-INFO` & `moto-4.1.9.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moto
-Version: 4.1.9.dev3
+Version: 4.1.9.dev5
 Home-page: https://github.com/getmoto/moto
 Author: Steve Pulec
 Author-email: "spulec@gmail.com"
 License: Apache License 2.0
 Project-URL: Documentation, http://docs.getmoto.org/en/latest/
 Project-URL: Issue tracker, https://github.com/getmoto/moto/issues
 Project-URL: Changelog, https://github.com/getmoto/moto/blob/master/CHANGELOG.md
```

### Comparing `moto-4.1.9.dev3/README.md` & `moto-4.1.9.dev5/README.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/__init__.py` & `moto-4.1.9.dev5/moto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
 mock_all = MockAll
 
 # import logging
 # logging.getLogger('boto').setLevel(logging.CRITICAL)
 
 __title__ = "moto"
-__version__ = "4.1.9.dev3"
+__version__ = "4.1.9.dev5"
 
 
 try:
     # Need to monkey-patch botocore requests back to underlying urllib3 classes
     from botocore.awsrequest import (
         HTTPSConnectionPool,
         HTTPConnectionPool,
```

### Comparing `moto-4.1.9.dev3/moto/acm/models.py` & `moto-4.1.9.dev5/moto/acm/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/acm/responses.py` & `moto-4.1.9.dev5/moto/acm/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/acmpca/models.py` & `moto-4.1.9.dev5/moto/acmpca/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/acmpca/responses.py` & `moto-4.1.9.dev5/moto/acmpca/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/amp/exceptions.py` & `moto-4.1.9.dev5/moto/amp/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/amp/models.py` & `moto-4.1.9.dev5/moto/amp/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/amp/responses.py` & `moto-4.1.9.dev5/moto/amp/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/amp/urls.py` & `moto-4.1.9.dev5/moto/amp/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigateway/exceptions.py` & `moto-4.1.9.dev5/moto/apigateway/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigateway/integration_parsers/aws_parser.py` & `moto-4.1.9.dev5/moto/apigateway/integration_parsers/aws_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigateway/integration_parsers/http_parser.py` & `moto-4.1.9.dev5/moto/apigateway/integration_parsers/http_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigateway/models.py` & `moto-4.1.9.dev5/moto/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigateway/responses.py` & `moto-4.1.9.dev5/moto/apigateway/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigateway/urls.py` & `moto-4.1.9.dev5/moto/apigateway/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigateway/utils.py` & `moto-4.1.9.dev5/moto/apigateway/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigatewayv2/exceptions.py` & `moto-4.1.9.dev5/moto/apigatewayv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigatewayv2/models.py` & `moto-4.1.9.dev5/moto/apigatewayv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigatewayv2/responses.py` & `moto-4.1.9.dev5/moto/apigatewayv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/apigatewayv2/urls.py` & `moto-4.1.9.dev5/moto/apigatewayv2/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/applicationautoscaling/models.py` & `moto-4.1.9.dev5/moto/applicationautoscaling/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/applicationautoscaling/responses.py` & `moto-4.1.9.dev5/moto/applicationautoscaling/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/appsync/models.py` & `moto-4.1.9.dev5/moto/appsync/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/appsync/responses.py` & `moto-4.1.9.dev5/moto/appsync/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/appsync/urls.py` & `moto-4.1.9.dev5/moto/appsync/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/athena/exceptions.py` & `moto-4.1.9.dev5/moto/athena/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/athena/models.py` & `moto-4.1.9.dev5/moto/athena/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/athena/responses.py` & `moto-4.1.9.dev5/moto/athena/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/autoscaling/exceptions.py` & `moto-4.1.9.dev5/moto/autoscaling/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/autoscaling/models.py` & `moto-4.1.9.dev5/moto/autoscaling/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/autoscaling/responses.py` & `moto-4.1.9.dev5/moto/autoscaling/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/awslambda/exceptions.py` & `moto-4.1.9.dev5/moto/awslambda/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/awslambda/models.py` & `moto-4.1.9.dev5/moto/awslambda/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/awslambda/policy.py` & `moto-4.1.9.dev5/moto/awslambda/policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/awslambda/responses.py` & `moto-4.1.9.dev5/moto/awslambda/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/awslambda/urls.py` & `moto-4.1.9.dev5/moto/awslambda/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/awslambda/utils.py` & `moto-4.1.9.dev5/moto/awslambda/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/backend_index.py` & `moto-4.1.9.dev5/moto/backend_index.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/backends.py` & `moto-4.1.9.dev5/moto/backends.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/batch/models.py` & `moto-4.1.9.dev5/moto/batch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/batch/responses.py` & `moto-4.1.9.dev5/moto/batch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/batch/urls.py` & `moto-4.1.9.dev5/moto/batch/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/batch/utils.py` & `moto-4.1.9.dev5/moto/batch/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/batch_simple/models.py` & `moto-4.1.9.dev5/moto/batch_simple/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/budgets/exceptions.py` & `moto-4.1.9.dev5/moto/budgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/budgets/models.py` & `moto-4.1.9.dev5/moto/budgets/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/budgets/responses.py` & `moto-4.1.9.dev5/moto/budgets/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ce/models.py` & `moto-4.1.9.dev5/moto/ce/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ce/responses.py` & `moto-4.1.9.dev5/moto/ce/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudformation/custom_model.py` & `moto-4.1.9.dev5/moto/cloudformation/custom_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudformation/exceptions.py` & `moto-4.1.9.dev5/moto/cloudformation/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudformation/models.py` & `moto-4.1.9.dev5/moto/cloudformation/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudformation/parsing.py` & `moto-4.1.9.dev5/moto/cloudformation/parsing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudformation/responses.py` & `moto-4.1.9.dev5/moto/cloudformation/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudformation/utils.py` & `moto-4.1.9.dev5/moto/cloudformation/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudfront/exceptions.py` & `moto-4.1.9.dev5/moto/cloudfront/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudfront/models.py` & `moto-4.1.9.dev5/moto/cloudfront/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudfront/responses.py` & `moto-4.1.9.dev5/moto/cloudfront/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudfront/urls.py` & `moto-4.1.9.dev5/moto/cloudfront/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudtrail/exceptions.py` & `moto-4.1.9.dev5/moto/cloudtrail/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudtrail/models.py` & `moto-4.1.9.dev5/moto/cloudtrail/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudtrail/responses.py` & `moto-4.1.9.dev5/moto/cloudtrail/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudwatch/exceptions.py` & `moto-4.1.9.dev5/moto/cloudwatch/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudwatch/models.py` & `moto-4.1.9.dev5/moto/cloudwatch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cloudwatch/responses.py` & `moto-4.1.9.dev5/moto/cloudwatch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codebuild/exceptions.py` & `moto-4.1.9.dev5/moto/codebuild/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codebuild/models.py` & `moto-4.1.9.dev5/moto/codebuild/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codebuild/responses.py` & `moto-4.1.9.dev5/moto/codebuild/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codecommit/exceptions.py` & `moto-4.1.9.dev5/moto/codecommit/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codecommit/models.py` & `moto-4.1.9.dev5/moto/codecommit/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codecommit/responses.py` & `moto-4.1.9.dev5/moto/codecommit/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codepipeline/exceptions.py` & `moto-4.1.9.dev5/moto/codepipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codepipeline/models.py` & `moto-4.1.9.dev5/moto/codepipeline/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/codepipeline/responses.py` & `moto-4.1.9.dev5/moto/codepipeline/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cognitoidentity/exceptions.py` & `moto-4.1.9.dev5/moto/cognitoidentity/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cognitoidentity/models.py` & `moto-4.1.9.dev5/moto/cognitoidentity/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cognitoidentity/responses.py` & `moto-4.1.9.dev5/moto/cognitoidentity/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cognitoidp/exceptions.py` & `moto-4.1.9.dev5/moto/cognitoidp/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cognitoidp/models.py` & `moto-4.1.9.dev5/moto/cognitoidp/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cognitoidp/resources/jwks-private.json` & `moto-4.1.9.dev5/moto/cognitoidp/resources/jwks-private.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cognitoidp/responses.py` & `moto-4.1.9.dev5/moto/cognitoidp/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/cognitoidp/utils.py` & `moto-4.1.9.dev5/moto/cognitoidp/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/comprehend/models.py` & `moto-4.1.9.dev5/moto/comprehend/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/comprehend/responses.py` & `moto-4.1.9.dev5/moto/comprehend/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/config/exceptions.py` & `moto-4.1.9.dev5/moto/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/config/models.py` & `moto-4.1.9.dev5/moto/config/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/config/resources/aws_managed_rules.json` & `moto-4.1.9.dev5/moto/config/resources/aws_managed_rules.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/config/responses.py` & `moto-4.1.9.dev5/moto/config/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/core/base_backend.py` & `moto-4.1.9.dev5/moto/core/base_backend.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/core/botocore_stubber.py` & `moto-4.1.9.dev5/moto/core/botocore_stubber.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/core/common_models.py` & `moto-4.1.9.dev5/moto/core/common_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/core/custom_responses_mock.py` & `moto-4.1.9.dev5/moto/core/custom_responses_mock.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/core/exceptions.py` & `moto-4.1.9.dev5/moto/core/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 # TODO: add "<Type>Sender</Type>" to error responses below?
 
 
 SINGLE_ERROR_RESPONSE = """<?xml version="1.0" encoding="UTF-8"?>
 <Error>
     <Code>{{error_type}}</Code>
-    <Message>{{message}}</Message>
+    <Message><![CDATA[{{message}}]]></Message>
     {% block extra %}{% endblock %}
     <{{request_id_tag}}>7a62c49f-347e-4fc4-9331-6e8eEXAMPLE</{{request_id_tag}}>
 </Error>
 """
 
 WRAPPED_SINGLE_ERROR_RESPONSE = """<?xml version="1.0" encoding="UTF-8"?>
 <ErrorResponse{% if xmlns is defined %} xmlns="{{xmlns}}"{% endif %}>
     <Error>
         <Code>{{error_type}}</Code>
-        <Message>{{message}}</Message>
+        <Message><![CDATA[{{message}}]]></Message>
         {% block extra %}{% endblock %}
         <{{request_id_tag}}>7a62c49f-347e-4fc4-9331-6e8eEXAMPLE</{{request_id_tag}}>
     </Error>
 </ErrorResponse>"""
 
 ERROR_RESPONSE = """<?xml version="1.0" encoding="UTF-8"?>
   <ErrorResponse>
```

### Comparing `moto-4.1.9.dev3/moto/core/models.py` & `moto-4.1.9.dev5/moto/core/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/core/responses.py` & `moto-4.1.9.dev5/moto/core/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/core/responses_custom_registry.py` & `moto-4.1.9.dev5/moto/core/responses_custom_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/core/utils.py` & `moto-4.1.9.dev5/moto/core/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/databrew/exceptions.py` & `moto-4.1.9.dev5/moto/databrew/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/databrew/models.py` & `moto-4.1.9.dev5/moto/databrew/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/databrew/responses.py` & `moto-4.1.9.dev5/moto/databrew/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/databrew/urls.py` & `moto-4.1.9.dev5/moto/databrew/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/datapipeline/models.py` & `moto-4.1.9.dev5/moto/datapipeline/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/datapipeline/responses.py` & `moto-4.1.9.dev5/moto/datapipeline/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/datapipeline/utils.py` & `moto-4.1.9.dev5/moto/datapipeline/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/datasync/models.py` & `moto-4.1.9.dev5/moto/datasync/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/datasync/responses.py` & `moto-4.1.9.dev5/moto/datasync/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dax/exceptions.py` & `moto-4.1.9.dev5/moto/dax/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dax/models.py` & `moto-4.1.9.dev5/moto/dax/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dax/responses.py` & `moto-4.1.9.dev5/moto/dax/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dms/exceptions.py` & `moto-4.1.9.dev5/moto/dms/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dms/models.py` & `moto-4.1.9.dev5/moto/dms/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dms/responses.py` & `moto-4.1.9.dev5/moto/dms/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dms/utils.py` & `moto-4.1.9.dev5/moto/dms/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ds/exceptions.py` & `moto-4.1.9.dev5/moto/ds/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ds/models.py` & `moto-4.1.9.dev5/moto/ds/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ds/responses.py` & `moto-4.1.9.dev5/moto/ds/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ds/validations.py` & `moto-4.1.9.dev5/moto/ds/validations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/comparisons.py` & `moto-4.1.9.dev5/moto/dynamodb/comparisons.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/exceptions.py` & `moto-4.1.9.dev5/moto/dynamodb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/models/__init__.py` & `moto-4.1.9.dev5/moto/dynamodb/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/models/dynamo_type.py` & `moto-4.1.9.dev5/moto/dynamodb/models/dynamo_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/models/table.py` & `moto-4.1.9.dev5/moto/dynamodb/models/table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/parsing/ast_nodes.py` & `moto-4.1.9.dev5/moto/dynamodb/parsing/ast_nodes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/parsing/executors.py` & `moto-4.1.9.dev5/moto/dynamodb/parsing/executors.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/parsing/expressions.py` & `moto-4.1.9.dev5/moto/dynamodb/parsing/expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/parsing/key_condition_expression.py` & `moto-4.1.9.dev5/moto/dynamodb/parsing/key_condition_expression.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/parsing/reserved_keywords.py` & `moto-4.1.9.dev5/moto/dynamodb/parsing/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/parsing/reserved_keywords.txt` & `moto-4.1.9.dev5/moto/dynamodb/parsing/reserved_keywords.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/parsing/tokens.py` & `moto-4.1.9.dev5/moto/dynamodb/parsing/tokens.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/parsing/validators.py` & `moto-4.1.9.dev5/moto/dynamodb/parsing/validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb/responses.py` & `moto-4.1.9.dev5/moto/dynamodb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb_v20111205/comparisons.py` & `moto-4.1.9.dev5/moto/dynamodb_v20111205/comparisons.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb_v20111205/models.py` & `moto-4.1.9.dev5/moto/dynamodb_v20111205/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodb_v20111205/responses.py` & `moto-4.1.9.dev5/moto/dynamodb_v20111205/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodbstreams/models.py` & `moto-4.1.9.dev5/moto/dynamodbstreams/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/dynamodbstreams/responses.py` & `moto-4.1.9.dev5/moto/dynamodbstreams/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ebs/models.py` & `moto-4.1.9.dev5/moto/ebs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ebs/responses.py` & `moto-4.1.9.dev5/moto/ebs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ebs/urls.py` & `moto-4.1.9.dev5/moto/ebs/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/exceptions.py` & `moto-4.1.9.dev5/moto/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/__init__.py` & `moto-4.1.9.dev5/moto/ec2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/amis.py` & `moto-4.1.9.dev5/moto/ec2/models/amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/availability_zones_and_regions.py` & `moto-4.1.9.dev5/moto/ec2/models/availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/carrier_gateways.py` & `moto-4.1.9.dev5/moto/ec2/models/carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/core.py` & `moto-4.1.9.dev5/moto/ec2/models/core.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/customer_gateways.py` & `moto-4.1.9.dev5/moto/ec2/models/customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/dhcp_options.py` & `moto-4.1.9.dev5/moto/ec2/models/dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/elastic_block_store.py` & `moto-4.1.9.dev5/moto/ec2/models/elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/elastic_ip_addresses.py` & `moto-4.1.9.dev5/moto/ec2/models/elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/elastic_network_interfaces.py` & `moto-4.1.9.dev5/moto/ec2/models/elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/fleets.py` & `moto-4.1.9.dev5/moto/ec2/models/fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/flow_logs.py` & `moto-4.1.9.dev5/moto/ec2/models/flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/hosts.py` & `moto-4.1.9.dev5/moto/ec2/models/hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/iam_instance_profile.py` & `moto-4.1.9.dev5/moto/ec2/models/iam_instance_profile.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/instance_types.py` & `moto-4.1.9.dev5/moto/ec2/models/instance_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/instances.py` & `moto-4.1.9.dev5/moto/ec2/models/instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/internet_gateways.py` & `moto-4.1.9.dev5/moto/ec2/models/internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/key_pairs.py` & `moto-4.1.9.dev5/moto/ec2/models/key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/launch_templates.py` & `moto-4.1.9.dev5/moto/ec2/models/launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/managed_prefixes.py` & `moto-4.1.9.dev5/moto/ec2/models/managed_prefixes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/nat_gateways.py` & `moto-4.1.9.dev5/moto/ec2/models/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/network_acls.py` & `moto-4.1.9.dev5/moto/ec2/models/network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/route_tables.py` & `moto-4.1.9.dev5/moto/ec2/models/route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/security_groups.py` & `moto-4.1.9.dev5/moto/ec2/models/security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/spot_requests.py` & `moto-4.1.9.dev5/moto/ec2/models/spot_requests.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/subnets.py` & `moto-4.1.9.dev5/moto/ec2/models/subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/tags.py` & `moto-4.1.9.dev5/moto/ec2/models/tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/transit_gateway.py` & `moto-4.1.9.dev5/moto/ec2/models/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/transit_gateway_attachments.py` & `moto-4.1.9.dev5/moto/ec2/models/transit_gateway_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/transit_gateway_route_tables.py` & `moto-4.1.9.dev5/moto/ec2/models/transit_gateway_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/vpc_peering_connections.py` & `moto-4.1.9.dev5/moto/ec2/models/vpc_peering_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/vpc_service_configuration.py` & `moto-4.1.9.dev5/moto/ec2/models/vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/vpcs.py` & `moto-4.1.9.dev5/moto/ec2/models/vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/vpn_connections.py` & `moto-4.1.9.dev5/moto/ec2/models/vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/models/vpn_gateway.py` & `moto-4.1.9.dev5/moto/ec2/models/vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/amis.json` & `moto-4.1.9.dev5/moto/ec2/resources/amis.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/af-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/me-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/me-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/us-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/us-east-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/us-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/ecs/optimized_amis/us-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/af-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/me-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/me-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/us-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/us-east-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/us-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_type_offerings/region/us-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/instance_types.json` & `moto-4.1.9.dev5/moto/ec2/resources/instance_types.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/af-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-northeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-northeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-northeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-southeast-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-southeast-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ap-southeast-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/ca-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-central-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-north-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-south-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/eu-west-3.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/me-central-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/me-south-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/sa-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/us-east-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/us-east-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/us-west-1.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/resources/latest_amis/us-west-2.json` & `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/__init__.py` & `moto-4.1.9.dev5/moto/ec2/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/_base_response.py` & `moto-4.1.9.dev5/moto/ec2/responses/_base_response.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/account_attributes.py` & `moto-4.1.9.dev5/moto/ec2/responses/account_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/amis.py` & `moto-4.1.9.dev5/moto/ec2/responses/amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/availability_zones_and_regions.py` & `moto-4.1.9.dev5/moto/ec2/responses/availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/carrier_gateways.py` & `moto-4.1.9.dev5/moto/ec2/responses/carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/customer_gateways.py` & `moto-4.1.9.dev5/moto/ec2/responses/customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/dhcp_options.py` & `moto-4.1.9.dev5/moto/ec2/responses/dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/egress_only_internet_gateways.py` & `moto-4.1.9.dev5/moto/ec2/responses/egress_only_internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/elastic_block_store.py` & `moto-4.1.9.dev5/moto/ec2/responses/elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/elastic_ip_addresses.py` & `moto-4.1.9.dev5/moto/ec2/responses/elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/elastic_network_interfaces.py` & `moto-4.1.9.dev5/moto/ec2/responses/elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/fleets.py` & `moto-4.1.9.dev5/moto/ec2/responses/fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/flow_logs.py` & `moto-4.1.9.dev5/moto/ec2/responses/flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/general.py` & `moto-4.1.9.dev5/moto/ec2/responses/general.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/hosts.py` & `moto-4.1.9.dev5/moto/ec2/responses/hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/iam_instance_profiles.py` & `moto-4.1.9.dev5/moto/ec2/responses/iam_instance_profiles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/instances.py` & `moto-4.1.9.dev5/moto/ec2/responses/instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/internet_gateways.py` & `moto-4.1.9.dev5/moto/ec2/responses/internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/key_pairs.py` & `moto-4.1.9.dev5/moto/ec2/responses/key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/launch_templates.py` & `moto-4.1.9.dev5/moto/ec2/responses/launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/nat_gateways.py` & `moto-4.1.9.dev5/moto/ec2/responses/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/network_acls.py` & `moto-4.1.9.dev5/moto/ec2/responses/network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/reserved_instances.py` & `moto-4.1.9.dev5/moto/ec2/responses/reserved_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/route_tables.py` & `moto-4.1.9.dev5/moto/ec2/responses/route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/security_groups.py` & `moto-4.1.9.dev5/moto/ec2/responses/security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/settings.py` & `moto-4.1.9.dev5/moto/ec2/responses/settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/spot_fleets.py` & `moto-4.1.9.dev5/moto/ec2/responses/spot_fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/spot_instances.py` & `moto-4.1.9.dev5/moto/ec2/responses/spot_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/subnets.py` & `moto-4.1.9.dev5/moto/ec2/responses/subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/tags.py` & `moto-4.1.9.dev5/moto/ec2/responses/tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/transit_gateway_attachments.py` & `moto-4.1.9.dev5/moto/ec2/responses/transit_gateway_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/transit_gateway_route_tables.py` & `moto-4.1.9.dev5/moto/ec2/responses/transit_gateway_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/transit_gateways.py` & `moto-4.1.9.dev5/moto/ec2/responses/transit_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/virtual_private_gateways.py` & `moto-4.1.9.dev5/moto/ec2/responses/virtual_private_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/vpc_peering_connections.py` & `moto-4.1.9.dev5/moto/ec2/responses/vpc_peering_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/vpc_service_configuration.py` & `moto-4.1.9.dev5/moto/ec2/responses/vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/vpcs.py` & `moto-4.1.9.dev5/moto/ec2/responses/vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/vpn_connections.py` & `moto-4.1.9.dev5/moto/ec2/responses/vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/responses/windows.py` & `moto-4.1.9.dev5/moto/ec2/responses/windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2/utils.py` & `moto-4.1.9.dev5/moto/ec2/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ec2instanceconnect/responses.py` & `moto-4.1.9.dev5/moto/ec2instanceconnect/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ecr/exceptions.py` & `moto-4.1.9.dev5/moto/ecr/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ecr/models.py` & `moto-4.1.9.dev5/moto/ecr/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ecr/policy_validation.py` & `moto-4.1.9.dev5/moto/ecr/policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ecr/responses.py` & `moto-4.1.9.dev5/moto/ecr/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ecs/exceptions.py` & `moto-4.1.9.dev5/moto/ecs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ecs/models.py` & `moto-4.1.9.dev5/moto/ecs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ecs/responses.py` & `moto-4.1.9.dev5/moto/ecs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/efs/exceptions.py` & `moto-4.1.9.dev5/moto/efs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/efs/models.py` & `moto-4.1.9.dev5/moto/efs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/efs/responses.py` & `moto-4.1.9.dev5/moto/efs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/efs/urls.py` & `moto-4.1.9.dev5/moto/efs/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/eks/exceptions.py` & `moto-4.1.9.dev5/moto/eks/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/eks/models.py` & `moto-4.1.9.dev5/moto/eks/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/eks/responses.py` & `moto-4.1.9.dev5/moto/eks/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/eks/urls.py` & `moto-4.1.9.dev5/moto/eks/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/eks/utils.py` & `moto-4.1.9.dev5/moto/eks/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elasticache/exceptions.py` & `moto-4.1.9.dev5/moto/elasticache/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elasticache/models.py` & `moto-4.1.9.dev5/moto/elasticache/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elasticache/responses.py` & `moto-4.1.9.dev5/moto/elasticache/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elasticbeanstalk/models.py` & `moto-4.1.9.dev5/moto/elasticbeanstalk/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elasticbeanstalk/responses.py` & `moto-4.1.9.dev5/moto/elasticbeanstalk/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elastictranscoder/models.py` & `moto-4.1.9.dev5/moto/elastictranscoder/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elastictranscoder/responses.py` & `moto-4.1.9.dev5/moto/elastictranscoder/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elb/exceptions.py` & `moto-4.1.9.dev5/moto/elb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elb/models.py` & `moto-4.1.9.dev5/moto/elb/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elb/policies.py` & `moto-4.1.9.dev5/moto/elb/policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elb/responses.py` & `moto-4.1.9.dev5/moto/elb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elb/urls.py` & `moto-4.1.9.dev5/moto/elb/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elbv2/exceptions.py` & `moto-4.1.9.dev5/moto/elbv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elbv2/models.py` & `moto-4.1.9.dev5/moto/elbv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/elbv2/responses.py` & `moto-4.1.9.dev5/moto/elbv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emr/models.py` & `moto-4.1.9.dev5/moto/emr/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emr/responses.py` & `moto-4.1.9.dev5/moto/emr/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emr/utils.py` & `moto-4.1.9.dev5/moto/emr/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emrcontainers/models.py` & `moto-4.1.9.dev5/moto/emrcontainers/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emrcontainers/responses.py` & `moto-4.1.9.dev5/moto/emrcontainers/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emrcontainers/urls.py` & `moto-4.1.9.dev5/moto/emrcontainers/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emrcontainers/utils.py` & `moto-4.1.9.dev5/moto/emrcontainers/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emrserverless/models.py` & `moto-4.1.9.dev5/moto/emrserverless/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emrserverless/responses.py` & `moto-4.1.9.dev5/moto/emrserverless/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emrserverless/urls.py` & `moto-4.1.9.dev5/moto/emrserverless/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/emrserverless/utils.py` & `moto-4.1.9.dev5/moto/emrserverless/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/es/exceptions.py` & `moto-4.1.9.dev5/moto/es/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/es/models.py` & `moto-4.1.9.dev5/moto/es/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/es/responses.py` & `moto-4.1.9.dev5/moto/es/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/es/urls.py` & `moto-4.1.9.dev5/moto/es/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/events/exceptions.py` & `moto-4.1.9.dev5/moto/events/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/events/models.py` & `moto-4.1.9.dev5/moto/events/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/events/notifications.py` & `moto-4.1.9.dev5/moto/events/notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/events/responses.py` & `moto-4.1.9.dev5/moto/events/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/firehose/exceptions.py` & `moto-4.1.9.dev5/moto/firehose/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/firehose/models.py` & `moto-4.1.9.dev5/moto/firehose/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/firehose/responses.py` & `moto-4.1.9.dev5/moto/firehose/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/forecast/exceptions.py` & `moto-4.1.9.dev5/moto/forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/forecast/models.py` & `moto-4.1.9.dev5/moto/forecast/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/forecast/responses.py` & `moto-4.1.9.dev5/moto/forecast/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glacier/models.py` & `moto-4.1.9.dev5/moto/glacier/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glacier/responses.py` & `moto-4.1.9.dev5/moto/glacier/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glacier/urls.py` & `moto-4.1.9.dev5/moto/glacier/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glue/exceptions.py` & `moto-4.1.9.dev5/moto/glue/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glue/glue_schema_registry_constants.py` & `moto-4.1.9.dev5/moto/glue/glue_schema_registry_constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glue/glue_schema_registry_utils.py` & `moto-4.1.9.dev5/moto/glue/glue_schema_registry_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glue/models.py` & `moto-4.1.9.dev5/moto/glue/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glue/responses.py` & `moto-4.1.9.dev5/moto/glue/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/glue/utils.py` & `moto-4.1.9.dev5/moto/glue/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/greengrass/exceptions.py` & `moto-4.1.9.dev5/moto/greengrass/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/greengrass/models.py` & `moto-4.1.9.dev5/moto/greengrass/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/greengrass/responses.py` & `moto-4.1.9.dev5/moto/greengrass/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/greengrass/urls.py` & `moto-4.1.9.dev5/moto/greengrass/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/guardduty/exceptions.py` & `moto-4.1.9.dev5/moto/guardduty/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/guardduty/models.py` & `moto-4.1.9.dev5/moto/guardduty/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/guardduty/responses.py` & `moto-4.1.9.dev5/moto/guardduty/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/guardduty/urls.py` & `moto-4.1.9.dev5/moto/guardduty/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iam/access_control.py` & `moto-4.1.9.dev5/moto/iam/access_control.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iam/aws_managed_policies.py` & `moto-4.1.9.dev5/moto/iam/aws_managed_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iam/config.py` & `moto-4.1.9.dev5/moto/iam/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iam/exceptions.py` & `moto-4.1.9.dev5/moto/iam/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iam/models.py` & `moto-4.1.9.dev5/moto/iam/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iam/policy_validation.py` & `moto-4.1.9.dev5/moto/iam/policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iam/responses.py` & `moto-4.1.9.dev5/moto/iam/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iam/utils.py` & `moto-4.1.9.dev5/moto/iam/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/identitystore/models.py` & `moto-4.1.9.dev5/moto/identitystore/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/identitystore/responses.py` & `moto-4.1.9.dev5/moto/identitystore/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/instance_metadata/responses.py` & `moto-4.1.9.dev5/moto/instance_metadata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iot/exceptions.py` & `moto-4.1.9.dev5/moto/iot/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iot/models.py` & `moto-4.1.9.dev5/moto/iot/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iot/responses.py` & `moto-4.1.9.dev5/moto/iot/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iot/urls.py` & `moto-4.1.9.dev5/moto/iot/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iotdata/exceptions.py` & `moto-4.1.9.dev5/moto/iotdata/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iotdata/models.py` & `moto-4.1.9.dev5/moto/iotdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/iotdata/responses.py` & `moto-4.1.9.dev5/moto/iotdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesis/exceptions.py` & `moto-4.1.9.dev5/moto/kinesis/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesis/models.py` & `moto-4.1.9.dev5/moto/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesis/responses.py` & `moto-4.1.9.dev5/moto/kinesis/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesis/urls.py` & `moto-4.1.9.dev5/moto/kinesis/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesis/utils.py` & `moto-4.1.9.dev5/moto/kinesis/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesisvideo/exceptions.py` & `moto-4.1.9.dev5/moto/kinesisvideo/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesisvideo/models.py` & `moto-4.1.9.dev5/moto/kinesisvideo/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesisvideo/responses.py` & `moto-4.1.9.dev5/moto/kinesisvideo/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesisvideoarchivedmedia/models.py` & `moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kinesisvideoarchivedmedia/responses.py` & `moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kms/exceptions.py` & `moto-4.1.9.dev5/moto/kms/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kms/models.py` & `moto-4.1.9.dev5/moto/kms/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kms/policy_validator.py` & `moto-4.1.9.dev5/moto/kms/policy_validator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kms/responses.py` & `moto-4.1.9.dev5/moto/kms/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/kms/utils.py` & `moto-4.1.9.dev5/moto/kms/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/lakeformation/models.py` & `moto-4.1.9.dev5/moto/lakeformation/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/lakeformation/responses.py` & `moto-4.1.9.dev5/moto/lakeformation/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/lakeformation/urls.py` & `moto-4.1.9.dev5/moto/lakeformation/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/logs/exceptions.py` & `moto-4.1.9.dev5/moto/logs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/logs/metric_filters.py` & `moto-4.1.9.dev5/moto/logs/metric_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/logs/models.py` & `moto-4.1.9.dev5/moto/logs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/logs/responses.py` & `moto-4.1.9.dev5/moto/logs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/logs/utils.py` & `moto-4.1.9.dev5/moto/logs/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/managedblockchain/exceptions.py` & `moto-4.1.9.dev5/moto/managedblockchain/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/managedblockchain/models.py` & `moto-4.1.9.dev5/moto/managedblockchain/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/managedblockchain/responses.py` & `moto-4.1.9.dev5/moto/managedblockchain/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/managedblockchain/urls.py` & `moto-4.1.9.dev5/moto/managedblockchain/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/managedblockchain/utils.py` & `moto-4.1.9.dev5/moto/managedblockchain/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediaconnect/models.py` & `moto-4.1.9.dev5/moto/mediaconnect/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediaconnect/responses.py` & `moto-4.1.9.dev5/moto/mediaconnect/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediaconnect/urls.py` & `moto-4.1.9.dev5/moto/mediaconnect/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/medialive/models.py` & `moto-4.1.9.dev5/moto/medialive/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/medialive/responses.py` & `moto-4.1.9.dev5/moto/medialive/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/medialive/urls.py` & `moto-4.1.9.dev5/moto/medialive/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediapackage/models.py` & `moto-4.1.9.dev5/moto/mediapackage/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediapackage/responses.py` & `moto-4.1.9.dev5/moto/mediapackage/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediastore/exceptions.py` & `moto-4.1.9.dev5/moto/mediastore/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediastore/models.py` & `moto-4.1.9.dev5/moto/mediastore/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediastore/responses.py` & `moto-4.1.9.dev5/moto/mediastore/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediastoredata/models.py` & `moto-4.1.9.dev5/moto/mediastoredata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mediastoredata/responses.py` & `moto-4.1.9.dev5/moto/mediastoredata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/meteringmarketplace/models.py` & `moto-4.1.9.dev5/moto/meteringmarketplace/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/meteringmarketplace/responses.py` & `moto-4.1.9.dev5/moto/meteringmarketplace/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_api/_internal/managed_state_model.py` & `moto-4.1.9.dev5/moto/moto_api/_internal/managed_state_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_api/_internal/models.py` & `moto-4.1.9.dev5/moto/moto_api/_internal/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_api/_internal/moto_random.py` & `moto-4.1.9.dev5/moto/moto_api/_internal/moto_random.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_api/_internal/recorder/models.py` & `moto-4.1.9.dev5/moto/moto_api/_internal/recorder/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_api/_internal/recorder/responses.py` & `moto-4.1.9.dev5/moto/moto_api/_internal/recorder/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_api/_internal/responses.py` & `moto-4.1.9.dev5/moto/moto_api/_internal/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_api/_internal/state_manager.py` & `moto-4.1.9.dev5/moto/moto_api/_internal/state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_api/_internal/urls.py` & `moto-4.1.9.dev5/moto/moto_api/_internal/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_server/templates/dashboard.html` & `moto-4.1.9.dev5/moto/moto_server/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_server/threaded_moto_server.py` & `moto-4.1.9.dev5/moto/moto_server/threaded_moto_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_server/utilities.py` & `moto-4.1.9.dev5/moto/moto_server/utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/moto_server/werkzeug_app.py` & `moto-4.1.9.dev5/moto/moto_server/werkzeug_app.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mq/configuration.py` & `moto-4.1.9.dev5/moto/mq/configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mq/exceptions.py` & `moto-4.1.9.dev5/moto/mq/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mq/models.py` & `moto-4.1.9.dev5/moto/mq/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mq/responses.py` & `moto-4.1.9.dev5/moto/mq/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/mq/urls.py` & `moto-4.1.9.dev5/moto/mq/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/neptune/exceptions.py` & `moto-4.1.9.dev5/moto/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/neptune/models.py` & `moto-4.1.9.dev5/moto/neptune/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/neptune/responses.py` & `moto-4.1.9.dev5/moto/neptune/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/opensearch/data.py` & `moto-4.1.9.dev5/moto/opensearch/data.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/opensearch/models.py` & `moto-4.1.9.dev5/moto/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/opensearch/responses.py` & `moto-4.1.9.dev5/moto/opensearch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/opsworks/models.py` & `moto-4.1.9.dev5/moto/opsworks/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/opsworks/responses.py` & `moto-4.1.9.dev5/moto/opsworks/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/organizations/exceptions.py` & `moto-4.1.9.dev5/moto/organizations/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/organizations/models.py` & `moto-4.1.9.dev5/moto/organizations/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/organizations/responses.py` & `moto-4.1.9.dev5/moto/organizations/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/organizations/utils.py` & `moto-4.1.9.dev5/moto/organizations/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/packages/boto/ec2/blockdevicemapping.py` & `moto-4.1.9.dev5/moto/packages/boto/ec2/blockdevicemapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/packages/boto/ec2/ec2object.py` & `moto-4.1.9.dev5/moto/packages/boto/ec2/ec2object.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/packages/boto/ec2/image.py` & `moto-4.1.9.dev5/moto/packages/boto/ec2/image.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/packages/boto/ec2/instance.py` & `moto-4.1.9.dev5/moto/packages/boto/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/packages/boto/ec2/instancetype.py` & `moto-4.1.9.dev5/moto/packages/boto/ec2/instancetype.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/packages/boto/ec2/tag.py` & `moto-4.1.9.dev5/moto/packages/boto/ec2/tag.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/packages/cfnresponse/cfnresponse.py` & `moto-4.1.9.dev5/moto/packages/cfnresponse/cfnresponse.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/personalize/models.py` & `moto-4.1.9.dev5/moto/personalize/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/personalize/responses.py` & `moto-4.1.9.dev5/moto/personalize/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/pinpoint/models.py` & `moto-4.1.9.dev5/moto/pinpoint/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/pinpoint/responses.py` & `moto-4.1.9.dev5/moto/pinpoint/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/pinpoint/urls.py` & `moto-4.1.9.dev5/moto/pinpoint/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/polly/models.py` & `moto-4.1.9.dev5/moto/polly/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/polly/resources.py` & `moto-4.1.9.dev5/moto/polly/resources.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/polly/responses.py` & `moto-4.1.9.dev5/moto/polly/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/quicksight/models.py` & `moto-4.1.9.dev5/moto/quicksight/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/quicksight/responses.py` & `moto-4.1.9.dev5/moto/quicksight/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/quicksight/urls.py` & `moto-4.1.9.dev5/moto/quicksight/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ram/exceptions.py` & `moto-4.1.9.dev5/moto/ram/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ram/models.py` & `moto-4.1.9.dev5/moto/ram/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ram/responses.py` & `moto-4.1.9.dev5/moto/ram/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rds/exceptions.py` & `moto-4.1.9.dev5/moto/rds/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rds/models.py` & `moto-4.1.9.dev5/moto/rds/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rds/resources/cluster_options/aurora-postgresql.json` & `moto-4.1.9.dev5/moto/rds/resources/cluster_options/aurora-postgresql.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rds/resources/cluster_options/neptune.json` & `moto-4.1.9.dev5/moto/rds/resources/cluster_options/neptune.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rds/responses.py` & `moto-4.1.9.dev5/moto/rds/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rds/utils.py` & `moto-4.1.9.dev5/moto/rds/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rdsdata/models.py` & `moto-4.1.9.dev5/moto/rdsdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rdsdata/responses.py` & `moto-4.1.9.dev5/moto/rdsdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/redshift/exceptions.py` & `moto-4.1.9.dev5/moto/redshift/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/redshift/models.py` & `moto-4.1.9.dev5/moto/redshift/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/redshift/responses.py` & `moto-4.1.9.dev5/moto/redshift/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/redshiftdata/models.py` & `moto-4.1.9.dev5/moto/redshiftdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/redshiftdata/responses.py` & `moto-4.1.9.dev5/moto/redshiftdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rekognition/models.py` & `moto-4.1.9.dev5/moto/rekognition/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/rekognition/responses.py` & `moto-4.1.9.dev5/moto/rekognition/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/resourcegroups/models.py` & `moto-4.1.9.dev5/moto/resourcegroups/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/resourcegroups/responses.py` & `moto-4.1.9.dev5/moto/resourcegroups/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/resourcegroups/urls.py` & `moto-4.1.9.dev5/moto/resourcegroups/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/resourcegroupstaggingapi/models.py` & `moto-4.1.9.dev5/moto/resourcegroupstaggingapi/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/resourcegroupstaggingapi/responses.py` & `moto-4.1.9.dev5/moto/resourcegroupstaggingapi/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53/exceptions.py` & `moto-4.1.9.dev5/moto/route53/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53/models.py` & `moto-4.1.9.dev5/moto/route53/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53/responses.py` & `moto-4.1.9.dev5/moto/route53/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53/urls.py` & `moto-4.1.9.dev5/moto/route53/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53resolver/exceptions.py` & `moto-4.1.9.dev5/moto/route53resolver/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53resolver/models.py` & `moto-4.1.9.dev5/moto/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53resolver/responses.py` & `moto-4.1.9.dev5/moto/route53resolver/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53resolver/utils.py` & `moto-4.1.9.dev5/moto/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/route53resolver/validations.py` & `moto-4.1.9.dev5/moto/route53resolver/validations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/cloud_formation.py` & `moto-4.1.9.dev5/moto/s3/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/config.py` & `moto-4.1.9.dev5/moto/s3/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/exceptions.py` & `moto-4.1.9.dev5/moto/s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/models.py` & `moto-4.1.9.dev5/moto/s3/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/notifications.py` & `moto-4.1.9.dev5/moto/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/responses.py` & `moto-4.1.9.dev5/moto/s3/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/select_object_content.py` & `moto-4.1.9.dev5/moto/s3/select_object_content.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/urls.py` & `moto-4.1.9.dev5/moto/s3/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3/utils.py` & `moto-4.1.9.dev5/moto/s3/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3control/config.py` & `moto-4.1.9.dev5/moto/s3control/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3control/exceptions.py` & `moto-4.1.9.dev5/moto/s3control/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3control/models.py` & `moto-4.1.9.dev5/moto/s3control/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3control/responses.py` & `moto-4.1.9.dev5/moto/s3control/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/s3control/urls.py` & `moto-4.1.9.dev5/moto/s3control/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sagemaker/exceptions.py` & `moto-4.1.9.dev5/moto/sagemaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sagemaker/models.py` & `moto-4.1.9.dev5/moto/sagemaker/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sagemaker/responses.py` & `moto-4.1.9.dev5/moto/sagemaker/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sagemaker/utils.py` & `moto-4.1.9.dev5/moto/sagemaker/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sagemaker/validators.py` & `moto-4.1.9.dev5/moto/sagemaker/validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/scheduler/models.py` & `moto-4.1.9.dev5/moto/scheduler/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/scheduler/responses.py` & `moto-4.1.9.dev5/moto/scheduler/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/scheduler/urls.py` & `moto-4.1.9.dev5/moto/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sdb/exceptions.py` & `moto-4.1.9.dev5/moto/sdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sdb/models.py` & `moto-4.1.9.dev5/moto/sdb/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sdb/responses.py` & `moto-4.1.9.dev5/moto/sdb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/secretsmanager/exceptions.py` & `moto-4.1.9.dev5/moto/secretsmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/secretsmanager/list_secrets/filters.py` & `moto-4.1.9.dev5/moto/secretsmanager/list_secrets/filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/secretsmanager/models.py` & `moto-4.1.9.dev5/moto/secretsmanager/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/secretsmanager/responses.py` & `moto-4.1.9.dev5/moto/secretsmanager/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/secretsmanager/utils.py` & `moto-4.1.9.dev5/moto/secretsmanager/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/server.py` & `moto-4.1.9.dev5/moto/server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/servicediscovery/exceptions.py` & `moto-4.1.9.dev5/moto/servicediscovery/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/servicediscovery/models.py` & `moto-4.1.9.dev5/moto/servicediscovery/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/servicediscovery/responses.py` & `moto-4.1.9.dev5/moto/servicediscovery/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/servicequotas/models.py` & `moto-4.1.9.dev5/moto/servicequotas/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/servicequotas/resources/default_quotas/vpc.py` & `moto-4.1.9.dev5/moto/servicequotas/resources/default_quotas/vpc.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/servicequotas/responses.py` & `moto-4.1.9.dev5/moto/servicequotas/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ses/exceptions.py` & `moto-4.1.9.dev5/moto/ses/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ses/feedback.py` & `moto-4.1.9.dev5/moto/ses/feedback.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ses/models.py` & `moto-4.1.9.dev5/moto/ses/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ses/responses.py` & `moto-4.1.9.dev5/moto/ses/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ses/template.py` & `moto-4.1.9.dev5/moto/ses/template.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ses/utils.py` & `moto-4.1.9.dev5/moto/ses/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/settings.py` & `moto-4.1.9.dev5/moto/settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/signer/models.py` & `moto-4.1.9.dev5/moto/signer/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/signer/responses.py` & `moto-4.1.9.dev5/moto/signer/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sns/exceptions.py` & `moto-4.1.9.dev5/moto/sns/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sns/models.py` & `moto-4.1.9.dev5/moto/sns/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -297,18 +297,19 @@
                             if not isinstance(attribute_values, list):
                                 attribute_values = [attribute_values]
                         except (ValueError, TypeError):
                             return False
                     else:
                         return False
 
-                    for attribute_values in attribute_values:
+                    for attribute_value in attribute_values:
+                        attribute_value = float(attribute_value)
                         # Even the official documentation states a 5 digits of accuracy after the decimal point for numerics, in reality it is 6
                         # https://docs.aws.amazon.com/sns/latest/dg/sns-subscription-filter-policies.html#subscription-filter-policy-constraints
-                        if int(attribute_values * 1000000) == int(rule * 1000000):
+                        if int(attribute_value * 1000000) == int(rule * 1000000):
                             return True
                 if isinstance(rule, dict):
                     keyword = list(rule.keys())[0]
                     value = list(rule.values())[0]
                     if keyword == "exists":
                         if value and field in message_attributes:
                             return True
@@ -343,44 +344,43 @@
                             ):
                                 return True
                         else:
                             undesired_values = (
                                 [value] if isinstance(value, str) else value
                             )
                             if attr["Type"] == "Number":
-                                actual_values = [str(attr["Value"])]
+                                actual_values = [float(attr["Value"])]
                             elif attr["Type"] == "String":
                                 actual_values = [attr["Value"]]
                             else:
                                 actual_values = [v for v in attr["Value"]]
                             if all([v not in undesired_values for v in actual_values]):
                                 return True
                     elif keyword == "numeric" and isinstance(value, list):
                         # [(< x), (=, y), (>=, z)]
                         numeric_ranges = zip(value[0::2], value[1::2])
                         if (
                             message_attributes.get(field, {}).get("Type", "")
                             == "Number"
                         ):
-                            msg_value = message_attributes[field]["Value"]
+                            msg_value = float(message_attributes[field]["Value"])
                             matches = []
                             for operator, test_value in numeric_ranges:
-                                test_value = int(test_value)
+                                test_value = test_value
                                 if operator == ">":
                                     matches.append((msg_value > test_value))
                                 if operator == ">=":
                                     matches.append((msg_value >= test_value))
                                 if operator == "=":
                                     matches.append((msg_value == test_value))
                                 if operator == "<":
                                     matches.append((msg_value < test_value))
                                 if operator == "<=":
                                     matches.append((msg_value <= test_value))
                             return all(matches)
-                        attr = message_attributes[field]
             return False
 
         return all(
             _field_match(field, rules, message_attributes)
             for field, rules in self._filter_policy.items()
         )
 
@@ -828,14 +828,78 @@
                     elif keyword == "exists":
                         if not isinstance(attributes, bool):
                             raise SNSInvalidParameter(
                                 "Invalid parameter: FilterPolicy: exists match pattern must be either true or false."
                             )
                         continue
                     elif keyword == "numeric":
+                        # TODO: All of the exceptions listed below contain column pointing where the error is (in AWS response)
+                        # Example: 'Value of < must be numeric\n at [Source: (String)"{"price":[{"numeric":["<","100"]}]}"; line: 1, column: 28]'
+                        # While it probably can be implemented, it doesn't feel as important as the general parameter checking
+
+                        attributes_copy = attributes[:]
+                        if not attributes_copy:
+                            raise SNSInvalidParameter(
+                                "Invalid parameter: Attributes Reason: FilterPolicy: Invalid member in numeric match: ]\n at ..."
+                            )
+
+                        operator = attributes_copy.pop(0)
+
+                        if not isinstance(operator, str):
+                            raise SNSInvalidParameter(
+                                f"Invalid parameter: Attributes Reason: FilterPolicy: Invalid member in numeric match: {(str(operator))}\n at ..."
+                            )
+
+                        if operator not in ("<", "<=", "=", ">", ">="):
+                            raise SNSInvalidParameter(
+                                f"Invalid parameter: Attributes Reason: FilterPolicy: Unrecognized numeric range operator: {(str(operator))}\n at ..."
+                            )
+
+                        try:
+                            value = attributes_copy.pop(0)
+                        except IndexError:
+                            value = None
+
+                        if value is None or not isinstance(value, (int, float)):
+                            raise SNSInvalidParameter(
+                                f"Invalid parameter: Attributes Reason: FilterPolicy: Value of {(str(operator))} must be numeric\n at ..."
+                            )
+
+                        if not attributes_copy:
+                            continue
+
+                        if operator not in (">", ">="):
+                            raise SNSInvalidParameter(
+                                "Invalid parameter: Attributes Reason: FilterPolicy: Too many elements in numeric expression\n at ..."
+                            )
+
+                        second_operator = attributes_copy.pop(0)
+
+                        if second_operator not in ("<", "<="):
+                            raise SNSInvalidParameter(
+                                f"Invalid parameter: Attributes Reason: FilterPolicy: Bad numeric range operator: {(str(second_operator))}\n at ..."
+                            )
+
+                        try:
+                            second_value = attributes_copy.pop(0)
+                        except IndexError:
+                            second_value = None
+
+                        if second_value is None or not isinstance(
+                            second_value, (int, float)
+                        ):
+                            raise SNSInvalidParameter(
+                                f"Invalid parameter: Attributes Reason: FilterPolicy: Value of {(str(second_operator))} must be numeric\n at ..."
+                            )
+
+                        if second_value <= value:
+                            raise SNSInvalidParameter(
+                                "Invalid parameter: Attributes Reason: FilterPolicy: Bottom must be less than top\n at ..."
+                            )
+
                         continue
                     elif keyword == "prefix":
                         continue
                     else:
                         raise SNSInvalidParameter(
                             f"Invalid parameter: FilterPolicy: Unrecognized match type {keyword}"
                         )
```

### Comparing `moto-4.1.9.dev3/moto/sns/responses.py` & `moto-4.1.9.dev5/moto/sns/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,28 +62,27 @@
                     f"The message attribute '{name}' has an invalid message "
                     "attribute type, the set of supported type prefixes is "
                     "Binary, Number, and String."
                 )
 
             transform_value = None
             if "StringValue" in value:
+                transform_value = value["StringValue"]
                 if data_type == "Number":
                     try:
-                        transform_value = int(value["StringValue"])
+                        int(transform_value)
                     except ValueError:
                         try:
-                            transform_value = float(value["StringValue"])
+                            float(transform_value)
                         except ValueError:
                             raise InvalidParameterValue(
                                 "An error occurred (ParameterValueInvalid) "
                                 "when calling the Publish operation: "
                                 f"Could not cast message attribute '{name}' value to number."
                             )
-                else:
-                    transform_value = value["StringValue"]
             elif "BinaryValue" in value:
                 transform_value = value["BinaryValue"]
             if transform_value == "":
                 raise InvalidParameterValue(
                     f"The message attribute '{name}' must contain non-empty "
                     "message attribute value for message attribute "
                     f"type '{data_type[0]}'."
```

### Comparing `moto-4.1.9.dev3/moto/sqs/exceptions.py` & `moto-4.1.9.dev5/moto/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sqs/models.py` & `moto-4.1.9.dev5/moto/sqs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sqs/responses.py` & `moto-4.1.9.dev5/moto/sqs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sqs/utils.py` & `moto-4.1.9.dev5/moto/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/exceptions.py` & `moto-4.1.9.dev5/moto/ssm/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,141 +1,141 @@
 from moto.core.exceptions import JsonRESTError
 
 
 class InvalidFilterKey(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidFilterKey", message)
 
 
 class InvalidFilterOption(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidFilterOption", message)
 
 
 class InvalidFilterValue(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidFilterValue", message)
 
 
 class InvalidResourceId(JsonRESTError):
     code = 400
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("InvalidResourceId", "Invalid Resource Id")
 
 
 class InvalidResourceType(JsonRESTError):
     code = 400
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("InvalidResourceType", "Invalid Resource Type")
 
 
 class ParameterNotFound(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("ParameterNotFound", message)
 
 
 class ParameterVersionNotFound(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("ParameterVersionNotFound", message)
 
 
 class ParameterVersionLabelLimitExceeded(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("ParameterVersionLabelLimitExceeded", message)
 
 
 class ValidationException(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("ValidationException", message)
 
 
 class DocumentAlreadyExists(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("DocumentAlreadyExists", message)
 
 
 class DocumentPermissionLimit(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("DocumentPermissionLimit", message)
 
 
 class InvalidPermissionType(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidPermissionType", message)
 
 
 class InvalidDocument(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidDocument", message)
 
 
 class InvalidDocumentOperation(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidDocumentOperation", message)
 
 
 class AccessDeniedException(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("AccessDeniedException", message)
 
 
 class InvalidDocumentContent(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidDocumentContent", message)
 
 
 class InvalidDocumentVersion(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidDocumentVersion", message)
 
 
 class DuplicateDocumentVersionName(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("DuplicateDocumentVersionName", message)
 
 
 class DuplicateDocumentContent(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("DuplicateDocumentContent", message)
 
 
 class ParameterMaxVersionLimitExceeded(JsonRESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("ParameterMaxVersionLimitExceeded", message)
```

### Comparing `moto-4.1.9.dev3/moto/ssm/models.py` & `moto-4.1.9.dev5/moto/ssm/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from dataclasses import dataclass
-from typing import Dict
+from typing import Any, Dict, List, Iterator, Optional, Tuple
+from typing import DefaultDict
 
 from collections import defaultdict
 
 from moto.core import BaseBackend, BackendDict, BaseModel, CloudFormationModel
 from moto.core.exceptions import RESTError
 from moto.ec2 import ec2_backends
 from moto.secretsmanager import secretsmanager_backends
@@ -38,27 +39,27 @@
     DocumentPermissionLimit,
     InvalidPermissionType,
     InvalidResourceId,
     InvalidResourceType,
 )
 
 
-class ParameterDict(defaultdict):
-    def __init__(self, account_id, region_name):
-        # each value is a list of all of the versions for a parameter
+class ParameterDict(DefaultDict[str, List["Parameter"]]):
+    def __init__(self, account_id: str, region_name: str):
+        # each value is a list of all the versions for a parameter
         # to get the current value, grab the last item of the list
         super().__init__(list)
         self.latest_amis_loaded = False
         self.latest_region_defaults_loaded = False
         self.latest_service_defaults_loaded = False
         self.latest_ecs_amis_loaded = False
         self.account_id = account_id
         self.region_name = region_name
 
-    def _check_loading_status(self, key):
+    def _check_loading_status(self, key: str) -> None:
         key = str(key or "")
         if key.startswith("/aws/service/ami-amazon-linux-latest"):
             if not self.latest_amis_loaded:
                 self._load_latest_amis()
                 self.latest_amis_loaded = True
         if key.startswith("/aws/service/global-infrastructure/regions"):
             if not self.latest_region_defaults_loaded:
@@ -71,15 +72,15 @@
         if key.startswith("/aws/service/ecs/optimized-ami"):
             if not self.latest_ecs_amis_loaded:
                 self._load_tree_parameters(
                     f"resources/ecs/optimized_amis/{self.region_name}.json"
                 )
                 self.latest_ecs_amis_loaded = True
 
-    def _load_latest_amis(self):
+    def _load_latest_amis(self) -> None:
         try:
             latest_amis_linux = load_resource(
                 __name__, f"resources/ami-amazon-linux-latest/{self.region_name}.json"
             )
         except FileNotFoundError:
             latest_amis_linux = []
         for param in latest_amis_linux:
@@ -95,15 +96,15 @@
                     keyid=None,
                     last_modified_date=param["LastModifiedDate"],
                     version=param["Version"],
                     data_type=param["DataType"],
                 )
             )
 
-    def _load_tree_parameters(self, path: str):
+    def _load_tree_parameters(self, path: str) -> None:
         try:
             params = convert_to_params(load_resource(__name__, path))
         except FileNotFoundError:
             params = []
 
         for param in params:
             last_modified_date = time.time()
@@ -123,15 +124,15 @@
                     keyid=None,
                     last_modified_date=last_modified_date,
                     version=version,
                     data_type="text",
                 )
             )
 
-    def _get_secretsmanager_parameter(self, secret_name):
+    def _get_secretsmanager_parameter(self, secret_name: str) -> List["Parameter"]:
         secrets_backend = secretsmanager_backends[self.account_id][self.region_name]
         secret = secrets_backend.describe_secret(secret_name)
         version_id_to_stage = secret["VersionIdsToStages"]
         # Sort version ID's so that AWSCURRENT is last
         sorted_version_ids = [
             k for k in version_id_to_stage if "AWSCURRENT" not in version_id_to_stage[k]
         ] + [k for k in version_id_to_stage if "AWSCURRENT" in version_id_to_stage[k]]
@@ -157,33 +158,33 @@
                 data_type="text",
                 labels=[val.get("VersionId")] + val.get("VersionStages", []),
                 source_result=json.dumps(secret),
             )
             for val in values
         ]
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: str) -> List["Parameter"]:
         if item.startswith("/aws/reference/secretsmanager/"):
             return self._get_secretsmanager_parameter("/".join(item.split("/")[4:]))
         self._check_loading_status(item)
         return super().__getitem__(item)
 
-    def __contains__(self, k):
+    def __contains__(self, k: str) -> bool:  # type: ignore[override]
         if k and k.startswith("/aws/reference/secretsmanager/"):
             try:
                 param = self._get_secretsmanager_parameter("/".join(k.split("/")[4:]))
                 return param is not None
             except SecretsManagerClientError:
                 raise ParameterNotFound(
                     f"An error occurred (ParameterNotFound) when referencing Secrets Manager: Secret {k} not found."
                 )
         self._check_loading_status(k)
         return super().__contains__(k)
 
-    def get_keys_beginning_with(self, path, recursive):
+    def get_keys_beginning_with(self, path: str, recursive: bool) -> Iterator[str]:
         self._check_loading_status(path)
         for param_name in self:
             if path != "/" and not param_name.startswith(path):
                 continue
             if "/" in param_name[len(path) + 1 :] and not recursive:
                 continue
             yield param_name
@@ -192,27 +193,27 @@
 PARAMETER_VERSION_LIMIT = 100
 PARAMETER_HISTORY_MAX_RESULTS = 50
 
 
 class Parameter(CloudFormationModel):
     def __init__(
         self,
-        account_id,
-        name,
-        value,
-        parameter_type,
-        description,
-        allowed_pattern,
-        keyid,
-        last_modified_date,
-        version,
-        data_type,
-        tags=None,
-        labels=None,
-        source_result=None,
+        account_id: str,
+        name: str,
+        value: str,
+        parameter_type: str,
+        description: Optional[str],
+        allowed_pattern: Optional[str],
+        keyid: Optional[str],
+        last_modified_date: float,
+        version: int,
+        data_type: str,
+        tags: Optional[List[Dict[str, str]]] = None,
+        labels: Optional[List[str]] = None,
+        source_result: Optional[str] = None,
     ):
         self.account_id = account_id
         self.name = name
         self.type = parameter_type
         self.description = description
         self.allowed_pattern = allowed_pattern
         self.keyid = keyid
@@ -227,27 +228,30 @@
             if not self.keyid:
                 self.keyid = "alias/aws/ssm"
 
             self.value = self.encrypt(value)
         else:
             self.value = value
 
-    def encrypt(self, value):
+    def encrypt(self, value: str) -> str:
         return f"kms:{self.keyid}:" + value
 
-    def decrypt(self, value):
+    def decrypt(self, value: str) -> Optional[str]:
         if self.type != "SecureString":
             return value
 
         prefix = f"kms:{self.keyid or 'default'}:"
         if value.startswith(prefix):
             return value[len(prefix) :]
+        return None
 
-    def response_object(self, decrypt=False, region=None):
-        r = {
+    def response_object(
+        self, decrypt: bool = False, region: Optional[str] = None
+    ) -> Dict[str, Any]:
+        r: Dict[str, Any] = {
             "Name": self.name,
             "Type": self.type,
             "Value": self.decrypt(self.value) if decrypt else self.value,
             "Version": self.version,
             "LastModifiedDate": round(self.last_modified_date, 3),
             "DataType": self.data_type,
         }
@@ -255,16 +259,18 @@
             r["SourceResult"] = self.source_result
 
         if region:
             r["ARN"] = parameter_arn(self.account_id, region, self.name)
 
         return r
 
-    def describe_response_object(self, decrypt=False, include_labels=False):
-        r = self.response_object(decrypt)
+    def describe_response_object(
+        self, decrypt: bool = False, include_labels: bool = False
+    ) -> Dict[str, Any]:
+        r: Dict[str, Any] = self.response_object(decrypt)
         r["LastModifiedDate"] = round(self.last_modified_date, 3)
         r["LastModifiedUser"] = "N/A"
 
         if self.description:
             r["Description"] = self.description
 
         if self.keyid:
@@ -275,26 +281,31 @@
 
         if include_labels:
             r["Labels"] = self.labels
 
         return r
 
     @staticmethod
-    def cloudformation_name_type():
+    def cloudformation_name_type() -> str:
         return "Name"
 
     @staticmethod
-    def cloudformation_type():
+    def cloudformation_type() -> str:
         # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ssm-parameter.html
         return "AWS::SSM::Parameter"
 
     @classmethod
-    def create_from_cloudformation_json(
-        cls, resource_name, cloudformation_json, account_id, region_name, **kwargs
-    ):
+    def create_from_cloudformation_json(  # type: ignore[misc]
+        cls,
+        resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+        **kwargs: Any,
+    ) -> "Parameter":
         ssm_backend = ssm_backends[account_id][region_name]
         properties = cloudformation_json["Properties"]
 
         parameter_args = {
             "name": properties.get("Name"),
             "description": properties.get("Description", None),
             "value": properties.get("Value", None),
@@ -306,43 +317,49 @@
             "data_type": properties.get("DataType", "text"),
         }
         ssm_backend.put_parameter(**parameter_args)
         parameter = ssm_backend.get_parameter(properties.get("Name"))
         return parameter
 
     @classmethod
-    def update_from_cloudformation_json(
+    def update_from_cloudformation_json(  # type: ignore[misc]
         cls,
-        original_resource,
-        new_resource_name,
-        cloudformation_json,
-        account_id,
-        region_name,
-    ):
+        original_resource: Any,
+        new_resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+    ) -> "Parameter":
         cls.delete_from_cloudformation_json(
             original_resource.name, cloudformation_json, account_id, region_name
         )
         return cls.create_from_cloudformation_json(
             new_resource_name, cloudformation_json, account_id, region_name
         )
 
     @classmethod
-    def delete_from_cloudformation_json(
-        cls, resource_name, cloudformation_json, account_id, region_name
-    ):
+    def delete_from_cloudformation_json(  # type: ignore[misc]
+        cls,
+        resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+    ) -> None:
         ssm_backend = ssm_backends[account_id][region_name]
         properties = cloudformation_json["Properties"]
 
         ssm_backend.delete_parameter(properties.get("Name"))
 
 
 MAX_TIMEOUT_SECONDS = 3600
 
 
-def generate_ssm_doc_param_list(parameters):
+def generate_ssm_doc_param_list(
+    parameters: Dict[str, Any]
+) -> Optional[List[Dict[str, Any]]]:
     if not parameters:
         return None
     param_list = []
     for param_name, param_info in parameters.items():
         final_dict = {
             "Name": param_name,
         }
@@ -366,102 +383,118 @@
     return param_list
 
 
 @dataclass(frozen=True)
 class AccountPermission:
     account_id: str
     version: str
-    created_at: datetime
+    created_at: datetime.datetime
 
 
 class Documents(BaseModel):
-    def __init__(self, ssm_document):
+    def __init__(self, ssm_document: "Document"):
         version = ssm_document.document_version
         self.versions = {version: ssm_document}
         self.default_version = version
         self.latest_version = version
-        self.permissions = {}  # {AccountID: AccountPermission }
+        self.permissions: Dict[
+            str, AccountPermission
+        ] = {}  # {AccountID: AccountPermission }
 
-    def get_default_version(self):
-        return self.versions.get(self.default_version)
+    def get_default_version(self) -> "Document":
+        return self.versions[self.default_version]
 
-    def get_latest_version(self):
-        return self.versions.get(self.latest_version)
+    def get_latest_version(self) -> "Document":
+        return self.versions[self.latest_version]
 
-    def find_by_version_name(self, version_name):
+    def find_by_version_name(self, version_name: str) -> Optional["Document"]:
         return next(
             (
                 document
                 for document in self.versions.values()
                 if document.version_name == version_name
             ),
             None,
         )
 
-    def find_by_version(self, version):
+    def find_by_version(self, version: str) -> Optional["Document"]:
         return self.versions.get(version)
 
-    def find_by_version_and_version_name(self, version, version_name):
+    def find_by_version_and_version_name(
+        self, version: str, version_name: str
+    ) -> Optional["Document"]:
         return next(
             (
                 document
                 for doc_version, document in self.versions.items()
                 if doc_version == version and document.version_name == version_name
             ),
             None,
         )
 
-    def find(self, document_version=None, version_name=None, strict=True):
+    def find(
+        self,
+        document_version: Optional[str] = None,
+        version_name: Optional[str] = None,
+        strict: bool = True,
+    ) -> "Document":
 
         if document_version == "$LATEST":
-            ssm_document = self.get_latest_version()
+            ssm_document: Optional["Document"] = self.get_latest_version()
         elif version_name and document_version:
             ssm_document = self.find_by_version_and_version_name(
                 document_version, version_name
             )
         elif version_name:
             ssm_document = self.find_by_version_name(version_name)
         elif document_version:
             ssm_document = self.find_by_version(document_version)
         else:
             ssm_document = self.get_default_version()
 
         if strict and not ssm_document:
             raise InvalidDocument("The specified document does not exist.")
 
-        return ssm_document
+        return ssm_document  # type: ignore
 
-    def exists(self, document_version=None, version_name=None):
+    def exists(
+        self, document_version: Optional[str] = None, version_name: Optional[str] = None
+    ) -> bool:
         return self.find(document_version, version_name, strict=False) is not None
 
-    def add_new_version(self, new_document_version):
+    def add_new_version(self, new_document_version: "Document") -> None:
         version = new_document_version.document_version
         self.latest_version = version
         self.versions[version] = new_document_version
 
-    def update_default_version(self, version):
+    def update_default_version(self, version: str) -> "Document":
         ssm_document = self.find_by_version(version)
         if not ssm_document:
             raise InvalidDocument("The specified document does not exist.")
         self.default_version = version
         return ssm_document
 
-    def delete(self, *versions):
+    def delete(self, *versions: str) -> None:
         for version in versions:
             if version in self.versions:
                 del self.versions[version]
 
         if self.versions and self.latest_version not in self.versions:
             ordered_versions = sorted(self.versions.keys())
             new_latest_version = ordered_versions[-1]
             self.latest_version = new_latest_version
 
-    def describe(self, document_version=None, version_name=None, tags=None):
+    def describe(
+        self,
+        document_version: Optional[str] = None,
+        version_name: Optional[str] = None,
+        tags: Optional[List[Dict[str, str]]] = None,
+    ) -> Dict[str, Any]:
         document = self.find(document_version, version_name)
-        base = {
+        base: Dict[str, Any] = {
             "Hash": document.hash,
             "HashType": "Sha256",
             "Name": document.name,
             "Owner": document.owner,
             "CreatedDate": document.created_date.strftime("%Y-%m-%dT%H:%M:%SZ"),
             "Status": document.status,
             "DocumentVersion": document.document_version,
@@ -479,15 +512,17 @@
         if document.target_type:
             base["TargetType"] = document.target_type
         if tags:
             base["Tags"] = tags
 
         return base
 
-    def modify_permissions(self, accounts_to_add, accounts_to_remove, version):
+    def modify_permissions(
+        self, accounts_to_add: List[str], accounts_to_remove: List[str], version: str
+    ) -> None:
         version = version or "$DEFAULT"
         if accounts_to_add:
             if "all" in accounts_to_add:
                 self.permissions.clear()
             else:
                 self.permissions.pop("all", None)
 
@@ -502,45 +537,45 @@
         if accounts_to_remove:
             if "all" in accounts_to_remove:
                 self.permissions.clear()
             else:
                 for account_id in accounts_to_remove:
                     self.permissions.pop(account_id, None)
 
-    def describe_permissions(self):
+    def describe_permissions(self) -> Dict[str, Any]:
 
         permissions_ordered_by_date = sorted(
             self.permissions.values(), key=lambda p: p.created_at
         )
 
         return {
             "AccountIds": [p.account_id for p in permissions_ordered_by_date],
             "AccountSharingInfoList": [
                 {"AccountId": p.account_id, "SharedDocumentVersion": p.version}
                 for p in permissions_ordered_by_date
             ],
         }
 
-    def is_shared(self):
+    def is_shared(self) -> bool:
         return len(self.permissions) > 0
 
 
 class Document(BaseModel):
     def __init__(
         self,
-        account_id,
-        name,
-        version_name,
-        content,
-        document_type,
-        document_format,
-        requires,
-        attachments,
-        target_type,
-        document_version="1",
+        account_id: str,
+        name: str,
+        version_name: str,
+        content: str,
+        document_type: str,
+        document_format: str,
+        requires: List[Dict[str, str]],
+        attachments: List[Dict[str, Any]],
+        target_type: str,
+        document_version: str = "1",
     ):
         self.name = name
         self.version_name = version_name
         self.content = content
         self.document_type = document_type
         self.document_format = document_format
         self.requires = requires
@@ -587,19 +622,21 @@
             elif self.schema_version == "1.2":
                 self.runtimeConfig = content_json.get("runtimeConfig")
 
         except KeyError:
             raise InvalidDocumentContent("The content for the document is not valid.")
 
     @property
-    def hash(self):
+    def hash(self) -> str:
         return hashlib.sha256(self.content.encode("utf-8")).hexdigest()
 
-    def list_describe(self, tags=None):
-        base = {
+    def list_describe(
+        self, tags: Optional[List[Dict[str, str]]] = None
+    ) -> Dict[str, Any]:
+        base: Dict[str, Any] = {
             "Name": self.name,
             "Owner": self.owner,
             "DocumentVersion": self.document_version,
             "DocumentType": self.document_type,
             "SchemaVersion": self.schema_version,
             "DocumentFormat": self.document_format,
         }
@@ -616,60 +653,62 @@
 
         return base
 
 
 class Command(BaseModel):
     def __init__(
         self,
-        account_id,
-        comment="",
-        document_name="",
-        timeout_seconds=MAX_TIMEOUT_SECONDS,
-        instance_ids=None,
-        max_concurrency="",
-        max_errors="",
-        notification_config=None,
-        output_s3_bucket_name="",
-        output_s3_key_prefix="",
-        output_s3_region="",
-        parameters=None,
-        service_role_arn="",
-        targets=None,
-        backend_region="us-east-1",
+        account_id: str,
+        comment: str = "",
+        document_name: Optional[str] = "",
+        timeout_seconds: Optional[int] = MAX_TIMEOUT_SECONDS,
+        instance_ids: Optional[List[str]] = None,
+        max_concurrency: str = "",
+        max_errors: str = "",
+        notification_config: Optional[Dict[str, Any]] = None,
+        output_s3_bucket_name: str = "",
+        output_s3_key_prefix: str = "",
+        output_s3_region: str = "",
+        parameters: Optional[Dict[str, List[str]]] = None,
+        service_role_arn: str = "",
+        targets: Optional[List[Dict[str, Any]]] = None,
+        backend_region: str = "us-east-1",
     ):
 
         if instance_ids is None:
             instance_ids = []
 
-        if notification_config is None:
-            notification_config = {}
-
         if parameters is None:
             parameters = {}
 
         if targets is None:
             targets = []
 
         self.command_id = str(random.uuid4())
         self.status = "Success"
         self.status_details = "Details placeholder"
         self.account_id = account_id
 
+        self.timeout_seconds = timeout_seconds or MAX_TIMEOUT_SECONDS
         self.requested_date_time = datetime.datetime.now()
         self.requested_date_time_iso = self.requested_date_time.isoformat()
         expires_after = self.requested_date_time + datetime.timedelta(
-            0, timeout_seconds
+            0, self.timeout_seconds
         )
         self.expires_after = expires_after.isoformat()
 
         self.comment = comment
         self.document_name = document_name
         self.max_concurrency = max_concurrency
         self.max_errors = max_errors
-        self.notification_config = notification_config
+        self.notification_config = notification_config or {
+            "NotificationArn": "string",
+            "NotificationEvents": ["Success"],
+            "NotificationType": "Command",
+        }
         self.output_s3_bucket_name = output_s3_bucket_name
         self.output_s3_key_prefix = output_s3_key_prefix
         self.output_s3_region = output_s3_region
         self.parameters = parameters
         self.service_role_arn = service_role_arn
         self.targets = targets
         self.backend_region = backend_region
@@ -691,26 +730,26 @@
         # Create invocations with a single run command plugin.
         self.invocations = []
         for instance_id in self.instance_ids:
             self.invocations.append(
                 self.invocation_response(instance_id, "aws:runShellScript")
             )
 
-    def _get_instance_ids_from_targets(self):
+    def _get_instance_ids_from_targets(self) -> List[str]:
         target_instance_ids = []
         ec2_backend = ec2_backends[self.account_id][self.backend_region]
         ec2_filters = {target["Key"]: target["Values"] for target in self.targets}
         reservations = ec2_backend.all_reservations(filters=ec2_filters)
         for reservation in reservations:
             for instance in reservation.instances:
                 target_instance_ids.append(instance.id)
         return target_instance_ids
 
-    def response_object(self):
-        r = {
+    def response_object(self) -> Dict[str, Any]:
+        return {
             "CommandId": self.command_id,
             "Comment": self.comment,
             "CompletedCount": self.completed_count,
             "DeliveryTimedOutCount": 0,
             "DocumentName": self.document_name,
             "ErrorCount": self.error_count,
             "ExpiresAfter": self.expires_after,
@@ -724,27 +763,26 @@
             "Parameters": self.parameters,
             "RequestedDateTime": self.requested_date_time_iso,
             "ServiceRole": self.service_role_arn,
             "Status": self.status,
             "StatusDetails": self.status_details,
             "TargetCount": self.target_count,
             "Targets": self.targets,
+            "TimeoutSeconds": self.timeout_seconds,
         }
 
-        return r
-
-    def invocation_response(self, instance_id, plugin_name):
+    def invocation_response(self, instance_id: str, plugin_name: str) -> Dict[str, Any]:
         # Calculate elapsed time from requested time and now. Use a hardcoded
         # elapsed time since there is no easy way to convert a timedelta to
         # an ISO 8601 duration string.
         elapsed_time_iso = "PT5M"
         elapsed_time_delta = datetime.timedelta(minutes=5)
         end_time = self.requested_date_time + elapsed_time_delta
 
-        r = {
+        return {
             "CommandId": self.command_id,
             "InstanceId": instance_id,
             "Comment": self.comment,
             "DocumentName": self.document_name,
             "PluginName": plugin_name,
             "ResponseCode": 0,
             "ExecutionStartDateTime": self.requested_date_time_iso,
@@ -753,17 +791,17 @@
             "Status": "Success",
             "StatusDetails": "Success",
             "StandardOutputContent": "",
             "StandardOutputUrl": "",
             "StandardErrorContent": "",
         }
 
-        return r
-
-    def get_invocation(self, instance_id, plugin_name):
+    def get_invocation(
+        self, instance_id: str, plugin_name: Optional[str]
+    ) -> Dict[str, Any]:
         invocation = next(
             (
                 invocation
                 for invocation in self.invocations
                 if invocation["InstanceId"] == instance_id
             ),
             None,
@@ -780,21 +818,27 @@
                 "InvocationDoesNotExist",
                 "An error occurred (InvocationDoesNotExist) when calling the GetCommandInvocation operation",
             )
 
         return invocation
 
 
-def _validate_document_format(document_format):
+def _validate_document_format(document_format: str) -> None:
     aws_doc_formats = ["JSON", "YAML"]
     if document_format not in aws_doc_formats:
         raise ValidationException("Invalid document format " + str(document_format))
 
 
-def _validate_document_info(content, name, document_type, document_format, strict=True):
+def _validate_document_info(
+    content: str,
+    name: str,
+    document_type: Optional[str],
+    document_format: str,
+    strict: bool = True,
+) -> None:
     aws_ssm_name_regex = r"^[a-zA-Z0-9_\-.]{3,128}$"
     aws_name_reject_list = ["aws-", "amazon", "amzn"]
     aws_doc_types = [
         "Command",
         "Policy",
         "Automation",
         "Session",
@@ -817,29 +861,35 @@
         raise ValidationException("Invalid document name " + str(name))
 
     if strict and document_type not in aws_doc_types:
         # Update document doesn't use document type
         raise ValidationException("Invalid document type " + str(document_type))
 
 
-def _document_filter_equal_comparator(keyed_value, _filter):
+def _document_filter_equal_comparator(
+    keyed_value: str, _filter: Dict[str, Any]
+) -> bool:
     for v in _filter["Values"]:
         if keyed_value == v:
             return True
     return False
 
 
-def _document_filter_list_includes_comparator(keyed_value_list, _filter):
+def _document_filter_list_includes_comparator(
+    keyed_value_list: List[str], _filter: Dict[str, Any]
+) -> bool:
     for v in _filter["Values"]:
         if v in keyed_value_list:
             return True
     return False
 
 
-def _document_filter_match(account_id, filters, ssm_doc):
+def _document_filter_match(
+    account_id: str, filters: List[Dict[str, Any]], ssm_doc: Document
+) -> bool:
     for _filter in filters:
         if _filter["Key"] == "Name" and not _document_filter_equal_comparator(
             ssm_doc.name, _filter
         ):
             return False
 
         elif _filter["Key"] == "Owner":
@@ -867,73 +917,71 @@
             ssm_doc.target_type, _filter
         ):
             return False
 
     return True
 
 
-def _valid_parameter_type(type_):
+def _valid_parameter_type(type_: str) -> bool:
     """
     Parameter Type field only allows `SecureString`, `StringList` and `String` (not `str`) values
 
     """
     return type_ in ("SecureString", "StringList", "String")
 
 
-def _valid_parameter_data_type(data_type):
+def _valid_parameter_data_type(data_type: str) -> bool:
     """
     Parameter DataType field allows only `text` and `aws:ec2:image` values
 
     """
     return data_type in ("text", "aws:ec2:image")
 
 
 class FakeMaintenanceWindow:
     def __init__(
         self,
-        name,
-        description,
-        enabled,
-        duration,
-        cutoff,
-        schedule,
-        schedule_timezone,
-        schedule_offset,
-        start_date,
-        end_date,
+        name: str,
+        description: str,
+        duration: int,
+        cutoff: int,
+        schedule: str,
+        schedule_timezone: str,
+        schedule_offset: int,
+        start_date: str,
+        end_date: str,
     ):
         self.id = FakeMaintenanceWindow.generate_id()
         self.name = name
         self.description = description
-        self.enabled = enabled
         self.duration = duration
         self.cutoff = cutoff
         self.schedule = schedule
         self.schedule_timezone = schedule_timezone
         self.schedule_offset = schedule_offset
         self.start_date = start_date
         self.end_date = end_date
 
-    def to_json(self):
+    def to_json(self) -> Dict[str, Any]:
         return {
             "WindowId": self.id,
             "Name": self.name,
             "Description": self.description,
-            "Enabled": self.enabled,
+            "Enabled": True,
             "Duration": self.duration,
             "Cutoff": self.cutoff,
             "Schedule": self.schedule,
             "ScheduleTimezone": self.schedule_timezone,
             "ScheduleOffset": self.schedule_offset,
             "StartDate": self.start_date,
             "EndDate": self.end_date,
         }
 
     @staticmethod
-    def generate_id():
+    def generate_id() -> str:
         chars = list(range(10)) + ["a", "b", "c", "d", "e", "f"]
         return "mw-" + "".join(str(random.choice(chars)) for _ in range(17))
 
 
 class SimpleSystemManagerBackend(BaseBackend):
     """
     Moto supports the following default parameters out of the box:
@@ -942,37 +990,43 @@
      - /aws/service/global-infrastructure/services
 
     Note that these are hardcoded, so they may be out of date for new services/regions.
 
     Integration with SecretsManager is also supported.
     """
 
-    def __init__(self, region_name, account_id):
+    def __init__(self, region_name: str, account_id: str):
         super().__init__(region_name, account_id)
         self._parameters = ParameterDict(account_id, region_name)
 
-        self._resource_tags = defaultdict(lambda: defaultdict(dict))
-        self._commands = []
-        self._errors = []
+        self._resource_tags: DefaultDict[
+            str, DefaultDict[str, Dict[str, str]]
+        ] = defaultdict(lambda: defaultdict(dict))
+        self._commands: List[Command] = []
+        self._errors: List[str] = []
         self._documents: Dict[str, Documents] = {}
 
         self.windows: Dict[str, FakeMaintenanceWindow] = dict()
 
     @staticmethod
-    def default_vpc_endpoint_service(service_region, zones):
+    def default_vpc_endpoint_service(
+        service_region: str, zones: List[str]
+    ) -> List[Dict[str, str]]:
         """Default VPC endpoint services."""
         return BaseBackend.default_vpc_endpoint_service_factory(
             service_region, zones, "ssm"
         ) + BaseBackend.default_vpc_endpoint_service_factory(
             service_region, zones, "ssmmessages"
         )
 
-    def _generate_document_information(self, ssm_document, document_format):
+    def _generate_document_information(
+        self, ssm_document: Document, document_format: str
+    ) -> Dict[str, Any]:
         content = self._get_document_content(document_format, ssm_document)
-        base = {
+        base: Dict[str, Any] = {
             "Name": ssm_document.name,
             "DocumentVersion": ssm_document.document_version,
             "Status": ssm_document.status,
             "Content": content,
             "DocumentType": ssm_document.document_type,
             "DocumentFormat": document_format,
         }
@@ -983,52 +1037,52 @@
             base["Requires"] = ssm_document.requires
         if ssm_document.attachments:
             base["AttachmentsContent"] = ssm_document.attachments
 
         return base
 
     @staticmethod
-    def _get_document_content(document_format, ssm_document):
+    def _get_document_content(document_format: str, ssm_document: Document) -> str:
         if document_format == ssm_document.document_format:
             content = ssm_document.content
         elif document_format == "JSON":
             content = json.dumps(ssm_document.content_json)
         elif document_format == "YAML":
             content = yaml.dump(ssm_document.content_json)
         else:
             raise ValidationException("Invalid document format " + str(document_format))
         return content
 
-    def _get_documents(self, name):
+    def _get_documents(self, name: str) -> Documents:
         documents = self._documents.get(name)
         if not documents:
             raise InvalidDocument("The specified document does not exist.")
         return documents
 
-    def _get_documents_tags(self, name):
+    def _get_documents_tags(self, name: str) -> List[Dict[str, str]]:
         docs_tags = self._resource_tags.get("Document")
         if docs_tags:
             document_tags = docs_tags.get(name, {})
             return [
                 {"Key": tag, "Value": value} for tag, value in document_tags.items()
             ]
         return []
 
     def create_document(
         self,
-        content,
-        requires,
-        attachments,
-        name,
-        version_name,
-        document_type,
-        document_format,
-        target_type,
-        tags,
-    ):
+        content: str,
+        requires: List[Dict[str, str]],
+        attachments: List[Dict[str, Any]],
+        name: str,
+        version_name: str,
+        document_type: str,
+        document_format: str,
+        target_type: str,
+        tags: List[Dict[str, str]],
+    ) -> Dict[str, Any]:
         ssm_document = Document(
             account_id=self.account_id,
             name=name,
             version_name=version_name,
             content=content,
             document_type=document_type,
             document_format=document_format,
@@ -1052,15 +1106,17 @@
 
         if tags:
             document_tags = {t["Key"]: t["Value"] for t in tags}
             self.add_tags_to_resource("Document", name, document_tags)
 
         return documents.describe(tags=tags)
 
-    def delete_document(self, name, document_version, version_name, force):
+    def delete_document(
+        self, name: str, document_version: str, version_name: str, force: bool
+    ) -> None:
         documents = self._get_documents(name)
 
         if documents.is_shared():
             raise InvalidDocumentOperation("Must unshare document first before delete")
 
         keys_to_delete = set()
 
@@ -1101,53 +1157,57 @@
             else:
                 # We are deleting all versions
                 keys_to_delete = set(documents.versions.keys())
 
             documents.delete(*keys_to_delete)
 
             if len(documents.versions) == 0:
-                self._resource_tags.get("Document", {}).pop(name, None)
+                self._resource_tags.get("Document", {}).pop(name, None)  # type: ignore
                 del self._documents[name]
 
-    def get_document(self, name, document_version, version_name, document_format):
+    def get_document(
+        self, name: str, document_version: str, version_name: str, document_format: str
+    ) -> Dict[str, Any]:
 
         documents = self._get_documents(name)
         ssm_document = documents.find(document_version, version_name)
 
         if not document_format:
             document_format = ssm_document.document_format
         else:
             _validate_document_format(document_format=document_format)
 
         return self._generate_document_information(ssm_document, document_format)
 
-    def update_document_default_version(self, name, document_version):
+    def update_document_default_version(
+        self, name: str, document_version: str
+    ) -> Dict[str, Any]:
         documents = self._get_documents(name)
         ssm_document = documents.update_default_version(document_version)
 
-        result = {
+        result: Dict[str, Any] = {
             "Name": ssm_document.name,
             "DefaultVersion": document_version,
         }
 
         if ssm_document.version_name:
             result["DefaultVersionName"] = ssm_document.version_name
 
         return result
 
     def update_document(
         self,
-        content,
-        attachments,
-        name,
-        version_name,
-        document_version,
-        document_format,
-        target_type,
-    ):
+        content: str,
+        attachments: List[Dict[str, Any]],
+        name: str,
+        version_name: str,
+        document_version: str,
+        document_format: str,
+        target_type: str,
+    ) -> Dict[str, Any]:
         _validate_document_info(
             content=content,
             name=name,
             document_type=None,
             document_format=document_format,
             strict=False,
         )
@@ -1194,29 +1254,35 @@
                         "Change the content of the document and try again."
                     )
 
         documents.add_new_version(new_ssm_document)
         tags = self._get_documents_tags(name)
         return documents.describe(document_version=new_version, tags=tags)
 
-    def describe_document(self, name, document_version, version_name):
+    def describe_document(
+        self, name: str, document_version: str, version_name: str
+    ) -> Dict[str, Any]:
         documents = self._get_documents(name)
         tags = self._get_documents_tags(name)
         return documents.describe(document_version, version_name, tags=tags)
 
     def list_documents(
-        self, document_filter_list, filters, max_results=10, next_token="0"
-    ):
+        self,
+        document_filter_list: Any,
+        filters: List[Dict[str, Any]],
+        max_results: int = 10,
+        token: str = "0",
+    ) -> Tuple[List[Dict[str, Any]], str]:
         if document_filter_list:
             raise ValidationException(
                 "DocumentFilterList is deprecated. Instead use Filters."
             )
 
-        next_token = int(next_token)
-        results = []
+        next_token = int(token or "0")
+        results: List[Dict[str, Any]] = []
         dummy_token_tracker = 0
         # Sort to maintain next token adjacency
         for _, documents in sorted(self._documents.items()):
             if len(results) == max_results:
                 # There's still more to go so we need a next token
                 return results, str(next_token + len(results))
 
@@ -1231,32 +1297,32 @@
                 # If we have filters enabled, and we don't match them,
                 continue
             else:
                 tags = self._get_documents_tags(ssm_doc.name)
                 doc_describe = ssm_doc.list_describe(tags=tags)
                 results.append(doc_describe)
 
-        # If we've fallen out of the loop, theres no more documents. No next token.
+        # If we've fallen out of the loop, there are no more documents. No next token.
         return results, ""
 
-    def describe_document_permission(self, name):
+    def describe_document_permission(self, name: str) -> Dict[str, Any]:
         """
         Parameters max_results, permission_type, and next_token not yet implemented
         """
         document = self._get_documents(name)
         return document.describe_permissions()
 
     def modify_document_permission(
         self,
-        name,
-        account_ids_to_add,
-        account_ids_to_remove,
-        shared_document_version,
-        permission_type,
-    ):
+        name: str,
+        account_ids_to_add: List[str],
+        account_ids_to_remove: List[str],
+        shared_document_version: str,
+        permission_type: str,
+    ) -> None:
 
         account_id_regex = re.compile(r"^(all|[0-9]{12})$", re.IGNORECASE)
         version_regex = re.compile(r"^([$]LATEST|[$]DEFAULT|[$]ALL)$")
 
         account_ids_to_add = account_ids_to_add or []
         account_ids_to_remove = account_ids_to_remove or []
 
@@ -1297,71 +1363,73 @@
             )
 
         document = self._get_documents(name)
         document.modify_permissions(
             account_ids_to_add, account_ids_to_remove, shared_document_version
         )
 
-    def delete_parameter(self, name):
-        self._resource_tags.get("Parameter", {}).pop(name, None)
-        return self._parameters.pop(name, None)
+    def delete_parameter(self, name: str) -> Optional[Parameter]:
+        self._resource_tags.get("Parameter", {}).pop(name, None)  # type: ignore
+        return self._parameters.pop(name, None)  # type: ignore
 
-    def delete_parameters(self, names):
+    def delete_parameters(self, names: List[str]) -> List[str]:
         result = []
         for name in names:
             try:
                 del self._parameters[name]
                 result.append(name)
-                self._resource_tags.get("Parameter", {}).pop(name, None)
+                self._resource_tags.get("Parameter", {}).pop(name, None)  # type: ignore
             except KeyError:
                 pass
         return result
 
-    def describe_parameters(self, filters, parameter_filters):
+    def describe_parameters(
+        self, filters: List[Dict[str, Any]], parameter_filters: List[Dict[str, Any]]
+    ) -> List[Parameter]:
         if filters and parameter_filters:
             raise ValidationException(
                 "You can use either Filters or ParameterFilters in a single request."
             )
 
         self._validate_parameter_filters(parameter_filters, by_path=False)
 
         result = []
         for param_name in self._parameters:
-            ssm_parameter = self.get_parameter(param_name)
+            ssm_parameter: Parameter = self.get_parameter(param_name)  # type: ignore[assignment]
             if not self._match_filters(ssm_parameter, parameter_filters):
                 continue
 
             if filters:
                 for _filter in filters:
                     if _filter["Key"] == "Name":
-                        k = ssm_parameter.name
                         for v in _filter["Values"]:
-                            if k.startswith(v):
+                            if ssm_parameter.name.startswith(v):
                                 result.append(ssm_parameter)
                                 break
                     elif _filter["Key"] == "Type":
-                        k = ssm_parameter.type
                         for v in _filter["Values"]:
-                            if k == v:
+                            if ssm_parameter.type == v:
                                 result.append(ssm_parameter)
                                 break
                     elif _filter["Key"] == "KeyId":
-                        k = ssm_parameter.keyid
-                        if k:
+                        keyid = ssm_parameter.keyid
+                        if keyid:
                             for v in _filter["Values"]:
-                                if k == v:
+                                if keyid == v:
                                     result.append(ssm_parameter)
                                     break
                 continue
 
             result.append(ssm_parameter)
 
         return result
 
-    def _validate_parameter_filters(self, parameter_filters, by_path):
+    def _validate_parameter_filters(
+        self, parameter_filters: Optional[List[Dict[str, Any]]], by_path: bool
+    ) -> None:
         for index, filter_obj in enumerate(parameter_filters or []):
             key = filter_obj["Key"]
             values = filter_obj.get("Values", [])
 
             if key == "Path":
                 option = filter_obj.get("Option", "OneLevel")
             else:
@@ -1493,35 +1561,29 @@
             if key != "Path" and option not in allowed_options:
                 raise InvalidFilterOption(
                     f"The following filter option is not valid: {option}. Valid options include: [BeginsWith, Equals]."
                 )
 
             filter_keys.append(key)
 
-    def _format_error(self, key, value, constraint):
+    def _format_error(self, key: str, value: Any, constraint: str) -> str:
         return f'Value "{value}" at "{key}" failed to satisfy constraint: {constraint}'
 
-    def _raise_errors(self):
+    def _raise_errors(self) -> None:
         if self._errors:
             count = len(self._errors)
             plural = "s" if len(self._errors) > 1 else ""
             errors = "; ".join(self._errors)
             self._errors = []  # reset collected errors
 
             raise ValidationException(
                 f"{count} validation error{plural} detected: {errors}"
             )
 
-    def get_all_parameters(self):
-        result = []
-        for k, _ in self._parameters.items():
-            result.append(self._parameters[k])
-        return result
-
-    def get_parameters(self, names):
+    def get_parameters(self, names: List[str]) -> Dict[str, Parameter]:
         result = {}
 
         if len(names) > 10:
             all_names = ", ".join(names)
             raise ValidationException(
                 "1 validation error detected: "
                 f"Value '[{all_names}]' at 'names' failed to satisfy constraint: Member must have length less than or equal to 10."
@@ -1536,89 +1598,95 @@
                         result[name] = param
                 except ParameterVersionNotFound:
                     pass
         return result
 
     def get_parameters_by_path(
         self,
-        path,
-        recursive,
-        filters=None,
-        next_token=None,
-        max_results=10,
-    ):
+        path: str,
+        recursive: bool,
+        filters: Optional[List[Dict[str, Any]]] = None,
+        next_token: Optional[str] = None,
+        max_results: int = 10,
+    ) -> Tuple[List[Parameter], Optional[str]]:
         """Implement the get-parameters-by-path-API in the backend."""
 
         self._validate_parameter_filters(filters, by_path=True)
 
-        result = []
+        result: List[Parameter] = []
         # path could be with or without a trailing /. we handle this
         # difference here.
         path = path.rstrip("/") + "/"
         for param_name in self._parameters.get_keys_beginning_with(path, recursive):
-            parameter = self.get_parameter(param_name)
+            parameter: Parameter = self.get_parameter(param_name)  # type: ignore[assignment]
             if not self._match_filters(parameter, filters):
                 continue
             result.append(parameter)
 
         return self._get_values_nexttoken(result, max_results, next_token)
 
-    def _get_values_nexttoken(self, values_list, max_results, next_token=None):
-        if next_token is None:
-            next_token = 0
-        next_token = int(next_token)
+    def _get_values_nexttoken(
+        self,
+        values_list: List[Parameter],
+        max_results: int,
+        token: Optional[str] = None,
+    ) -> Tuple[List[Parameter], Optional[str]]:
+        next_token = int(token or "0")
         max_results = int(max_results)
         values = values_list[next_token : next_token + max_results]
-        if len(values) == max_results:
-            next_token = str(next_token + max_results)
-        else:
-            next_token = None
-        return values, next_token
+        return (
+            values,
+            str(next_token + max_results) if len(values) == max_results else None,
+        )
 
-    def get_parameter_history(self, name, next_token, max_results=50):
+    def get_parameter_history(
+        self, name: str, next_token: Optional[str], max_results: int = 50
+    ) -> Tuple[Optional[List[Parameter]], Optional[str]]:
 
         if max_results > PARAMETER_HISTORY_MAX_RESULTS:
             raise ValidationException(
                 "1 validation error detected: "
                 f"Value '{max_results}' at 'maxResults' failed to satisfy constraint: "
                 f"Member must have value less than or equal to {PARAMETER_HISTORY_MAX_RESULTS}."
             )
 
         if name in self._parameters:
             history = self._parameters[name]
             return self._get_history_nexttoken(history, next_token, max_results)
 
         return None, None
 
-    def _get_history_nexttoken(self, history, next_token, max_results):
-        if next_token is None:
-            next_token = 0
-        next_token = int(next_token)
+    def _get_history_nexttoken(
+        self, history: List[Parameter], token: Optional[str], max_results: int
+    ) -> Tuple[List[Parameter], Optional[str]]:
+        next_token = int(token or "0")
         max_results = int(max_results)
         history_to_return = history[next_token : next_token + max_results]
         if (
             len(history_to_return) == max_results
             and len(history) > next_token + max_results
         ):
             new_next_token = next_token + max_results
             return history_to_return, str(new_next_token)
         return history_to_return, None
 
-    def _match_filters(self, parameter, filters=None):
+    def _match_filters(
+        self, parameter: Parameter, filters: Optional[List[Dict[str, Any]]] = None
+    ) -> bool:
         """Return True if the given parameter matches all the filters"""
         for filter_obj in filters or []:
             key = filter_obj["Key"]
             values = filter_obj.get("Values", [])
 
             if key == "Path":
                 option = filter_obj.get("Option", "OneLevel")
             else:
                 option = filter_obj.get("Option", "Equals")
 
-            what = None
+            what: Any = None
             if key == "KeyId":
                 what = parameter.keyid
             elif key == "Name":
                 what = "/" + parameter.name.lstrip("/")
                 if option != "Contains":
                     values = ["/" + value.lstrip("/") for value in values]
             elif key == "Path":
@@ -1675,15 +1743,15 @@
                 elif any(what.startswith(value + "/") for value in values):
                     continue
                 else:
                     return False
         # True if no false match (or no filters at all)
         return True
 
-    def get_parameter(self, name):
+    def get_parameter(self, name: str) -> Optional[Parameter]:
         name_parts = name.split(":")
         name_prefix = name_parts[0]
 
         if len(name_parts) > 2:
             return None
 
         if name_prefix in self._parameters:
@@ -1710,15 +1778,17 @@
                     filter(lambda x: version_or_label in x.labels, parameters)
                 )
                 if len(result) > 0:
                     return result[-1]
 
         return None
 
-    def label_parameter_version(self, name, version, labels):
+    def label_parameter_version(
+        self, name: str, version: int, labels: List[str]
+    ) -> Tuple[List[str], int]:
         previous_parameter_versions = self._parameters[name]
         if not previous_parameter_versions:
             raise ParameterNotFound(f"Parameter {name} not found.")
         found_parameter = None
         labels_needing_removal = []
         if not version:
             version = 1
@@ -1766,40 +1836,40 @@
             )
         found_parameter.labels = found_parameter.labels + labels_to_append
         for parameter in previous_parameter_versions:
             if parameter.version != version:
                 for label in parameter.labels[:]:
                     if label in labels_needing_removal:
                         parameter.labels.remove(label)
-        return [invalid_labels, version]
+        return (invalid_labels, version)
 
-    def _check_for_parameter_version_limit_exception(self, name):
+    def _check_for_parameter_version_limit_exception(self, name: str) -> None:
         # https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-paramstore-versions.html
         parameter_versions = self._parameters[name]
         oldest_parameter = parameter_versions[0]
         if oldest_parameter.labels:
             raise ParameterMaxVersionLimitExceeded(
                 f"You attempted to create a new version of {name} by calling the PutParameter API "
                 f"with the overwrite flag. Version {oldest_parameter.version}, the oldest version, can't be deleted "
                 "because it has a label associated with it. Move the label to another version "
                 "of the parameter, and try again."
             )
 
     def put_parameter(
         self,
-        name,
-        description,
-        value,
-        parameter_type,
-        allowed_pattern,
-        keyid,
-        overwrite,
-        tags,
-        data_type,
-    ):
+        name: str,
+        description: str,
+        value: str,
+        parameter_type: str,
+        allowed_pattern: str,
+        keyid: str,
+        overwrite: bool,
+        tags: List[Dict[str, str]],
+        data_type: str,
+    ) -> Optional[int]:
         if not value:
             raise ValidationException(
                 "1 validation error detected: Value '' at 'value' failed to satisfy"
                 " constraint: Member must have length greater than or equal to 1."
             )
         if overwrite and tags:
             raise ValidationException(
@@ -1843,15 +1913,15 @@
             previous_parameter = None
             version = 1
         else:
             previous_parameter = previous_parameter_versions[-1]
             version = previous_parameter.version + 1
 
             if not overwrite:
-                return
+                return None
 
             if len(previous_parameter_versions) >= PARAMETER_VERSION_LIMIT:
                 self._check_for_parameter_version_limit_exception(name)
                 previous_parameter_versions.pop(0)
 
         last_modified_date = time.time()
         self._parameters[name].append(
@@ -1867,36 +1937,44 @@
                 version=version,
                 tags=tags or [],
                 data_type=data_type,
             )
         )
 
         if tags:
-            tags = {t["Key"]: t["Value"] for t in tags}
-            self.add_tags_to_resource("Parameter", name, tags)
+            tag_dict = {t["Key"]: t["Value"] for t in tags}
+            self.add_tags_to_resource("Parameter", name, tag_dict)
 
         return version
 
-    def add_tags_to_resource(self, resource_type, resource_id, tags):
+    def add_tags_to_resource(
+        self, resource_type: str, resource_id: str, tags: Dict[str, str]
+    ) -> None:
         self._validate_resource_type_and_id(resource_type, resource_id)
         for key, value in tags.items():
             self._resource_tags[resource_type][resource_id][key] = value
 
-    def remove_tags_from_resource(self, resource_type, resource_id, keys):
+    def remove_tags_from_resource(
+        self, resource_type: str, resource_id: str, keys: List[str]
+    ) -> None:
         self._validate_resource_type_and_id(resource_type, resource_id)
         tags = self._resource_tags[resource_type][resource_id]
         for key in keys:
             if key in tags:
                 del tags[key]
 
-    def list_tags_for_resource(self, resource_type, resource_id):
+    def list_tags_for_resource(
+        self, resource_type: str, resource_id: str
+    ) -> Dict[str, str]:
         self._validate_resource_type_and_id(resource_type, resource_id)
         return self._resource_tags[resource_type][resource_id]
 
-    def _validate_resource_type_and_id(self, resource_type, resource_id):
+    def _validate_resource_type_and_id(
+        self, resource_type: str, resource_id: str
+    ) -> None:
         if resource_type == "Parameter":
             if resource_id not in self._parameters:
                 raise InvalidResourceId()
             else:
                 return
         elif resource_type == "Document":
             if resource_id not in self._documents:
@@ -1911,138 +1989,138 @@
             "OpsItem",
             "OpsMetadata",
         ):
             raise InvalidResourceType()
         else:
             raise InvalidResourceId()
 
-    def send_command(self, **kwargs):
+    def send_command(
+        self,
+        comment: str,
+        document_name: Optional[str],
+        timeout_seconds: int,
+        instance_ids: List[str],
+        max_concurrency: str,
+        max_errors: str,
+        notification_config: Optional[Dict[str, Any]],
+        output_s3_bucket_name: str,
+        output_s3_key_prefix: str,
+        output_s3_region: str,
+        parameters: Dict[str, List[str]],
+        service_role_arn: str,
+        targets: List[Dict[str, Any]],
+    ) -> Command:
         command = Command(
             account_id=self.account_id,
-            comment=kwargs.get("Comment", ""),
-            document_name=kwargs.get("DocumentName"),
-            timeout_seconds=kwargs.get("TimeoutSeconds", 3600),
-            instance_ids=kwargs.get("InstanceIds", []),
-            max_concurrency=kwargs.get("MaxConcurrency", "50"),
-            max_errors=kwargs.get("MaxErrors", "0"),
-            notification_config=kwargs.get(
-                "NotificationConfig",
-                {
-                    "NotificationArn": "string",
-                    "NotificationEvents": ["Success"],
-                    "NotificationType": "Command",
-                },
-            ),
-            output_s3_bucket_name=kwargs.get("OutputS3BucketName", ""),
-            output_s3_key_prefix=kwargs.get("OutputS3KeyPrefix", ""),
-            output_s3_region=kwargs.get("OutputS3Region", ""),
-            parameters=kwargs.get("Parameters", {}),
-            service_role_arn=kwargs.get("ServiceRoleArn", ""),
-            targets=kwargs.get("Targets", []),
+            comment=comment,
+            document_name=document_name,
+            timeout_seconds=timeout_seconds,
+            instance_ids=instance_ids,
+            max_concurrency=max_concurrency,
+            max_errors=max_errors,
+            notification_config=notification_config,
+            output_s3_bucket_name=output_s3_bucket_name,
+            output_s3_key_prefix=output_s3_key_prefix,
+            output_s3_region=output_s3_region,
+            parameters=parameters,
+            service_role_arn=service_role_arn,
+            targets=targets,
             backend_region=self.region_name,
         )
 
         self._commands.append(command)
-        return {"Command": command.response_object()}
+        return command
 
-    def list_commands(self, **kwargs):
+    def list_commands(
+        self, command_id: Optional[str], instance_id: Optional[str]
+    ) -> List[Command]:
         """
-        https://docs.aws.amazon.com/systems-manager/latest/APIReference/API_ListCommands.html
+        Pagination and the Filters-parameter is not yet implemented
         """
-        commands = self._commands
-
-        command_id = kwargs.get("CommandId", None)
         if command_id:
-            commands = [self.get_command_by_id(command_id)]
-        instance_id = kwargs.get("InstanceId", None)
+            return [self.get_command_by_id(command_id)]
         if instance_id:
-            commands = self.get_commands_by_instance_id(instance_id)
+            return self.get_commands_by_instance_id(instance_id)
 
-        return {"Commands": [command.response_object() for command in commands]}
+        return self._commands
 
-    def get_command_by_id(self, command_id):
+    def get_command_by_id(self, command_id: str) -> Command:
         command = next(
             (command for command in self._commands if command.command_id == command_id),
             None,
         )
 
         if command is None:
             raise RESTError("InvalidCommandId", "Invalid command id.")
 
         return command
 
-    def get_commands_by_instance_id(self, instance_id):
+    def get_commands_by_instance_id(self, instance_id: str) -> List[Command]:
         return [
             command for command in self._commands if instance_id in command.instance_ids
         ]
 
-    def get_command_invocation(self, **kwargs):
-        """
-        https://docs.aws.amazon.com/systems-manager/latest/APIReference/API_GetCommandInvocation.html
-        """
-
-        command_id = kwargs.get("CommandId")
-        instance_id = kwargs.get("InstanceId")
-        plugin_name = kwargs.get("PluginName", None)
-
+    def get_command_invocation(
+        self, command_id: str, instance_id: str, plugin_name: Optional[str]
+    ) -> Dict[str, Any]:
         command = self.get_command_by_id(command_id)
         return command.get_invocation(instance_id, plugin_name)
 
     def create_maintenance_window(
         self,
-        name,
-        description,
-        enabled,
-        duration,
-        cutoff,
-        schedule,
-        schedule_timezone,
-        schedule_offset,
-        start_date,
-        end_date,
-    ):
+        name: str,
+        description: str,
+        duration: int,
+        cutoff: int,
+        schedule: str,
+        schedule_timezone: str,
+        schedule_offset: int,
+        start_date: str,
+        end_date: str,
+    ) -> str:
         """
         Creates a maintenance window. No error handling or input validation has been implemented yet.
         """
         window = FakeMaintenanceWindow(
             name,
             description,
-            enabled,
             duration,
             cutoff,
             schedule,
             schedule_timezone,
             schedule_offset,
             start_date,
             end_date,
         )
         self.windows[window.id] = window
         return window.id
 
-    def get_maintenance_window(self, window_id):
+    def get_maintenance_window(self, window_id: str) -> FakeMaintenanceWindow:
         """
         The window is assumed to exist - no error handling has been implemented yet.
         The NextExecutionTime-field is not returned.
         """
         return self.windows[window_id]
 
-    def describe_maintenance_windows(self, filters):
+    def describe_maintenance_windows(
+        self, filters: Optional[List[Dict[str, Any]]]
+    ) -> List[FakeMaintenanceWindow]:
         """
         Returns all windows. No pagination has been implemented yet. Only filtering for Name is supported.
         The NextExecutionTime-field is not returned.
 
         """
         res = [window for window in self.windows.values()]
         if filters:
             for f in filters:
                 if f["Key"] == "Name":
                     res = [w for w in res if w.name in f["Values"]]
         return res
 
-    def delete_maintenance_window(self, window_id):
+    def delete_maintenance_window(self, window_id: str) -> None:
         """
         Assumes the provided WindowId exists. No error handling has been implemented yet.
         """
         del self.windows[window_id]
 
 
 ssm_backends = BackendDict(SimpleSystemManagerBackend, "ssm")
```

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/af-south-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/me-central-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/me-south-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/us-east-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/us-east-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/us-west-1.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/ecs/optimized_amis/us-west-2.json` & `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/regions.json` & `moto-4.1.9.dev5/moto/ssm/resources/regions.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/resources/services.json` & `moto-4.1.9.dev5/moto/ssm/resources/services.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssm/responses.py` & `moto-4.1.9.dev5/moto/ssm/responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 import json
+from typing import Any, Dict, Tuple, Union
 
 from moto.core.responses import BaseResponse
 from .exceptions import ValidationException
 from .models import ssm_backends, SimpleSystemManagerBackend
 
 
 class SimpleSystemManagerResponse(BaseResponse):
     def __init__(self) -> None:
         super().__init__(service_name="ssm")
 
     @property
     def ssm_backend(self) -> SimpleSystemManagerBackend:
         return ssm_backends[self.current_account][self.region]
 
-    @property
-    def request_params(self):
-        try:
-            return json.loads(self.body)
-        except ValueError:
-            return {}
-
-    def create_document(self):
+    def create_document(self) -> str:
         content = self._get_param("Content")
         requires = self._get_param("Requires")
         attachments = self._get_param("Attachments")
         name = self._get_param("Name")
         version_name = self._get_param("VersionName")
         document_type = self._get_param("DocumentType")
         document_format = self._get_param("DocumentFormat", "JSON")
@@ -41,55 +35,55 @@
             document_format=document_format,
             target_type=target_type,
             tags=tags,
         )
 
         return json.dumps({"DocumentDescription": result})
 
-    def delete_document(self):
+    def delete_document(self) -> str:
         name = self._get_param("Name")
         document_version = self._get_param("DocumentVersion")
         version_name = self._get_param("VersionName")
         force = self._get_param("Force", False)
         self.ssm_backend.delete_document(
             name=name,
             document_version=document_version,
             version_name=version_name,
             force=force,
         )
 
         return json.dumps({})
 
-    def get_document(self):
+    def get_document(self) -> str:
         name = self._get_param("Name")
         version_name = self._get_param("VersionName")
         document_version = self._get_param("DocumentVersion")
         document_format = self._get_param("DocumentFormat", "JSON")
 
         document = self.ssm_backend.get_document(
             name=name,
             document_version=document_version,
             document_format=document_format,
             version_name=version_name,
         )
 
         return json.dumps(document)
 
-    def describe_document(self):
+    def describe_document(self) -> str:
         name = self._get_param("Name")
         document_version = self._get_param("DocumentVersion")
         version_name = self._get_param("VersionName")
 
         result = self.ssm_backend.describe_document(
             name=name, document_version=document_version, version_name=version_name
         )
 
         return json.dumps({"Document": result})
 
-    def update_document(self):
+    def update_document(self) -> str:
         content = self._get_param("Content")
         attachments = self._get_param("Attachments")
         name = self._get_param("Name")
         version_name = self._get_param("VersionName")
         document_version = self._get_param("DocumentVersion")
         document_format = self._get_param("DocumentFormat", "JSON")
         target_type = self._get_param("TargetType")
@@ -102,87 +96,85 @@
             document_version=document_version,
             document_format=document_format,
             target_type=target_type,
         )
 
         return json.dumps({"DocumentDescription": result})
 
-    def update_document_default_version(self):
+    def update_document_default_version(self) -> str:
         name = self._get_param("Name")
         document_version = self._get_param("DocumentVersion")
 
         result = self.ssm_backend.update_document_default_version(
             name=name, document_version=document_version
         )
         return json.dumps({"Description": result})
 
-    def list_documents(self):
+    def list_documents(self) -> str:
         document_filter_list = self._get_param("DocumentFilterList")
         filters = self._get_param("Filters")
         max_results = self._get_param("MaxResults", 10)
         next_token = self._get_param("NextToken", "0")
 
         documents, token = self.ssm_backend.list_documents(
             document_filter_list=document_filter_list,
             filters=filters,
             max_results=max_results,
-            next_token=next_token,
+            token=next_token,
         )
 
         return json.dumps({"DocumentIdentifiers": documents, "NextToken": token})
 
-    def describe_document_permission(self):
+    def describe_document_permission(self) -> str:
         name = self._get_param("Name")
 
         result = self.ssm_backend.describe_document_permission(name=name)
         return json.dumps(result)
 
-    def modify_document_permission(self):
+    def modify_document_permission(self) -> str:
         account_ids_to_add = self._get_param("AccountIdsToAdd")
         account_ids_to_remove = self._get_param("AccountIdsToRemove")
         name = self._get_param("Name")
         permission_type = self._get_param("PermissionType")
         shared_document_version = self._get_param("SharedDocumentVersion")
 
         self.ssm_backend.modify_document_permission(
             name=name,
             account_ids_to_add=account_ids_to_add,
             account_ids_to_remove=account_ids_to_remove,
             shared_document_version=shared_document_version,
             permission_type=permission_type,
         )
+        return "{}"
 
-    def _get_param(self, param_name, if_none=None):
-        return self.request_params.get(param_name, if_none)
-
-    def delete_parameter(self):
+    def delete_parameter(self) -> Union[str, Tuple[str, Dict[str, int]]]:
         name = self._get_param("Name")
         result = self.ssm_backend.delete_parameter(name)
         if result is None:
             error = {
                 "__type": "ParameterNotFound",
                 "message": f"Parameter {name} not found.",
             }
             return json.dumps(error), dict(status=400)
         return json.dumps({})
 
-    def delete_parameters(self):
+    def delete_parameters(self) -> str:
         names = self._get_param("Names")
         result = self.ssm_backend.delete_parameters(names)
 
-        response = {"DeletedParameters": [], "InvalidParameters": []}
+        response: Dict[str, Any] = {"DeletedParameters": [], "InvalidParameters": []}
 
         for name in names:
             if name in result:
                 response["DeletedParameters"].append(name)
             else:
                 response["InvalidParameters"].append(name)
         return json.dumps(response)
 
-    def get_parameter(self):
+    def get_parameter(self) -> Union[str, Tuple[str, Dict[str, int]]]:
         name = self._get_param("Name")
         with_decryption = self._get_param("WithDecryption")
 
         if (
             name.startswith("/aws/reference/secretsmanager/")
             and with_decryption is not True
         ):
@@ -198,33 +190,33 @@
                 "message": f"Parameter {name} not found.",
             }
             return json.dumps(error), dict(status=400)
 
         response = {"Parameter": result.response_object(with_decryption, self.region)}
         return json.dumps(response)
 
-    def get_parameters(self):
+    def get_parameters(self) -> str:
         names = self._get_param("Names")
         with_decryption = self._get_param("WithDecryption")
 
         result = self.ssm_backend.get_parameters(names)
 
-        response = {"Parameters": [], "InvalidParameters": []}
+        response: Dict[str, Any] = {"Parameters": [], "InvalidParameters": []}
 
         for name, parameter in result.items():
             param_data = parameter.response_object(with_decryption, self.region)
             response["Parameters"].append(param_data)
 
         valid_param_names = [name for name, parameter in result.items()]
         for name in names:
             if name not in valid_param_names:
                 response["InvalidParameters"].append(name)
         return json.dumps(response)
 
-    def get_parameters_by_path(self):
+    def get_parameters_by_path(self) -> str:
         path = self._get_param("Path")
         with_decryption = self._get_param("WithDecryption")
         recursive = self._get_param("Recursive", False)
         filters = self._get_param("ParameterFilters")
         token = self._get_param("NextToken")
         max_results = self._get_param("MaxResults", 10)
 
@@ -232,49 +224,49 @@
             path,
             recursive,
             filters,
             next_token=token,
             max_results=max_results,
         )
 
-        response = {"Parameters": [], "NextToken": next_token}
+        response: Dict[str, Any] = {"Parameters": [], "NextToken": next_token}
 
         for parameter in result:
             param_data = parameter.response_object(with_decryption, self.region)
             response["Parameters"].append(param_data)
 
         return json.dumps(response)
 
-    def describe_parameters(self):
+    def describe_parameters(self) -> str:
         page_size = 10
         filters = self._get_param("Filters")
         parameter_filters = self._get_param("ParameterFilters")
         token = self._get_param("NextToken")
         if hasattr(token, "strip"):
             token = token.strip()
         if not token:
             token = "0"
         token = int(token)
 
         result = self.ssm_backend.describe_parameters(filters, parameter_filters)
 
-        response = {"Parameters": []}
+        response: Dict[str, Any] = {"Parameters": []}
 
         end = token + page_size
         for parameter in result[token:]:
             response["Parameters"].append(parameter.describe_response_object(False))
 
             token += 1
             if len(response["Parameters"]) == page_size:
                 response["NextToken"] = str(end)
                 break
 
         return json.dumps(response)
 
-    def put_parameter(self):
+    def put_parameter(self) -> Union[str, Tuple[str, Dict[str, int]]]:
         name = self._get_param("Name")
         description = self._get_param("Description")
         value = self._get_param("Value")
         type_ = self._get_param("Type")
         allowed_pattern = self._get_param("AllowedPattern")
         keyid = self._get_param("KeyId")
         overwrite = self._get_param("Overwrite", False)
@@ -299,15 +291,15 @@
                 "message": f"Parameter {name} already exists.",
             }
             return json.dumps(error), dict(status=400)
 
         response = {"Version": result}
         return json.dumps(response)
 
-    def get_parameter_history(self):
+    def get_parameter_history(self) -> Union[str, Tuple[str, Dict[str, int]]]:
         name = self._get_param("Name")
         with_decryption = self._get_param("WithDecryption")
         next_token = self._get_param("NextToken")
         max_results = self._get_param("MaxResults", 50)
 
         result, new_next_token = self.ssm_backend.get_parameter_history(
             name, next_token, max_results
@@ -316,112 +308,146 @@
         if result is None:
             error = {
                 "__type": "ParameterNotFound",
                 "message": f"Parameter {name} not found.",
             }
             return json.dumps(error), dict(status=400)
 
-        response = {"Parameters": []}
-        for parameter_version in result:
-            param_data = parameter_version.describe_response_object(
-                decrypt=with_decryption, include_labels=True
-            )
-            response["Parameters"].append(param_data)
-
-        if new_next_token is not None:
-            response["NextToken"] = new_next_token
+        response = {
+            "Parameters": [
+                p_v.describe_response_object(
+                    decrypt=with_decryption, include_labels=True
+                )
+                for p_v in result
+            ],
+            "NextToken": new_next_token,
+        }
 
         return json.dumps(response)
 
-    def label_parameter_version(self):
+    def label_parameter_version(self) -> str:
         name = self._get_param("Name")
         version = self._get_param("ParameterVersion")
         labels = self._get_param("Labels")
 
         invalid_labels, version = self.ssm_backend.label_parameter_version(
             name, version, labels
         )
 
         response = {"InvalidLabels": invalid_labels, "ParameterVersion": version}
         return json.dumps(response)
 
-    def add_tags_to_resource(self):
+    def add_tags_to_resource(self) -> str:
         resource_id = self._get_param("ResourceId")
         resource_type = self._get_param("ResourceType")
         tags = {t["Key"]: t["Value"] for t in self._get_param("Tags")}
         self.ssm_backend.add_tags_to_resource(
             resource_type=resource_type, resource_id=resource_id, tags=tags
         )
         return json.dumps({})
 
-    def remove_tags_from_resource(self):
+    def remove_tags_from_resource(self) -> str:
         resource_id = self._get_param("ResourceId")
         resource_type = self._get_param("ResourceType")
         keys = self._get_param("TagKeys")
         self.ssm_backend.remove_tags_from_resource(
             resource_type=resource_type, resource_id=resource_id, keys=keys
         )
         return json.dumps({})
 
-    def list_tags_for_resource(self):
+    def list_tags_for_resource(self) -> str:
         resource_id = self._get_param("ResourceId")
         resource_type = self._get_param("ResourceType")
         tags = self.ssm_backend.list_tags_for_resource(
             resource_type=resource_type, resource_id=resource_id
         )
         tag_list = [{"Key": k, "Value": v} for (k, v) in tags.items()]
         response = {"TagList": tag_list}
         return json.dumps(response)
 
-    def send_command(self):
-        return json.dumps(self.ssm_backend.send_command(**self.request_params))
-
-    def list_commands(self):
-        return json.dumps(self.ssm_backend.list_commands(**self.request_params))
+    def send_command(self) -> str:
+        comment = self._get_param("Comment", "")
+        document_name = self._get_param("DocumentName")
+        timeout_seconds = self._get_int_param("TimeoutSeconds")
+        instance_ids = self._get_param("InstanceIds", [])
+        max_concurrency = self._get_param("MaxConcurrency", "50")
+        max_errors = self._get_param("MaxErrors", "0")
+        notification_config = self._get_param("NotificationConfig")
+        output_s3_bucket_name = self._get_param("OutputS3BucketName", "")
+        output_s3_key_prefix = self._get_param("OutputS3KeyPrefix", "")
+        output_s3_region = self._get_param("OutputS3Region", "")
+        parameters = self._get_param("Parameters", {})
+        service_role_arn = self._get_param("ServiceRoleArn", "")
+        targets = self._get_param("Targets", [])
+        command = self.ssm_backend.send_command(
+            comment=comment,
+            document_name=document_name,
+            timeout_seconds=timeout_seconds,
+            instance_ids=instance_ids,
+            max_concurrency=max_concurrency,
+            max_errors=max_errors,
+            notification_config=notification_config,
+            output_s3_bucket_name=output_s3_bucket_name,
+            output_s3_key_prefix=output_s3_key_prefix,
+            output_s3_region=output_s3_region,
+            parameters=parameters,
+            service_role_arn=service_role_arn,
+            targets=targets,
+        )
+        return json.dumps({"Command": command.response_object()})
+
+    def list_commands(self) -> str:
+        command_id = self._get_param("CommandId")
+        instance_id = self._get_param("InstanceId")
+        commands = self.ssm_backend.list_commands(command_id, instance_id)
+        response = {"Commands": [command.response_object() for command in commands]}
+        return json.dumps(response)
 
-    def get_command_invocation(self):
-        return json.dumps(
-            self.ssm_backend.get_command_invocation(**self.request_params)
+    def get_command_invocation(self) -> str:
+        command_id = self._get_param("CommandId")
+        instance_id = self._get_param("InstanceId")
+        plugin_name = self._get_param("PluginName")
+        response = self.ssm_backend.get_command_invocation(
+            command_id, instance_id, plugin_name
         )
+        return json.dumps(response)
 
-    def create_maintenance_window(self):
+    def create_maintenance_window(self) -> str:
         name = self._get_param("Name")
         desc = self._get_param("Description", None)
-        enabled = self._get_bool_param("Enabled", True)
         duration = self._get_int_param("Duration")
         cutoff = self._get_int_param("Cutoff")
         schedule = self._get_param("Schedule")
         schedule_timezone = self._get_param("ScheduleTimezone")
         schedule_offset = self._get_int_param("ScheduleOffset")
         start_date = self._get_param("StartDate")
         end_date = self._get_param("EndDate")
         window_id = self.ssm_backend.create_maintenance_window(
             name=name,
             description=desc,
-            enabled=enabled,
             duration=duration,
             cutoff=cutoff,
             schedule=schedule,
             schedule_timezone=schedule_timezone,
             schedule_offset=schedule_offset,
             start_date=start_date,
             end_date=end_date,
         )
         return json.dumps({"WindowId": window_id})
 
-    def get_maintenance_window(self):
+    def get_maintenance_window(self) -> str:
         window_id = self._get_param("WindowId")
         window = self.ssm_backend.get_maintenance_window(window_id)
         return json.dumps(window.to_json())
 
-    def describe_maintenance_windows(self):
+    def describe_maintenance_windows(self) -> str:
         filters = self._get_param("Filters", None)
         windows = [
             window.to_json()
             for window in self.ssm_backend.describe_maintenance_windows(filters)
         ]
         return json.dumps({"WindowIdentities": windows})
 
-    def delete_maintenance_window(self):
+    def delete_maintenance_window(self) -> str:
         window_id = self._get_param("WindowId")
         self.ssm_backend.delete_maintenance_window(window_id)
         return "{}"
```

### Comparing `moto-4.1.9.dev3/moto/ssm/utils.py` & `moto-4.1.9.dev5/moto/ssm/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-def parameter_arn(account_id, region, parameter_name):
+from typing import Any, Dict, List
+
+
+def parameter_arn(account_id: str, region: str, parameter_name: str) -> str:
     if parameter_name[0] == "/":
         parameter_name = parameter_name[1:]
     return f"arn:aws:ssm:{region}:{account_id}:parameter/{parameter_name}"
 
 
-def convert_to_tree(parameters):
+def convert_to_tree(parameters: List[Dict[str, Any]]) -> Dict[str, Any]:
     """
     Convert input into a smaller, less redundant data set in tree form
     Input: [{"Name": "/a/b/c", "Value": "af-south-1", ...}, ..]
     Output: {"a": {"b": {"c": {"Value": af-south-1}, ..}, ..}, ..}
     """
-    tree_dict = {}
+    tree_dict: Dict[str, Any] = {}
     for p in parameters:
         current_level = tree_dict
         for path in p["Name"].split("/"):
             if path == "":
                 continue
             if path not in current_level:
                 current_level[path] = {}
             current_level = current_level[path]
         current_level["Value"] = p["Value"]
     return tree_dict
 
 
-def convert_to_params(tree):
+def convert_to_params(tree: Dict[str, Any]) -> List[Dict[str, Any]]:
     """
     Inverse of 'convert_to_tree'
     """
 
-    def m(tree, params, current_path=""):
+    def m(
+        tree: Dict[str, Any], params: List[Dict[str, Any]], current_path: str = ""
+    ) -> None:
         for key, value in tree.items():
             if key == "Value":
                 params.append({"Name": current_path, "Value": value})
             else:
                 m(value, params, current_path + "/" + key)
 
-    params = []
+    params: List[Dict[str, Any]] = []
     m(tree, params)
     return params
```

### Comparing `moto-4.1.9.dev3/moto/ssoadmin/models.py` & `moto-4.1.9.dev5/moto/ssoadmin/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/ssoadmin/responses.py` & `moto-4.1.9.dev5/moto/ssoadmin/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/stepfunctions/exceptions.py` & `moto-4.1.9.dev5/moto/stepfunctions/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/stepfunctions/models.py` & `moto-4.1.9.dev5/moto/stepfunctions/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/stepfunctions/responses.py` & `moto-4.1.9.dev5/moto/stepfunctions/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/stepfunctions/utils.py` & `moto-4.1.9.dev5/moto/stepfunctions/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sts/models.py` & `moto-4.1.9.dev5/moto/sts/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sts/responses.py` & `moto-4.1.9.dev5/moto/sts/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/sts/utils.py` & `moto-4.1.9.dev5/moto/sts/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/support/models.py` & `moto-4.1.9.dev5/moto/support/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/support/resources/describe_trusted_advisor_checks.json` & `moto-4.1.9.dev5/moto/support/resources/describe_trusted_advisor_checks.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/support/responses.py` & `moto-4.1.9.dev5/moto/support/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/constants.py` & `moto-4.1.9.dev5/moto/swf/constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/exceptions.py` & `moto-4.1.9.dev5/moto/swf/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/models/__init__.py` & `moto-4.1.9.dev5/moto/swf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/models/activity_task.py` & `moto-4.1.9.dev5/moto/swf/models/activity_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/models/decision_task.py` & `moto-4.1.9.dev5/moto/swf/models/decision_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/models/domain.py` & `moto-4.1.9.dev5/moto/swf/models/domain.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/models/generic_type.py` & `moto-4.1.9.dev5/moto/swf/models/generic_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/models/history_event.py` & `moto-4.1.9.dev5/moto/swf/models/history_event.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/models/workflow_execution.py` & `moto-4.1.9.dev5/moto/swf/models/workflow_execution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/swf/responses.py` & `moto-4.1.9.dev5/moto/swf/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/textract/exceptions.py` & `moto-4.1.9.dev5/moto/textract/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/textract/models.py` & `moto-4.1.9.dev5/moto/textract/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/textract/responses.py` & `moto-4.1.9.dev5/moto/textract/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/timestreamwrite/models.py` & `moto-4.1.9.dev5/moto/timestreamwrite/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/timestreamwrite/responses.py` & `moto-4.1.9.dev5/moto/timestreamwrite/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/transcribe/models.py` & `moto-4.1.9.dev5/moto/transcribe/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/transcribe/responses.py` & `moto-4.1.9.dev5/moto/transcribe/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/utilities/aws_headers.py` & `moto-4.1.9.dev5/moto/utilities/aws_headers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/utilities/distutils_version.py` & `moto-4.1.9.dev5/moto/utilities/distutils_version.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/utilities/docker_utilities.py` & `moto-4.1.9.dev5/moto/utilities/docker_utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/utilities/paginator.py` & `moto-4.1.9.dev5/moto/utilities/paginator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/utilities/tagging_service.py` & `moto-4.1.9.dev5/moto/utilities/tagging_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/utilities/tokenizer.py` & `moto-4.1.9.dev5/moto/utilities/tokenizer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/utilities/utils.py` & `moto-4.1.9.dev5/moto/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/wafv2/exceptions.py` & `moto-4.1.9.dev5/moto/wafv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/wafv2/models.py` & `moto-4.1.9.dev5/moto/wafv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/wafv2/responses.py` & `moto-4.1.9.dev5/moto/wafv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/xray/exceptions.py` & `moto-4.1.9.dev5/moto/xray/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/xray/mock_client.py` & `moto-4.1.9.dev5/moto/xray/mock_client.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/xray/models.py` & `moto-4.1.9.dev5/moto/xray/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto/xray/responses.py` & `moto-4.1.9.dev5/moto/xray/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto.egg-info/PKG-INFO` & `moto-4.1.9.dev5/moto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moto
-Version: 4.1.9.dev3
+Version: 4.1.9.dev5
 Home-page: https://github.com/getmoto/moto
 Author: Steve Pulec
 Author-email: "spulec@gmail.com"
 License: Apache License 2.0
 Project-URL: Documentation, http://docs.getmoto.org/en/latest/
 Project-URL: Issue tracker, https://github.com/getmoto/moto/issues
 Project-URL: Changelog, https://github.com/getmoto/moto/blob/master/CHANGELOG.md
```

### Comparing `moto-4.1.9.dev3/moto.egg-info/SOURCES.txt` & `moto-4.1.9.dev5/moto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/moto.egg-info/requires.txt` & `moto-4.1.9.dev5/moto.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/setup.cfg` & `moto-4.1.9.dev5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = moto
-version = 4.1.9.dev3
+version = 4.1.9.dev5
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Steve Pulec
 author_email = "spulec@gmail.com"
 url = https://github.com/getmoto/moto
 license = Apache License 2.0
 test_suite = tests
@@ -232,15 +232,15 @@
 ignore-paths = moto/packages
 
 [pylint.'MESSAGES CONTROL']
 disable = W,C,R,E
 enable = anomalous-backslash-in-string, arguments-renamed, dangerous-default-value, deprecated-module, function-redefined, import-self, redefined-builtin, redefined-outer-name, reimported, pointless-statement, super-with-arguments, unused-argument, unused-import, unused-variable, useless-else-on-loop, wildcard-import
 
 [mypy]
-files = moto/a*,moto/b*,moto/c*,moto/d*,moto/e*,moto/f*,moto/g*,moto/i*,moto/k*,moto/l*,moto/m*,moto/n*,moto/o*,moto/p*,moto/q*,moto/r*,moto/s3*,moto/sagemaker,moto/secretsmanager,moto/scheduler
+files = moto/a*,moto/b*,moto/c*,moto/d*,moto/e*,moto/f*,moto/g*,moto/i*,moto/k*,moto/l*,moto/m*,moto/n*,moto/o*,moto/p*,moto/q*,moto/r*,moto/s3*,moto/sagemaker,moto/secretsmanager,moto/ssm,moto/scheduler
 show_column_numbers = True
 show_error_codes = True
 disable_error_code = abstract
 disallow_any_unimported = False
 disallow_any_expr = False
 disallow_any_decorated = True
 disallow_any_explicit = False
```

### Comparing `moto-4.1.9.dev3/tests/__init__.py` & `moto-4.1.9.dev5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/helpers.py` & `moto-4.1.9.dev5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acm/resources/README.md` & `moto-4.1.9.dev5/tests/test_acm/resources/README.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acm/resources/ca.key` & `moto-4.1.9.dev5/tests/test_acm/resources/ca.key`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acm/resources/ca.pem` & `moto-4.1.9.dev5/tests/test_acm/resources/ca.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acm/resources/star_moto_com-bad.pem` & `moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com-bad.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acm/resources/star_moto_com.csr` & `moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.csr`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acm/resources/star_moto_com.key` & `moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.key`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acm/resources/star_moto_com.pem` & `moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acm/test_acm.py` & `moto-4.1.9.dev5/tests/test_acm/test_acm.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_acmpca/test_acmpca.py` & `moto-4.1.9.dev5/tests/test_acmpca/test_acmpca.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_amp/test_amp_logging_config.py` & `moto-4.1.9.dev5/tests/test_amp/test_amp_logging_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_amp/test_amp_rulegroupnamespaces.py` & `moto-4.1.9.dev5/tests/test_amp/test_amp_rulegroupnamespaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_amp/test_amp_workspaces.py` & `moto-4.1.9.dev5/tests/test_amp/test_amp_workspaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/resources/petstore-swagger-v3.yaml` & `moto-4.1.9.dev5/tests/test_apigateway/resources/petstore-swagger-v3.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/resources/test_api.json` & `moto-4.1.9.dev5/tests/test_apigateway/resources/test_api.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/resources/test_api.yaml` & `moto-4.1.9.dev5/tests/test_apigateway/resources/test_api.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/resources/test_api_invalid.json` & `moto-4.1.9.dev5/tests/test_apigateway/resources/test_api_invalid.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/resources/test_api_invalid_version.json` & `moto-4.1.9.dev5/tests/test_apigateway/resources/test_api_invalid_version.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/resources/test_deep_api.yaml` & `moto-4.1.9.dev5/tests/test_apigateway/resources/test_deep_api.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_cloudformation.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_deployments.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_deployments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_export.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_export.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_gatewayresponses.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_gatewayresponses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_importrestapi.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_importrestapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_integration.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_putrestapi.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_putrestapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_stage.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_stage.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_validators.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_apigateway_vpclink.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_vpclink.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigateway/test_server.py` & `moto-4.1.9.dev5/tests/test_apigateway/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_domains.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_integrations.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_mappings.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_mappings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_models.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_reimport.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_reimport.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_routes.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_routes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_tags.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py` & `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_applicationautoscaling/test_applicationautoscaling.py` & `moto-4.1.9.dev5/tests/test_applicationautoscaling/test_applicationautoscaling.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_applicationautoscaling/test_validation.py` & `moto-4.1.9.dev5/tests/test_applicationautoscaling/test_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_appsync/test_appsync.py` & `moto-4.1.9.dev5/tests/test_appsync/test_appsync.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_appsync/test_appsync_apikeys.py` & `moto-4.1.9.dev5/tests/test_appsync/test_appsync_apikeys.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_appsync/test_appsync_schema.py` & `moto-4.1.9.dev5/tests/test_appsync/test_appsync_schema.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_appsync/test_appsync_tags.py` & `moto-4.1.9.dev5/tests/test_appsync/test_appsync_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_athena/test_athena.py` & `moto-4.1.9.dev5/tests/test_athena/test_athena.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_athena/test_athena_server_api.py` & `moto-4.1.9.dev5/tests/test_athena/test_athena_server_api.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_cloudformation.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_groups.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_metrics.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_metrics.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_scheduledactions.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_scheduledactions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_autoscaling_tags.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_elb.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_elb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_elbv2.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_elbv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_launch_configurations.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_launch_configurations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/test_policies.py` & `moto-4.1.9.dev5/tests/test_autoscaling/test_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_autoscaling/utils.py` & `moto-4.1.9.dev5/tests/test_autoscaling/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_awslambda_cloudformation.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_awslambda_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda_alias.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_alias.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda_concurrency.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_concurrency.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda_eventsourcemapping.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_eventsourcemapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda_function_urls.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_function_urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda_invoke.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_invoke.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda_layers.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_layers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda_policy.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_lambda_tags.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/test_policy.py` & `moto-4.1.9.dev5/tests/test_awslambda/test_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_awslambda/utilities.py` & `moto-4.1.9.dev5/tests/test_awslambda/utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/__init__.py` & `moto-4.1.9.dev5/tests/test_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/test_batch_cloudformation.py` & `moto-4.1.9.dev5/tests/test_batch/test_batch_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/test_batch_compute_envs.py` & `moto-4.1.9.dev5/tests/test_batch/test_batch_compute_envs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/test_batch_job_queue.py` & `moto-4.1.9.dev5/tests/test_batch/test_batch_job_queue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/test_batch_jobs.py` & `moto-4.1.9.dev5/tests/test_batch/test_batch_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/test_batch_scheduling_policy.py` & `moto-4.1.9.dev5/tests/test_batch/test_batch_scheduling_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/test_batch_tags_job_definition.py` & `moto-4.1.9.dev5/tests/test_batch/test_batch_tags_job_definition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/test_batch_tags_job_queue.py` & `moto-4.1.9.dev5/tests/test_batch/test_batch_tags_job_queue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch/test_batch_task_definition.py` & `moto-4.1.9.dev5/tests/test_batch/test_batch_task_definition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch_simple/test_batch_cloudformation.py` & `moto-4.1.9.dev5/tests/test_batch_simple/test_batch_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch_simple/test_batch_compute_envs.py` & `moto-4.1.9.dev5/tests/test_batch_simple/test_batch_compute_envs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_batch_simple/test_batch_jobs.py` & `moto-4.1.9.dev5/tests/test_batch_simple/test_batch_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_budgets/test_budgets.py` & `moto-4.1.9.dev5/tests/test_budgets/test_budgets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_budgets/test_notifications.py` & `moto-4.1.9.dev5/tests/test_budgets/test_notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_budgets/test_server.py` & `moto-4.1.9.dev5/tests/test_budgets/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ce/test_ce.py` & `moto-4.1.9.dev5/tests/test_ce/test_ce.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ce/test_ce_tags.py` & `moto-4.1.9.dev5/tests/test_ce/test_ce_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/custom_lambda.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/custom_lambda.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/kms_key.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/kms_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/redshift.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/redshift.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/route53_health_check.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_health_check.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/route53_roundrobin.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_roundrobin.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/vpc_eni.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_eni.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py` & `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_custom_resources.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_custom_resources.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_depends_on.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_depends_on.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_multi_accounts.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_multi_accounts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_nested_stacks.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_nested_stacks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_stack_integration.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_cloudformation_stack_policies.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_import_value.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_import_value.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_server.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_stack_parsing.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_stack_parsing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudformation/test_validate.py` & `moto-4.1.9.dev5/tests/test_cloudformation/test_validate.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudfront/cloudfront_test_scaffolding.py` & `moto-4.1.9.dev5/tests/test_cloudfront/cloudfront_test_scaffolding.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudfront/test_cloudfront.py` & `moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudfront/test_cloudfront_dist_tags.py` & `moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_dist_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudfront/test_cloudfront_distributions.py` & `moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_distributions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudfront/test_cloudfront_invalidation.py` & `moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_invalidation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudtrail/test_cloudtrail.py` & `moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudtrail/test_cloudtrail_eventselectors.py` & `moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail_eventselectors.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudtrail/test_cloudtrail_tags.py` & `moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudtrail/test_server.py` & `moto-4.1.9.dev5/tests/test_cloudtrail/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudwatch/test_cloudwatch_alarms.py` & `moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_alarms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudwatch/test_cloudwatch_boto3.py` & `moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudwatch/test_cloudwatch_dashboards.py` & `moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_dashboards.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cloudwatch/test_cloudwatch_tags.py` & `moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_codebuild/test_codebuild.py` & `moto-4.1.9.dev5/tests/test_codebuild/test_codebuild.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_codecommit/test_codecommit.py` & `moto-4.1.9.dev5/tests/test_codecommit/test_codecommit.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_codepipeline/test_codepipeline.py` & `moto-4.1.9.dev5/tests/test_codepipeline/test_codepipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cognitoidentity/test_cognitoidentity.py` & `moto-4.1.9.dev5/tests/test_cognitoidentity/test_cognitoidentity.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cognitoidentity/test_server.py` & `moto-4.1.9.dev5/tests/test_cognitoidentity/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cognitoidp/test_cognitoidp.py` & `moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cognitoidp/test_cognitoidp_exceptions.py` & `moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cognitoidp/test_cognitoidp_replay.py` & `moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp_replay.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_cognitoidp/test_server.py` & `moto-4.1.9.dev5/tests/test_cognitoidp/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_comprehend/test_comprehend.py` & `moto-4.1.9.dev5/tests/test_comprehend/test_comprehend.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_config/test_config.py` & `moto-4.1.9.dev5/tests/test_config/test_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_config/test_config_rules.py` & `moto-4.1.9.dev5/tests/test_config/test_config_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_config/test_config_rules_integration.py` & `moto-4.1.9.dev5/tests/test_config/test_config_rules_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_config/test_config_tags.py` & `moto-4.1.9.dev5/tests/test_config/test_config_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_account_id_resolution.py` & `moto-4.1.9.dev5/tests/test_core/test_account_id_resolution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_auth.py` & `moto-4.1.9.dev5/tests/test_core/test_auth.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_backenddict.py` & `moto-4.1.9.dev5/tests/test_core/test_backenddict.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_decorator_calls.py` & `moto-4.1.9.dev5/tests/test_core/test_decorator_calls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_docker.py` & `moto-4.1.9.dev5/tests/test_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_environ_patching.py` & `moto-4.1.9.dev5/tests/test_core/test_environ_patching.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_importorder.py` & `moto-4.1.9.dev5/tests/test_core/test_importorder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_instance_metadata.py` & `moto-4.1.9.dev5/tests/test_core/test_instance_metadata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_mock_all.py` & `moto-4.1.9.dev5/tests/test_core/test_mock_all.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_mock_regions.py` & `moto-4.1.9.dev5/tests/test_core/test_mock_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_moto_api.py` & `moto-4.1.9.dev5/tests/test_core/test_moto_api.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_nested.py` & `moto-4.1.9.dev5/tests/test_core/test_nested.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_request_mocking.py` & `moto-4.1.9.dev5/tests/test_core/test_request_mocking.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_responses.py` & `moto-4.1.9.dev5/tests/test_core/test_responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_responses_module.py` & `moto-4.1.9.dev5/tests/test_core/test_responses_module.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_server.py` & `moto-4.1.9.dev5/tests/test_core/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_settings.py` & `moto-4.1.9.dev5/tests/test_core/test_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_url_base_regex.py` & `moto-4.1.9.dev5/tests/test_core/test_url_base_regex.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_url_mapping.py` & `moto-4.1.9.dev5/tests/test_core/test_url_mapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_core/test_utils.py` & `moto-4.1.9.dev5/tests/test_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_databrew/test_databrew_datasets.py` & `moto-4.1.9.dev5/tests/test_databrew/test_databrew_datasets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_databrew/test_databrew_jobs.py` & `moto-4.1.9.dev5/tests/test_databrew/test_databrew_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_databrew/test_databrew_recipes.py` & `moto-4.1.9.dev5/tests/test_databrew/test_databrew_recipes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_databrew/test_databrew_rulesets.py` & `moto-4.1.9.dev5/tests/test_databrew/test_databrew_rulesets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_datapipeline/test_datapipeline.py` & `moto-4.1.9.dev5/tests/test_datapipeline/test_datapipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_datapipeline/test_datapipeline_cloudformation.py` & `moto-4.1.9.dev5/tests/test_datapipeline/test_datapipeline_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_datapipeline/test_server.py` & `moto-4.1.9.dev5/tests/test_datapipeline/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_datasync/test_datasync.py` & `moto-4.1.9.dev5/tests/test_datasync/test_datasync.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dax/test_dax.py` & `moto-4.1.9.dev5/tests/test_dax/test_dax.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dms/test_dms.py` & `moto-4.1.9.dev5/tests/test_dms/test_dms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ds/test_ds.py` & `moto-4.1.9.dev5/tests/test_ds/test_ds.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ds/test_ds_ad_connect.py` & `moto-4.1.9.dev5/tests/test_ds/test_ds_ad_connect.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ds/test_ds_microsoft_ad.py` & `moto-4.1.9.dev5/tests/test_ds/test_ds_microsoft_ad.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ds/test_ds_simple_ad_directory.py` & `moto-4.1.9.dev5/tests/test_ds/test_ds_simple_ad_directory.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ds/test_ds_tags.py` & `moto-4.1.9.dev5/tests/test_ds/test_ds_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/conftest.py` & `moto-4.1.9.dev5/tests/test_dynamodb/conftest.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py` & `moto-4.1.9.dev5/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/exceptions/test_key_length_exceptions.py` & `moto-4.1.9.dev5/tests/test_dynamodb/exceptions/test_key_length_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/models/test_key_condition_expression_parser.py` & `moto-4.1.9.dev5/tests/test_dynamodb/models/test_key_condition_expression_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_batch_get_item.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_batch_get_item.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_cloudformation.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_condition_expressions.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_condition_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_consumedcapacity.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_consumedcapacity.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_create_table.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_create_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_executor.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_executor.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_expressions.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_statements.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_statements.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_table_with_range_key.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_table_with_range_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_table_without_range_key.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_table_without_range_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_update_expressions.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_update_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_update_table.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_update_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_dynamodb_validation.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb/test_server.py` & `moto-4.1.9.dev5/tests/test_dynamodb/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb_v20111205/test_server.py` & `moto-4.1.9.dev5/tests/test_dynamodb_v20111205/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodb_v20111205/test_servermode.py` & `moto-4.1.9.dev5/tests/test_dynamodb_v20111205/test_servermode.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_dynamodbstreams/test_dynamodbstreams.py` & `moto-4.1.9.dev5/tests/test_dynamodbstreams/test_dynamodbstreams.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ebs/test_ebs.py` & `moto-4.1.9.dev5/tests/test_ebs/test_ebs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_account_attributes.py` & `moto-4.1.9.dev5/tests/test_ec2/test_account_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_amis.py` & `moto-4.1.9.dev5/tests/test_ec2/test_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_availability_zones_and_regions.py` & `moto-4.1.9.dev5/tests/test_ec2/test_availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_carrier_gateways.py` & `moto-4.1.9.dev5/tests/test_ec2/test_carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_customer_gateways.py` & `moto-4.1.9.dev5/tests/test_ec2/test_customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_dhcp_options.py` & `moto-4.1.9.dev5/tests/test_ec2/test_dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_ec2_cloudformation.py` & `moto-4.1.9.dev5/tests/test_ec2/test_ec2_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_ec2_integration.py` & `moto-4.1.9.dev5/tests/test_ec2/test_ec2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_egress_only_igw.py` & `moto-4.1.9.dev5/tests/test_ec2/test_egress_only_igw.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_elastic_block_store.py` & `moto-4.1.9.dev5/tests/test_ec2/test_elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_elastic_ip_addresses.py` & `moto-4.1.9.dev5/tests/test_ec2/test_elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_elastic_network_interfaces.py` & `moto-4.1.9.dev5/tests/test_ec2/test_elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_fleets.py` & `moto-4.1.9.dev5/tests/test_ec2/test_fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_flow_logs.py` & `moto-4.1.9.dev5/tests/test_ec2/test_flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_flow_logs_cloudformation.py` & `moto-4.1.9.dev5/tests/test_ec2/test_flow_logs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_general.py` & `moto-4.1.9.dev5/tests/test_ec2/test_general.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_hosts.py` & `moto-4.1.9.dev5/tests/test_ec2/test_hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_iam_integration.py` & `moto-4.1.9.dev5/tests/test_ec2/test_iam_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_instance_type_offerings.py` & `moto-4.1.9.dev5/tests/test_ec2/test_instance_type_offerings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_instance_types.py` & `moto-4.1.9.dev5/tests/test_ec2/test_instance_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_instances.py` & `moto-4.1.9.dev5/tests/test_ec2/test_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_internet_gateways.py` & `moto-4.1.9.dev5/tests/test_ec2/test_internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_key_pairs.py` & `moto-4.1.9.dev5/tests/test_ec2/test_key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_launch_templates.py` & `moto-4.1.9.dev5/tests/test_ec2/test_launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_nat_gateway.py` & `moto-4.1.9.dev5/tests/test_ec2/test_nat_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_network_acls.py` & `moto-4.1.9.dev5/tests/test_ec2/test_network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_prefix_lists.py` & `moto-4.1.9.dev5/tests/test_ec2/test_prefix_lists.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_regions.py` & `moto-4.1.9.dev5/tests/test_ec2/test_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_route_tables.py` & `moto-4.1.9.dev5/tests/test_ec2/test_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_security_groups.py` & `moto-4.1.9.dev5/tests/test_ec2/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_security_groups_cloudformation.py` & `moto-4.1.9.dev5/tests/test_ec2/test_security_groups_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_server.py` & `moto-4.1.9.dev5/tests/test_ec2/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_settings.py` & `moto-4.1.9.dev5/tests/test_ec2/test_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_spot_fleet.py` & `moto-4.1.9.dev5/tests/test_ec2/test_spot_fleet.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_spot_instances.py` & `moto-4.1.9.dev5/tests/test_ec2/test_spot_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_subnets.py` & `moto-4.1.9.dev5/tests/test_ec2/test_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_tags.py` & `moto-4.1.9.dev5/tests/test_ec2/test_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_transit_gateway.py` & `moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_transit_gateway_cloudformation.py` & `moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_transit_gateway_peering_attachments.py` & `moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway_peering_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_utils.py` & `moto-4.1.9.dev5/tests/test_ec2/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_virtual_private_gateways.py` & `moto-4.1.9.dev5/tests/test_ec2/test_virtual_private_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_vpc_endpoint_services_integration.py` & `moto-4.1.9.dev5/tests/test_ec2/test_vpc_endpoint_services_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_vpc_peering.py` & `moto-4.1.9.dev5/tests/test_ec2/test_vpc_peering.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_vpc_service_configuration.py` & `moto-4.1.9.dev5/tests/test_ec2/test_vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_vpcs.py` & `moto-4.1.9.dev5/tests/test_ec2/test_vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_vpn_connections.py` & `moto-4.1.9.dev5/tests/test_ec2/test_vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2/test_windows.py` & `moto-4.1.9.dev5/tests/test_ec2/test_windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py` & `moto-4.1.9.dev5/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecr/test_ecr_boto3.py` & `moto-4.1.9.dev5/tests/test_ecr/test_ecr_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecr/test_ecr_cloudformation.py` & `moto-4.1.9.dev5/tests/test_ecr/test_ecr_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecr/test_ecr_helpers.py` & `moto-4.1.9.dev5/tests/test_ecr/test_ecr_helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecr/test_ecr_policy_validation.py` & `moto-4.1.9.dev5/tests/test_ecr/test_ecr_policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecs/test_ecs_account_settings.py` & `moto-4.1.9.dev5/tests/test_ecs/test_ecs_account_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecs/test_ecs_boto3.py` & `moto-4.1.9.dev5/tests/test_ecs/test_ecs_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecs/test_ecs_capacity_provider.py` & `moto-4.1.9.dev5/tests/test_ecs/test_ecs_capacity_provider.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecs/test_ecs_cloudformation.py` & `moto-4.1.9.dev5/tests/test_ecs/test_ecs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecs/test_ecs_efs.py` & `moto-4.1.9.dev5/tests/test_ecs/test_ecs_efs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecs/test_ecs_task_def_tags.py` & `moto-4.1.9.dev5/tests/test_ecs/test_ecs_task_def_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ecs/test_ecs_tasksets.py` & `moto-4.1.9.dev5/tests/test_ecs/test_ecs_tasksets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_efs/test_access_point_tagging.py` & `moto-4.1.9.dev5/tests/test_efs/test_access_point_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_efs/test_access_points.py` & `moto-4.1.9.dev5/tests/test_efs/test_access_points.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_efs/test_file_system.py` & `moto-4.1.9.dev5/tests/test_efs/test_file_system.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_efs/test_filesystem_tagging.py` & `moto-4.1.9.dev5/tests/test_efs/test_filesystem_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_efs/test_lifecycle_config.py` & `moto-4.1.9.dev5/tests/test_efs/test_lifecycle_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_efs/test_mount_target.py` & `moto-4.1.9.dev5/tests/test_efs/test_mount_target.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_efs/test_mount_target_security_groups.py` & `moto-4.1.9.dev5/tests/test_efs/test_mount_target_security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_efs/test_server.py` & `moto-4.1.9.dev5/tests/test_efs/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_eks/test_eks.py` & `moto-4.1.9.dev5/tests/test_eks/test_eks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_eks/test_eks_constants.py` & `moto-4.1.9.dev5/tests/test_eks/test_eks_constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_eks/test_eks_ec2.py` & `moto-4.1.9.dev5/tests/test_eks/test_eks_ec2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_eks/test_eks_utils.py` & `moto-4.1.9.dev5/tests/test_eks/test_eks_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_eks/test_server.py` & `moto-4.1.9.dev5/tests/test_eks/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elasticache/test_elasticache.py` & `moto-4.1.9.dev5/tests/test_elasticache/test_elasticache.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elasticbeanstalk/test_eb.py` & `moto-4.1.9.dev5/tests/test_elasticbeanstalk/test_eb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elastictranscoder/test_elastictranscoder.py` & `moto-4.1.9.dev5/tests/test_elastictranscoder/test_elastictranscoder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elb/test_elb.py` & `moto-4.1.9.dev5/tests/test_elb/test_elb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elb/test_elb_availabilityzones.py` & `moto-4.1.9.dev5/tests/test_elb/test_elb_availabilityzones.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elb/test_elb_cloudformation.py` & `moto-4.1.9.dev5/tests/test_elb/test_elb_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elb/test_elb_policies.py` & `moto-4.1.9.dev5/tests/test_elb/test_elb_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elb/test_elb_subnets.py` & `moto-4.1.9.dev5/tests/test_elb/test_elb_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elbv2/test_elbv2.py` & `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_cloudformation.py` & `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_integration.py` & `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_listener_rule_tags.py` & `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_rule_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_listener_rules.py` & `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_listener_tags.py` & `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_set_subnets.py` & `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_set_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_elbv2/test_elbv2_target_groups.py` & `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_target_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_emr/test_emr_boto3.py` & `moto-4.1.9.dev5/tests/test_emr/test_emr_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_emr/test_emr_integration.py` & `moto-4.1.9.dev5/tests/test_emr/test_emr_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_emr/test_utils.py` & `moto-4.1.9.dev5/tests/test_emr/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_emrcontainers/test_emrcontainers.py` & `moto-4.1.9.dev5/tests/test_emrcontainers/test_emrcontainers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_emrserverless/test_emrserverless.py` & `moto-4.1.9.dev5/tests/test_emrserverless/test_emrserverless.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_es/test_es.py` & `moto-4.1.9.dev5/tests/test_es/test_es.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_events/test_event_pattern.py` & `moto-4.1.9.dev5/tests/test_events/test_event_pattern.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_events/test_events.py` & `moto-4.1.9.dev5/tests/test_events/test_events.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_events/test_events_cloudformation.py` & `moto-4.1.9.dev5/tests/test_events/test_events_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_events/test_events_integration.py` & `moto-4.1.9.dev5/tests/test_events/test_events_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_events/test_events_lambdatriggers_integration.py` & `moto-4.1.9.dev5/tests/test_events/test_events_lambdatriggers_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_firehose/test_firehose.py` & `moto-4.1.9.dev5/tests/test_firehose/test_firehose.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_firehose/test_firehose_destination_types.py` & `moto-4.1.9.dev5/tests/test_firehose/test_firehose_destination_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_firehose/test_firehose_encryption.py` & `moto-4.1.9.dev5/tests/test_firehose/test_firehose_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_firehose/test_firehose_put.py` & `moto-4.1.9.dev5/tests/test_firehose/test_firehose_put.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_firehose/test_firehose_tags.py` & `moto-4.1.9.dev5/tests/test_firehose/test_firehose_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_firehose/test_http_destinations.py` & `moto-4.1.9.dev5/tests/test_firehose/test_http_destinations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_forecast/test_forecast.py` & `moto-4.1.9.dev5/tests/test_forecast/test_forecast.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glacier/test_glacier_archives.py` & `moto-4.1.9.dev5/tests/test_glacier/test_glacier_archives.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glacier/test_glacier_jobs.py` & `moto-4.1.9.dev5/tests/test_glacier/test_glacier_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glacier/test_glacier_vaults.py` & `moto-4.1.9.dev5/tests/test_glacier/test_glacier_vaults.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glue/fixtures/datacatalog.py` & `moto-4.1.9.dev5/tests/test_glue/fixtures/datacatalog.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glue/fixtures/schema_registry.py` & `moto-4.1.9.dev5/tests/test_glue/fixtures/schema_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glue/helpers.py` & `moto-4.1.9.dev5/tests/test_glue/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glue/test_datacatalog.py` & `moto-4.1.9.dev5/tests/test_glue/test_datacatalog.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glue/test_glue.py` & `moto-4.1.9.dev5/tests/test_glue/test_glue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glue/test_glue_job_runs.py` & `moto-4.1.9.dev5/tests/test_glue/test_glue_job_runs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glue/test_partition_filter.py` & `moto-4.1.9.dev5/tests/test_glue/test_partition_filter.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_glue/test_schema_registry.py` & `moto-4.1.9.dev5/tests/test_glue/test_schema_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_core.py` & `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_core.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_deployment.py` & `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_deployment.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_device.py` & `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_device.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_functions.py` & `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_functions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_groups.py` & `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_resource.py` & `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_resource.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_greengrass/test_greengrass_subscriptions.py` & `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_subscriptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_guardduty/test_guardduty.py` & `moto-4.1.9.dev5/tests/test_guardduty/test_guardduty.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_guardduty/test_guardduty_filters.py` & `moto-4.1.9.dev5/tests/test_guardduty/test_guardduty_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_guardduty/test_guardduty_organization.py` & `moto-4.1.9.dev5/tests/test_guardduty/test_guardduty_organization.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam_access_integration.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam_access_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam_account_aliases.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam_account_aliases.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam_cloudformation.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam_groups.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam_oidc.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam_oidc.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam_password_last_used.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam_password_last_used.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam_policies.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_iam_server_certificates.py` & `moto-4.1.9.dev5/tests/test_iam/test_iam_server_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iam/test_server.py` & `moto-4.1.9.dev5/tests/test_iam/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_identitystore/test_identitystore.py` & `moto-4.1.9.dev5/tests/test_identitystore/test_identitystore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_ca_certificates.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_ca_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_certificates.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_deprecate_thing_type.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_deprecate_thing_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_domain_configuration.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_domain_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_job_executions.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_job_executions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_jobs.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_policies.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_search.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_search.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_thing_groups.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_thing_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_thing_types.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_thing_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_things.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_things.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_iot_topic_rules.py` & `moto-4.1.9.dev5/tests/test_iot/test_iot_topic_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iot/test_server.py` & `moto-4.1.9.dev5/tests/test_iot/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iotdata/test_iotdata.py` & `moto-4.1.9.dev5/tests/test_iotdata/test_iotdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_iotdata/test_server.py` & `moto-4.1.9.dev5/tests/test_iotdata/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesis/test_kinesis.py` & `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_boto3.py` & `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_cloudformation.py` & `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_encryption.py` & `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_monitoring.py` & `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_monitoring.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_stream_consumers.py` & `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_stream_consumers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesis/test_kinesis_stream_limits.py` & `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_stream_limits.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesisvideo/test_kinesisvideo.py` & `moto-4.1.9.dev5/tests/test_kinesisvideo/test_kinesisvideo.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py` & `moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kms/test_kms_boto3.py` & `moto-4.1.9.dev5/tests/test_kms/test_kms_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kms/test_kms_encrypt.py` & `moto-4.1.9.dev5/tests/test_kms/test_kms_encrypt.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kms/test_kms_grants.py` & `moto-4.1.9.dev5/tests/test_kms/test_kms_grants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kms/test_kms_policy_enforcement.py` & `moto-4.1.9.dev5/tests/test_kms/test_kms_policy_enforcement.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kms/test_model.py` & `moto-4.1.9.dev5/tests/test_kms/test_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_kms/test_utils.py` & `moto-4.1.9.dev5/tests/test_kms/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_lakeformation/test_lakeformation.py` & `moto-4.1.9.dev5/tests/test_lakeformation/test_lakeformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_logs/test_integration.py` & `moto-4.1.9.dev5/tests/test_logs/test_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_logs/test_logs.py` & `moto-4.1.9.dev5/tests/test_logs/test_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_logs/test_logs_filter.py` & `moto-4.1.9.dev5/tests/test_logs/test_logs_filter.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_logs/test_models.py` & `moto-4.1.9.dev5/tests/test_logs/test_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_managedblockchain/helpers.py` & `moto-4.1.9.dev5/tests/test_managedblockchain/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_invitations.py` & `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_invitations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_members.py` & `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_members.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_networks.py` & `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_networks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_nodes.py` & `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_nodes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_proposals.py` & `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_proposals.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py` & `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mediaconnect/test_mediaconnect.py` & `moto-4.1.9.dev5/tests/test_mediaconnect/test_mediaconnect.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_medialive/test_medialive.py` & `moto-4.1.9.dev5/tests/test_medialive/test_medialive.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_medialive/test_server.py` & `moto-4.1.9.dev5/tests/test_medialive/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mediapackage/test_mediapackage.py` & `moto-4.1.9.dev5/tests/test_mediapackage/test_mediapackage.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mediapackage/test_server.py` & `moto-4.1.9.dev5/tests/test_mediapackage/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mediastore/test_mediastore.py` & `moto-4.1.9.dev5/tests/test_mediastore/test_mediastore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mediastoredata/test_mediastoredata.py` & `moto-4.1.9.dev5/tests/test_mediastoredata/test_mediastoredata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_meteringmarketplace/test_meteringmarketplace.py` & `moto-4.1.9.dev5/tests/test_meteringmarketplace/test_meteringmarketplace.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_moto_api/mock_random/test_mock_random.py` & `moto-4.1.9.dev5/tests/test_moto_api/mock_random/test_mock_random.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_moto_api/recorder/test_recorder.py` & `moto-4.1.9.dev5/tests/test_moto_api/recorder/test_recorder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py` & `moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_moto_api/state_manager/servermode/test_state_manager.py` & `moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/test_state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_moto_api/state_manager/test_batch_integration.py` & `moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_batch_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_moto_api/state_manager/test_managed_state_model.py` & `moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_managed_state_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_moto_api/state_manager/test_state_manager.py` & `moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mq/test_mq.py` & `moto-4.1.9.dev5/tests/test_mq/test_mq.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mq/test_mq_configuration.py` & `moto-4.1.9.dev5/tests/test_mq/test_mq_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mq/test_mq_tags.py` & `moto-4.1.9.dev5/tests/test_mq/test_mq_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_mq/test_mq_users.py` & `moto-4.1.9.dev5/tests/test_mq/test_mq_users.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_neptune/test_cluster_options.py` & `moto-4.1.9.dev5/tests/test_neptune/test_cluster_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_neptune/test_cluster_tags.py` & `moto-4.1.9.dev5/tests/test_neptune/test_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_neptune/test_clusters.py` & `moto-4.1.9.dev5/tests/test_neptune/test_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_neptune/test_global_clusters.py` & `moto-4.1.9.dev5/tests/test_neptune/test_global_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_opensearch/test_domain_tags.py` & `moto-4.1.9.dev5/tests/test_opensearch/test_domain_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_opensearch/test_opensearch.py` & `moto-4.1.9.dev5/tests/test_opensearch/test_opensearch.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_opsworks/test_apps.py` & `moto-4.1.9.dev5/tests/test_opsworks/test_apps.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_opsworks/test_instances.py` & `moto-4.1.9.dev5/tests/test_opsworks/test_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_opsworks/test_layers.py` & `moto-4.1.9.dev5/tests/test_opsworks/test_layers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_opsworks/test_stack.py` & `moto-4.1.9.dev5/tests/test_opsworks/test_stack.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_organizations/organizations_test_utils.py` & `moto-4.1.9.dev5/tests/test_organizations/organizations_test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_organizations/test_organizations_boto3.py` & `moto-4.1.9.dev5/tests/test_organizations/test_organizations_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_personalize/test_personalize_schema.py` & `moto-4.1.9.dev5/tests/test_personalize/test_personalize_schema.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_pinpoint/test_pinpoint.py` & `moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_pinpoint/test_pinpoint_application_tags.py` & `moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint_application_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_pinpoint/test_pinpoint_event_stream.py` & `moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint_event_stream.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_polly/test_polly.py` & `moto-4.1.9.dev5/tests/test_polly/test_polly.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_quicksight/test_quicksight_datasets.py` & `moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_datasets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_quicksight/test_quicksight_groups.py` & `moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_quicksight/test_quicksight_users.py` & `moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_users.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ram/test_ram.py` & `moto-4.1.9.dev5/tests/test_ram/test_ram.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_db_cluster_param_group.py` & `moto-4.1.9.dev5/tests/test_rds/test_db_cluster_param_group.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_filters.py` & `moto-4.1.9.dev5/tests/test_rds/test_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_global_clusters.py` & `moto-4.1.9.dev5/tests/test_rds/test_global_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_rds.py` & `moto-4.1.9.dev5/tests/test_rds/test_rds.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_rds_cloudformation.py` & `moto-4.1.9.dev5/tests/test_rds/test_rds_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_rds_clusters.py` & `moto-4.1.9.dev5/tests/test_rds/test_rds_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_rds_clusters_with_instances.py` & `moto-4.1.9.dev5/tests/test_rds/test_rds_clusters_with_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_rds_event_subscriptions.py` & `moto-4.1.9.dev5/tests/test_rds/test_rds_event_subscriptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_rds_export_tasks.py` & `moto-4.1.9.dev5/tests/test_rds/test_rds_export_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_server.py` & `moto-4.1.9.dev5/tests/test_rds/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rds/test_utils.py` & `moto-4.1.9.dev5/tests/test_rds/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rdsdata/test_rdsdata.py` & `moto-4.1.9.dev5/tests/test_rdsdata/test_rdsdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_redshift/test_redshift.py` & `moto-4.1.9.dev5/tests/test_redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_redshift/test_redshift_cloudformation.py` & `moto-4.1.9.dev5/tests/test_redshift/test_redshift_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_redshift/test_server.py` & `moto-4.1.9.dev5/tests/test_redshift/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_redshiftdata/test_redshiftdata.py` & `moto-4.1.9.dev5/tests/test_redshiftdata/test_redshiftdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_redshiftdata/test_server.py` & `moto-4.1.9.dev5/tests/test_redshiftdata/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_rekognition/test_rekognition.py` & `moto-4.1.9.dev5/tests/test_rekognition/test_rekognition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_resourcegroups/test_resourcegroups.py` & `moto-4.1.9.dev5/tests/test_resourcegroups/test_resourcegroups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py` & `moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_resourcegroupstaggingapi/test_server.py` & `moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53/test_change_set_model.py` & `moto-4.1.9.dev5/tests/test_route53/test_change_set_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53/test_route53.py` & `moto-4.1.9.dev5/tests/test_route53/test_route53.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53/test_route53_cloudformation.py` & `moto-4.1.9.dev5/tests/test_route53/test_route53_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53/test_route53_delegationsets.py` & `moto-4.1.9.dev5/tests/test_route53/test_route53_delegationsets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53/test_route53_healthchecks.py` & `moto-4.1.9.dev5/tests/test_route53/test_route53_healthchecks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53/test_route53_query_logging_config.py` & `moto-4.1.9.dev5/tests/test_route53/test_route53_query_logging_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53/test_route53_vpcs.py` & `moto-4.1.9.dev5/tests/test_route53/test_route53_vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53/test_server.py` & `moto-4.1.9.dev5/tests/test_route53/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53resolver/test_route53resolver_endpoint.py` & `moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53resolver/test_route53resolver_rule.py` & `moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_rule.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53resolver/test_route53resolver_rule_associations.py` & `moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_rule_associations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_route53resolver/test_route53resolver_tags.py` & `moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_multiple_accounts_server.py` & `moto-4.1.9.dev5/tests/test_s3/test_multiple_accounts_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_acl.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_acl.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_auth.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_auth.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_bucket_policy.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_classdecorator.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_classdecorator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_cloudformation.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_config.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_copyobject.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_copyobject.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_custom_endpoint.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_custom_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_encryption.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_file_handles.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_file_handles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_lambda_integration.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_lambda_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_lifecycle.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_lifecycle.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_lock.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_lock.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_logging.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_logging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_metadata.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_metadata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_multipart.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_multipart.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_object_attributes.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_object_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_ownership.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_ownership.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_replication.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_replication.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_select.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_select.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_storageclass.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_storageclass.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_tagging.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_s3_utils.py` & `moto-4.1.9.dev5/tests/test_s3/test_s3_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3/test_server.py` & `moto-4.1.9.dev5/tests/test_s3/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3bucket_path/test_server.py` & `moto-4.1.9.dev5/tests/test_s3bucket_path/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3control/test_s3control.py` & `moto-4.1.9.dev5/tests/test_s3control/test_s3control.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3control/test_s3control_access_points.py` & `moto-4.1.9.dev5/tests/test_s3control/test_s3control_access_points.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3control/test_s3control_accesspoint_policy.py` & `moto-4.1.9.dev5/tests/test_s3control/test_s3control_accesspoint_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3control/test_s3control_config_integration.py` & `moto-4.1.9.dev5/tests/test_s3control/test_s3control_config_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_s3control/test_s3control_s3.py` & `moto-4.1.9.dev5/tests/test_s3control/test_s3control_s3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/cloudformation_test_configs.py` & `moto-4.1.9.dev5/tests/test_sagemaker/cloudformation_test_configs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_cloudformation.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_endpoint.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_experiment.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_experiment.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_models.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_notebooks.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_notebooks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_pipeline.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_pipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_processing.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_processing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_search.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_search.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_training.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_training.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_trial.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_trial.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sagemaker/test_sagemaker_trial_component.py` & `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_trial_component.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_scheduler/test_schedule_groups.py` & `moto-4.1.9.dev5/tests/test_scheduler/test_schedule_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_scheduler/test_scheduler.py` & `moto-4.1.9.dev5/tests/test_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_scheduler/test_scheduler_tags.py` & `moto-4.1.9.dev5/tests/test_scheduler/test_scheduler_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sdb/test_sdb_attributes.py` & `moto-4.1.9.dev5/tests/test_sdb/test_sdb_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sdb/test_sdb_domains.py` & `moto-4.1.9.dev5/tests/test_sdb/test_sdb_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_secretsmanager/test_list_secrets.py` & `moto-4.1.9.dev5/tests/test_secretsmanager/test_list_secrets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_secretsmanager/test_policy.py` & `moto-4.1.9.dev5/tests/test_secretsmanager/test_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_secretsmanager/test_secretsmanager.py` & `moto-4.1.9.dev5/tests/test_secretsmanager/test_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_secretsmanager/test_server.py` & `moto-4.1.9.dev5/tests/test_secretsmanager/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py` & `moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_servicediscovery/test_servicediscovery_operations.py` & `moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_operations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_servicediscovery/test_servicediscovery_service.py` & `moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_servicediscovery/test_servicediscovery_tags.py` & `moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_servicequotas/test_servicequotas.py` & `moto-4.1.9.dev5/tests/test_servicequotas/test_servicequotas.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ses/test_server.py` & `moto-4.1.9.dev5/tests/test_ses/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ses/test_ses_boto3.py` & `moto-4.1.9.dev5/tests/test_ses/test_ses_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ses/test_ses_sns_boto3.py` & `moto-4.1.9.dev5/tests/test_ses/test_ses_sns_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ses/test_templating.py` & `moto-4.1.9.dev5/tests/test_ses/test_templating.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_signer/test_signing_platforms.py` & `moto-4.1.9.dev5/tests/test_signer/test_signing_platforms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_signer/test_signing_profiles.py` & `moto-4.1.9.dev5/tests/test_signer/test_signing_profiles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sns/test_application_boto3.py` & `moto-4.1.9.dev5/tests/test_sns/test_application_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sns/test_publish_batch.py` & `moto-4.1.9.dev5/tests/test_sns/test_publish_batch.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sns/test_publishing_boto3.py` & `moto-4.1.9.dev5/tests/test_sns/test_publishing_boto3.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         Message="test message",
         MessageAttributes={"retries": {"DataType": "Number", "StringValue": "0"}},
     )
 
     message = json.loads(queue.receive_messages()[0].body)
     message["Message"].should.equal("test message")
     message["MessageAttributes"].should.equal(
-        {"retries": {"Type": "Number", "Value": 0}}
+        {"retries": {"Type": "Number", "Value": "0"}}
     )
 
     message = queue_raw.receive_messages()[0]
     message.body.should.equal("test message")
 
 
 @mock_sqs
@@ -727,15 +727,15 @@
         MessageAttributes={"price": {"DataType": "Number", "StringValue": "100"}},
     )
 
     messages = queue.receive_messages(MaxNumberOfMessages=5)
     message_bodies = [json.loads(m.body)["Message"] for m in messages]
     message_bodies.should.equal(["match"])
     message_attributes = [json.loads(m.body)["MessageAttributes"] for m in messages]
-    message_attributes.should.equal([{"price": {"Type": "Number", "Value": 100}}])
+    message_attributes.should.equal([{"price": {"Type": "Number", "Value": "100"}}])
 
 
 @mock_sqs
 @mock_sns
 def test_filtering_exact_number_float():
     topic, queue = _setup_filter_policy_test({"price": [100.1]})
 
@@ -744,35 +744,35 @@
         MessageAttributes={"price": {"DataType": "Number", "StringValue": "100.1"}},
     )
 
     messages = queue.receive_messages(MaxNumberOfMessages=5)
     message_bodies = [json.loads(m.body)["Message"] for m in messages]
     message_bodies.should.equal(["match"])
     message_attributes = [json.loads(m.body)["MessageAttributes"] for m in messages]
-    message_attributes.should.equal([{"price": {"Type": "Number", "Value": 100.1}}])
+    message_attributes.should.equal([{"price": {"Type": "Number", "Value": "100.1"}}])
 
 
 @mock_sqs
 @mock_sns
 def test_filtering_exact_number_float_accuracy():
     topic, queue = _setup_filter_policy_test({"price": [100.123456789]})
 
     topic.publish(
         Message="match",
         MessageAttributes={
-            "price": {"DataType": "Number", "StringValue": "100.1234561"}
+            "price": {"DataType": "Number", "StringValue": "100.1234567"}
         },
     )
 
     messages = queue.receive_messages(MaxNumberOfMessages=5)
     message_bodies = [json.loads(m.body)["Message"] for m in messages]
     message_bodies.should.equal(["match"])
     message_attributes = [json.loads(m.body)["MessageAttributes"] for m in messages]
     message_attributes.should.equal(
-        [{"price": {"Type": "Number", "Value": 100.1234561}}]
+        [{"price": {"Type": "Number", "Value": "100.1234567"}}]
     )
 
 
 @mock_sqs
 @mock_sns
 def test_filtering_exact_number_no_match():
     topic, queue = _setup_filter_policy_test({"price": [100]})
@@ -888,25 +888,25 @@
     topic, queue = _setup_filter_policy_test({"price": [100.123456789, 500]})
 
     topic.publish(
         Message="match",
         MessageAttributes={
             "price": {
                 "DataType": "String.Array",
-                "StringValue": json.dumps([100.1234561, 50]),
+                "StringValue": json.dumps([100.1234567, 50]),
             }
         },
     )
 
     messages = queue.receive_messages(MaxNumberOfMessages=5)
     message_bodies = [json.loads(m.body)["Message"] for m in messages]
     message_bodies.should.equal(["match"])
     message_attributes = [json.loads(m.body)["MessageAttributes"] for m in messages]
     message_attributes.should.equal(
-        [{"price": {"Type": "String.Array", "Value": json.dumps([100.1234561, 50])}}]
+        [{"price": {"Type": "String.Array", "Value": json.dumps([100.1234567, 50])}}]
     )
 
 
 @mock_sqs
 @mock_sns
 # this is the correct behavior from SNS
 def test_filtering_string_array_with_number_no_array_match():
@@ -1079,15 +1079,15 @@
             {
                 "store": {"Type": "String", "Value": "example_corp"},
                 "event": {"Type": "String", "Value": "order_cancelled"},
                 "customer_interests": {
                     "Type": "String.Array",
                     "Value": json.dumps(["basketball", "rugby"]),
                 },
-                "price": {"Type": "Number", "Value": 100},
+                "price": {"Type": "Number", "Value": "100"},
             }
         ]
     )
 
 
 @mock_sqs
 @mock_sns
@@ -1224,15 +1224,15 @@
     message_bodies.should.equal([])
 
 
 @mock_sqs
 @mock_sns
 def test_filtering_anything_but_numeric():
     topic, queue = _setup_filter_policy_test(
-        {"customer_interests": [{"anything-but": ["100"]}]}
+        {"customer_interests": [{"anything-but": [100]}]}
     )
 
     for nr, idx in [("50", "1"), ("100", "2"), ("150", "3")]:
         topic.publish(
             Message=f"match{idx}",
             MessageAttributes={
                 "customer_interests": {"DataType": "Number", "StringValue": nr},
@@ -1244,15 +1244,15 @@
     set(message_bodies).should.equal({"match1", "match3"})
 
 
 @mock_sqs
 @mock_sns
 def test_filtering_numeric_match():
     topic, queue = _setup_filter_policy_test(
-        {"customer_interests": [{"numeric": ["=", "100"]}]}
+        {"customer_interests": [{"numeric": ["=", 100]}]}
     )
 
     for nr, idx in [("50", "1"), ("100", "2"), ("150", "3")]:
         topic.publish(
             Message=f"match{idx}",
             MessageAttributes={
                 "customer_interests": {"DataType": "Number", "StringValue": nr},
@@ -1264,15 +1264,15 @@
     set(message_bodies).should.equal({"match2"})
 
 
 @mock_sqs
 @mock_sns
 def test_filtering_numeric_range():
     topic, queue = _setup_filter_policy_test(
-        {"customer_interests": [{"numeric": [">", "49", "<=", "100"]}]}
+        {"customer_interests": [{"numeric": [">", 49, "<=", 100]}]}
     )
 
     for nr, idx in [("50", "1"), ("100", "2"), ("150", "3")]:
         topic.publish(
             Message=f"match{idx}",
             MessageAttributes={
                 "customer_interests": {"DataType": "Number", "StringValue": nr},
```

### Comparing `moto-4.1.9.dev3/tests/test_sns/test_server.py` & `moto-4.1.9.dev5/tests/test_sns/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sns/test_sns_cloudformation.py` & `moto-4.1.9.dev5/tests/test_sns/test_sns_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sns/test_subscriptions_boto3.py` & `moto-4.1.9.dev5/tests/test_sns/test_subscriptions_boto3.py`

 * *Files 19% similar despite different names*

```diff
@@ -412,77 +412,238 @@
 @mock_sns
 def test_subscribe_invalid_filter_policy():
     conn = boto3.client("sns", region_name="us-east-1")
     conn.create_topic(Name="some-topic")
     response = conn.list_topics()
     topic_arn = response["Topics"][0]["TopicArn"]
 
-    try:
+    with pytest.raises(ClientError) as err_info:
         conn.subscribe(
             TopicArn=topic_arn,
             Protocol="http",
             Endpoint="http://example.com/",
             Attributes={
                 "FilterPolicy": json.dumps({"store": [str(i) for i in range(151)]})
             },
         )
-    except ClientError as err:
-        err.response["Error"]["Code"].should.equal("InvalidParameter")
-        err.response["Error"]["Message"].should.equal(
-            "Invalid parameter: FilterPolicy: Filter policy is too complex"
-        )
 
-    try:
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: FilterPolicy: Filter policy is too complex"
+    )
+
+    with pytest.raises(ClientError) as err_info:
         conn.subscribe(
             TopicArn=topic_arn,
             Protocol="http",
             Endpoint="http://example.com/",
             Attributes={"FilterPolicy": json.dumps({"store": [["example_corp"]]})},
         )
-    except ClientError as err:
-        err.response["Error"]["Code"].should.equal("InvalidParameter")
-        err.response["Error"]["Message"].should.equal(
-            "Invalid parameter: FilterPolicy: Match value must be String, number, true, false, or null"
-        )
 
-    try:
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: FilterPolicy: Match value must be String, number, true, false, or null"
+    )
+
+    with pytest.raises(ClientError) as err_info:
         conn.subscribe(
             TopicArn=topic_arn,
             Protocol="http",
             Endpoint="http://example.com/",
             Attributes={"FilterPolicy": json.dumps({"store": [{"exists": None}]})},
         )
-    except ClientError as err:
-        err.response["Error"]["Code"].should.equal("InvalidParameter")
-        err.response["Error"]["Message"].should.equal(
-            "Invalid parameter: FilterPolicy: exists match pattern must be either true or false."
-        )
 
-    try:
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: FilterPolicy: exists match pattern must be either true or false."
+    )
+
+    with pytest.raises(ClientError) as err_info:
         conn.subscribe(
             TopicArn=topic_arn,
             Protocol="http",
             Endpoint="http://example.com/",
             Attributes={"FilterPolicy": json.dumps({"store": [{"error": True}]})},
         )
-    except ClientError as err:
-        err.response["Error"]["Code"].should.equal("InvalidParameter")
-        err.response["Error"]["Message"].should.equal(
-            "Invalid parameter: FilterPolicy: Unrecognized match type error"
-        )
 
-    try:
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: FilterPolicy: Unrecognized match type error"
+    )
+
+    with pytest.raises(ClientError) as err_info:
         conn.subscribe(
             TopicArn=topic_arn,
             Protocol="http",
             Endpoint="http://example.com/",
             Attributes={"FilterPolicy": json.dumps({"store": [1000000001]})},
         )
-    except ClientError as err:
-        err.response["Error"]["Code"].should.equal("InternalFailure")
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InternalFailure")
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={
+                "FilterPolicy": json.dumps({"price": [{"numeric": ["<", "100"]}]})
+            },
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Value of < must be numeric\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={
+                "FilterPolicy": json.dumps(
+                    {"price": [{"numeric": [">", 50, "<=", "100"]}]}
+                )
+            },
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Value of <= must be numeric\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={"FilterPolicy": json.dumps({"price": [{"numeric": []}]})},
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Invalid member in numeric match: ]\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={
+                "FilterPolicy": json.dumps({"price": [{"numeric": [50, "<=", "100"]}]})
+            },
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Invalid member in numeric match: 50\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={"FilterPolicy": json.dumps({"price": [{"numeric": ["<"]}]})},
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Value of < must be numeric\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={"FilterPolicy": json.dumps({"price": [{"numeric": ["0"]}]})},
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Unrecognized numeric range operator: 0\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={
+                "FilterPolicy": json.dumps({"price": [{"numeric": ["<", 20, ">", 1]}]})
+            },
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Too many elements in numeric expression\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={
+                "FilterPolicy": json.dumps({"price": [{"numeric": [">", 20, ">", 1]}]})
+            },
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Bad numeric range operator: >\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={
+                "FilterPolicy": json.dumps({"price": [{"numeric": [">", 20, "<", 1]}]})
+            },
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Bottom must be less than top\n at ..."
+    )
+
+    with pytest.raises(ClientError) as err_info:
+        conn.subscribe(
+            TopicArn=topic_arn,
+            Protocol="http",
+            Endpoint="http://example.com/",
+            Attributes={
+                "FilterPolicy": json.dumps({"price": [{"numeric": [">", 20, "<"]}]})
+            },
+        )
+
+    err = err_info.value
+    err.response["Error"]["Code"].should.equal("InvalidParameter")
+    err.response["Error"]["Message"].should.equal(
+        "Invalid parameter: Attributes Reason: FilterPolicy: Value of < must be numeric\n at ..."
+    )
 
 
 @mock_sns
 def test_check_not_opted_out():
     conn = boto3.client("sns", region_name="us-east-1")
     response = conn.check_if_phone_number_is_opted_out(phoneNumber="+447428545375")
```

### Comparing `moto-4.1.9.dev3/tests/test_sns/test_topics_boto3.py` & `moto-4.1.9.dev5/tests/test_sns/test_topics_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_special_cases/test_custom_amis.py` & `moto-4.1.9.dev5/tests/test_special_cases/test_custom_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sqs/test_server.py` & `moto-4.1.9.dev5/tests/test_sqs/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sqs/test_sqs.py` & `moto-4.1.9.dev5/tests/test_sqs/test_sqs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sqs/test_sqs_cloudformation.py` & `moto-4.1.9.dev5/tests/test_sqs/test_sqs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sqs/test_sqs_integration.py` & `moto-4.1.9.dev5/tests/test_sqs/test_sqs_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sqs/test_sqs_multiaccount.py` & `moto-4.1.9.dev5/tests/test_sqs/test_sqs_multiaccount.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_boto3.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_boto3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1735,34 +1735,43 @@
     params = {"commands": ["#!/bin/bash\necho 'hello world'"]}
 
     client = boto3.client("ssm", region_name="us-east-1")
     # note the timeout is determined server side, so this is a simpler check.
     before = datetime.datetime.now()
 
     response = client.send_command(
+        Comment="some comment",
         InstanceIds=["i-123456"],
         DocumentName=ssm_document,
+        TimeoutSeconds=42,
+        MaxConcurrency="360",
+        MaxErrors="2",
         Parameters=params,
         OutputS3Region="us-east-2",
         OutputS3BucketName="the-bucket",
         OutputS3KeyPrefix="pref",
     )
     cmd = response["Command"]
 
     cmd["CommandId"].should_not.be(None)
+    assert cmd["Comment"] == "some comment"
     cmd["DocumentName"].should.equal(ssm_document)
     cmd["Parameters"].should.equal(params)
 
     cmd["OutputS3Region"].should.equal("us-east-2")
     cmd["OutputS3BucketName"].should.equal("the-bucket")
     cmd["OutputS3KeyPrefix"].should.equal("pref")
 
     cmd["ExpiresAfter"].should.be.greater_than(before)
     cmd["DeliveryTimedOutCount"].should.equal(0)
 
+    assert cmd["TimeoutSeconds"] == 42
+    assert cmd["MaxConcurrency"] == "360"
+    assert cmd["MaxErrors"] == "2"
+
     # test sending a command without any optional parameters
     response = client.send_command(DocumentName=ssm_document)
 
     cmd = response["Command"]
 
     cmd["CommandId"].should_not.be(None)
     cmd["DocumentName"].should.equal(ssm_document)
```

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_cloudformation.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_default_amis.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_default_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_defaults.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_defaults.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_doc_permissions.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_doc_permissions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_docs.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_docs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_ecs_images.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_ecs_images.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_maintenance_windows.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_maintenance_windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_parameterstore.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_parameterstore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_secretsmanager.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_ssm_utils.py` & `moto-4.1.9.dev5/tests/test_ssm/test_ssm_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssm/test_templates/good.yaml` & `moto-4.1.9.dev5/tests/test_ssm/test_templates/good.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssoadmin/test_server.py` & `moto-4.1.9.dev5/tests/test_ssoadmin/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_ssoadmin/test_ssoadmin.py` & `moto-4.1.9.dev5/tests/test_ssoadmin/test_ssoadmin.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_stepfunctions/test_stepfunctions.py` & `moto-4.1.9.dev5/tests/test_stepfunctions/test_stepfunctions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_stepfunctions/test_stepfunctions_cloudformation.py` & `moto-4.1.9.dev5/tests/test_stepfunctions/test_stepfunctions_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sts/test_server.py` & `moto-4.1.9.dev5/tests/test_sts/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sts/test_sts.py` & `moto-4.1.9.dev5/tests/test_sts/test_sts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_sts/test_sts_integration.py` & `moto-4.1.9.dev5/tests/test_sts/test_sts_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_support/test_server.py` & `moto-4.1.9.dev5/tests/test_support/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_support/test_support.py` & `moto-4.1.9.dev5/tests/test_support/test_support.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/models/test_activity_task.py` & `moto-4.1.9.dev5/tests/test_swf/models/test_activity_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/models/test_decision_task.py` & `moto-4.1.9.dev5/tests/test_swf/models/test_decision_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/models/test_domain.py` & `moto-4.1.9.dev5/tests/test_swf/models/test_domain.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/models/test_generic_type.py` & `moto-4.1.9.dev5/tests/test_swf/models/test_generic_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/models/test_history_event.py` & `moto-4.1.9.dev5/tests/test_swf/models/test_history_event.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/models/test_timeout.py` & `moto-4.1.9.dev5/tests/test_swf/models/test_timeout.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/models/test_timer.py` & `moto-4.1.9.dev5/tests/test_swf/models/test_timer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/models/test_workflow_execution.py` & `moto-4.1.9.dev5/tests/test_swf/models/test_workflow_execution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/responses/test_activity_tasks.py` & `moto-4.1.9.dev5/tests/test_swf/responses/test_activity_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/responses/test_activity_types.py` & `moto-4.1.9.dev5/tests/test_swf/responses/test_activity_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/responses/test_decision_tasks.py` & `moto-4.1.9.dev5/tests/test_swf/responses/test_decision_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/responses/test_domains.py` & `moto-4.1.9.dev5/tests/test_swf/responses/test_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/responses/test_timeouts.py` & `moto-4.1.9.dev5/tests/test_swf/responses/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/responses/test_workflow_executions.py` & `moto-4.1.9.dev5/tests/test_swf/responses/test_workflow_executions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/responses/test_workflow_types.py` & `moto-4.1.9.dev5/tests/test_swf/responses/test_workflow_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/test_exceptions.py` & `moto-4.1.9.dev5/tests/test_swf/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_swf/utils.py` & `moto-4.1.9.dev5/tests/test_swf/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_textract/test_server.py` & `moto-4.1.9.dev5/tests/test_textract/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_textract/test_textract.py` & `moto-4.1.9.dev5/tests/test_textract/test_textract.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_timestreamwrite/test_server.py` & `moto-4.1.9.dev5/tests/test_timestreamwrite/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_timestreamwrite/test_timestreamwrite_database.py` & `moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_database.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_timestreamwrite/test_timestreamwrite_table.py` & `moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_timestreamwrite/test_timestreamwrite_tagging.py` & `moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_transcribe/test_transcribe_boto3.py` & `moto-4.1.9.dev5/tests/test_transcribe/test_transcribe_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_utilities/test_docker_utilities.py` & `moto-4.1.9.dev5/tests/test_utilities/test_docker_utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_utilities/test_paginator.py` & `moto-4.1.9.dev5/tests/test_utilities/test_paginator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_utilities/test_tagging_service.py` & `moto-4.1.9.dev5/tests/test_utilities/test_tagging_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_utilities/test_threaded_server.py` & `moto-4.1.9.dev5/tests/test_utilities/test_threaded_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_wafv2/test_server.py` & `moto-4.1.9.dev5/tests/test_wafv2/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_wafv2/test_utils.py` & `moto-4.1.9.dev5/tests/test_wafv2/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_wafv2/test_wafv2.py` & `moto-4.1.9.dev5/tests/test_wafv2/test_wafv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_wafv2/test_wafv2_integration.py` & `moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_wafv2/test_wafv2_tags.py` & `moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_xray/test_xray_boto3.py` & `moto-4.1.9.dev5/tests/test_xray/test_xray_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev3/tests/test_xray/test_xray_client.py` & `moto-4.1.9.dev5/tests/test_xray/test_xray_client.py`

 * *Files identical despite different names*


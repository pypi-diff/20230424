# Comparing `tmp/composer-0.13.4.tar.gz` & `tmp/composer-0.13.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composer-0.13.4.tar", last modified: Wed Apr  5 03:00:56 2023, max compression
+gzip compressed data, was "composer-0.13.5.tar", last modified: Mon Apr 24 20:59:01 2023, max compression
```

## Comparing `composer-0.13.4.tar` & `composer-0.13.5.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.467648 composer-0.13.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-04-05 03:00:38.000000 composer-0.13.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 03:00:38.000000 composer-0.13.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-04-05 03:00:56.467648 composer-0.13.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-04-05 03:00:38.000000 composer-0.13.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.427648 composer-0.13.4/composer/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-05 03:00:38.000000 composer-0.13.4/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-05 03:00:38.000000 composer-0.13.4/composer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-05 03:00:38.000000 composer-0.13.4/composer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.427648 composer-0.13.4/composer/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.427648 composer-0.13.4/composer/algorithms/alibi/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/alibi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/alibi/alibi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/alibi/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/augmix/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/augmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/augmix/augmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/augmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/blurpool/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/blurpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/blurpool/blurpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/blurpool/blurpool_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/blurpool/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/channels_last/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/channels_last/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/channels_last/channels_last.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/channels_last/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/colout/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/colout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/colout/colout.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/colout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/cutmix/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/cutmix/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/cutmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/cutout/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/cutout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/cutout/cutout.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/cutout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/ema/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/ema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19897 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/ema/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/ema/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/factorize/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/factorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/factorize/factorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/factorize/factorize_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/factorize/factorize_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/factorize/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.431648 composer-0.13.4/composer/algorithms/fused_layernorm/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/fused_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/fused_layernorm/fused_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/fused_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/gated_linear_units/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gated_linear_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gated_linear_units/gated_linear_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gated_linear_units/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/ghost_batchnorm/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/ghost_batchnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/ghost_batchnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/gradient_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gradient_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gradient_clipping/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gradient_clipping/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/gyro_dropout/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gyro_dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gyro_dropout/gyro_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/gyro_dropout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/label_smoothing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/label_smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/label_smoothing/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/label_smoothing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/layer_freezing/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/layer_freezing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/layer_freezing/layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/layer_freezing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/low_precision_groupnorm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/low_precision_groupnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/low_precision_groupnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/low_precision_layernorm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/low_precision_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/low_precision_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.435648 composer-0.13.4/composer/algorithms/mixup/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/mixup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/mixup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/mixup/mixup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/no_op_model/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/no_op_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/no_op_model/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/no_op_model/no_op_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/progressive_resizing/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/progressive_resizing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/progressive_resizing/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/progressive_resizing/progressive_resizing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/randaugment/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/randaugment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/randaugment/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/randaugment/randaugment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/sam/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/sam/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/selective_backprop/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/selective_backprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/selective_backprop/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/selective_backprop/selective_backprop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/seq_length_warmup/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/seq_length_warmup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/seq_length_warmup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/seq_length_warmup/seq_length_warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/squeeze_excite/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/squeeze_excite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/squeeze_excite/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/squeeze_excite/squeeze_excite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/stochastic_depth/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/stochastic_depth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/stochastic_depth/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/stochastic_depth/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/stochastic_depth/stochastic_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.439648 composer-0.13.4/composer/algorithms/swa/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/swa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/swa/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/swa/swa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.443648 composer-0.13.4/composer/algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/utils/augmentation_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/utils/augmentation_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.443648 composer-0.13.4/composer/algorithms/weight_standardization/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/weight_standardization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/weight_standardization/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-05 03:00:38.000000 composer-0.13.4/composer/algorithms/weight_standardization/weight_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.443648 composer-0.13.4/composer/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/early_stopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/export_for_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17899 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/mlperf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/optimizer_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/runtime_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16037 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/speed_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-05 03:00:38.000000 composer-0.13.4/composer/callbacks/threshold_stopper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.443648 composer-0.13.4/composer/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-05 03:00:38.000000 composer-0.13.4/composer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-05 03:00:38.000000 composer-0.13.4/composer/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21453 2023-04-05 03:00:38.000000 composer-0.13.4/composer/cli/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.447648 composer-0.13.4/composer/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/data_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)    60941 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-05 03:00:38.000000 composer-0.13.4/composer/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.447648 composer-0.13.4/composer/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/c4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/ffcv_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/in_context_learning_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/lm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-05 03:00:38.000000 composer-0.13.4/composer/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.447648 composer-0.13.4/composer/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-05 03:00:38.000000 composer-0.13.4/composer/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-05 03:00:38.000000 composer-0.13.4/composer/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-05 03:00:38.000000 composer-0.13.4/composer/devices/device_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-05 03:00:38.000000 composer-0.13.4/composer/devices/device_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-05 03:00:38.000000 composer-0.13.4/composer/devices/device_mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-05 03:00:38.000000 composer-0.13.4/composer/devices/device_tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.447648 composer-0.13.4/composer/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-05 03:00:38.000000 composer-0.13.4/composer/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.451648 composer-0.13.4/composer/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/cometml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/file_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/in_memory_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/logger_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/progress_bar_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/remote_uploader_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.451648 composer-0.13.4/composer/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-05 03:00:38.000000 composer-0.13.4/composer/loss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.451648 composer-0.13.4/composer/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-05 03:00:38.000000 composer-0.13.4/composer/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-04-05 03:00:38.000000 composer-0.13.4/composer/metrics/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-05 03:00:38.000000 composer-0.13.4/composer/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-04-05 03:00:38.000000 composer-0.13.4/composer/metrics/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.451648 composer-0.13.4/composer/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.451648 composer-0.13.4/composer/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/bert/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.451648 composer-0.13.4/composer/models/classify_mnist/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/classify_mnist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/classify_mnist/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.451648 composer-0.13.4/composer/models/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/deeplabv3/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.455648 composer-0.13.4/composer/models/efficientnetb0/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/efficientnetb0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/efficientnetb0/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/efficientnetb0/efficientnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/efficientnetb0/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.455648 composer-0.13.4/composer/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/gpt2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    30490 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/mmdetection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.455648 composer-0.13.4/composer/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/resnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/resnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.455648 composer-0.13.4/composer/models/resnet_cifar/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/resnet_cifar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/resnet_cifar/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/resnet_cifar/resnets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.455648 composer-0.13.4/composer/models/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/tasks/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.455648 composer-0.13.4/composer/models/timm/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.455648 composer-0.13.4/composer/models/unet/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/unet/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/unet/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.455648 composer-0.13.4/composer/models/vit_small_patch16/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/vit_small_patch16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-05 03:00:38.000000 composer-0.13.4/composer/models/vit_small_patch16/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.459648 composer-0.13.4/composer/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-05 03:00:38.000000 composer-0.13.4/composer/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-04-05 03:00:38.000000 composer-0.13.4/composer/optim/decoupled_weight_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-04-05 03:00:38.000000 composer-0.13.4/composer/optim/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.459648 composer-0.13.4/composer/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/json_trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/json_trace_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/profiler_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/profiler_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/system_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/torch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-05 03:00:38.000000 composer-0.13.4/composer/profiler/trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:38.000000 composer-0.13.4/composer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.459648 composer-0.13.4/composer/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-05 03:00:38.000000 composer-0.13.4/composer/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-05 03:00:38.000000 composer-0.13.4/composer/trainer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-05 03:00:38.000000 composer-0.13.4/composer/trainer/_scale_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-04-05 03:00:38.000000 composer-0.13.4/composer/trainer/_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-05 03:00:38.000000 composer-0.13.4/composer/trainer/dist_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-05 03:00:38.000000 composer-0.13.4/composer/trainer/meta_safe_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-05 03:00:38.000000 composer-0.13.4/composer/trainer/mosaic_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)   152656 2023-04-05 03:00:38.000000 composer-0.13.4/composer/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.463648 composer-0.13.4/composer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/auto_log_hparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/batch_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28956 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/fx_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/iter_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/module_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.463648 composer-0.13.4/composer/utils/object_store/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/object_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/object_store/libcloud_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/object_store/object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/object_store/oci_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/object_store/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/object_store/sftp_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/retrying.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-05 03:00:38.000000 composer-0.13.4/composer/utils/string_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.427648 composer-0.13.4/composer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-04-05 03:00:56.000000 composer-0.13.4/composer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-04-05 03:00:56.000000 composer-0.13.4/composer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-05 03:00:56.000000 composer-0.13.4/composer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-05 03:00:56.000000 composer-0.13.4/composer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-05 03:00:56.000000 composer-0.13.4/composer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 03:00:56.000000 composer-0.13.4/composer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34926 2023-04-05 03:00:38.000000 composer-0.13.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 03:00:56.467648 composer-0.13.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-05 03:00:38.000000 composer-0.13.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:00:56.467648 composer-0.13.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_full_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_simple_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_split_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-05 03:00:38.000000 composer-0.13.4/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.473396 composer-0.13.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-04-24 20:58:47.000000 composer-0.13.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 20:58:47.000000 composer-0.13.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-04-24 20:59:01.473396 composer-0.13.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-04-24 20:58:47.000000 composer-0.13.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-24 20:58:47.000000 composer-0.13.5/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 20:58:47.000000 composer-0.13.5/composer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 20:58:47.000000 composer-0.13.5/composer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer/algorithms/alibi/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/alibi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/alibi/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/augmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/augmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/augmix/augmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/augmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/blurpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/blurpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/blurpool/blurpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/blurpool/blurpool_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/blurpool/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/channels_last/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/channels_last/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/channels_last/channels_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/channels_last/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/colout/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/colout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/colout/colout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/colout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutmix/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.441396 composer-0.13.5/composer/algorithms/cutout/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutout/cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/cutout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/ema/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21563 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ema/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ema/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/factorize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/factorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/factorize_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/factorize_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/factorize/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/fused_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/fused_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/fused_layernorm/fused_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/fused_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/gated_linear_units/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gated_linear_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gated_linear_units/gated_linear_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gated_linear_units/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/ghost_batchnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ghost_batchnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/ghost_batchnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/gradient_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gradient_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gradient_clipping/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gradient_clipping/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.445396 composer-0.13.5/composer/algorithms/gyro_dropout/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gyro_dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gyro_dropout/gyro_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/gyro_dropout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/label_smoothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/label_smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/label_smoothing/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/label_smoothing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/layer_freezing/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/layer_freezing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/layer_freezing/layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/layer_freezing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/low_precision_groupnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_groupnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_groupnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/low_precision_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/low_precision_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/mixup/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/mixup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/mixup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/mixup/mixup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/no_op_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/no_op_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/no_op_model/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/no_op_model/no_op_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/progressive_resizing/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/progressive_resizing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/progressive_resizing/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/progressive_resizing/progressive_resizing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/randaugment/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/randaugment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/randaugment/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/randaugment/randaugment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/sam/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/sam/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/selective_backprop/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/selective_backprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/selective_backprop/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/selective_backprop/selective_backprop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.449396 composer-0.13.5/composer/algorithms/seq_length_warmup/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/seq_length_warmup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/seq_length_warmup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/seq_length_warmup/seq_length_warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/squeeze_excite/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/squeeze_excite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/squeeze_excite/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/squeeze_excite/squeeze_excite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/stochastic_depth/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/stochastic_depth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/stochastic_depth/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/stochastic_depth/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/stochastic_depth/stochastic_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/swa/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/swa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/swa/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/swa/swa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/utils/augmentation_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/utils/augmentation_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/algorithms/weight_standardization/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/weight_standardization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/weight_standardization/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-24 20:58:47.000000 composer-0.13.5/composer/algorithms/weight_standardization/weight_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.453396 composer-0.13.5/composer/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/early_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/export_for_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17899 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/mlperf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/optimizer_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/runtime_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16037 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/speed_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-24 20:58:47.000000 composer-0.13.5/composer/callbacks/threshold_stopper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.457396 composer-0.13.5/composer/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 20:58:47.000000 composer-0.13.5/composer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-24 20:58:47.000000 composer-0.13.5/composer/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21453 2023-04-24 20:58:47.000000 composer-0.13.5/composer/cli/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.457396 composer-0.13.5/composer/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60941 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-24 20:58:47.000000 composer-0.13.5/composer/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.457396 composer-0.13.5/composer/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/c4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/ffcv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/in_context_learning_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/lm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-24 20:58:47.000000 composer-0.13.5/composer/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device_mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 20:58:47.000000 composer-0.13.5/composer/devices/device_tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-24 20:58:47.000000 composer-0.13.5/composer/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/cometml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/file_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/in_memory_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/logger_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/progress_bar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/remote_uploader_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-24 20:58:47.000000 composer-0.13.5/composer/loss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-24 20:58:47.000000 composer-0.13.5/composer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-04-24 20:58:47.000000 composer-0.13.5/composer/metrics/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-24 20:58:47.000000 composer-0.13.5/composer/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-04-24 20:58:47.000000 composer-0.13.5/composer/metrics/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/bert/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.461396 composer-0.13.5/composer/models/classify_mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/classify_mnist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/classify_mnist/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/deeplabv3/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/efficientnetb0/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/efficientnetb0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/efficientnetb0/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/efficientnetb0/efficientnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/efficientnetb0/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-24 20:58:47.000000 composer-0.13.5/composer/models/gpt2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30490 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/mmdetection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/resnet_cifar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet_cifar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet_cifar/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/resnet_cifar/resnets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/tasks/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/unet/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/unet/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/models/vit_small_patch16/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/vit_small_patch16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-24 20:58:48.000000 composer-0.13.5/composer/models/vit_small_patch16/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.465397 composer-0.13.5/composer/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-24 20:58:48.000000 composer-0.13.5/composer/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-04-24 20:58:48.000000 composer-0.13.5/composer/optim/decoupled_weight_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-04-24 20:58:48.000000 composer-0.13.5/composer/optim/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.469396 composer-0.13.5/composer/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/json_trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/json_trace_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/profiler_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/profiler_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/system_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/torch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-24 20:58:48.000000 composer-0.13.5/composer/profiler/trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:58:48.000000 composer-0.13.5/composer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.469396 composer-0.13.5/composer/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/_scale_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/dist_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/meta_safe_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/mosaic_fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152656 2023-04-24 20:58:48.000000 composer-0.13.5/composer/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.469396 composer-0.13.5/composer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/auto_log_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/batch_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28956 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/fx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/iter_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/module_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.473396 composer-0.13.5/composer/utils/object_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/libcloud_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/oci_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/object_store/sftp_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 20:58:48.000000 composer-0.13.5/composer/utils/string_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.437396 composer-0.13.5/composer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 20:59:01.000000 composer-0.13.5/composer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34926 2023-04-24 20:58:48.000000 composer-0.13.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:59:01.473396 composer-0.13.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-24 20:58:48.000000 composer-0.13.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:59:01.473396 composer-0.13.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_full_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_simple_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_smoketest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_split_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-24 20:58:48.000000 composer-0.13.5/tests/test_time.py
```

### Comparing `composer-0.13.4/LICENSE` & `composer-0.13.5/LICENSE`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/PKG-INFO` & `composer-0.13.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.13.4
+Version: 0.13.5
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: composer Version: 0.13.4 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.13.5 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
```

### Comparing `composer-0.13.4/README.md` & `composer-0.13.5/README.md`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/__init__.py` & `composer-0.13.5/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/__init__.py` & `composer-0.13.5/composer/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/alibi/__init__.py` & `composer-0.13.5/composer/algorithms/alibi/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/alibi/alibi.py` & `composer-0.13.5/composer/algorithms/alibi/alibi.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/__init__.py` & `composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/_bert.py` & `composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/_bert.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py` & `composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/alibi/attention_surgery_functions/utils.py` & `composer-0.13.5/composer/algorithms/alibi/attention_surgery_functions/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/augmix/__init__.py` & `composer-0.13.5/composer/algorithms/augmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/augmix/augmix.py` & `composer-0.13.5/composer/algorithms/augmix/augmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/blurpool/__init__.py` & `composer-0.13.5/composer/algorithms/blurpool/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/blurpool/blurpool.py` & `composer-0.13.5/composer/algorithms/blurpool/blurpool.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/blurpool/blurpool_layers.py` & `composer-0.13.5/composer/algorithms/blurpool/blurpool_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/channels_last/__init__.py` & `composer-0.13.5/composer/algorithms/channels_last/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/channels_last/channels_last.py` & `composer-0.13.5/composer/algorithms/channels_last/channels_last.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/channels_last/metadata.json` & `composer-0.13.5/composer/algorithms/channels_last/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/colout/__init__.py` & `composer-0.13.5/composer/algorithms/colout/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/colout/colout.py` & `composer-0.13.5/composer/algorithms/colout/colout.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/cutmix/__init__.py` & `composer-0.13.5/composer/algorithms/cutmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/cutmix/cutmix.py` & `composer-0.13.5/composer/algorithms/cutmix/cutmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/cutmix/metadata.json` & `composer-0.13.5/composer/algorithms/cutmix/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/cutout/cutout.py` & `composer-0.13.5/composer/algorithms/cutout/cutout.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/ema/ema.py` & `composer-0.13.5/composer/algorithms/ema/ema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Core Exponential Moving Average (EMA) classes and functions."""
 
 from __future__ import annotations
 
+import contextlib
 import itertools
 import logging
 from typing import Any, Dict, Optional, Union
 
 import torch
 
+import composer.utils.misc as misc
 from composer.callbacks.checkpoint_saver import CheckpointSaver
 from composer.core import Algorithm, Event, State, Time, TimeUnit
 from composer.loggers import Logger
 
 log = logging.getLogger(__name__)
 
 __all__ = ['EMA', 'compute_ema']
@@ -52,33 +54,45 @@
 
                 import composer.functional as cf
                 from torchvision import models
                 model = models.resnet50()
                 ema_model = models.resnet50()
                 cf.compute_ema(model, ema_model, smoothing=0.9)
     """
-    with torch.no_grad():
-        # If the ema model is a pytorch module, can just use the state_dict
-        if isinstance(ema_model, torch.nn.Module):
-            ema_params = ema_model.state_dict()
-            for name, param in itertools.chain(model.named_parameters(), model.named_buffers()):
-                if name in ema_params:
-                    ema_params[name].copy_(ema_params[name] * smoothing + param.data * (1. - smoothing))
-        # Otherwise, the ema model needs to define the named_parameters and named_buffers dictionaries
-        # These should contain the parameters and buffers to average.
-        elif isinstance(ema_model, EMAParameters):
-            ema_parameters = ema_model.named_parameters_dict
-            ema_buffers = ema_model.named_buffers_dict
-            for name, param in itertools.chain(model.named_parameters(), model.named_buffers()):
-                if name in ema_parameters:
-                    ema_parameters[name].copy_(ema_parameters[name] * smoothing + param.data * (1. - smoothing))
-                if name in ema_buffers:
-                    ema_buffers[name].copy_(ema_buffers[name] * smoothing + param.data * (1. - smoothing))
-        else:
-            raise ValueError('ema_model must be a torch.nn.Module or EMAParameters')
+    model_context_manager = get_model_context_manager(model)
+
+    with model_context_manager:
+        with torch.no_grad():
+            # If the ema model is a pytorch module, can just use the state_dict
+            if isinstance(ema_model, torch.nn.Module):
+                ema_params = ema_model.state_dict()
+                for name, param in itertools.chain(model.named_parameters(), model.named_buffers()):
+                    if name in ema_params:
+                        ema_params[name].copy_(ema_params[name] * smoothing + param.data * (1. - smoothing))
+            # Otherwise, the ema model needs to define the named_parameters and named_buffers dictionaries
+            # These should contain the parameters and buffers to average.
+            elif isinstance(ema_model, EMAParameters):
+                ema_parameters = ema_model.named_parameters_dict
+                ema_buffers = ema_model.named_buffers_dict
+                for name, param in itertools.chain(model.named_parameters(), model.named_buffers()):
+                    if name in ema_parameters:
+                        ema_parameters[name].copy_(ema_parameters[name] * smoothing + param.data * (1. - smoothing))
+                    if name in ema_buffers:
+                        ema_buffers[name].copy_(ema_buffers[name] * smoothing + param.data * (1. - smoothing))
+            else:
+                raise ValueError('ema_model must be a torch.nn.Module or EMAParameters')
+
+
+def get_model_context_manager(model: torch.nn.Module):
+    """Summons full params for FSDP, which is required to update sharded params."""
+    fsdp_enabled = misc.is_model_fsdp(model)
+    model_context_manager = contextlib.nullcontext()
+    if fsdp_enabled:
+        model_context_manager = model.module.summon_full_params(model.module)  # type: ignore
+    return model_context_manager
 
 
 class EMA(Algorithm):
     r"""Maintains a set of weights that follow the exponential moving average of the training model weights.
 
     Weights are updated according to
 
@@ -113,14 +127,15 @@
             an ``update_interval='1ep'`` means updates are done every epoch, while ``update_interval='10ba'`` means
             updates are done once every ten batches. Units must match the units used to specify ``half_life`` if not
             using ``smoothing``. If not specified, ``update_interval`` will default to ``1`` in the units of
             ``half_life``, or ``"1ba"`` if ``smoothing`` is specified. Time must be an integer value in the units
             specified. Default: ``None``.
 
     Example:
+
         .. testcode::
 
             from composer.algorithms import EMA
             algorithm = EMA(half_life='1000ba', update_interval='1ba')
             trainer = Trainer(
                 model=model,
                 train_dataloader=train_dataloader,
@@ -366,54 +381,74 @@
 
 
 class EMAParameters:
     """A class that stores the parameters and buffers of a model needed for averaging."""
 
     def __init__(self, model: Union[None, torch.nn.Module]):
         if model is not None:
-            # Copy the trainable parameters and buffers.
-            self.named_parameters_dict = {
-                name: param.data.clone() for name, param in model.named_parameters() if param.requires_grad
-            }
-            self.named_buffers_dict = {name: buffer.data.clone() for name, buffer in model.named_buffers()}
+            model_context_manager = get_model_context_manager(model)
+            with model_context_manager:
+                # Copy the trainable parameters and buffers.
+                self.named_parameters_dict = {
+                    name: param.data.clone() for name, param in model.named_parameters() if param.requires_grad
+                }
+                self.named_buffers_dict = {name: buffer.data.clone() for name, buffer in model.named_buffers()}
         else:
             # Empty storage
             self.named_parameters_dict = {}
             self.named_buffers_dict = {}
 
     def named_parameters(self):
         return self.named_parameters_dict.items()
 
     def named_buffers(self):
         return self.named_buffers_dict.items()
 
     def swap_params(self, model: torch.nn.Module):
         """Swaps the parameters and buffers of a model with the ema parameters."""
+        model_context_manager = get_model_context_manager(model)
+
         with torch.no_grad():
             ema_params = self.named_parameters_dict
             ema_buffers = self.named_buffers_dict
 
-            for name, param in model.named_parameters():
-                if name in ema_params:
-                    param.data, ema_params[name] = ema_params[name], param.data
-
-            for name, buffer in model.named_buffers():
-                buffer.data, ema_buffers[name] = ema_buffers[name], buffer.data
+            with model_context_manager:
+                for name, param in model.named_parameters():
+                    if name in ema_params:
+                        # Use copy instead of raw data access (eg .data) doesn't work with FSDP
+                        dummy_param = param.clone()
+                        param.copy_(ema_params[name])
+                        ema_params[name].copy_(dummy_param)
+
+                for name, buffer in model.named_buffers():
+                    if name in ema_buffers:
+                        # Use copy instead of raw data access (eg .data) doesn't work with FSDP
+                        dummy_buffer = buffer.clone()
+                        buffer.copy_(ema_buffers[name])
+                        ema_buffers[name].copy_(dummy_buffer)
 
     def transfer_ema_params(self, model: torch.nn.Module):
         """Transfers the parameters and buffers from the ema model to the supplied model."""
-        with torch.no_grad():
-            for name, param in model.named_parameters():
-                if name in self.named_parameters_dict:
-                    param.data = self.named_parameters_dict[name]
+        model_context_manager = get_model_context_manager(model)
 
-            for name, buffer in model.named_buffers():
-                buffer.data = self.named_buffers_dict[name]
+        with model_context_manager:
+            with torch.no_grad():
+                for name, param in model.named_parameters():
+                    if name in self.named_parameters_dict:
+                        param.copy_(self.named_parameters_dict[name])
+
+                for name, buffer in model.named_buffers():
+                    if name in self.named_buffers_dict:
+                        buffer.copy_(self.named_buffers_dict[name])
 
     def move_params_to_device(self, destination_model: torch.nn.Module):
         """Moves the ema parameters and buffers to the device of a destination model."""
-        model_state_dict = destination_model.state_dict()
-        for name, param in self.named_parameters_dict.items():
-            self.named_parameters_dict[name] = param.to(model_state_dict[name].device)
+        model_context_manager = get_model_context_manager(destination_model)
+
+        with model_context_manager:
+            for name, param in destination_model.named_parameters():
+                if name in self.named_parameters_dict:
+                    self.named_parameters_dict[name] = self.named_parameters_dict[name].to(param.device)
 
-        for name, buffer in self.named_buffers_dict.items():
-            self.named_buffers_dict[name] = buffer.to(model_state_dict[name].device)
+            for name, buffer in destination_model.named_buffers():
+                if name in self.named_buffers_dict:
+                    self.named_buffers_dict[name] = self.named_buffers_dict[name].to(buffer.device)
```

### Comparing `composer-0.13.4/composer/algorithms/factorize/__init__.py` & `composer-0.13.5/composer/algorithms/factorize/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/factorize/factorize.py` & `composer-0.13.5/composer/algorithms/factorize/factorize.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/factorize/factorize_core.py` & `composer-0.13.5/composer/algorithms/factorize/factorize_core.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/factorize/factorize_modules.py` & `composer-0.13.5/composer/algorithms/factorize/factorize_modules.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/fused_layernorm/__init__.py` & `composer-0.13.5/composer/algorithms/fused_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/fused_layernorm/fused_layernorm.py` & `composer-0.13.5/composer/algorithms/fused_layernorm/fused_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/fused_layernorm/metadata.json` & `composer-0.13.5/composer/algorithms/fused_layernorm/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/gated_linear_units/__init__.py` & `composer-0.13.5/composer/algorithms/gated_linear_units/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py` & `composer-0.13.5/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/gated_linear_units/gated_linear_units.py` & `composer-0.13.5/composer/algorithms/gated_linear_units/gated_linear_units.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/gated_linear_units/metadata.json` & `composer-0.13.5/composer/algorithms/gated_linear_units/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/ghost_batchnorm/__init__.py` & `composer-0.13.5/composer/algorithms/ghost_batchnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py` & `composer-0.13.5/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/ghost_batchnorm/metadata.json` & `composer-0.13.5/composer/algorithms/ghost_batchnorm/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/gradient_clipping/gradient_clipping.py` & `composer-0.13.5/composer/algorithms/gradient_clipping/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/gradient_clipping/metadata.json` & `composer-0.13.5/composer/algorithms/gradient_clipping/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/gyro_dropout/gyro_dropout.py` & `composer-0.13.5/composer/algorithms/gyro_dropout/gyro_dropout.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/label_smoothing/__init__.py` & `composer-0.13.5/composer/algorithms/label_smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/label_smoothing/label_smoothing.py` & `composer-0.13.5/composer/algorithms/label_smoothing/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/label_smoothing/metadata.json` & `composer-0.13.5/composer/algorithms/label_smoothing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/layer_freezing/layer_freezing.py` & `composer-0.13.5/composer/algorithms/layer_freezing/layer_freezing.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/layer_freezing/metadata.json` & `composer-0.13.5/composer/algorithms/layer_freezing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/low_precision_groupnorm/__init__.py` & `composer-0.13.5/composer/algorithms/low_precision_groupnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py` & `composer-0.13.5/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/low_precision_layernorm/__init__.py` & `composer-0.13.5/composer/algorithms/low_precision_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py` & `composer-0.13.5/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/mixup/metadata.json` & `composer-0.13.5/composer/algorithms/mixup/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/mixup/mixup.py` & `composer-0.13.5/composer/algorithms/mixup/mixup.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/no_op_model/__init__.py` & `composer-0.13.5/composer/algorithms/no_op_model/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/no_op_model/no_op_model.py` & `composer-0.13.5/composer/algorithms/no_op_model/no_op_model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/progressive_resizing/__init__.py` & `composer-0.13.5/composer/algorithms/progressive_resizing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/progressive_resizing/metadata.json` & `composer-0.13.5/composer/algorithms/progressive_resizing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/progressive_resizing/progressive_resizing.py` & `composer-0.13.5/composer/algorithms/progressive_resizing/progressive_resizing.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/randaugment/metadata.json` & `composer-0.13.5/composer/algorithms/randaugment/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/randaugment/randaugment.py` & `composer-0.13.5/composer/algorithms/randaugment/randaugment.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/sam/__init__.py` & `composer-0.13.5/composer/algorithms/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/sam/sam.py` & `composer-0.13.5/composer/algorithms/sam/sam.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/selective_backprop/__init__.py` & `composer-0.13.5/composer/algorithms/selective_backprop/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/selective_backprop/metadata.json` & `composer-0.13.5/composer/algorithms/selective_backprop/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/selective_backprop/selective_backprop.py` & `composer-0.13.5/composer/algorithms/selective_backprop/selective_backprop.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/seq_length_warmup/metadata.json` & `composer-0.13.5/composer/algorithms/seq_length_warmup/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/seq_length_warmup/seq_length_warmup.py` & `composer-0.13.5/composer/algorithms/seq_length_warmup/seq_length_warmup.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/squeeze_excite/__init__.py` & `composer-0.13.5/composer/algorithms/squeeze_excite/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/squeeze_excite/squeeze_excite.py` & `composer-0.13.5/composer/algorithms/squeeze_excite/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/stochastic_depth/__init__.py` & `composer-0.13.5/composer/algorithms/stochastic_depth/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/stochastic_depth/metadata.json` & `composer-0.13.5/composer/algorithms/stochastic_depth/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/stochastic_depth/stochastic_depth.py` & `composer-0.13.5/composer/algorithms/stochastic_depth/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/stochastic_depth/stochastic_layers.py` & `composer-0.13.5/composer/algorithms/stochastic_depth/stochastic_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/swa/swa.py` & `composer-0.13.5/composer/algorithms/swa/swa.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/utils/augmentation_common.py` & `composer-0.13.5/composer/algorithms/utils/augmentation_common.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/utils/augmentation_primitives.py` & `composer-0.13.5/composer/algorithms/utils/augmentation_primitives.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/warnings.py` & `composer-0.13.5/composer/algorithms/warnings.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/weight_standardization/metadata.json` & `composer-0.13.5/composer/algorithms/weight_standardization/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/algorithms/weight_standardization/weight_standardization.py` & `composer-0.13.5/composer/algorithms/weight_standardization/weight_standardization.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/__init__.py` & `composer-0.13.5/composer/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/checkpoint_saver.py` & `composer-0.13.5/composer/callbacks/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/early_stopper.py` & `composer-0.13.5/composer/callbacks/early_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/export_for_inference.py` & `composer-0.13.5/composer/callbacks/export_for_inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/health_checker.py` & `composer-0.13.5/composer/callbacks/health_checker.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/image_visualizer.py` & `composer-0.13.5/composer/callbacks/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/lr_monitor.py` & `composer-0.13.5/composer/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/memory_monitor.py` & `composer-0.13.5/composer/callbacks/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/mlperf.py` & `composer-0.13.5/composer/callbacks/mlperf.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/optimizer_monitor.py` & `composer-0.13.5/composer/callbacks/optimizer_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/runtime_estimator.py` & `composer-0.13.5/composer/callbacks/runtime_estimator.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/speed_monitor.py` & `composer-0.13.5/composer/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/callbacks/threshold_stopper.py` & `composer-0.13.5/composer/callbacks/threshold_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/cli/launcher.py` & `composer-0.13.5/composer/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/__init__.py` & `composer-0.13.5/composer/core/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/algorithm.py` & `composer-0.13.5/composer/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/callback.py` & `composer-0.13.5/composer/core/callback.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/data_spec.py` & `composer-0.13.5/composer/core/data_spec.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/engine.py` & `composer-0.13.5/composer/core/engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/evaluator.py` & `composer-0.13.5/composer/core/evaluator.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/event.py` & `composer-0.13.5/composer/core/event.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/passes.py` & `composer-0.13.5/composer/core/passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/precision.py` & `composer-0.13.5/composer/core/precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/serializable.py` & `composer-0.13.5/composer/core/serializable.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/state.py` & `composer-0.13.5/composer/core/state.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/time.py` & `composer-0.13.5/composer/core/time.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/core/types.py` & `composer-0.13.5/composer/core/types.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/__init__.py` & `composer-0.13.5/composer/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/ade20k.py` & `composer-0.13.5/composer/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/brats.py` & `composer-0.13.5/composer/datasets/brats.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/c4.py` & `composer-0.13.5/composer/datasets/c4.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/cifar.py` & `composer-0.13.5/composer/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/ffcv_utils.py` & `composer-0.13.5/composer/datasets/ffcv_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/imagenet.py` & `composer-0.13.5/composer/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/in_context_learning_evaluation.py` & `composer-0.13.5/composer/datasets/in_context_learning_evaluation.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/lm_dataset.py` & `composer-0.13.5/composer/datasets/lm_dataset.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/mnist.py` & `composer-0.13.5/composer/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/synthetic.py` & `composer-0.13.5/composer/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/datasets/utils.py` & `composer-0.13.5/composer/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/devices/device.py` & `composer-0.13.5/composer/devices/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/devices/device_cpu.py` & `composer-0.13.5/composer/devices/device_cpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/devices/device_gpu.py` & `composer-0.13.5/composer/devices/device_gpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/devices/device_mps.py` & `composer-0.13.5/composer/devices/device_mps.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/devices/device_tpu.py` & `composer-0.13.5/composer/devices/device_tpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/functional/__init__.py` & `composer-0.13.5/composer/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/__init__.py` & `composer-0.13.5/composer/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/cometml_logger.py` & `composer-0.13.5/composer/loggers/cometml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/console_logger.py` & `composer-0.13.5/composer/loggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/file_logger.py` & `composer-0.13.5/composer/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/in_memory_logger.py` & `composer-0.13.5/composer/loggers/in_memory_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/logger.py` & `composer-0.13.5/composer/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/logger_destination.py` & `composer-0.13.5/composer/loggers/logger_destination.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/mlflow_logger.py` & `composer-0.13.5/composer/loggers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/progress_bar_logger.py` & `composer-0.13.5/composer/loggers/progress_bar_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/remote_uploader_downloader.py` & `composer-0.13.5/composer/loggers/remote_uploader_downloader.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/tensorboard_logger.py` & `composer-0.13.5/composer/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loggers/wandb_logger.py` & `composer-0.13.5/composer/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loss/loss.py` & `composer-0.13.5/composer/loss/loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/loss/utils.py` & `composer-0.13.5/composer/loss/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/metrics/__init__.py` & `composer-0.13.5/composer/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/metrics/map.py` & `composer-0.13.5/composer/metrics/map.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/metrics/metrics.py` & `composer-0.13.5/composer/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/metrics/nlp.py` & `composer-0.13.5/composer/metrics/nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/__init__.py` & `composer-0.13.5/composer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/base.py` & `composer-0.13.5/composer/models/base.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/bert/model.py` & `composer-0.13.5/composer/models/bert/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/classify_mnist/model.py` & `composer-0.13.5/composer/models/classify_mnist/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/deeplabv3/model.py` & `composer-0.13.5/composer/models/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/efficientnetb0/__init__.py` & `composer-0.13.5/composer/models/efficientnetb0/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/efficientnetb0/_layers.py` & `composer-0.13.5/composer/models/efficientnetb0/_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/efficientnetb0/efficientnets.py` & `composer-0.13.5/composer/models/efficientnetb0/efficientnets.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/efficientnetb0/model.py` & `composer-0.13.5/composer/models/efficientnetb0/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/gpt2/__init__.py` & `composer-0.13.5/composer/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/gpt2/model.py` & `composer-0.13.5/composer/models/gpt2/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/huggingface.py` & `composer-0.13.5/composer/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/initializers.py` & `composer-0.13.5/composer/models/initializers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/mmdetection.py` & `composer-0.13.5/composer/models/mmdetection.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/resnet/__init__.py` & `composer-0.13.5/composer/models/resnet/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/resnet/model.py` & `composer-0.13.5/composer/models/resnet/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/resnet_cifar/__init__.py` & `composer-0.13.5/composer/models/resnet_cifar/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/resnet_cifar/model.py` & `composer-0.13.5/composer/models/resnet_cifar/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/resnet_cifar/resnets.py` & `composer-0.13.5/composer/models/resnet_cifar/resnets.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/tasks/classification.py` & `composer-0.13.5/composer/models/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/timm/model.py` & `composer-0.13.5/composer/models/timm/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/unet/_layers.py` & `composer-0.13.5/composer/models/unet/_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/unet/model.py` & `composer-0.13.5/composer/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/unet/unet.py` & `composer-0.13.5/composer/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/models/vit_small_patch16/model.py` & `composer-0.13.5/composer/models/vit_small_patch16/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/optim/__init__.py` & `composer-0.13.5/composer/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/optim/decoupled_weight_decay.py` & `composer-0.13.5/composer/optim/decoupled_weight_decay.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/optim/scheduler.py` & `composer-0.13.5/composer/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/__init__.py` & `composer-0.13.5/composer/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/json_trace_handler.py` & `composer-0.13.5/composer/profiler/json_trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/json_trace_merger.py` & `composer-0.13.5/composer/profiler/json_trace_merger.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/marker.py` & `composer-0.13.5/composer/profiler/marker.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/profiler.py` & `composer-0.13.5/composer/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/profiler_action.py` & `composer-0.13.5/composer/profiler/profiler_action.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/profiler_schedule.py` & `composer-0.13.5/composer/profiler/profiler_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/system_profiler.py` & `composer-0.13.5/composer/profiler/system_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/torch_profiler.py` & `composer-0.13.5/composer/profiler/torch_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/profiler/trace_handler.py` & `composer-0.13.5/composer/profiler/trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/trainer/_deepspeed.py` & `composer-0.13.5/composer/trainer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/trainer/_scale_schedule.py` & `composer-0.13.5/composer/trainer/_scale_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/trainer/_scaler.py` & `composer-0.13.5/composer/trainer/_scaler.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/trainer/dist_strategy.py` & `composer-0.13.5/composer/trainer/dist_strategy.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/trainer/meta_safe_apply.py` & `composer-0.13.5/composer/trainer/meta_safe_apply.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/trainer/mosaic_fsdp.py` & `composer-0.13.5/composer/trainer/mosaic_fsdp.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/trainer/trainer.py` & `composer-0.13.5/composer/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/__init__.py` & `composer-0.13.5/composer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/auto_log_hparams.py` & `composer-0.13.5/composer/utils/auto_log_hparams.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/batch_helpers.py` & `composer-0.13.5/composer/utils/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/checkpoint.py` & `composer-0.13.5/composer/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/collect_env.py` & `composer-0.13.5/composer/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/device.py` & `composer-0.13.5/composer/utils/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/dist.py` & `composer-0.13.5/composer/utils/dist.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/file_helpers.py` & `composer-0.13.5/composer/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/fx_utils.py` & `composer-0.13.5/composer/utils/fx_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/import_helpers.py` & `composer-0.13.5/composer/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/inference.py` & `composer-0.13.5/composer/utils/inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/iter_helpers.py` & `composer-0.13.5/composer/utils/iter_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/misc.py` & `composer-0.13.5/composer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/module_surgery.py` & `composer-0.13.5/composer/utils/module_surgery.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/object_store/__init__.py` & `composer-0.13.5/composer/utils/object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/object_store/libcloud_object_store.py` & `composer-0.13.5/composer/utils/object_store/libcloud_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/object_store/object_store.py` & `composer-0.13.5/composer/utils/object_store/object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/object_store/oci_object_store.py` & `composer-0.13.5/composer/utils/object_store/oci_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/object_store/s3_object_store.py` & `composer-0.13.5/composer/utils/object_store/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/object_store/sftp_object_store.py` & `composer-0.13.5/composer/utils/object_store/sftp_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/reproducibility.py` & `composer-0.13.5/composer/utils/reproducibility.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/retrying.py` & `composer-0.13.5/composer/utils/retrying.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer/utils/string_enum.py` & `composer-0.13.5/composer/utils/string_enum.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer.egg-info/PKG-INFO` & `composer-0.13.5/composer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.13.4
+Version: 0.13.5
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: composer Version: 0.13.4 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.13.5 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
```

### Comparing `composer-0.13.4/composer.egg-info/SOURCES.txt` & `composer-0.13.5/composer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/composer.egg-info/requires.txt` & `composer-0.13.5/composer.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -10,73 +10,73 @@
 coolname<3,>=1.1.0
 tabulate==0.9.0
 py-cpuinfo<10,>=8.0.0
 packaging<23,>=21.3.0
 importlib-metadata<7,>=5.0.0
 
 [all]
-fasteners==0.18
-onnx<2,>=1.12.0
-ipykernel==6.20.1
-deepspeed==0.7.7
-sphinx_markdown_tables==0.0.17
-oci<3.0.0,>=2.88.2
+GitPython==3.1.31
+tensorboard<3.0.0,>=2.9.1
+pycocotools<3,>=2.0.4
+setuptools<=59.5.0
 jupyter==1.0.0
-myst-parser==0.16.1
-transformers<4.27,>=4.11
-pre-commit<3,>=2.18.1
+moto[s3]<5,>=4.0.1
+fasteners==0.18
+coverage[toml]==7.2.1
 timm<0.6,>=0.5.4
-testbook==0.4.2
-tensorboard<3.0.0,>=2.9.1
+pytest_codeblocks==0.16.1
 apache-libcloud<4,>=3.3.1
-GitPython==3.1.31
-pandoc==2.3
-paramiko<3,>=2.11.0
+oci<3.0.0,>=2.88.2
+custom_inherit==2.4.1
+recommonmark==0.7.1
+junitparser==2.8.0
 docutils==0.17.1
-mlflow<3.0,>=2.0.1
-toml==0.10.2
+myst-parser==0.16.1
+ipykernel==6.20.1
+pypandoc==1.11
+sphinxcontrib.katex==0.9.4
+sphinx==4.4.0
+testbook==0.4.2
+sphinxemoji==0.2.0
+onnx<2,>=1.12.0
+pytest-httpserver<1.1,>=1.0.4
 vit_pytorch==0.35.8
-sphinxext.opengraph==0.7.4
-onnxruntime<2,>=1.12.1
-setuptools<=59.5.0
+paramiko<3,>=2.11.0
 nbsphinx==0.8.12
-boto3<2,>=1.21.45
-datasets<3,>=2.4
-sphinxcontrib.katex==0.9.4
-wandb<0.14,>=0.13.2
-pycocotools<3,>=2.0.4
-ipython==8.11.0
-mosaicml-streaming<1.0
 sphinx-copybutton==0.5.0
-pytest-httpserver<1.1,>=1.0.4
 scikit-learn<2,>=1.0.1
-sphinx==4.4.0
-recommonmark==0.7.1
-furo==2022.9.29
-pynvml<12,>=11.5.0
 py-cpuinfo<10,>=8.0.0
-pypandoc==1.11
-sphinxcontrib-images==0.9.4
-slack_sdk<4,>=3.19.5
-custom_inherit==2.4.1
-pytest_codeblocks==0.16.1
-pytest==7.2.2
-sphinx_panels==0.6.0
-monai<1.2,>=0.9.1
+onnxruntime<2,>=1.12.1
+furo==2022.9.29
+sphinx_markdown_tables==0.0.17
 mock-ssh-server==0.9.1
-junitparser==2.8.0
+monai<1.2,>=0.9.1
+mosaicml-streaming<1.0
+traitlets==5.9.0
+wandb<0.14,>=0.13.2
 yamllint==1.28.0
-sphinxemoji==0.2.0
-cryptography==38.0.4
-coverage[toml]==7.2.1
-moto[s3]<5,>=4.0.1
+sphinxcontrib-images==0.9.4
+sphinxext.opengraph==0.7.4
+pynvml<12,>=11.5.0
+deepspeed==0.7.7
+sphinx-argparse==0.4.0
 comet_ml<4.0.0,>=3.31.12
+mlflow<3.0,>=2.0.1
 sentencepiece==0.1.97
-traitlets==5.9.0
-sphinx-argparse==0.4.0
+pandoc==2.3
+toml==0.10.2
+sphinx_panels==0.6.0
+ipython==8.11.0
+boto3<2,>=1.21.45
+pytest==7.2.2
+pre-commit<3,>=2.18.1
+transformers<4.27,>=4.11
+slack_sdk<4,>=3.19.5
+datasets<3,>=2.4
+cryptography==38.0.4
 
 [base]
 
 [coco]
 pycocotools<3,>=2.0.4
 
 [comet_ml]
@@ -120,16 +120,16 @@
 moto[s3]<5,>=4.0.1
 mock-ssh-server==0.9.1
 cryptography==38.0.4
 pytest-httpserver<1.1,>=1.0.4
 setuptools<=59.5.0
 
 [health_checker]
-slack_sdk<4,>=3.19.5
 pynvml<12,>=11.5.0
+slack_sdk<4,>=3.19.5
 
 [libcloud]
 apache-libcloud<4,>=3.3.1
 
 [mlflow]
 mlflow<3.0,>=2.0.1
```

### Comparing `composer-0.13.4/pyproject.toml` & `composer-0.13.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/setup.py` & `composer-0.13.5/setup.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_device.py` & `composer-0.13.5/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_docker.py` & `composer-0.13.5/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_docs.py` & `composer-0.13.5/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_engine.py` & `composer-0.13.5/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_events.py` & `composer-0.13.5/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_full_nlp.py` & `composer-0.13.5/tests/test_full_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_loss.py` & `composer-0.13.5/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_notebooks.py` & `composer-0.13.5/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_passes.py` & `composer-0.13.5/tests/test_passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_precision.py` & `composer-0.13.5/tests/test_precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_simple_nlp.py` & `composer-0.13.5/tests/test_simple_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_smoketest.py` & `composer-0.13.5/tests/test_smoketest.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_split_batch.py` & `composer-0.13.5/tests/test_split_batch.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_state.py` & `composer-0.13.5/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `composer-0.13.4/tests/test_time.py` & `composer-0.13.5/tests/test_time.py`

 * *Files identical despite different names*


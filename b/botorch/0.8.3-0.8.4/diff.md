# Comparing `tmp/botorch-0.8.3.tar.gz` & `tmp/botorch-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botorch-0.8.3.tar", last modified: Wed Mar 15 21:23:44 2023, max compression
+gzip compressed data, was "botorch-0.8.4.tar", last modified: Mon Apr 24 15:50:22 2023, max compression
```

## Comparing `botorch-0.8.3.tar` & `botorch-0.8.4.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.314098 botorch-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.230097 botorch-0.8.3/.conda/
--rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-03-15 21:20:54.000000 botorch-0.8.3/.conda/build_conda.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-15 21:20:54.000000 botorch-0.8.3/.conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.234097 botorch-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.234097 botorch-0.8.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.246097 botorch-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/deploy_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/reusable_tutorials.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/reusable_website.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/test_stable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/tutorials_smoke_test_on_pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-15 21:20:54.000000 botorch-0.8.3/.github/workflows/tutorials_smoke_test_on_push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-15 21:20:54.000000 botorch-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    48550 2023-03-15 21:20:54.000000 botorch-0.8.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-15 21:20:54.000000 botorch-0.8.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-03-15 21:20:54.000000 botorch-0.8.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-15 21:20:54.000000 botorch-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 21:20:54.000000 botorch-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-03-15 21:23:44.314098 botorch-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-03-15 21:20:54.000000 botorch-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.246097 botorch-0.8.3/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.262097 botorch-0.8.3/botorch/acquisition/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)    47072 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/cached_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/cost_aware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/fixed_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    44051 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/input_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/joint_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    26678 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/knowledge_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    42039 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/max_value_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/monte_carlo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.266097 botorch-0.8.3/botorch/acquisition/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)    31296 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/joint_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/max_value_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    33366 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/multi_output_risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    48822 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/predictive_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_objective/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/multi_step_lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)    22017 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/penalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/predictive_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/proximal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13908 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/acquisition/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.266097 botorch-0.8.3/botorch/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/exceptions/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/exceptions/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.270097 botorch-0.8.3/botorch/generation/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20210 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/generation/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/generation/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/generation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.278097 botorch-0.8.3/botorch/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/approximate_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/contextual_multioutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/fully_bayesian_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/gp_regression_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/gp_regression_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    35041 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/gpytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24453 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/higher_order_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.282097 botorch-0.8.3/botorch/models/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/kernels/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/kernels/contextual_lcea.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/kernels/contextual_sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/kernels/downsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/kernels/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/kernels/linear_truncated_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.282097 botorch-0.8.3/botorch/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/likelihoods/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/model_list_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    32955 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    41592 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/pairwise_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.286097 botorch-0.8.3/botorch/models/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/transforms/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    63408 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/transforms/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    30085 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/transforms/outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.286097 botorch-0.8.3/botorch/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/utils/assorted.py
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/utils/inducing_point_allocators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/models/utils/parse_training_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.290097 botorch-0.8.3/botorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.290097 botorch-0.8.3/botorch/optim/closures/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/closures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/closures/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/closures/model_closures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    35615 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/numpy_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51921 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.294097 botorch-0.8.3/botorch/optim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/utils/acquisition_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/optim/utils/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.298097 botorch-0.8.3/botorch/posteriors/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/base_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/gpytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/higher_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/posterior_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/posteriors/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.298097 botorch-0.8.3/botorch/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/get_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/index_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/list_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pairwise_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.302097 botorch-0.8.3/botorch/sampling/pathwise/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.302097 botorch-0.8.3/botorch/sampling/pathwise/features/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/features/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/features/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/posterior_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/prior_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/update_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/pathwise/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/qmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/sampling/stochastic_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.302097 botorch-0.8.3/botorch/test_functions/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/test_functions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/test_functions/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    48773 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/test_functions/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/test_functions/multi_objective_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/test_functions/sensitivity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    24768 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/test_functions/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.306097 botorch-0.8.3/botorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/feasible_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    20040 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/gp_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/low_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.310097 botorch-0.8.3/botorch/utils/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.310097 botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/box_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/dominated.py
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/non_dominated.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/multi_objective/scalarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.314098 botorch-0.8.3/botorch/utils/probability/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/probability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/probability/bvn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/probability/lin_ess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/probability/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/probability/mvnxpb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/probability/truncated_multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/probability/unified_skew_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/probability/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/safe_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    33852 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-15 21:23:43.000000 botorch-0.8.3/botorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.250097 botorch-0.8.3/botorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-03-15 21:23:44.000000 botorch-0.8.3/botorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-03-15 21:23:44.000000 botorch-0.8.3/botorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:23:44.000000 botorch-0.8.3/botorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-15 21:23:44.000000 botorch-0.8.3/botorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 21:23:44.000000 botorch-0.8.3/botorch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    79395 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch_logo_lockup.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    63261 2023-03-15 21:20:54.000000 botorch-0.8.3/botorch_logo_lockup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-15 21:20:54.000000 botorch-0.8.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:23:44.314098 botorch-0.8.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-03-15 21:20:54.000000 botorch-0.8.3/notebooks/tutorials_performance_tracking.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-15 21:20:54.000000 botorch-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-15 21:20:54.000000 botorch-0.8.3/requirements-fmt.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-15 21:20:54.000000 botorch-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-15 21:23:44.314098 botorch-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-15 21:20:54.000000 botorch-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.006487 botorch-0.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.958487 botorch-0.8.4/.conda/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-04-24 15:47:10.000000 botorch-0.8.4/.conda/build_conda.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-24 15:47:10.000000 botorch-0.8.4/.conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.958487 botorch-0.8.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.962487 botorch-0.8.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.966487 botorch-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/deploy_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/reusable_tutorials.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/reusable_website.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/test_stable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/tutorials_smoke_test_on_pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-24 15:47:10.000000 botorch-0.8.4/.github/workflows/tutorials_smoke_test_on_push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-24 15:47:10.000000 botorch-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    49792 2023-04-24 15:47:10.000000 botorch-0.8.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-24 15:47:10.000000 botorch-0.8.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-24 15:47:10.000000 botorch-0.8.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-24 15:47:10.000000 botorch-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 15:47:10.000000 botorch-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-24 15:50:22.006487 botorch-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-24 15:47:10.000000 botorch-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.966487 botorch-0.8.4/botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.974487 botorch-0.8.4/botorch/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47072 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/cached_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/cost_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/fixed_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45121 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/input_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/joint_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26678 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/knowledge_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42039 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/max_value_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23047 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/monte_carlo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.978487 botorch-0.8.4/botorch/acquisition/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31296 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/joint_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/max_value_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33366 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/multi_output_risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48822 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/predictive_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_objective/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/multi_step_lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/penalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/predictive_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13908 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/acquisition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/cross_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.978487 botorch-0.8.4/botorch/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/exceptions/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/exceptions/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.978487 botorch-0.8.4/botorch/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/generation/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/generation/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/generation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.982487 botorch-0.8.4/botorch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/approximate_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/contextual_multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/fully_bayesian_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/gp_regression_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/gp_regression_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/gpytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/higher_order_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.986487 botorch-0.8.4/botorch/models/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/contextual_lcea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/contextual_sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/kernels/linear_truncated_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.986487 botorch-0.8.4/botorch/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/likelihoods/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/model_list_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46666 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/pairwise_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.986487 botorch-0.8.4/botorch/models/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63408 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30085 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.986487 botorch-0.8.4/botorch/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/utils/assorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/utils/inducing_point_allocators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/models/utils/parse_training_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.990487 botorch-0.8.4/botorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.990487 botorch-0.8.4/botorch/optim/closures/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/closures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/closures/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/closures/model_closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42398 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/numpy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56177 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.990487 botorch-0.8.4/botorch/optim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/acquisition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/optim/utils/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.994487 botorch-0.8.4/botorch/posteriors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/base_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/gpytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/higher_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/posterior_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/posteriors/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.994487 botorch-0.8.4/botorch/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/get_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/index_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/list_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pairwise_samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.998487 botorch-0.8.4/botorch/sampling/pathwise/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.998487 botorch-0.8.4/botorch/sampling/pathwise/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/features/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/features/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/posterior_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/prior_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/update_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/pathwise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/qmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/sampling/stochastic_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.998487 botorch-0.8.4/botorch/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48773 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/multi_objective_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/sensitivity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24915 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/test_functions/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.002487 botorch-0.8.4/botorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/feasible_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20040 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/gp_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/low_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.002487 botorch-0.8.4/botorch/utils/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.006487 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/box_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/dominated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/non_dominated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/multi_objective/scalarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.006487 botorch-0.8.4/botorch/utils/probability/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/bvn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/lin_ess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/mvnxpb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/truncated_multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/unified_skew_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/probability/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/rounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/safe_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36647 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:21.970487 botorch-0.8.4/botorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 15:50:21.000000 botorch-0.8.4/botorch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    79395 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch_logo_lockup.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63261 2023-04-24 15:47:10.000000 botorch-0.8.4/botorch_logo_lockup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 15:47:10.000000 botorch-0.8.4/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:50:22.006487 botorch-0.8.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-04-24 15:47:10.000000 botorch-0.8.4/notebooks/tutorials_performance_tracking.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 15:47:10.000000 botorch-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 15:47:10.000000 botorch-0.8.4/requirements-fmt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 15:47:10.000000 botorch-0.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 15:50:22.010487 botorch-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-24 15:47:10.000000 botorch-0.8.4/setup.py
```

### Comparing `botorch-0.8.3/.conda/meta.yaml` & `botorch-0.8.4/.conda/meta.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 requirements:
   host:
     - python>=3.8
     - setuptools
     - setuptools_scm
   run:
     - pytorch >=1.12
-    - gpytorch ==1.9.1
-    - linear_operator ==0.3.0
+    - gpytorch ==1.10
+    - linear_operator ==0.4.0
     - scipy
     - multipledispatch
     - pyro-ppl >=1.8.4
 
 test:
   imports:
     - botorch
```

### Comparing `botorch-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md` & `botorch-0.8.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md` & `botorch-0.8.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/ISSUE_TEMPLATE.md` & `botorch-0.8.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/PULL_REQUEST_TEMPLATE.md` & `botorch-0.8.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/workflows/deploy_on_release.yml` & `botorch-0.8.4/.github/workflows/deploy_on_release.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/workflows/docs.yml` & `botorch-0.8.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/workflows/lint.yml` & `botorch-0.8.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/workflows/nightly.yml` & `botorch-0.8.4/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/workflows/reusable_tutorials.yml` & `botorch-0.8.4/.github/workflows/reusable_tutorials.yml`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,16 @@
         python scripts/run_tutorials.py -p "$(pwd)" -s
     - if: ${{ !inputs.smoke_test }}
       name: Run tutorials without smoke test
       run: |
         python scripts/run_tutorials.py -p "$(pwd)"
     - if: ${{ inputs.upload_artifact }}
       name: Upload performance data to artifacts branch
+      # Sometimes pushing to this branch doesn't work -- fix planned
+      continue-on-error: true
       # 1) Switch to artifacts branch
       # 2) Add the new CSV file
       # 3) Get .py and .ipynb files needed for analyzing tutorials data from main
       # 4) Run `scripts/analyze_tutorials_performance.py` to merge CSVs and
       #  update notebook
       # 5) Commit updated notebook and new CSVs to artifacts branch
       run: |
```

### Comparing `botorch-0.8.3/.github/workflows/reusable_website.yml` & `botorch-0.8.4/.github/workflows/reusable_website.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/workflows/test.yml` & `botorch-0.8.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.github/workflows/test_stable.yml` & `botorch-0.8.4/.github/workflows/test_stable.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/.gitignore` & `botorch-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/CHANGELOG.md` & `botorch-0.8.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # Changelog
 
 The release log for BoTorch.
 
+## [0.8.4] - Apr 24, 2023
+
+#### Compatibility
+* Require GPyTorch == 1.10 and linear_operator == 0.4.0 (#1803).
+
+#### New Features
+* Polytope sampling for linear constraints along the q-dimension (#1757).
+* Single-objective joint entropy search with additional conditioning, various improvements to entropy-based acquisition functions (#1738).
+
+#### Other changes
+* Various updates to improve numerical stability of `PairwiseGP` (#1754, #1755).
+* Change batch range for `FullyBayesianPosterior` (1176a38352b69d01def0a466233e6633c17d6862, #1773).
+* Make `gen_batch_initial_conditions` more flexible (#1779).
+* Deprecate `objective` in favor of `posterior_transform` for `MultiObjectiveAnalyticAcquisitionFunction` (#1781).
+* Use `prune_baseline=True` as default for `qNoisyExpectedImprovement` (#1796).
+* Add `batch_shape` property to `SingleTaskVariationalGP` (#1799).
+* Change minimum inferred noise level for `SaasFullyBayesianSingleTaskGP` (#1800).
+
+#### Bug fixes
+* Add `output_task` to `MultiTaskGP.construct_inputs` (#1753).
+* Fix custom bounds handling in test problems (#1760).
+* Remove incorrect `BotorchTensorDimensionWarning` (#1790).
+* Fix handling of non-Container-typed positional arguments in `SupervisedDatasetMeta` (#1663).
+
+
 ## [0.8.3] - Mar 15, 2023
 
 #### New Features
 * Add BAxUS tutorial (#1559).
 
 #### Other changes
 * Various improvements to tutorials (#1703, #1706, #1707, #1708, #1710, #1711, #1718, #1719, #1739, #1740, #1742).
```

### Comparing `botorch-0.8.3/CODE_OF_CONDUCT.md` & `botorch-0.8.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/CONTRIBUTING.md` & `botorch-0.8.4/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,52 +14,47 @@
 ```
 
 
 ## Our Development Process
 
 #### Code Style
 
-BoTorch uses the [black](https://github.com/ambv/black) code formatter to
-enforce a common code style across the code base. black is installed easily via
-pip using `pip install black`, and run locally by calling
-```bash
-black .
-```
-from the repository root. No additional configuration should be needed (see the
-[black documentation](https://black.readthedocs.io/en/stable/installation_and_usage.html#usage)
-for advanced usage).
-
-Docstring formatting: We recommend [Google-style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) docstrings.
-To make sure documentation is rendered correctly, we require that every `__init__`
-function contains an "Args" block.
-We use `flake8-docstrings` to check this, as well as `flake8` to check code style. To use these tools, run
-`pip install flake8` and `pip install flake8-docstrings`, and then run
+BoTorch uses [ufmt](https://github.com/omnilib/ufmt) to enforce consistent
+code formatting (based on [black](https://github.com/ambv/black)) and
+import sorting (based on [µsort](https://github.com/facebook/usort))
+across the code base. Install via `pip install ufmt`, and
+auto-format and auto-sort by running
 ```bash
-flake8 .
+ufmt format .
 ```
+from the repository root.
 
 
-#### Import Sorting
+#### Flake8 linting
 
-BoTorch uses [ufmt]https://github.com/omnilib/ufmt library for consistent
-sorting of imports across the codebase. Install via `pip install ufmt`, and
-auto-sort with
+BoTorch uses `flake8` for linting. To run the linter locally, install
+`flake8` via `pip install flake8`, and then run
 ```bash
-ufmt format .
+flake8 .
 ```
 from the repository root.
 
-We feel strongly that having a consistent code style and imports is important,
-so CI will fail on your PR if it does not pass ufmt muster (note: under the
-hood ufmt also checks black code style).
+
+#### Docstring formatting
+
+BoTorch uses [Google-style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) docstrings.
+To make sure documentation is rendered correctly, we require that every
+`__init__` function contains an `Args:` block. We use the `flake8-docstrings`
+plugin to check this - install via `pip install flake8-docstrings` and
+run `flake8` as above to check.
 
 
 #### Type Hints
 
-BoTorch is fully typed using python 3.7+
+BoTorch is fully typed using python 3.8+
 [type hints](https://www.python.org/dev/peps/pep-0484/).
 We expect any contributions to also use proper type annotations. While we
 currently do not enforce full consistency of these in our continuous integration
 test, you should strive to type check your code locally. For this we recommend
 using [pyre](https://pyre-check.org/).
 
 
@@ -108,15 +103,15 @@
 
 1. Fork the repo and create your branch from `main`.
 2. If you have added code that should be tested, add unit tests.
    In other words, add unit tests.
 3. If you have changed APIs, update the documentation. Make sure the
    documentation builds.
 4. Ensure the test suite passes.
-5. Make sure your code passes both `black` and `flake8` formatting checks.
+5. Make sure your code passes both `ufmt` and `flake8` formatting checks.
 6. If you haven't already, complete the Contributor License Agreement ("CLA").
 
 
 ## Contributor License Agreement ("CLA")
 
 In order to accept your pull request, we need you to submit a CLA. You only need
 to do this once to work on any of Facebook's open source projects. You can
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `botorch-0.8.3/LICENSE` & `botorch-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/PKG-INFO` & `botorch-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botorch
-Version: 0.8.3
+Version: 0.8.4
 Summary: Bayesian Optimization in PyTorch
 Home-page: https://botorch.org
 Author: Meta Platforms, Inc.
 License: MIT
 Project-URL: Documentation, https://botorch.org
 Project-URL: Source, https://github.com/pytorch/botorch
 Project-URL: conda, https://anaconda.org/pytorch/botorch
@@ -77,16 +77,16 @@
 
 
 ## Installation
 
 **Installation Requirements**
 - Python >= 3.8
 - PyTorch >= 1.12
-- gpytorch == 1.9.1
-- linear_operator == 0.3.0
+- gpytorch == 1.10
+- linear_operator == 0.4.0
 - pyro-ppl >= 1.8.4
 - scipy
 - multiple-dispatch
 
 ### Prerequisite only for MacOS users with Intel processors:
 Before installing BoTorch, we recommend first manually installing PyTorch, a required dependency of
 BoTorch. Installing it according to the [PyTorch installation instructions](https://pytorch.org/get-started/locally/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botorch Version: 0.8.3 Summary: Bayesian
+Metadata-Version: 2.1 Name: botorch Version: 0.8.4 Summary: Bayesian
 Optimization in PyTorch Home-page: https://botorch.org Author: Meta Platforms,
 Inc. License: MIT Project-URL: Documentation, https://botorch.org Project-URL:
 Source, https://github.com/pytorch/botorch Project-URL: conda, https://
 anaconda.org/pytorch/botorch Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Intended Audience ::
@@ -44,85 +44,84 @@
 recommend using BoTorch as a low-level API for implementing new algorithms for
 [Ax](https://ax.dev). Ax has been designed to be an easy-to-use platform for
 end-users, which at the same time is flexible enough for Bayesian Optimization
 researchers to plug into for handling of feature transformations, (meta-)data
 management, storage, etc. We recommend that end-users who are not actively
 doing research on Bayesian Optimization simply use Ax. ## Installation
 **Installation Requirements** - Python >= 3.8 - PyTorch >= 1.12 - gpytorch ==
-1.9.1 - linear_operator == 0.3.0 - pyro-ppl >= 1.8.4 - scipy - multiple-
-dispatch ### Prerequisite only for MacOS users with Intel processors: Before
-installing BoTorch, we recommend first manually installing PyTorch, a required
-dependency of BoTorch. Installing it according to the [PyTorch installation
-instructions](https://pytorch.org/get-started/locally/) ensures that it is
-properly linked against MKL, a library that optimizes mathematical computation
-for Intel processors. This will result in up to an order-of-magnitude speed-up
-for Bayesian optimization, as at the moment, installing PyTorch from pip does
-not link against MKL. The PyTorch installation instructions currently
-recommend: 1. Install [Anaconda](https://www.anaconda.com/distribution/
-#download-section). Note that there are different installers for Intel and M1
-Macs. 2. Install PyTorch following the [PyTorch installation instructions]
-(https://pytorch.org/get-started/locally/). Currently, this suggests running
-`conda install pytorch torchvision -c pytorch`. If you want to customize your
-installation, please follow the [PyTorch installation instructions](https://
-pytorch.org/get-started/locally/) to build from source. ### Option 1:
-Installing the latest release The latest release of BoTorch is easily installed
-either via [Anaconda](https://www.anaconda.com/distribution/#download-section)
-(recommended) or pip. **To install BoTorch from Anaconda**, run ```bash conda
-install botorch -c pytorch -c gpytorch -c conda-forge ``` The above command
-installs BoTorch and any needed dependencies. ` -c pytorch -c gpytorch -
-c conda-forge` means that the most preferred source to install from is the
-PyTorch channel, the next most preferred is the GPyTorch channel, and the least
-preferred is conda-forge. **Alternatively, to install with `pip`**, do ```bash
-pip install botorch ``` _Note_: Make sure the `pip` being used is actually the
-one from the newly created Conda environment. If you're using a Unix-based OS,
-you can use `which pip` to check. ### Option 2: Installing from latest main
-branch If you would like to try our bleeding edge features (and don't mind
-potentially running into the occasional bug here or there), you can install the
-latest development version directly from GitHub. If you want to also install
-the current `gpytorch` and `linear_operator` development versions, you will
-need to ensure that the `ALLOW_LATEST_GPYTORCH_LINOP` environment variable is
-set: ```bash pip install --upgrade git+https://github.com/cornellius-gp/
-linear_operator.git pip install --upgrade git+https://github.com/cornellius-gp/
-gpytorch.git export ALLOW_LATEST_GPYTORCH_LINOP=true pip install --upgrade
-git+https://github.com/pytorch/botorch.git ``` ### Option 3: Editable/dev
-install If you want to [contribute](CONTRIBUTING.md) to BoTorch, you will want
-to install editably so that you can change files and have the changes reflected
-in your local install. If you want to install the current `gpytorch` and
-`linear_operator` development versions, as in Option 2, do that before
-proceeding. #### Option 3a: Bare-bones editable install ```bash git clone
-https://github.com/pytorch/botorch.git cd botorch pip install -e . ``` ####
-Option 3b: Editable install with development and tutorials dependencies ```bash
-git clone https://github.com/pytorch/botorch.git cd botorch export
-ALLOW_BOTORCH_LATEST=true pip install -e ".[dev, tutorials]" ``` * `dev`:
-Specifies tools necessary for development (testing, linting, docs building; see
-[Contributing](#contributing) below). * `tutorials`: Also installs all packages
-necessary for running the tutorial notebooks. * You can also install either the
-dev or tutorials dependencies without installing both, e.g. by changing the
-last command to `pip install -e ".[dev]"`. ## Getting Started Here's a quick
-run down of the main components of a Bayesian optimization loop. For more
-details see our [Documentation](https://botorch.org/docs/introduction) and the
-[Tutorials](https://botorch.org/tutorials). 1. Fit a Gaussian Process model to
-data ```python import torch from botorch.models import SingleTaskGP from
-botorch.fit import fit_gpytorch_mll from gpytorch.mlls import
-ExactMarginalLogLikelihood train_X = torch.rand(10, 2) Y = 1 - (train_X -
-0.5).norm(dim=-1, keepdim=True) # explicit output dimension Y += 0.1 *
-torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std() gp = SingleTaskGP
-(train_X, train_Y) mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
-fit_gpytorch_mll(mll) ``` 2. Construct an acquisition function ```python from
-botorch.acquisition import UpperConfidenceBound UCB = UpperConfidenceBound(gp,
-beta=0.1) ``` 3. Optimize the acquisition function ```python from botorch.optim
-import optimize_acqf bounds = torch.stack([torch.zeros(2), torch.ones(2)])
-candidate, acq_value = optimize_acqf( UCB, bounds=bounds, q=1, num_restarts=5,
-raw_samples=20, ) ``` ## Citing BoTorch If you use BoTorch, please cite the
-following paper: > [M. Balandat, B. Karrer, D. R. Jiang, S. Daulton, B. Letham,
-A. G. Wilson, and E. Bakshy. BoTorch: A Framework for Efficient Monte-Carlo
-Bayesian Optimization. Advances in Neural Information Processing Systems 33,
-2020.](https://arxiv.org/abs/1910.06403) ``` @inproceedings
-{balandat2020botorch, title={{BoTorch: A Framework for Efficient Monte-Carlo
-Bayesian Optimization}}, author={Balandat, Maximilian and Karrer, Brian and
-Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson, Andrew
-Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
+1.10 - linear_operator == 0.4.0 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
+### Prerequisite only for MacOS users with Intel processors: Before installing
+BoTorch, we recommend first manually installing PyTorch, a required dependency
+of BoTorch. Installing it according to the [PyTorch installation instructions]
+(https://pytorch.org/get-started/locally/) ensures that it is properly linked
+against MKL, a library that optimizes mathematical computation for Intel
+processors. This will result in up to an order-of-magnitude speed-up for
+Bayesian optimization, as at the moment, installing PyTorch from pip does not
+link against MKL. The PyTorch installation instructions currently recommend: 1.
+Install [Anaconda](https://www.anaconda.com/distribution/#download-section).
+Note that there are different installers for Intel and M1 Macs. 2. Install
+PyTorch following the [PyTorch installation instructions](https://pytorch.org/
+get-started/locally/). Currently, this suggests running `conda install pytorch
+torchvision -c pytorch`. If you want to customize your installation, please
+follow the [PyTorch installation instructions](https://pytorch.org/get-started/
+locally/) to build from source. ### Option 1: Installing the latest release The
+latest release of BoTorch is easily installed either via [Anaconda](https://
+www.anaconda.com/distribution/#download-section) (recommended) or pip. **To
+install BoTorch from Anaconda**, run ```bash conda install botorch -c pytorch -
+c gpytorch -c conda-forge ``` The above command installs BoTorch and any needed
+dependencies. ` -c pytorch -c gpytorch -c conda-forge` means that the most
+preferred source to install from is the PyTorch channel, the next most
+preferred is the GPyTorch channel, and the least preferred is conda-forge.
+**Alternatively, to install with `pip`**, do ```bash pip install botorch ```
+_Note_: Make sure the `pip` being used is actually the one from the newly
+created Conda environment. If you're using a Unix-based OS, you can use `which
+pip` to check. ### Option 2: Installing from latest main branch If you would
+like to try our bleeding edge features (and don't mind potentially running into
+the occasional bug here or there), you can install the latest development
+version directly from GitHub. If you want to also install the current
+`gpytorch` and `linear_operator` development versions, you will need to ensure
+that the `ALLOW_LATEST_GPYTORCH_LINOP` environment variable is set: ```bash pip
+install --upgrade git+https://github.com/cornellius-gp/linear_operator.git pip
+install --upgrade git+https://github.com/cornellius-gp/gpytorch.git export
+ALLOW_LATEST_GPYTORCH_LINOP=true pip install --upgrade git+https://github.com/
+pytorch/botorch.git ``` ### Option 3: Editable/dev install If you want to
+[contribute](CONTRIBUTING.md) to BoTorch, you will want to install editably so
+that you can change files and have the changes reflected in your local install.
+If you want to install the current `gpytorch` and `linear_operator` development
+versions, as in Option 2, do that before proceeding. #### Option 3a: Bare-bones
+editable install ```bash git clone https://github.com/pytorch/botorch.git cd
+botorch pip install -e . ``` #### Option 3b: Editable install with development
+and tutorials dependencies ```bash git clone https://github.com/pytorch/
+botorch.git cd botorch export ALLOW_BOTORCH_LATEST=true pip install -e ".[dev,
+tutorials]" ``` * `dev`: Specifies tools necessary for development (testing,
+linting, docs building; see [Contributing](#contributing) below). *
+`tutorials`: Also installs all packages necessary for running the tutorial
+notebooks. * You can also install either the dev or tutorials dependencies
+without installing both, e.g. by changing the last command to `pip install -
+e ".[dev]"`. ## Getting Started Here's a quick run down of the main components
+of a Bayesian optimization loop. For more details see our [Documentation]
+(https://botorch.org/docs/introduction) and the [Tutorials](https://
+botorch.org/tutorials). 1. Fit a Gaussian Process model to data ```python
+import torch from botorch.models import SingleTaskGP from botorch.fit import
+fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood train_X =
+torch.rand(10, 2) Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit
+output dimension Y += 0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std
+() gp = SingleTaskGP(train_X, train_Y) mll = ExactMarginalLogLikelihood
+(gp.likelihood, gp) fit_gpytorch_mll(mll) ``` 2. Construct an acquisition
+function ```python from botorch.acquisition import UpperConfidenceBound UCB =
+UpperConfidenceBound(gp, beta=0.1) ``` 3. Optimize the acquisition function
+```python from botorch.optim import optimize_acqf bounds = torch.stack(
+[torch.zeros(2), torch.ones(2)]) candidate, acq_value = optimize_acqf( UCB,
+bounds=bounds, q=1, num_restarts=5, raw_samples=20, ) ``` ## Citing BoTorch If
+you use BoTorch, please cite the following paper: > [M. Balandat, B. Karrer, D.
+R. Jiang, S. Daulton, B. Letham, A. G. Wilson, and E. Bakshy. BoTorch: A
+Framework for Efficient Monte-Carlo Bayesian Optimization. Advances in Neural
+Information Processing Systems 33, 2020.](https://arxiv.org/abs/1910.06403) ```
+@inproceedings{balandat2020botorch, title={{BoTorch: A Framework for Efficient
+Monte-Carlo Bayesian Optimization}}, author={Balandat, Maximilian and Karrer,
+Brian and Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson,
+Andrew Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
 Processing Systems 33}, year={2020}, url = {http://arxiv.org/abs/1910.06403} }
 ``` See [here](https://botorch.org/docs/papers) for an incomplete selection of
 peer-reviewed papers that build off of BoTorch. ## Contributing See the
 [CONTRIBUTING](CONTRIBUTING.md) file for how to help out. ## License BoTorch is
 MIT licensed, as found in the [LICENSE](LICENSE) file.
```

### Comparing `botorch-0.8.3/README.md` & `botorch-0.8.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
 
 ## Installation
 
 **Installation Requirements**
 - Python >= 3.8
 - PyTorch >= 1.12
-- gpytorch == 1.9.1
-- linear_operator == 0.3.0
+- gpytorch == 1.10
+- linear_operator == 0.4.0
 - pyro-ppl >= 1.8.4
 - scipy
 - multiple-dispatch
 
 ### Prerequisite only for MacOS users with Intel processors:
 Before installing BoTorch, we recommend first manually installing PyTorch, a required dependency of
 BoTorch. Installing it according to the [PyTorch installation instructions](https://pytorch.org/get-started/locally/)
```

#### html2text {}

```diff
@@ -34,85 +34,84 @@
 recommend using BoTorch as a low-level API for implementing new algorithms for
 [Ax](https://ax.dev). Ax has been designed to be an easy-to-use platform for
 end-users, which at the same time is flexible enough for Bayesian Optimization
 researchers to plug into for handling of feature transformations, (meta-)data
 management, storage, etc. We recommend that end-users who are not actively
 doing research on Bayesian Optimization simply use Ax. ## Installation
 **Installation Requirements** - Python >= 3.8 - PyTorch >= 1.12 - gpytorch ==
-1.9.1 - linear_operator == 0.3.0 - pyro-ppl >= 1.8.4 - scipy - multiple-
-dispatch ### Prerequisite only for MacOS users with Intel processors: Before
-installing BoTorch, we recommend first manually installing PyTorch, a required
-dependency of BoTorch. Installing it according to the [PyTorch installation
-instructions](https://pytorch.org/get-started/locally/) ensures that it is
-properly linked against MKL, a library that optimizes mathematical computation
-for Intel processors. This will result in up to an order-of-magnitude speed-up
-for Bayesian optimization, as at the moment, installing PyTorch from pip does
-not link against MKL. The PyTorch installation instructions currently
-recommend: 1. Install [Anaconda](https://www.anaconda.com/distribution/
-#download-section). Note that there are different installers for Intel and M1
-Macs. 2. Install PyTorch following the [PyTorch installation instructions]
-(https://pytorch.org/get-started/locally/). Currently, this suggests running
-`conda install pytorch torchvision -c pytorch`. If you want to customize your
-installation, please follow the [PyTorch installation instructions](https://
-pytorch.org/get-started/locally/) to build from source. ### Option 1:
-Installing the latest release The latest release of BoTorch is easily installed
-either via [Anaconda](https://www.anaconda.com/distribution/#download-section)
-(recommended) or pip. **To install BoTorch from Anaconda**, run ```bash conda
-install botorch -c pytorch -c gpytorch -c conda-forge ``` The above command
-installs BoTorch and any needed dependencies. ` -c pytorch -c gpytorch -
-c conda-forge` means that the most preferred source to install from is the
-PyTorch channel, the next most preferred is the GPyTorch channel, and the least
-preferred is conda-forge. **Alternatively, to install with `pip`**, do ```bash
-pip install botorch ``` _Note_: Make sure the `pip` being used is actually the
-one from the newly created Conda environment. If you're using a Unix-based OS,
-you can use `which pip` to check. ### Option 2: Installing from latest main
-branch If you would like to try our bleeding edge features (and don't mind
-potentially running into the occasional bug here or there), you can install the
-latest development version directly from GitHub. If you want to also install
-the current `gpytorch` and `linear_operator` development versions, you will
-need to ensure that the `ALLOW_LATEST_GPYTORCH_LINOP` environment variable is
-set: ```bash pip install --upgrade git+https://github.com/cornellius-gp/
-linear_operator.git pip install --upgrade git+https://github.com/cornellius-gp/
-gpytorch.git export ALLOW_LATEST_GPYTORCH_LINOP=true pip install --upgrade
-git+https://github.com/pytorch/botorch.git ``` ### Option 3: Editable/dev
-install If you want to [contribute](CONTRIBUTING.md) to BoTorch, you will want
-to install editably so that you can change files and have the changes reflected
-in your local install. If you want to install the current `gpytorch` and
-`linear_operator` development versions, as in Option 2, do that before
-proceeding. #### Option 3a: Bare-bones editable install ```bash git clone
-https://github.com/pytorch/botorch.git cd botorch pip install -e . ``` ####
-Option 3b: Editable install with development and tutorials dependencies ```bash
-git clone https://github.com/pytorch/botorch.git cd botorch export
-ALLOW_BOTORCH_LATEST=true pip install -e ".[dev, tutorials]" ``` * `dev`:
-Specifies tools necessary for development (testing, linting, docs building; see
-[Contributing](#contributing) below). * `tutorials`: Also installs all packages
-necessary for running the tutorial notebooks. * You can also install either the
-dev or tutorials dependencies without installing both, e.g. by changing the
-last command to `pip install -e ".[dev]"`. ## Getting Started Here's a quick
-run down of the main components of a Bayesian optimization loop. For more
-details see our [Documentation](https://botorch.org/docs/introduction) and the
-[Tutorials](https://botorch.org/tutorials). 1. Fit a Gaussian Process model to
-data ```python import torch from botorch.models import SingleTaskGP from
-botorch.fit import fit_gpytorch_mll from gpytorch.mlls import
-ExactMarginalLogLikelihood train_X = torch.rand(10, 2) Y = 1 - (train_X -
-0.5).norm(dim=-1, keepdim=True) # explicit output dimension Y += 0.1 *
-torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std() gp = SingleTaskGP
-(train_X, train_Y) mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
-fit_gpytorch_mll(mll) ``` 2. Construct an acquisition function ```python from
-botorch.acquisition import UpperConfidenceBound UCB = UpperConfidenceBound(gp,
-beta=0.1) ``` 3. Optimize the acquisition function ```python from botorch.optim
-import optimize_acqf bounds = torch.stack([torch.zeros(2), torch.ones(2)])
-candidate, acq_value = optimize_acqf( UCB, bounds=bounds, q=1, num_restarts=5,
-raw_samples=20, ) ``` ## Citing BoTorch If you use BoTorch, please cite the
-following paper: > [M. Balandat, B. Karrer, D. R. Jiang, S. Daulton, B. Letham,
-A. G. Wilson, and E. Bakshy. BoTorch: A Framework for Efficient Monte-Carlo
-Bayesian Optimization. Advances in Neural Information Processing Systems 33,
-2020.](https://arxiv.org/abs/1910.06403) ``` @inproceedings
-{balandat2020botorch, title={{BoTorch: A Framework for Efficient Monte-Carlo
-Bayesian Optimization}}, author={Balandat, Maximilian and Karrer, Brian and
-Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson, Andrew
-Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
+1.10 - linear_operator == 0.4.0 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
+### Prerequisite only for MacOS users with Intel processors: Before installing
+BoTorch, we recommend first manually installing PyTorch, a required dependency
+of BoTorch. Installing it according to the [PyTorch installation instructions]
+(https://pytorch.org/get-started/locally/) ensures that it is properly linked
+against MKL, a library that optimizes mathematical computation for Intel
+processors. This will result in up to an order-of-magnitude speed-up for
+Bayesian optimization, as at the moment, installing PyTorch from pip does not
+link against MKL. The PyTorch installation instructions currently recommend: 1.
+Install [Anaconda](https://www.anaconda.com/distribution/#download-section).
+Note that there are different installers for Intel and M1 Macs. 2. Install
+PyTorch following the [PyTorch installation instructions](https://pytorch.org/
+get-started/locally/). Currently, this suggests running `conda install pytorch
+torchvision -c pytorch`. If you want to customize your installation, please
+follow the [PyTorch installation instructions](https://pytorch.org/get-started/
+locally/) to build from source. ### Option 1: Installing the latest release The
+latest release of BoTorch is easily installed either via [Anaconda](https://
+www.anaconda.com/distribution/#download-section) (recommended) or pip. **To
+install BoTorch from Anaconda**, run ```bash conda install botorch -c pytorch -
+c gpytorch -c conda-forge ``` The above command installs BoTorch and any needed
+dependencies. ` -c pytorch -c gpytorch -c conda-forge` means that the most
+preferred source to install from is the PyTorch channel, the next most
+preferred is the GPyTorch channel, and the least preferred is conda-forge.
+**Alternatively, to install with `pip`**, do ```bash pip install botorch ```
+_Note_: Make sure the `pip` being used is actually the one from the newly
+created Conda environment. If you're using a Unix-based OS, you can use `which
+pip` to check. ### Option 2: Installing from latest main branch If you would
+like to try our bleeding edge features (and don't mind potentially running into
+the occasional bug here or there), you can install the latest development
+version directly from GitHub. If you want to also install the current
+`gpytorch` and `linear_operator` development versions, you will need to ensure
+that the `ALLOW_LATEST_GPYTORCH_LINOP` environment variable is set: ```bash pip
+install --upgrade git+https://github.com/cornellius-gp/linear_operator.git pip
+install --upgrade git+https://github.com/cornellius-gp/gpytorch.git export
+ALLOW_LATEST_GPYTORCH_LINOP=true pip install --upgrade git+https://github.com/
+pytorch/botorch.git ``` ### Option 3: Editable/dev install If you want to
+[contribute](CONTRIBUTING.md) to BoTorch, you will want to install editably so
+that you can change files and have the changes reflected in your local install.
+If you want to install the current `gpytorch` and `linear_operator` development
+versions, as in Option 2, do that before proceeding. #### Option 3a: Bare-bones
+editable install ```bash git clone https://github.com/pytorch/botorch.git cd
+botorch pip install -e . ``` #### Option 3b: Editable install with development
+and tutorials dependencies ```bash git clone https://github.com/pytorch/
+botorch.git cd botorch export ALLOW_BOTORCH_LATEST=true pip install -e ".[dev,
+tutorials]" ``` * `dev`: Specifies tools necessary for development (testing,
+linting, docs building; see [Contributing](#contributing) below). *
+`tutorials`: Also installs all packages necessary for running the tutorial
+notebooks. * You can also install either the dev or tutorials dependencies
+without installing both, e.g. by changing the last command to `pip install -
+e ".[dev]"`. ## Getting Started Here's a quick run down of the main components
+of a Bayesian optimization loop. For more details see our [Documentation]
+(https://botorch.org/docs/introduction) and the [Tutorials](https://
+botorch.org/tutorials). 1. Fit a Gaussian Process model to data ```python
+import torch from botorch.models import SingleTaskGP from botorch.fit import
+fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood train_X =
+torch.rand(10, 2) Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit
+output dimension Y += 0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std
+() gp = SingleTaskGP(train_X, train_Y) mll = ExactMarginalLogLikelihood
+(gp.likelihood, gp) fit_gpytorch_mll(mll) ``` 2. Construct an acquisition
+function ```python from botorch.acquisition import UpperConfidenceBound UCB =
+UpperConfidenceBound(gp, beta=0.1) ``` 3. Optimize the acquisition function
+```python from botorch.optim import optimize_acqf bounds = torch.stack(
+[torch.zeros(2), torch.ones(2)]) candidate, acq_value = optimize_acqf( UCB,
+bounds=bounds, q=1, num_restarts=5, raw_samples=20, ) ``` ## Citing BoTorch If
+you use BoTorch, please cite the following paper: > [M. Balandat, B. Karrer, D.
+R. Jiang, S. Daulton, B. Letham, A. G. Wilson, and E. Bakshy. BoTorch: A
+Framework for Efficient Monte-Carlo Bayesian Optimization. Advances in Neural
+Information Processing Systems 33, 2020.](https://arxiv.org/abs/1910.06403) ```
+@inproceedings{balandat2020botorch, title={{BoTorch: A Framework for Efficient
+Monte-Carlo Bayesian Optimization}}, author={Balandat, Maximilian and Karrer,
+Brian and Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson,
+Andrew Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
 Processing Systems 33}, year={2020}, url = {http://arxiv.org/abs/1910.06403} }
 ``` See [here](https://botorch.org/docs/papers) for an incomplete selection of
 peer-reviewed papers that build off of BoTorch. ## Contributing See the
 [CONTRIBUTING](CONTRIBUTING.md) file for how to help out. ## License BoTorch is
 MIT licensed, as found in the [LICENSE](LICENSE) file.
```

### Comparing `botorch-0.8.3/botorch/__init__.py` & `botorch-0.8.4/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/__init__.py` & `botorch-0.8.4/botorch/acquisition/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/acquisition.py` & `botorch-0.8.4/botorch/acquisition/acquisition.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/active_learning.py` & `botorch-0.8.4/botorch/acquisition/active_learning.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/analytic.py` & `botorch-0.8.4/botorch/acquisition/analytic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/cached_cholesky.py` & `botorch-0.8.4/botorch/acquisition/cached_cholesky.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,24 @@
         return False
     # Models that return a TransformedPosterior are not supported.
     if hasattr(model, "outcome_transform") and (not model.outcome_transform._is_linear):
         return False
     return True
 
 
+def _get_cache_root_not_supported_message(model_cls: type) -> str:
+    msg = (
+        "`cache_root` is only supported for GPyTorchModels that "
+        "are not MultiTask models and don't produce a "
+        f"TransformedPosterior. Got a model of type {model_cls}. Setting "
+        "`cache_root = False`."
+    )
+    return msg
+
+
 class CachedCholeskyMCAcquisitionFunction(ABC):
     r"""Abstract class for acquisition functions using a cached Cholesky.
 
     Specifically, this is for acquisition functions that require sampling from
     the posterior P(f(X_baseline, X) | D). The Cholesky of the posterior
     covariance over f(X_baseline) is cached.
 
@@ -68,18 +78,15 @@
         Args:
             model: A model.
             cache_root: A boolean indicating whether to cache the Cholesky.
                 This might be overridden in the model is not compatible.
         """
         if cache_root and not supports_cache_root(model):
             warnings.warn(
-                "`cache_root` is only supported for GPyTorchModels (with "
-                "the exception of MultiTask models & models producing a "
-                f"TransformedPosterior). Got model={model}. Setting "
-                "`cache_root = False",
+                _get_cache_root_not_supported_message(type(model)),
                 RuntimeWarning,
             )
             cache_root = False
         self._cache_root = cache_root
 
     def _compute_root_decomposition(
         self,
```

### Comparing `botorch-0.8.3/botorch/acquisition/cost_aware.py` & `botorch-0.8.4/botorch/acquisition/cost_aware.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/fixed_feature.py` & `botorch-0.8.4/botorch/acquisition/fixed_feature.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/input_constructors.py` & `botorch-0.8.4/botorch/acquisition/input_constructors.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     NoisyExpectedImprovement,
     PosteriorMean,
     ProbabilityOfImprovement,
     UpperConfidenceBound,
 )
 from botorch.acquisition.cost_aware import InverseCostWeightedUtility
 from botorch.acquisition.fixed_feature import FixedFeatureAcquisitionFunction
+from botorch.acquisition.joint_entropy_search import qJointEntropySearch
 from botorch.acquisition.knowledge_gradient import (
     qKnowledgeGradient,
     qMultiFidelityKnowledgeGradient,
 )
 from botorch.acquisition.max_value_entropy_search import (
     qMaxValueEntropy,
     qMultiFidelityMaxValueEntropy,
@@ -78,14 +79,15 @@
     ScalarizedObjective,
     ScalarizedPosteriorTransform,
 )
 from botorch.acquisition.preference import AnalyticExpectedUtilityOfBestOption
 from botorch.acquisition.risk_measures import RiskMeasureMCObjective
 from botorch.acquisition.utils import (
     expand_trace_observations,
+    get_optimal_samples,
     project_to_target_fidelity,
 )
 from botorch.exceptions.errors import UnsupportedError
 from botorch.models.cost import AffineFidelityCostModel
 from botorch.models.deterministic import FixedSingleSampleModel
 from botorch.models.gpytorch import GPyTorchModel
 from botorch.models.model import Model
@@ -506,15 +508,15 @@
     model: Model,
     training_data: MaybeDict[SupervisedDataset],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     X_pending: Optional[Tensor] = None,
     sampler: Optional[MCSampler] = None,
     X_baseline: Optional[Tensor] = None,
-    prune_baseline: Optional[bool] = False,
+    prune_baseline: Optional[bool] = True,
     cache_root: Optional[bool] = True,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for the `qNoisyExpectedImprovement` constructor.
 
     Args:
         model: The model to be used in the acquisition function.
@@ -1235,7 +1237,42 @@
         inequality_constraints=inequality_constraints,
         fixed_features=None,  # handled inside the acquisition function
         post_processing_func=post_processing_func,
         batch_initial_conditions=batch_initial_conditions,
         return_best_only=True,
         sequential=sequential,
     )
+
+
+@acqf_input_constructor(qJointEntropySearch)
+def construct_inputs_qJES(
+    model: Model,
+    training_data: MaybeDict[SupervisedDataset],
+    bounds: Tensor,
+    num_optima: int = 64,
+    maximize: bool = True,
+    condition_noiseless: bool = True,
+    X_pending: Optional[Tensor] = None,
+    estimation_type: str = "LB",
+    num_samples: int = 64,
+    **kwargs: Any,
+):
+    dtype = model.train_targets.dtype
+    optimal_inputs, optimal_outputs = get_optimal_samples(
+        model=model,
+        bounds=torch.as_tensor(bounds, dtype=dtype).T,
+        num_optima=num_optima,
+        maximize=maximize,
+    )
+
+    inputs = {
+        "model": model,
+        "optimal_inputs": optimal_inputs,
+        "optimal_outputs": optimal_outputs,
+        "condition_noiseless": condition_noiseless,
+        "maximize": maximize,
+        "X_pending": X_pending,
+        "estimation_type": estimation_type,
+        "num_samples": num_samples,
+        **kwargs,
+    }
+    return inputs
```

### Comparing `botorch-0.8.3/botorch/acquisition/joint_entropy_search.py` & `botorch-0.8.4/botorch/acquisition/predictive_entropy_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,104 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 r"""
-Acquisition function for joint entropy search (JES). The code utilizes the
+Acquisition function for predictive entropy search (PES). The code utilizes the
 implementation designed for the multi-objective batch setting.
 
+NOTE: The PES acquisition might not be differentiable. As a result, we recommend
+optimizing the acquisition function using finite differences.
+
 """
 
 from __future__ import annotations
 
 from typing import Any, Optional
 
-from botorch.acquisition.multi_objective.joint_entropy_search import (
-    qLowerBoundMultiObjectiveJointEntropySearch,
+from botorch.acquisition.multi_objective.predictive_entropy_search import (
+    qMultiObjectivePredictiveEntropySearch,
 )
-from botorch.acquisition.multi_objective.utils import compute_sample_box_decomposition
 from botorch.models.model import Model
 from botorch.utils.transforms import concatenate_pending_points, t_batch_mode_transform
 from torch import Tensor
 
 
-class qLowerBoundJointEntropySearch(qLowerBoundMultiObjectiveJointEntropySearch):
-    r"""The acquisition function for the Joint Entropy Search, where the batches
-    `q > 1` are supported through the lower bound formulation.
-
-    This acquisition function computes the mutual information between the observation
-    at a candidate point `X` and the optimal input-output pair.
+class qPredictiveEntropySearch(qMultiObjectivePredictiveEntropySearch):
+    r"""The acquisition function for Predictive Entropy Search.
 
-    See [Tu2022]_ for a discussion on the estimation procedure.
+    This acquisition function approximates the mutual information between the
+    observation at a candidate point `X` and the optimal set of inputs using
+    expectation propagation (EP).
 
     NOTES:
-    (i) The estimated acquisition value could be negative.
+    (i) The expectation propagation procedure can potentially fail due to the unstable
+    EP updates. This is however unlikely to happen in the single-objective setting
+    because we have much fewer EP factors. The jitter added in the training phase
+    (`ep_jitter`) and testing phase (`test_jitter`) can be increased to prevent
+    these failures from happening. More details in the description of
+    `qMultiObjectivePredictiveEntropySearch`.
 
-    (ii) The lower bound batch acquisition function might not be monotone in the
-    sense that adding more elements to the batch does not necessarily increase the
-    acquisition value. Specifically, the acquisition value can become smaller when
-    more inputs are added.
+    (ii) The estimated acquisition value could be negative.
     """
 
     def __init__(
         self,
         model: Model,
         optimal_inputs: Tensor,
-        optimal_outputs: Tensor,
         maximize: bool = True,
-        hypercell_bounds: Tensor = None,
         X_pending: Optional[Tensor] = None,
-        estimation_type: str = "LB",
-        num_samples: int = 64,
+        max_ep_iterations: int = 250,
+        ep_jitter: float = 1e-4,
+        test_jitter: float = 1e-4,
+        threshold: float = 1e-2,
         **kwargs: Any,
     ) -> None:
-        r"""Joint entropy search acquisition function.
+        r"""Predictive entropy search acquisition function.
 
         Args:
             model: A fitted single-outcome model.
             optimal_inputs: A `num_samples x d`-dim tensor containing the sampled
                 optimal inputs of dimension `d`. We assume for simplicity that each
                 sample only contains one optimal set of inputs.
-            optimal_outputs: A `num_samples x 1`-dim Tensor containing the optimal
-                set of objectives of dimension `1`.
             maximize: If true, we consider a maximization problem.
-            hypercell_bounds:  A `num_samples x 2 x J x 1`-dim Tensor containing the
-                hyper-rectangle bounds for integration, where `J` is the number of
-                hyper-rectangles. By default, the problem is assumed to be
-                unconstrained and therefore the region of integration for a sample
-                `(x*, y*)` is a `J=1` hyper-rectangle of the form  `(-infty, y^*]`
-                for a maximization problem and `[y^*, +infty)` for a minimization
-                problem. In the constrained setting, the region of integration also
-                includes the infeasible space.
             X_pending: A `m x d`-dim Tensor of `m` design points that have been
                 submitted for function evaluation, but have not yet been evaluated.
-            estimation_type: A string to determine which entropy estimate is
-                computed: "0", "LB", "LB2", or "MC". In the single-objective
-                setting, "LB" is equivalent to "LB2".
-            num_samples: The number of Monte Carlo samples used for the Monte Carlo
-                estimate.
+            max_ep_iterations: The maximum number of expectation propagation
+                iterations. (The minimum number of iterations is set at 3.)
+            ep_jitter: The amount of jitter added for the matrix inversion that
+                occurs during the expectation propagation update during the training
+                phase.
+            test_jitter: The amount of jitter added for the matrix inversion that
+                occurs during the expectation propagation update in the testing
+                phase.
+            threshold: The convergence threshold for expectation propagation. This
+                assesses the relative change in the mean and covariance. We default
+                to one percent change i.e. `threshold = 1e-2`.
         """
-        if hypercell_bounds is None:
-            hypercell_bounds = compute_sample_box_decomposition(
-                pareto_fronts=optimal_outputs.unsqueeze(-2), maximize=maximize
-            )
-
         super().__init__(
             model=model,
             pareto_sets=optimal_inputs.unsqueeze(-2),
-            pareto_fronts=optimal_outputs.unsqueeze(-2),
-            hypercell_bounds=hypercell_bounds,
+            maximize=maximize,
             X_pending=X_pending,
-            estimation_type=estimation_type,
-            num_samples=num_samples,
+            max_ep_iterations=max_ep_iterations,
+            ep_jitter=ep_jitter,
+            test_jitter=test_jitter,
+            threshold=threshold,
         )
 
     @concatenate_pending_points
     @t_batch_mode_transform()
     def forward(self, X: Tensor) -> Tensor:
-        r"""Evaluates qLowerBoundJointEntropySearch at the design points `X`.
+        r"""Evaluate qPredictiveEntropySearch on the candidate set `X`.
 
         Args:
-            X: A `batch_shape x q x d`-dim Tensor of `batch_shape` t-batches with `q`
-            `d`-dim design points each.
+            X: A `batch_shape x q x d`-dim Tensor of t-batches with `q` `d`-dim
+                design points each.
 
         Returns:
-            A `batch_shape`-dim Tensor of acquisition values at the given design
-            points `X`.
+            A `batch_shape'`-dim Tensor of Predictive Entropy Search values at the
+            given design points `X`.
         """
-
-        return self._compute_lower_bound_information_gain(X)
+        return self._compute_information_gain(X)
```

### Comparing `botorch-0.8.3/botorch/acquisition/knowledge_gradient.py` & `botorch-0.8.4/botorch/acquisition/knowledge_gradient.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/max_value_entropy_search.py` & `botorch-0.8.4/botorch/acquisition/max_value_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/monte_carlo.py` & `botorch-0.8.4/botorch/acquisition/monte_carlo.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         self,
         model: Model,
         X_baseline: Tensor,
         sampler: Optional[MCSampler] = None,
         objective: Optional[MCAcquisitionObjective] = None,
         posterior_transform: Optional[PosteriorTransform] = None,
         X_pending: Optional[Tensor] = None,
-        prune_baseline: bool = False,
+        prune_baseline: bool = True,
         cache_root: bool = True,
         **kwargs: Any,
     ) -> None:
         r"""q-Noisy Expected Improvement.
 
         Args:
             model: A fitted model.
```

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/__init__.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/analytic.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/analytic.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,49 +21,54 @@
 
 from abc import abstractmethod
 from itertools import product
 from typing import List, Optional
 
 import torch
 from botorch.acquisition.acquisition import AcquisitionFunction
-from botorch.acquisition.multi_objective.objective import (
-    AnalyticMultiOutputObjective,
-    IdentityAnalyticMultiOutputObjective,
-)
+from botorch.acquisition.objective import PosteriorTransform
 from botorch.exceptions.errors import UnsupportedError
 from botorch.models.model import Model
 from botorch.utils.multi_objective.box_decompositions.non_dominated import (
     NondominatedPartitioning,
 )
 from botorch.utils.transforms import t_batch_mode_transform
 from torch import Tensor
 from torch.distributions import Normal
 
 
 class MultiObjectiveAnalyticAcquisitionFunction(AcquisitionFunction):
     r"""Abstract base class for Multi-Objective batch acquisition functions."""
 
     def __init__(
-        self, model: Model, objective: Optional[AnalyticMultiOutputObjective] = None
+        self,
+        model: Model,
+        posterior_transform: Optional[PosteriorTransform] = None,
+        **kwargs,
     ) -> None:
         r"""Constructor for the MultiObjectiveAnalyticAcquisitionFunction base class.
 
         Args:
             model: A fitted model.
-            objective: An AnalyticMultiOutputObjective (optional).
+            posterior_transform: A PosteriorTransform (optional).
         """
         super().__init__(model=model)
-        if objective is None:
-            objective = IdentityAnalyticMultiOutputObjective()
-        elif not isinstance(objective, AnalyticMultiOutputObjective):
+        posterior_transform = self._deprecate_acqf_objective(
+            posterior_transform=posterior_transform,
+            objective=kwargs.get("objective"),
+        )
+        if posterior_transform is None or isinstance(
+            posterior_transform, PosteriorTransform
+        ):
+            self.posterior_transform = posterior_transform
+        else:
             raise UnsupportedError(
-                "Only objectives of type AnalyticMultiOutputObjective are supported "
-                "for Multi-Objective analytic acquisition functions."
+                "Only a posterior_transform of type PosteriorTransform is "
+                "supported for Multi-Objective analytic acquisition functions."
             )
-        self.objective = objective
 
     @abstractmethod
     def forward(self, X: Tensor) -> Tensor:
         r"""Takes in a `batch_shape x 1 x d` X Tensor of t-batches with `1` `d`-dim
         design point each, and returns a Tensor with shape `batch_shape'`, where
         `batch_shape'` is the broadcasted batch shape of model and input `X`.
         """
@@ -77,15 +82,16 @@
 
 class ExpectedHypervolumeImprovement(MultiObjectiveAnalyticAcquisitionFunction):
     def __init__(
         self,
         model: Model,
         ref_point: List[float],
         partitioning: NondominatedPartitioning,
-        objective: Optional[AnalyticMultiOutputObjective] = None,
+        posterior_transform: Optional[PosteriorTransform] = None,
+        **kwargs,
     ) -> None:
         r"""Expected Hypervolume Improvement supporting m>=2 outcomes.
 
         This implements the computes EHVI using the algorithm from [Yang2019]_, but
         additionally computes gradients via auto-differentiation as proposed by
         [Daulton2020qehvi]_.
 
@@ -114,15 +120,15 @@
             ref_point: A list with `m` elements representing the reference point (in the
                 outcome space) w.r.t. to which compute the hypervolume. This is a
                 reference point for the objective values (i.e. after applying
                 `objective` to the samples).
             partitioning: A `NondominatedPartitioning` module that provides the non-
                 dominated front and a partitioning of the non-dominated space in hyper-
                 rectangles.
-            objective: An `AnalyticMultiOutputObjective`.
+            posterior_transform: A `PosteriorTransform`.
         """
         # TODO: we could refactor this __init__ logic into a
         # HypervolumeAcquisitionFunction Mixin
         if len(ref_point) != partitioning.num_outcomes:
             raise ValueError(
                 "The length of the reference point must match the number of outcomes. "
                 f"Got ref_point with {len(ref_point)} elements, but expected "
@@ -134,15 +140,15 @@
             device=partitioning.pareto_Y.device,
         )
         better_than_ref = (partitioning.pareto_Y > ref_point).all(dim=1)
         if not better_than_ref.any() and partitioning.pareto_Y.shape[0] > 0:
             raise ValueError(
                 "At least one pareto point must be better than the reference point."
             )
-        super().__init__(model=model, objective=objective)
+        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
         self.register_buffer("ref_point", ref_point)
         self.partitioning = partitioning
         cell_bounds = self.partitioning.get_hypercell_bounds()
         self.register_buffer("cell_lower_bounds", cell_bounds[0])
         self.register_buffer("cell_upper_bounds", cell_bounds[1])
         # create indexing tensor of shape `2^m x m`
         self._cross_product_indices = torch.tensor(
@@ -199,15 +205,17 @@
         Returns:
             A `batch_shape x num_cells x m`-dim tensor of values.
         """
         return (upper - lower) * (1 - self.normal.cdf((upper - mu) / sigma))
 
     @t_batch_mode_transform()
     def forward(self, X: Tensor) -> Tensor:
-        posterior = self.objective(self.model.posterior(X))
+        posterior = self.model.posterior(
+            X, posterior_transform=self.posterior_transform
+        )
         mu = posterior.mean
         sigma = posterior.variance.clamp_min(1e-9).sqrt()
         # clamp here, since upper_bounds will contain `inf`s, which
         # are not differentiable
         cell_upper_bounds = self.cell_upper_bounds.clamp_max(
             1e10 if X.dtype == torch.double else 1e8
         )
```

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/joint_entropy_search.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/joint_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/max_value_entropy_search.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/max_value_entropy_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,17 @@
             model_list_to_batched(model) if isinstance(model, ModelListGP) else model
         )
         self._init_model = batched_mo_model
         self.mo_model = batched_mo_model
         self.model = batched_multi_output_to_single_output(
             batch_mo_model=batched_mo_model
         )
-        self.fantasies_sampler = SobolQMCNormalSampler(num_fantasies)
+        self.fantasies_sampler = SobolQMCNormalSampler(
+            sample_shape=torch.Size([num_fantasies])
+        )
         self.num_fantasies = num_fantasies
         # weight is used in _compute_information_gain
         self.maximize = True
         self.weight = 1.0
         self.sample_pareto_frontiers = sample_pareto_frontiers
 
         # this avoids unnecessary model conversion if X_pending is None
```

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/monte_carlo.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/multi_fidelity.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/multi_output_risk_measures.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/multi_output_risk_measures.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,15 +435,17 @@
                 ],
                 dim=-1,
             )
         else:
             y_grid = torch.stack(
                 [
                     torch.stack(
-                        torch.meshgrid([Y_sorted[b, :, i] for i in range(m)]),
+                        torch.meshgrid(
+                            [Y_sorted[b, :, i] for i in range(m)], indexing=None
+                        ),
                         dim=-1,
                     ).view(-1, m)
                     for b in range(batch)
                 ],
                 dim=0,
             )
         # Get the non-normalized CDF.
```

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/objective.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/objective.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
+import warnings
+
 from abc import abstractmethod
 from typing import List, Optional
 
 import torch
 from botorch.acquisition.objective import (
     AcquisitionObjective,
     GenericMCObjective,
     MCAcquisitionObjective,
+    UnstandardizePosteriorTransform,
 )
 from botorch.exceptions.errors import BotorchError, BotorchTensorDimensionError
 from botorch.models.model import Model
-from botorch.models.transforms.outcome import Standardize
 from botorch.posteriors import GPyTorchPosterior
 from botorch.utils import apply_constraints
 from botorch.utils.transforms import normalize_indices
 from torch import Tensor
 
 
 class MCMultiOutputObjective(MCAcquisitionObjective):
@@ -257,61 +259,53 @@
 
     def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
         samples = super().forward(samples=samples)
         return samples * self.Y_std + self.Y_mean
 
 
 class AnalyticMultiOutputObjective(AcquisitionObjective):
-    r"""Abstract base class for multi-output analyic objectives."""
-    # TODO: Refactor these as PosteriorTransform as well.
-
-    @abstractmethod
-    def forward(self, posterior: GPyTorchPosterior) -> GPyTorchPosterior:
-        r"""Transform the posterior
+    r"""Abstract base class for multi-output analyic objectives.
 
-        Args:
-            posterior: A posterior.
+    DEPRECATED - This will be removed in the next version.
 
-        Returns:
-            A transformed posterior.
-        """
-        pass  # pragma: no cover
+    """
+    pass  # pragma: no cover
 
 
 class IdentityAnalyticMultiOutputObjective(AnalyticMultiOutputObjective):
+    """DEPRECATED - This will be removed in the next version."""
+
+    def __init__(self):
+        """Initialize objective."""
+        warnings.warn(
+            "IdentityAnalyticMultiOutputObjective is deprecated. "
+            "Use IdentityPosteriorTransform instead.",
+            DeprecationWarning,
+        )
+        super().__init__()
+
     def forward(self, posterior: GPyTorchPosterior) -> GPyTorchPosterior:
         return posterior
 
 
-class UnstandardizeAnalyticMultiOutputObjective(AnalyticMultiOutputObjective):
+class UnstandardizeAnalyticMultiOutputObjective(
+    UnstandardizePosteriorTransform, AnalyticMultiOutputObjective
+):
     r"""Objective that unstandardizes the posterior.
 
-    TODO: remove this when MultiTask models support outcome transforms.
-
-    Example:
-        >>> unstd_objective = UnstandardizeAnalyticMultiOutputObjective(Y_mean, Y_std)
-        >>> unstd_posterior = unstd_objective(posterior)
+    DEPRECATED - This will be removed in the next version.
     """
 
     def __init__(self, Y_mean: Tensor, Y_std: Tensor) -> None:
         r"""Initialize objective.
 
         Args:
             Y_mean: `m`-dim tensor of outcome means
             Y_std: `m`-dim tensor of outcome standard deviations
 
         """
-        if Y_mean.ndim > 1 or Y_std.ndim > 1:
-            raise BotorchTensorDimensionError(
-                "Y_mean and Y_std must both be 1-dimensional, but got "
-                f"{Y_mean.ndim} and {Y_std.ndim}"
-            )
-        super().__init__()
-        self.outcome_transform = Standardize(m=Y_mean.shape[0]).to(Y_mean)
-        Y_std_unsqueezed = Y_std.unsqueeze(0)
-        self.outcome_transform.means = Y_mean.unsqueeze(0)
-        self.outcome_transform.stdvs = Y_std_unsqueezed
-        self.outcome_transform._stdvs_sq = Y_std_unsqueezed.pow(2)
-        self.outcome_transform.eval()
-
-    def forward(self, posterior: GPyTorchPosterior) -> Tensor:
-        return self.outcome_transform.untransform_posterior(posterior)
+        warnings.warn(
+            "UnstandardizeAnalyticMultiOutputObjective is deprecated. "
+            "Use UnstandardizePosteriorTransform instead.",
+            DeprecationWarning,
+        )
+        super().__init__(Y_mean=Y_mean, Y_std=Y_std)
```

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/predictive_entropy_search.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/predictive_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/multi_objective/utils.py` & `botorch-0.8.4/botorch/acquisition/multi_objective/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/multi_step_lookahead.py` & `botorch-0.8.4/botorch/acquisition/multi_step_lookahead.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/objective.py` & `botorch-0.8.4/botorch/acquisition/objective.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 import inspect
 import warnings
 from abc import ABC, abstractmethod
 from typing import Callable, List, Optional, TYPE_CHECKING, Union
 
 import torch
-from botorch.exceptions.errors import UnsupportedError
+from botorch.exceptions.errors import BotorchTensorDimensionError, UnsupportedError
 from botorch.models.model import Model
+from botorch.models.transforms.outcome import Standardize
 from botorch.posteriors.gpytorch import GPyTorchPosterior, scalarize_posterior
 from botorch.sampling import IIDNormalSampler, MCSampler
 from botorch.utils import apply_constraints
 from gpytorch.distributions import MultitaskMultivariateNormal, MultivariateNormal
 from linear_operator.operators.dense_linear_operator import to_linear_operator
 from torch import Tensor
 from torch.nn import Module
@@ -254,14 +255,52 @@
             # Using MTMVN since we pass a single loc and covar for all `m` outputs.
             new_mvn = MultitaskMultivariateNormal(
                 new_loc, to_linear_operator(new_cov), interleaved=False
             )
         return GPyTorchPosterior(distribution=new_mvn)
 
 
+class UnstandardizePosteriorTransform(PosteriorTransform):
+    r"""Posterior transform that unstandardizes the posterior.
+
+    TODO: remove this when MultiTask models support outcome transforms.
+
+    Example:
+        >>> unstd_transform = UnstandardizePosteriorTransform(Y_mean, Y_std)
+        >>> unstd_posterior = unstd_transform(posterior)
+    """
+
+    def __init__(self, Y_mean: Tensor, Y_std: Tensor) -> None:
+        r"""Initialize objective.
+
+        Args:
+            Y_mean: `m`-dim tensor of outcome means
+            Y_std: `m`-dim tensor of outcome standard deviations
+
+        """
+        if Y_mean.ndim > 1 or Y_std.ndim > 1:
+            raise BotorchTensorDimensionError(
+                "Y_mean and Y_std must both be 1-dimensional, but got "
+                f"{Y_mean.ndim} and {Y_std.ndim}"
+            )
+        super().__init__()
+        self.outcome_transform = Standardize(m=Y_mean.shape[0]).to(Y_mean)
+        Y_std_unsqueezed = Y_std.unsqueeze(0)
+        self.outcome_transform.means = Y_mean.unsqueeze(0)
+        self.outcome_transform.stdvs = Y_std_unsqueezed
+        self.outcome_transform._stdvs_sq = Y_std_unsqueezed.pow(2)
+        self.outcome_transform.eval()
+
+    def evaluate(self, Y: Tensor) -> Tensor:
+        return self.outcome_transform.untransform(Y)[0]
+
+    def forward(self, posterior: GPyTorchPosterior) -> Tensor:
+        return self.outcome_transform.untransform_posterior(posterior)
+
+
 class MCAcquisitionObjective(Module, ABC):
     r"""Abstract base class for MC-based objectives.
 
     Args:
         _verify_output_shape: If True and `X` is given, check that the q-batch
             shape of the objectives agrees with that of X.
         _is_mo: A boolean denoting whether the objectives are multi-output.
```

### Comparing `botorch-0.8.3/botorch/acquisition/penalized.py` & `botorch-0.8.4/botorch/acquisition/penalized.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/preference.py` & `botorch-0.8.4/botorch/acquisition/preference.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/proximal.py` & `botorch-0.8.4/botorch/acquisition/proximal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/risk_measures.py` & `botorch-0.8.4/botorch/acquisition/risk_measures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/acquisition/utils.py` & `botorch-0.8.4/botorch/acquisition/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 r"""
 Utilities for acquisition functions.
 """
 
 from __future__ import annotations
 
 import math
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 from botorch.acquisition import analytic, monte_carlo, multi_objective  # noqa F401
 from botorch.acquisition.acquisition import AcquisitionFunction
 from botorch.acquisition.multi_objective import monte_carlo as moo_monte_carlo
 from botorch.acquisition.objective import (
     IdentityMCObjective,
@@ -23,18 +23,20 @@
     PosteriorTransform,
 )
 from botorch.exceptions.errors import UnsupportedError
 from botorch.models.fully_bayesian import MCMC_DIM
 from botorch.models.model import Model
 from botorch.sampling.base import MCSampler
 from botorch.sampling.get_sampler import get_sampler
+from botorch.sampling.pathwise import draw_matheron_paths
 from botorch.utils.multi_objective.box_decompositions.non_dominated import (
     FastNondominatedPartitioning,
     NondominatedPartitioning,
 )
+from botorch.utils.sampling import optimize_posterior_samples
 from botorch.utils.transforms import is_fully_bayesian
 from torch import Tensor
 
 
 def get_acquisition_function(
     acquisition_function_name: str,
     model: Model,
@@ -125,15 +127,15 @@
         return monte_carlo.qNoisyExpectedImprovement(
             model=model,
             X_baseline=X_observed,
             sampler=sampler,
             objective=objective,
             posterior_transform=posterior_transform,
             X_pending=X_pending,
-            prune_baseline=kwargs.get("prune_baseline", False),
+            prune_baseline=kwargs.get("prune_baseline", True),
             marginalize_dim=kwargs.get("marginalize_dim"),
             cache_root=kwargs.get("cache_root", True),
         )
     elif acquisition_function_name == "qSR":
         return monte_carlo.qSimpleRegret(
             model=model,
             sampler=sampler,
@@ -469,7 +471,43 @@
         A `batch_shape x p x d` Tensor where the q-batch includes the `p` sample points.
     """
     batch_shape = X.shape[:-2]
     p, d_prime = sample_points.shape
     X_new = X.repeat(*(1 for _ in batch_shape), p, 1)  # batch_shape x p x d
     X_new[..., -d_prime:] = sample_points
     return X_new
+
+
+def get_optimal_samples(
+    model: Model,
+    bounds: Tensor,
+    num_optima: int,
+    raw_samples: int = 1024,
+    num_restarts: int = 20,
+    maximize: bool = True,
+) -> Tuple[Tensor, Tensor]:
+    """Draws sample paths from the posterior and maximizes the samples using GD.
+
+    Args:
+        model (Model): The model from which samples are drawn.
+        bounds: (Tensor): Bounds of the search space. If the model inputs are
+            normalized, the bounds should be normalized as well.
+        num_optima (int): The number of paths to be drawn and optimized.
+        raw_samples (int, optional): The number of candidates randomly sample.
+            Defaults to 1024.
+        num_restarts (int, optional): The number of candidates to do gradient-based
+            optimization on. Defaults to 20.
+        maximize: Whether to maximize or minimize the samples.
+    Returns:
+        Tuple[Tensor, Tensor]: The optimal input locations and corresponding
+        outputs, x* and f*.
+
+    """
+    paths = draw_matheron_paths(model, sample_shape=torch.Size([num_optima]))
+    optimal_inputs, optimal_outputs = optimize_posterior_samples(
+        paths,
+        bounds=bounds,
+        raw_samples=raw_samples,
+        num_restarts=num_restarts,
+        maximize=maximize,
+    )
+    return optimal_inputs, optimal_outputs
```

### Comparing `botorch-0.8.3/botorch/cross_validation.py` & `botorch-0.8.4/botorch/cross_validation.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/exceptions/__init__.py` & `botorch-0.8.4/botorch/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/exceptions/errors.py` & `botorch-0.8.4/botorch/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/exceptions/warnings.py` & `botorch-0.8.4/botorch/exceptions/warnings.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/fit.py` & `botorch-0.8.4/botorch/fit.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/generation/__init__.py` & `botorch-0.8.4/botorch/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/generation/gen.py` & `botorch-0.8.4/botorch/generation/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     make_scipy_linear_constraints,
     make_scipy_nonlinear_inequality_constraints,
     NLC_TOL,
 )
 from botorch.optim.stopping import ExpMAStoppingCriterion
 from botorch.optim.utils import _filter_kwargs, columnwise_clamp, fix_features
 from botorch.optim.utils.timeout import minimize_with_timeout
-from scipy.optimize.optimize import OptimizeResult
+from scipy.optimize import OptimizeResult
 from torch import Tensor
 from torch.optim import Optimizer
 
 logger = _get_logger()
 
 TGenCandidates = Callable[[Tensor, AcquisitionFunction, Any], Tuple[Tensor, Tensor]]
```

### Comparing `botorch-0.8.3/botorch/generation/sampling.py` & `botorch-0.8.4/botorch/generation/sampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/generation/utils.py` & `botorch-0.8.4/botorch/generation/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/logging.py` & `botorch-0.8.4/botorch/logging.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/__init__.py` & `botorch-0.8.4/botorch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/approximate_gp.py` & `botorch-0.8.4/botorch/models/approximate_gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,14 +422,25 @@
         # TODO: make this a flag?
         self.model.train_inputs = [transformed_X]
         if train_Y is not None:
             self.model.train_targets = train_Y.squeeze(-1)
 
         self.to(train_X)
 
+    @property
+    def batch_shape(self) -> torch.Size:
+        r"""The batch shape of the model.
+
+        This is a batch shape from an I/O perspective. For a model with `m`
+        outputs, a `test_batch_shape x q x d`-shaped input `X` to the `posterior`
+        method returns a Posterior object over an output of shape
+        `broadcast(test_batch_shape, model.batch_shape) x q x m`.
+        """
+        return self._input_batch_shape
+
     def init_inducing_points(
         self,
         inputs: Tensor,
     ) -> Tensor:
         r"""
         Reinitialize the inducing point locations in-place with the current kernel
         applied to `inputs` through the model's inducing point allocation strategy.
```

### Comparing `botorch-0.8.3/botorch/models/contextual.py` & `botorch-0.8.4/botorch/models/contextual.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/contextual_multioutput.py` & `botorch-0.8.4/botorch/models/contextual_multioutput.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/converter.py` & `botorch-0.8.4/botorch/models/converter.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/cost.py` & `botorch-0.8.4/botorch/models/cost.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/deterministic.py` & `botorch-0.8.4/botorch/models/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/ensemble.py` & `botorch-0.8.4/botorch/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/fully_bayesian.py` & `botorch-0.8.4/botorch/models/fully_bayesian.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import math
 from abc import abstractmethod
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
 import pyro
 import torch
 from botorch.acquisition.objective import PosteriorTransform
+from botorch.models.gp_regression import MIN_INFERRED_NOISE_LEVEL
 from botorch.models.gpytorch import BatchedMultiOutputGPyTorchModel
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
 from botorch.models.utils import validate_input_scaling
 from botorch.posteriors.fully_bayesian import FullyBayesianPosterior, MCMC_DIM
 from gpytorch.constraints import GreaterThan
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
@@ -54,15 +55,14 @@
 from gpytorch.likelihoods.likelihood import Likelihood
 from gpytorch.means.constant_mean import ConstantMean
 from gpytorch.means.mean import Mean
 from gpytorch.models.exact_gp import ExactGP
 from pyro.ops.integrator import register_exception_handler
 from torch import Tensor
 
-MIN_INFERRED_NOISE_LEVEL = 1e-6
 
 _sqrt5 = math.sqrt(5)
 
 
 def _handle_torch_linalg(exception: Exception) -> bool:
     return type(exception) == torch.linalg.LinAlgError
```

### Comparing `botorch-0.8.3/botorch/models/fully_bayesian_multitask.py` & `botorch-0.8.4/botorch/models/fully_bayesian_multitask.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/gp_regression.py` & `botorch-0.8.4/botorch/models/gp_regression.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/gp_regression_fidelity.py` & `botorch-0.8.4/botorch/models/gp_regression_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/gp_regression_mixed.py` & `botorch-0.8.4/botorch/models/gp_regression_mixed.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/gpytorch.py` & `botorch-0.8.4/botorch/models/gpytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,24 @@
 
 if TYPE_CHECKING:
     from botorch.posteriors.posterior_list import PosteriorList  # pragma: no cover
     from botorch.posteriors.transformed import TransformedPosterior  # pragma: no cover
     from gpytorch.likelihoods import Likelihood  # pragma: no cover
 
 
+def _get_single_precision_warning(dtype: torch.dtype) -> str:
+    msg = (
+        f"The model inputs are of type {dtype}. It is strongly recommended "
+        "to use double precision in BoTorch, as this improves both "
+        "precision and stability and can help avoid numerical errors. "
+        "See https://github.com/pytorch/botorch/discussions/1444"
+    )
+    return msg
+
+
 class GPyTorchModel(Model, ABC):
     r"""Abstract base class for models based on GPyTorch models.
 
     The easiest way to use this is to subclass a model from a GPyTorch model
     class (e.g. an `ExactGP`) and this `GPyTorchModel`. See e.g. `SingleTaskGP`.
 
     :meta private:
@@ -74,35 +84,35 @@
                 `batch_shape'` is the batch shape of the observations.
             Yvar: A `batch_shape' x n x m` tensor of observed measurement noise.
                 Note: this will be None when using a model that infers the noise
                 level (e.g. a `SingleTaskGP`).
             strict: A boolean indicating whether to check that `Y` and `Yvar`
                 have an explicit output dimension.
         """
-        if strict:
-            if X.dim() != Y.dim():
-                if (X.dim() - Y.dim() == 1) and (X.shape[:-1] == Y.shape):
-                    message = (
-                        "An explicit output dimension is required for targets."
-                        f" Expected Y with dimension: {Y.dim()} (got {X.dim()})."
-                    )
-                else:
-                    message = (
-                        "Expected X and Y to have the same number of dimensions"
-                        f" (got X with dimension {X.dim()} and Y with dimension"
-                        f" {Y.dim()}."
-                    )
+        if X.dim() != Y.dim():
+            if (X.dim() - Y.dim() == 1) and (X.shape[:-1] == Y.shape):
+                message = (
+                    "An explicit output dimension is required for targets."
+                    f" Expected Y with dimension {X.dim()} (got {Y.dim()=})."
+                )
+            else:
+                message = (
+                    "Expected X and Y to have the same number of dimensions"
+                    f" (got X with dimension {X.dim()} and Y with dimension"
+                    f" {Y.dim()})."
+                )
+            if strict:
                 raise BotorchTensorDimensionError(message)
-        else:
-            warnings.warn(
-                "Non-strict enforcement of botorch tensor conventions. Ensure that "
-                f"target tensors Y{' and Yvar have' if Yvar is not None else ' has an'}"
-                f" explicit output dimension{'s' if Yvar is not None else ''}.",
-                BotorchTensorDimensionWarning,
-            )
+            else:
+                warnings.warn(
+                    "Non-strict enforcement of botorch tensor conventions. The "
+                    "following error would have been raised with strict enforcement: "
+                    f"{message}",
+                    BotorchTensorDimensionWarning,
+                )
         # Yvar may not have the same batch dimensions, but the trailing dimensions
         # of Yvar should be the same as the trailing dimensions of Y.
         if Yvar is not None and Y.shape[-(Yvar.dim()) :] != Yvar.shape:
             raise BotorchTensorDimensionError(
                 "An explicit output dimension is required for observation noise."
                 f" Expected Yvar with shape: {Y.shape[-Yvar.dim() :]} (got"
                 f" {Yvar.shape})."
@@ -112,21 +122,15 @@
             raise InputDataError(
                 "Expected all inputs to share the same dtype. Got "
                 f"{X.dtype} for X, {Y.dtype} for Y, and "
                 f"{Yvar.dtype if Yvar is not None else None} for Yvar."
             )
         if X.dtype != torch.float64:
             # NOTE: Not using a BotorchWarning since those get ignored.
-            warnings.warn(
-                f"The model inputs are of type {X.dtype}. It is strongly recommended "
-                "to use double precision in BoTorch, as this improves both "
-                "precision and stability and can help avoid numerical errors. "
-                "See https://github.com/pytorch/botorch/discussions/1444",
-                UserWarning,
-            )
+            warnings.warn(_get_single_precision_warning(X.dtype), UserWarning)
 
     @property
     def batch_shape(self) -> torch.Size:
         r"""The batch shape of the model.
 
         This is a batch shape from an I/O perspective, independent of the internal
         representation of the model (as e.g. in BatchedMultiOutputGPyTorchModel).
```

### Comparing `botorch-0.8.3/botorch/models/higher_order_gp.py` & `botorch-0.8.4/botorch/models/higher_order_gp.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,15 +483,15 @@
                 )
             else:
                 train_inputs = self.train_inputs[0]
 
             # we now compute the data covariances for the training data, the testing
             # data, the joint covariances, and the test train cross-covariance
             train_train_covar = self.prediction_strategy.lik_train_train_covar.detach()
-            base_train_train_covar = train_train_covar.lazy_tensor
+            base_train_train_covar = train_train_covar.linear_op
 
             data_train_covar = base_train_train_covar.linear_ops[0]
             data_covar = self.covar_modules[0]
             data_train_test_covar = data_covar(X, train_inputs)
             data_test_test_covar = data_covar(X)
             data_joint_covar = data_train_covar.cat_rows(
                 cross_mat=data_train_test_covar,
@@ -567,15 +567,15 @@
             train_train_covar, *jcm_linops
         )
         full_test_test_covar = KroneckerProductLinearOperator(
             test_test_covar, *jcm_linops
         )
         full_test_train_covar_tuple = (test_train_covar,) + jcm_linops
 
-        train_evals, train_evecs = full_train_train_covar.symeig(eigenvectors=True)
+        train_evals, train_evecs = full_train_train_covar.eigh()
         # (\kron \Lambda_i + \sigma^2 I)^{-1}
         train_inv_evals = DiagLinearOperator(
             1.0 / (train_evals + self.likelihood.noise)
         )
 
         # compute K_i S_i \hadamard K_i S_i
         test_train_hadamard = KroneckerProductLinearOperator(
@@ -585,9 +585,9 @@
             ]
         )
 
         # and compute the column sums of
         #  (\kron K_i S_i * K_i S_i) \tilde{\Lambda}^{-1}
         test_train_pred_covar = test_train_hadamard.matmul(train_inv_evals).sum(dim=-1)
 
-        pred_variances = full_test_test_covar.diag() - test_train_pred_covar
+        pred_variances = full_test_test_covar.diagonal() - test_train_pred_covar
         return pred_variances
```

### Comparing `botorch-0.8.3/botorch/models/kernels/__init__.py` & `botorch-0.8.4/botorch/models/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/kernels/categorical.py` & `botorch-0.8.4/botorch/models/kernels/categorical.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/kernels/contextual_lcea.py` & `botorch-0.8.4/botorch/models/kernels/contextual_lcea.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/kernels/contextual_sac.py` & `botorch-0.8.4/botorch/models/kernels/contextual_sac.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/kernels/downsampling.py` & `botorch-0.8.4/botorch/models/kernels/downsampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/kernels/exponential_decay.py` & `botorch-0.8.4/botorch/models/kernels/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/kernels/linear_truncated_fidelity.py` & `botorch-0.8.4/botorch/models/kernels/linear_truncated_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/likelihoods/pairwise.py` & `botorch-0.8.4/botorch/models/likelihoods/pairwise.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/model.py` & `botorch-0.8.4/botorch/models/model.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/model_list_gp_regression.py` & `botorch-0.8.4/botorch/models/model_list_gp_regression.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/multitask.py` & `botorch-0.8.4/botorch/models/multitask.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,25 +241,28 @@
         return all_tasks, task_feature, d
 
     @classmethod
     def construct_inputs(
         cls,
         training_data: Dict[str, SupervisedDataset],
         task_feature: int,
+        output_tasks: Optional[List[int]] = None,
         task_covar_prior: Optional[Prior] = None,
         prior_config: Optional[dict] = None,
         rank: Optional[int] = None,
         **kwargs,
     ) -> Dict[str, Any]:
         r"""Construct `Model` keyword arguments from dictionary of `SupervisedDataset`.
 
         Args:
             training_data: Dictionary of `SupervisedDataset`.
             task_feature: Column index of embedded task indicator features. For details,
                 see `parse_training_data`.
+            output_tasks: A list of task indices for which to compute model
+                outputs for. If omitted, return outputs for all task indices.
             task_covar_prior: A GPyTorch `Prior` object to use as prior on
                 the cross-task covariance matrix,
             prior_config: Configuration for inter-task covariance prior.
                 Should only be used if `task_covar_prior` is not passed directly. Must
                 contain `use_LKJ_prior` indicator and should contain float value `eta`.
             rank: The rank of the cross-task covariance matrix.
         """
@@ -282,14 +285,15 @@
 
         base_inputs = super().construct_inputs(
             training_data=training_data, task_feature=task_feature, **kwargs
         )
         return {
             **base_inputs,
             "task_feature": task_feature,
+            "output_tasks": output_tasks,
             "task_covar_prior": task_covar_prior,
             "rank": rank,
         }
 
 
 class FixedNoiseMultiTaskGP(MultiTaskGP):
     r"""Multi-Task GP model using an ICM kernel, with known observation noise.
@@ -541,15 +545,15 @@
     def predictive_mean_cache(self):
         train_x = self.transform_inputs(self.train_inputs[0])
         train_noise = self.likelihood._shaped_noise_covar(train_x.shape)
         if detach_test_caches.on():
             train_noise = train_noise.detach()
 
         train_diff = self.train_targets - self.mean_module(train_x)
-        train_solve = (self.train_full_covar + train_noise).inv_matmul(
+        train_solve = (self.train_full_covar + train_noise).solve(
             train_diff.reshape(*train_diff.shape[:-2], -1)
         )
         if detach_test_caches.on():
             train_solve = train_solve.detach()
 
         return train_solve
 
@@ -665,15 +669,15 @@
         pred_mean = (
             test_obs_kernel.matmul(self.predictive_mean_cache).reshape_as(test_mean)
             + test_mean
         )
         # next the predictive variance, assume diagonal noise
         test_var_term = KroneckerProductLinearOperator(
             test_test_covar, task_covar
-        ).diag()
+        ).diagonal()
 
         if diagonal_noise:
             task_evals, task_evecs = self._task_covar_matrix.diagonalization()
             # TODO: make this be the default KPMatmulLT diagonal method in gpytorch
             full_data_inv_evals = (
                 KroneckerProductDiagLinearOperator(
                     DiagLinearOperator(data_data_evals), DiagLinearOperator(task_evals)
```

### Comparing `botorch-0.8.3/botorch/models/pairwise_gp.py` & `botorch-0.8.4/botorch/models/pairwise_gp.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,33 +30,97 @@
 from botorch.exceptions import UnsupportedError
 from botorch.models.likelihoods.pairwise import (
     PairwiseLikelihood,
     PairwiseProbitLikelihood,
 )
 from botorch.models.model import FantasizeMixin, Model
 from botorch.models.transforms.input import InputTransform
+from botorch.models.utils.assorted import consolidate_duplicates
 from botorch.posteriors.gpytorch import GPyTorchPosterior
 from botorch.posteriors.posterior import Posterior
 from gpytorch import settings
 from gpytorch.constraints import GreaterThan, Interval
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
 from gpytorch.kernels.rbf_kernel import RBFKernel
 from gpytorch.kernels.scale_kernel import ScaleKernel
 from gpytorch.means.constant_mean import ConstantMean
 from gpytorch.mlls import MarginalLogLikelihood
 from gpytorch.models.gp import GP
 from gpytorch.priors.smoothed_box_prior import SmoothedBoxPrior
 from gpytorch.priors.torch_priors import GammaPrior
 from linear_operator.operators import LinearOperator, RootLinearOperator
 from linear_operator.utils.cholesky import psd_safe_cholesky
+from linear_operator.utils.errors import NotPSDError
 from scipy import optimize
 from torch import float32, float64, Tensor
 from torch.nn.modules.module import _IncompatibleKeys
 
 
+# Helper functions
+def _check_strict_input(
+    inputs: List[Tensor], t_inputs: List[Tensor], target_or_inputs: str
+):
+    for input_, t_input in zip(inputs, t_inputs or (None,)):
+        for attr in {"shape", "dtype", "device"}:
+            expected_attr = getattr(t_input, attr, None)
+            found_attr = getattr(input_, attr, None)
+            if expected_attr != found_attr:
+                msg = (
+                    "Cannot modify {attr} of {t_or_i} "
+                    "(expected {e_attr}, found {f_attr})."
+                )
+                msg = msg.format(
+                    attr=attr,
+                    e_attr=expected_attr,
+                    f_attr=found_attr,
+                    t_or_i=target_or_inputs,
+                )
+                raise RuntimeError(msg)
+
+
+def _scaled_psd_safe_cholesky(
+    matrix: Tensor, scale: Union[float, Tensor], jitter: Optional[float] = None
+) -> Tensor:
+    r"""scale matrix by 1/outputscale before cholesky for better numerical stability"""
+    matrix = matrix / scale
+    chol = psd_safe_cholesky(matrix, jitter=jitter)
+    chol = chol * scale.sqrt()
+    return chol
+
+
+def _ensure_psd_with_jitter(
+    matrix: Tensor,
+    scale: Union[float, Tensor] = 1.0,
+    jitter: float = 1e-8,
+    max_tries: int = 3,
+) -> Tensor:
+    scaled_matrix = matrix / scale
+    new_jitter = 0
+    for i in range(max_tries):
+        scaled_matrix = scaled_matrix + new_jitter * torch.diag_embed(
+            torch.ones(
+                scaled_matrix.shape[:-1],
+                device=scaled_matrix.device,
+                dtype=scaled_matrix.dtype,
+            )
+        )
+        _, info = torch.linalg.cholesky_ex(scaled_matrix)
+        psd = (info == 0).all()
+        if psd:
+            break
+        else:
+            new_jitter = jitter * (10**i) - new_jitter
+    if not psd:
+        raise NotPSDError(
+            "Matrix not positive definite after repeatedly adding jitter "
+            f"up to {jitter * (10**i):.1e}."
+        )
+    return scaled_matrix * scale
+
+
 # Why we subclass GP even though it provides no functionality:
 # if this subclassing is removed, we get the following GPyTorch error:
 # "RuntimeError: All MarginalLogLikelihood objects must be given a GP object as
 # a model. If you are using a more complicated model involving a GP, pass the
 # underlying GP object as the model, not a full PyTorch module."
 class PairwiseGP(Model, GP, FantasizeMixin):
     r"""Probit GP for preference learning with Laplace approximation
@@ -73,34 +137,36 @@
     used in the denominator. To maintain consistency with usage of kernels
     elsewhere in BoTorch, we instead do not include :math:`\sigma` in the code
     (implicitly setting it to 1) and use ScaleKernel to scale the function.
 
     In the example below, the user/decision maker has stated that they prefer
     the first item over the second item and the third item over the second item,
     generating comparisons [0, 1] and [2, 1].
-
     Example:
         >>> from botorch.models import PairwiseGP
         >>> import torch
         >>> datapoints = torch.Tensor([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
         >>> comparisons = torch.Tensor([[0, 1], [2, 1]])
         >>> model = PairwiseGP(datapoints, comparisons)
     """
 
     _buffer_names = [
-        "datapoints",
-        "comparisons",
+        "consolidated_datapoints",
+        "consolidated_comparisons",
         "D",
         "DT",
         "utility",
         "covar_chol",
         "likelihood_hess",
         "hlcov_eye",
         "covar",
         "covar_inv",
+        "unconsolidated_datapoints",
+        "unconsolidated_comparisons",
+        "consolidated_indices",
     ]
 
     def __init__(
         self,
         datapoints: Tensor,
         comparisons: Tensor,
         likelihood: Optional[PairwiseLikelihood] = None,
@@ -117,14 +183,28 @@
             likelihood: A PairwiseLikelihood.
             covar_module: Covariance module.
             input_transform: An input transform that is applied in the model's
                 forward pass.
         """
         super().__init__()
 
+        # Set optional parameters
+        # Explicitly set jitter for numerical stability in psd_safe_cholesky
+        self._jitter = kwargs.get("jitter", 1e-6)
+        # Stopping creteria in scipy.optimize.fsolve used to find f_map in _update()
+        # If None, set to 1e-6 by default in _update
+        self._xtol = kwargs.get("xtol")
+        # atol rtol for consolidate_duplicates
+        self._consolidate_rtol = kwargs.get("consolidate_rtol", 0)
+        self._consolidate_atol = kwargs.get("consolidate_atol", 1e-4)
+        # The maximum number of calls to the function in scipy.optimize.fsolve
+        # If None, set to 100 by default in _update
+        # If zero, then 100*(N+1) is used by default by fsolve;
+        self._maxfev = kwargs.get("maxfev")
+
         if input_transform is not None:
             input_transform.to(datapoints)
             # input transformation is applied in set_train_data
             self.input_transform = input_transform
 
         # Compatibility variables with fit_gpytorch_*: Dummy likelihood
         # Likelihood is tightly tied with this model and
@@ -138,32 +218,26 @@
 
         self.train_inputs = []
         self.train_targets = None
         self.utility = None
 
         self.pred_cov_fac_need_update = True
         self.dim = None
+        self.unconsolidated_datapoints = None
+        self.unconsolidated_comparisons = None
+        self.consolidated_datapoints = None
+        self.consolidated_comparisons = None
+        self.consolidated_indices = None
 
         # See set_train_data for additional compatibility variables.
         # Not that the datapoints here are not transformed even if input_transform
         # is not None to avoid double transformation during model fitting.
         # self.transform_inputs is called in `forward`
         self.set_train_data(datapoints, comparisons, update_model=False)
 
-        # Set optional parameters
-        # Explicitly set jitter for numerical stability in psd_safe_cholesky
-        self._jitter = kwargs.get("jitter", 1e-6)
-        # Stopping creteria in scipy.optimize.fsolve used to find f_map in _update()
-        # If None, set to 1e-6 by default in _update
-        self._xtol = kwargs.get("xtol")
-        # The maximum number of calls to the function in scipy.optimize.fsolve
-        # If None, set to 100 by default in _update
-        # If zero, then 100*(N+1) is used by default by fsolve;
-        self._maxfev = kwargs.get("maxfev")
-
         # Set hyperparameters
         # Do not set the batch_shape explicitly so mean_module can operate in both mode
         # once fsolve used in _update can run in batch mode, we should explicitly set
         # the bacth shape here
         self.mean_module = ConstantMean()
         # Do not optimize constant mean prior
         for param in self.mean_module.parameters():
@@ -171,57 +245,63 @@
 
         # set covariance module
         # the default outputscale here is only a rule of thumb, meant to keep
         # estimates away from scale value that would make Phi(f(x)) saturate
         # at 0 or 1
         if covar_module is None:
             os_lb, os_ub = 1e-2, 1e2
-            ls_prior = GammaPrior(1.2, 0.5)
+            ls_prior = GammaPrior(concentration=2.4, rate=2.7)
             ls_prior_mode = (ls_prior.concentration - 1) / ls_prior.rate
             covar_module = ScaleKernel(
                 RBFKernel(
                     batch_shape=self.batch_shape,
                     ard_num_dims=self.dim,
                     lengthscale_prior=ls_prior,
                     lengthscale_constraint=GreaterThan(
                         lower_bound=1e-4, transform=None, initial_value=ls_prior_mode
                     ),
+                    dtype=torch.float64,
                 ),
                 outputscale_prior=SmoothedBoxPrior(a=os_lb, b=os_ub),
                 # make sure we won't get extreme values for the output scale
                 outputscale_constraint=Interval(
                     lower_bound=os_lb * 0.5,
                     upper_bound=os_ub * 2.0,
                     initial_value=1.0,
                 ),
+                dtype=torch.float64,
             )
         if not isinstance(covar_module, ScaleKernel):
             raise UnsupportedError("PairwiseGP must be used with a ScaleKernel.")
         self.covar_module = covar_module
 
         self._x0 = None  # will store temporary results for warm-starting
         if self.datapoints is not None and self.comparisons is not None:
             self.to(dtype=self.datapoints.dtype, device=self.datapoints.device)
             # Find f_map for initial parameters with transformed datapoints
-            transformed_dp = self.transform_inputs(datapoints)
+            transformed_dp = self.transform_inputs(self.datapoints)
             self._update(transformed_dp)
 
         self.to(self.datapoints)
 
     def __deepcopy__(self, memo) -> PairwiseGP:
         attrs = (
-            "datapoints",
-            "comparisons",
+            "consolidated_datapoints",
+            "consolidated_comparisons",
             "covar",
             "covar_inv",
             "covar_chol",
             "likelihood_hess",
             "utility",
             "hlcov_eye",
+            "unconsolidated_datapoints",
+            "unconsolidated_comparisons",
+            "consolidated_indices",
         )
+
         if any(getattr(self, attr) is not None for attr in attrs):
             # Temporarily remove non-leaf tensors so that pytorch allows deepcopy
             old_attr = {}
             for attr in attrs:
                 old_attr[attr] = getattr(self, attr)
                 setattr(self, attr, None)
             new_model = deepcopy(self, memo)
@@ -233,48 +313,49 @@
             dcp = self.__deepcopy__
             # make sure we don't fall into the infinite recursive loop
             self.__deepcopy__ = None
             new_model = deepcopy(self, memo)
             self.__deepcopy__ = dcp
             return new_model
 
-    def _scaled_psd_safe_cholesky(
-        self, M: Tensor, jitter: Optional[float] = None
-    ) -> Tensor:
-        r"""scale M by 1/outputscale before cholesky for better numerical stability"""
-        scale = self.covar_module.outputscale.unsqueeze(-1).unsqueeze(-1)
-        M = M / scale
-        chol = psd_safe_cholesky(M, jitter=jitter)
-        chol = chol * scale.sqrt()
-        return chol
-
     def _has_no_data(self):
         r"""Return true if the model does not have both datapoints and comparisons"""
         return (
             self.datapoints is None
             or len(self.datapoints.size()) == 0
             or self.comparisons is None
         )
 
     def _calc_covar(self, X1: Tensor, X2: Tensor) -> Union[Tensor, LinearOperator]:
         r"""Calculate the covariance matrix given two sets of datapoints"""
-        covar = self.covar_module(X1, X2)
-        return covar.to_dense()
+        covar = self.covar_module(X1, X2).to_dense()
+        # making sure covar is PSD when it's a covariance matrix
+        if X1 is X2:
+            scale = self.covar_module.outputscale.unsqueeze(-1).unsqueeze(-1).detach()
+            covar = _ensure_psd_with_jitter(
+                matrix=covar,
+                scale=scale,
+                jitter=self._jitter,
+            )
+        return covar
 
     def _update_covar(self, datapoints: Tensor) -> None:
         r"""Update values derived from the data and hyperparameters
 
         covar, covar_chol, and covar_inv will be of shape batch_shape x n x n
 
         Args:
             datapoints: (Transformed) datapoints for finding f_max
         """
         self.covar = self._calc_covar(datapoints, datapoints)
-        self.covar_chol = self._scaled_psd_safe_cholesky(
-            self.covar, jitter=self._jitter
+        scale = self.covar_module.outputscale.unsqueeze(-1).unsqueeze(-1).detach()
+        self.covar_chol = _scaled_psd_safe_cholesky(
+            matrix=self.covar,
+            scale=scale,
+            jitter=self._jitter,
         )
         self.covar_inv = torch.cholesky_inverse(self.covar_chol)
 
     def _prior_mean(self, X: Tensor) -> Union[Tensor, LinearOperator]:
         r"""Return point prediction using prior only
 
         Args:
@@ -426,16 +507,24 @@
                 sqrt_scale = (
                     self.covar_module.outputscale.sqrt()
                     .unsqueeze(-1)
                     .detach()
                     .cpu()
                     .numpy()
                 )
-                # initialize x0 using std normal but clip by 3 std to keep it bounded
-                x0 = np.random.standard_normal(init_x0_size).clip(min=-3, max=3)
+                # Heuristic intialization using winning count with perturbation
+                # to avoid extreme or unprobable likelihood values
+                win_count = self.D.sum(dim=-2).detach().cpu().numpy()
+                wc_mean, wc_std = (
+                    win_count.mean(axis=-1, keepdims=True),
+                    win_count.std(axis=-1, keepdims=True).clip(min=1e-6),
+                )
+                x0 = (win_count - wc_mean) / wc_std
+                # adding random perturbation to in case get stuck at strange init values
+                x0 = x0 + 0.05 * np.random.standard_normal(init_x0_size)
                 # scale x0 to be on roughly the right scale
                 x0 = x0 * sqrt_scale
             else:
                 x0 = self._x0
 
             if len(self.batch_shape) > 0:
                 # batch mode, do optimize.fsolve sequentially on CPU
@@ -583,33 +672,69 @@
             x_next = x - x_update
             diff = torch.norm(x - x_next)
             x = x_next
             i += 1
 
         return x
 
-    def _check_strict_input(self, inputs, t_inputs, target_or_inputs):
-        for input_, t_input in zip(inputs, t_inputs or (None,)):
-            for attr in {"shape", "dtype", "device"}:
-                expected_attr = getattr(t_input, attr, None)
-                found_attr = getattr(input_, attr, None)
-                if expected_attr != found_attr:
-                    msg = (
-                        "Cannot modify {attr} of {t_or_i} "
-                        "(expected {e_attr}, found {f_attr})."
-                    )
-                    msg = msg.format(
-                        attr=attr,
-                        e_attr=expected_attr,
-                        f_attr=found_attr,
-                        t_or_i=target_or_inputs,
-                    )
-                    raise RuntimeError(msg)
+    def _consolidate_duplicates(
+        self, datapoints: Tensor, comparisons: Tensor
+    ) -> Tuple[Tensor, Tensor]:
+        """Consolidate and cache datapoints and comparisons"""
+        # check if consolidated datapoints/comparisons are cached
+        if (
+            (datapoints is not self.unconsolidated_datapoints)
+            or (comparisons is not self.unconsolidated_comparisons)
+            or (self.consolidated_datapoints is None)
+            or (self.consolidated_comparisons is None)
+        ):
+            self.unconsolidated_datapoints, self.unconsolidated_comparisons = (
+                datapoints,
+                comparisons,
+            )
+
+            if len(datapoints.shape) > 2 or len(comparisons.shape) > 2:
+                # Do not perform consolidation in batch mode as block design
+                # cannot be guaranteed
+                self.consolidated_datapoints = datapoints
+                self.consolidated_comparisons = comparisons
+                self.consolidated_indices = None
+            else:
+                (
+                    self.consolidated_datapoints,
+                    self.consolidated_comparisons,
+                    self.consolidated_indices,
+                ) = consolidate_duplicates(
+                    datapoints,
+                    comparisons,
+                    rtol=self._consolidate_rtol,
+                    atol=self._consolidate_atol,
+                )
+
+        return self.consolidated_datapoints, self.consolidated_comparisons
 
     # ============== public APIs ==============
+    @property
+    def datapoints(self) -> Tensor:
+        r"""Alias for consolidated datapoints"""
+        return self.consolidated_datapoints
+
+    @property
+    def comparisons(self) -> Tensor:
+        r"""Alias for consolidated comparisons"""
+        return self.consolidated_comparisons
+
+    @property
+    def unconsolidated_utility(self) -> Tensor:
+        r"""Utility of the unconsolidated datapoints"""
+        if self.consolidated_indices is None:
+            # self.consolidated_indices is None in batch mode
+            return self.utility
+        else:
+            return self.utility[self.consolidated_indices]
 
     @property
     def num_outputs(self) -> int:
         r"""The number of outputs of the model."""
         return self._num_outputs
 
     @property
@@ -651,38 +776,41 @@
         # a prior-only model
         if datapoints is None or comparisons is None:
             return
 
         # following gpytorch.models.exact_gp.set_train_data
         if datapoints is not None:
             if torch.is_tensor(datapoints):
-                inputs = (datapoints,)
+                inputs = [datapoints]
 
             inputs = tuple(
                 input_.unsqueeze(-1) if input_.ndimension() == 1 else input_
                 for input_ in inputs
             )
             if strict:
-                self._check_strict_input(inputs, self.train_inputs, "inputs")
+                _check_strict_input(inputs, self.train_inputs, "inputs")
 
-            self.datapoints = inputs[0]
+            datapoints = inputs[0]
             # Compatibility variables with fit_gpytorch_*
             # alias for datapoints ("train_inputs")
             self.train_inputs = inputs
 
         if comparisons is not None:
             if strict:
-                self._check_strict_input([comparisons], [self.train_targets], "targets")
+                _check_strict_input([comparisons], [self.train_targets], "targets")
 
             # convert to long so that it can be used as index and
             # compatible with Tensor.scatter_
-            self.comparisons = comparisons.long()
+            comparisons = comparisons.long()
             # Compatibility variables with fit_gpytorch_*
             # alias for comparisons ("train_targets" here)
-            self.train_targets = self.comparisons
+            self.train_targets = comparisons
+
+        # self.datapoints and self.comparisons are being updated here
+        self._consolidate_duplicates(datapoints, comparisons)
 
         # Compatibility variables with optimize_acqf
         self._dtype = self.datapoints.dtype
         self._num_outputs = 1  # 1 latent value output per observation
 
         self.dim = self.datapoints.shape[-1]  # feature dimensions
         self.n = self.datapoints.shape[-2]  # num datapoints
@@ -700,15 +828,15 @@
         comp_view = self.comparisons.view(-1, self.m, 2).long()
         for i, sub_D in enumerate(self.D.view(-1, self.m, self.n)):
             sub_D.scatter_(1, comp_view[i, :, [0]], 1)
             sub_D.scatter_(1, comp_view[i, :, [1]], -1)
         self.DT = self.D.transpose(-1, -2)
 
         if update_model:
-            transformed_dp = self.transform_inputs(datapoints)
+            transformed_dp = self.transform_inputs(self.datapoints)
             self._update(transformed_dp)
 
         self.to(self.datapoints)
 
     def load_state_dict(
         self, state_dict: Dict[str, Tensor], strict: bool = False
     ) -> _IncompatibleKeys:
@@ -776,26 +904,27 @@
             if self._has_no_data():
                 raise RuntimeError(
                     "datapoints and comparisons cannot be None in training mode. "
                     "Call .eval() for prior predictions, "
                     "or call .set_train_data() to add training data."
                 )
 
-            if datapoints is not self.datapoints:
+            if datapoints is not self.unconsolidated_datapoints:
                 raise RuntimeError("Must train on training data")
 
-            transformed_dp = self.transform_inputs(datapoints)
-
             # We pass in the untransformed datapoints into set_train_data
             # as we will be setting self.datapoints as the untransformed datapoints
             # self.transform_inputs will be called inside before calling _update()
             self.set_train_data(datapoints, self.comparisons, update_model=True)
 
+            transformed_dp = self.transform_inputs(self.datapoints)
+
             hl = self.likelihood_hess
             covar = self.covar
+
             # Apply matrix inversion lemma on eq. in page 27 of [Brochu2010tutorial]_
             # (A + B)^-1 = A^-1 - A^-1 @ (I + BA^-1)^-1 @ BA^-1
             # where A = covar_inv, B = hl
             hl_cov = hl @ covar
             eye = torch.eye(
                 hl_cov.size(-1),
                 dtype=self.datapoints.dtype,
@@ -845,20 +974,25 @@
             # fac = (K + C^-1)^-1 @ k = pred_cov_fac_inv @ covar_x_xnew
             # used substitution method here to calculate fac
             fac = torch.linalg.solve(hlcov_eye, hl @ covar_x_xnew)
             pred_covar = covar_xnew - (covar_xnew_x @ fac)
 
             output_mean, output_covar = pred_mean, pred_covar
 
+        scale = self.covar_module.outputscale.unsqueeze(-1).unsqueeze(-1).detach()
         post = MultivariateNormal(
             mean=output_mean,
             # output_covar is sometimes non-PSD
             # perform a cholesky decomposition to check and amend
             covariance_matrix=RootLinearOperator(
-                self._scaled_psd_safe_cholesky(output_covar, jitter=self._jitter)
+                _scaled_psd_safe_cholesky(
+                    matrix=output_covar,
+                    scale=scale,
+                    jitter=self._jitter,
+                )
             ),
         )
         return post
 
     # ============== botorch.models.model.Model interfaces ==============
     def posterior(
         self,
@@ -971,15 +1105,15 @@
 
         Returns:
             The approximated evidence, i.e., the marginal log likelihood
         """
 
         model = self.model
         likelihood = self.likelihood
-        if comp is not model.comparisons:
+        if comp is not model.unconsolidated_comparisons:
             raise RuntimeError("Must train on training data")
 
         f_map = post.mean.squeeze(-1)
 
         log_likelihood = likelihood.log_p(utility=f_map, D=model.D)
         neg_log_likelihood_sum = -(torch.sum(log_likelihood, dim=-1))
```

### Comparing `botorch-0.8.3/botorch/models/transforms/__init__.py` & `botorch-0.8.4/botorch/models/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/transforms/factory.py` & `botorch-0.8.4/botorch/models/transforms/factory.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/transforms/input.py` & `botorch-0.8.4/botorch/models/transforms/input.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/transforms/outcome.py` & `botorch-0.8.4/botorch/models/transforms/outcome.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/transforms/utils.py` & `botorch-0.8.4/botorch/models/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/models/utils/__init__.py` & `botorch-0.8.4/botorch/models/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from botorch.models.utils.assorted import (
     _make_X_full,
     add_output_dim,
     check_min_max_scaling,
     check_no_nans,
     check_standardization,
+    consolidate_duplicates,
+    detect_duplicates,
     fantasize,
     gpt_posterior_settings,
     mod_batch_shape,
     multioutput_to_batch_mode_transform,
     validate_input_scaling,
 )
 
@@ -28,8 +30,10 @@
     "check_min_max_scaling",
     "check_standardization",
     "fantasize",
     "gpt_posterior_settings",
     "multioutput_to_batch_mode_transform",
     "mod_batch_shape",
     "validate_input_scaling",
+    "detect_duplicates",
+    "consolidate_duplicates",
 ]
```

### Comparing `botorch-0.8.3/botorch/models/utils/assorted.py` & `botorch-0.8.4/botorch/models/utils/assorted.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 r"""Assorted helper methods and objects for working with BoTorch models."""
 
 from __future__ import annotations
 
 import warnings
 from contextlib import contextmanager, ExitStack
-from typing import List, Optional, Tuple
+from typing import Iterator, List, Optional, Tuple
 
 import torch
 from botorch import settings
 from botorch.exceptions import InputDataError, InputDataWarning
 from botorch.settings import _Flag
 from gpytorch import settings as gpt_settings
 from gpytorch.module import Module
@@ -278,10 +278,100 @@
             es.enter_context(gpt_settings.fast_pred_var())
         es.enter_context(
             gpt_settings.detach_test_caches(settings.propagate_grads.off())
         )
         yield
 
 
+def detect_duplicates(
+    X: Tensor,
+    rtol: float = 0,
+    atol: float = 1e-8,
+) -> Iterator[Tuple[int, int]]:
+    """Returns an iterator over index pairs `(duplicate index, original index)` for all
+    duplicate entries of `X`. Supporting 2-d Tensor only.
+
+    Args:
+        X: the datapoints tensor with potential duplicated entries
+        rtol: relative tolerance
+        atol: absolute tolerance
+    """
+    if len(X.shape) != 2:
+        raise ValueError("X must have 2 dimensions.")
+
+    tols = atol
+    if rtol:
+        rval = X.abs().max(dim=-1, keepdim=True).values
+        tols = tols + rtol * rval.max(rval.transpose(-1, -2))
+
+    n = X.shape[-2]
+    dist = torch.full((n, n), float("inf"), device=X.device, dtype=X.dtype)
+    dist[torch.triu_indices(n, n, offset=1).unbind()] = torch.nn.functional.pdist(
+        X, p=float("inf")
+    )
+    return (
+        (i, int(j))
+        # pyre-fixme[19]: Expected 1 positional argument.
+        for diff, j, i in zip(*(dist - tols).min(dim=-2), range(n))
+        if diff < 0
+    )
+
+
+def consolidate_duplicates(
+    X: Tensor, Y: Tensor, rtol: float = 0, atol: float = 1e-8
+) -> Tuple[Tensor, Tensor, Tensor]:
+    """Drop duplicated Xs and update the indices tensor Y accordingly.
+    Supporting 2d Tensor only as in batch mode block design is not guaranteed.
+
+    Args:
+        X: the datapoints tensor
+        Y: the index tensor to be updated (e.g., pairwise comparisons)
+        rtol: relative tolerance
+        atol: absolute tolerance
+
+    Returns:
+        consolidated_X: the consolidated X
+        consolidated_Y: the consolidated Y (e.g., pairwise comparisons indices)
+        new_indices: new index of each original item in X, a tensor of size X.shape[-2]
+    """
+    if len(X.shape) != 2:
+        raise ValueError("X must have 2 dimensions.")
+
+    n = X.shape[-2]
+    dup_map = dict(detect_duplicates(X=X, rtol=rtol, atol=atol))
+
+    # Handle edge cases conservatively
+    # If a item is in both dup set and kept set, do not remove it
+    common_set = set(dup_map.keys()).intersection(dup_map.values())
+    for k in list(dup_map.keys()):
+        if k in common_set or dup_map[k] in common_set:
+            del dup_map[k]
+
+    if dup_map:
+        dup_indices, kept_indices = zip(*dup_map.items())
+
+        unique_indices = sorted(set(range(n)) - set(dup_indices))
+
+        # After dropping the duplicates,
+        # the kept ones' indices may also change by being shifted up
+        new_idx_map = dict(zip(unique_indices, range(len(unique_indices))))
+        new_indices_for_dup = (new_idx_map[idx] for idx in kept_indices)
+        new_idx_map.update(dict(zip(dup_indices, new_indices_for_dup)))
+        consolidated_X = X[list(unique_indices), :]
+        consolidated_Y = torch.tensor(
+            [[new_idx_map[item.item()] for item in row] for row in Y.unbind()],
+            dtype=torch.long,
+            device=Y.device,
+        )
+        new_indices = (
+            torch.arange(n, dtype=torch.long)
+            .apply_(lambda x: new_idx_map[x])
+            .to(Y.device)
+        )
+        return consolidated_X, consolidated_Y, new_indices
+    else:
+        return X, Y, torch.arange(n, device=Y.device, dtype=Y.dtype)
+
+
 class fantasize(_Flag):
     r"""A flag denoting whether we are currently in a `fantasize` context."""
     _state: bool = False
```

### Comparing `botorch-0.8.3/botorch/models/utils/inducing_point_allocators.py` & `botorch-0.8.4/botorch/models/utils/inducing_point_allocators.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
             "_pivoted_cholesky_init requires a quality score for each of train_inputs"
         )
 
     item_size = kernel_matrix.shape[-2]
     cis = torch.zeros(
         (max_length, item_size), device=kernel_matrix.device, dtype=kernel_matrix.dtype
     )
-    di2s = kernel_matrix.diag()
+    di2s = kernel_matrix.diagonal()
     scores = di2s * torch.square(quality_scores)
     selected_items = []
     selected_item = torch.argmax(scores)
     selected_items.append(selected_item)
 
     while len(selected_items) < max_length:
         k = len(selected_items) - 1
```

### Comparing `botorch-0.8.3/botorch/models/utils/parse_training_data.py` & `botorch-0.8.4/botorch/models/utils/parse_training_data.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/__init__.py` & `botorch-0.8.4/botorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/closures/__init__.py` & `botorch-0.8.4/botorch/optim/closures/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/closures/core.py` & `botorch-0.8.4/botorch/optim/closures/core.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/closures/model_closures.py` & `botorch-0.8.4/botorch/optim/closures/model_closures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/core.py` & `botorch-0.8.4/botorch/optim/core.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/fit.py` & `botorch-0.8.4/botorch/optim/fit.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/initializers.py` & `botorch-0.8.4/botorch/utils/sampling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,862 +1,948 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 r"""
+Utilities for MC and qMC sampling.
+
 References
 
-.. [Regis]
-    R. G. Regis, C. A. Shoemaker. Combining radial basis function
-    surrogates and dynamic coordinate search in high-dimensional
-    expensive black-box optimization, Engineering Optimization, 2013.
+.. [Trikalinos2014polytope]
+    T. A. Trikalinos and G. van Valkenhoef. Efficient sampling from uniform
+    density n-polytopes. Technical report, Brown University, 2014.
 """
+
 from __future__ import annotations
 
-import warnings
-from math import ceil
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from abc import ABC, abstractmethod
+from contextlib import contextmanager
+from typing import Any, Generator, Iterable, List, Optional, Tuple, TYPE_CHECKING
 
+import numpy as np
+import scipy
 import torch
-from botorch import settings
-from botorch.acquisition.acquisition import AcquisitionFunction
-from botorch.acquisition.knowledge_gradient import (
-    _get_value_function,
-    qKnowledgeGradient,
-)
-from botorch.acquisition.utils import is_nonnegative
-from botorch.exceptions.errors import BotorchTensorDimensionError, UnsupportedError
-from botorch.exceptions.warnings import (
-    BadInitialCandidatesWarning,
-    BotorchWarning,
-    SamplingWarning,
-)
-from botorch.models.model import Model
-from botorch.optim.utils import fix_features, get_X_baseline
-from botorch.utils.multi_objective.pareto import is_non_dominated
-from botorch.utils.sampling import (
-    batched_multinomial,
-    draw_sobol_samples,
-    get_polytope_samples,
-    manual_seed,
-)
-from botorch.utils.transforms import normalize, standardize, unnormalize
-from torch import Tensor
-from torch.distributions import Normal
+from botorch.exceptions.errors import BotorchError
+from botorch.sampling.qmc import NormalQMCEngine
+from botorch.utils.transforms import unnormalize
+from scipy.spatial import Delaunay, HalfspaceIntersection
+from torch import LongTensor, Tensor
 from torch.quasirandom import SobolEngine
 
-TGenInitialConditions = Callable[
-    [
-        # reasoning behind this annotation: contravariance
-        qKnowledgeGradient,
-        Tensor,
-        int,
-        int,
-        int,
-        Optional[Dict[int, float]],
-        Optional[Dict[str, Union[bool, float, int]]],
-        Optional[List[Tuple[Tensor, Tensor, float]]],
-        Optional[List[Tuple[Tensor, Tensor, float]]],
-    ],
-    Optional[Tensor],
-]
 
+if TYPE_CHECKING:
+    from botorch.sampling.pathwise.paths import SamplePath  # pragma: no cover
 
-def gen_batch_initial_conditions(
-    acq_function: AcquisitionFunction,
-    bounds: Tensor,
-    q: int,
-    num_restarts: int,
-    raw_samples: int,
-    fixed_features: Optional[Dict[int, float]] = None,
-    options: Optional[Dict[str, Union[bool, float, int]]] = None,
-    inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-    equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-) -> Tensor:
-    r"""Generate a batch of initial conditions for random-restart optimziation.
 
-    TODO: Support t-batches of initial conditions.
+@contextmanager
+def manual_seed(seed: Optional[int] = None) -> Generator[None, None, None]:
+    r"""Contextmanager for manual setting the torch.random seed.
 
     Args:
-        acq_function: The acquisition function to be optimized.
-        bounds: A `2 x d` tensor of lower and upper bounds for each column of `X`.
-        q: The number of candidates to consider.
-        num_restarts: The number of starting points for multistart acquisition
-            function optimization.
-        raw_samples: The number of raw samples to consider in the initialization
-            heuristic. Note: if `sample_around_best` is True (the default is False),
-            then `2 * raw_samples` samples are used.
-        fixed_features: A map `{feature_index: value}` for features that
-            should be fixed to a particular value during generation.
-        options: Options for initial condition generation. For valid options see
-            `initialize_q_batch` and `initialize_q_batch_nonneg`. If `options`
-            contains a `nonnegative=True` entry, then `acq_function` is
-            assumed to be non-negative (useful when using custom acquisition
-            functions). In addition, an "init_batch_limit" option can be passed
-            to specify the batch limit for the initialization. This is useful
-            for avoiding memory limits when computing the batch posterior over
-            raw samples.
-        inequality constraints: A list of tuples (indices, coefficients, rhs),
-            with each tuple encoding an inequality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
-        equality constraints: A list of tuples (indices, coefficients, rhs),
-            with each tuple encoding an inequality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+        seed: The seed to set the random number generator to.
 
     Returns:
-        A `num_restarts x q x d` tensor of initial conditions.
+        Generator
 
     Example:
-        >>> qEI = qExpectedImprovement(model, best_f=0.2)
-        >>> bounds = torch.tensor([[0.], [1.]])
-        >>> Xinit = gen_batch_initial_conditions(
-        >>>     qEI, bounds, q=3, num_restarts=25, raw_samples=500
-        >>> )
-    """
-    if bounds.isinf().any():
-        raise NotImplementedError(
-            "Currently only finite values in `bounds` are supported "
-            "for generating initial conditions for optimization."
-        )
-    options = options or {}
-    sample_around_best = options.get("sample_around_best", False)
-    if sample_around_best and equality_constraints:
-        raise UnsupportedError(
-            "Option 'sample_around_best' is not supported when equality"
-            "constraints are present."
-        )
-    seed: Optional[int] = options.get("seed")
-    batch_limit: Optional[int] = options.get(
-        "init_batch_limit", options.get("batch_limit")
-    )
-    factor, max_factor = 1, 5
-    init_kwargs = {}
-    device = bounds.device
-    bounds_cpu = bounds.cpu()
-    if "eta" in options:
-        init_kwargs["eta"] = options.get("eta")
-    if options.get("nonnegative") or is_nonnegative(acq_function):
-        init_func = initialize_q_batch_nonneg
-        if "alpha" in options:
-            init_kwargs["alpha"] = options.get("alpha")
-    else:
-        init_func = initialize_q_batch
-
-    q = 1 if q is None else q
-    # the dimension the samples are drawn from
-    effective_dim = bounds.shape[-1] * q
-    if effective_dim > SobolEngine.MAXDIM and settings.debug.on():
-        warnings.warn(
-            f"Sample dimension q*d={effective_dim} exceeding Sobol max dimension "
-            f"({SobolEngine.MAXDIM}). Using iid samples instead.",
-            SamplingWarning,
-        )
-
-    while factor < max_factor:
-        with warnings.catch_warnings(record=True) as ws:
-            n = raw_samples * factor
-            if inequality_constraints is None and equality_constraints is None:
-                if effective_dim <= SobolEngine.MAXDIM:
-                    X_rnd = draw_sobol_samples(bounds=bounds_cpu, n=n, q=q, seed=seed)
-                else:
-                    with manual_seed(seed):
-                        # load on cpu
-                        X_rnd_nlzd = torch.rand(
-                            n, q, bounds_cpu.shape[-1], dtype=bounds.dtype
-                        )
-                    X_rnd = bounds_cpu[0] + (bounds_cpu[1] - bounds_cpu[0]) * X_rnd_nlzd
-            else:
-                X_rnd = (
-                    get_polytope_samples(
-                        n=n * q,
-                        bounds=bounds,
-                        inequality_constraints=inequality_constraints,
-                        equality_constraints=equality_constraints,
-                        seed=seed,
-                        n_burnin=options.get("n_burnin", 10000),
-                        thinning=options.get("thinning", 32),
-                    )
-                    .view(n, q, -1)
-                    .cpu()
-                )
-            # sample points around best
-            if sample_around_best:
-                X_best_rnd = sample_points_around_best(
-                    acq_function=acq_function,
-                    n_discrete_points=n * q,
-                    sigma=options.get("sample_around_best_sigma", 1e-3),
-                    bounds=bounds,
-                    subset_sigma=options.get("sample_around_best_subset_sigma", 1e-1),
-                    prob_perturb=options.get("sample_around_best_prob_perturb"),
-                )
-                if X_best_rnd is not None:
-                    X_rnd = torch.cat(
-                        [
-                            X_rnd,
-                            X_best_rnd.view(n, q, bounds.shape[-1]).cpu(),
-                        ],
-                        dim=0,
-                    )
-            X_rnd = fix_features(X_rnd, fixed_features=fixed_features)
-            with torch.no_grad():
-                if batch_limit is None:
-                    batch_limit = X_rnd.shape[0]
-                Y_rnd_list = []
-                start_idx = 0
-                while start_idx < X_rnd.shape[0]:
-                    end_idx = min(start_idx + batch_limit, X_rnd.shape[0])
-                    Y_rnd_curr = acq_function(
-                        X_rnd[start_idx:end_idx].to(device=device)
-                    ).cpu()
-                    Y_rnd_list.append(Y_rnd_curr)
-                    start_idx += batch_limit
-                Y_rnd = torch.cat(Y_rnd_list)
-            batch_initial_conditions = init_func(
-                X=X_rnd, Y=Y_rnd, n=num_restarts, **init_kwargs
-            ).to(device=device)
-            if not any(issubclass(w.category, BadInitialCandidatesWarning) for w in ws):
-                return batch_initial_conditions
-            if factor < max_factor:
-                factor += 1
-                if seed is not None:
-                    seed += 1  # make sure to sample different X_rnd
-    warnings.warn(
-        "Unable to find non-zero acquisition function values - initial conditions "
-        "are being selected randomly.",
-        BadInitialCandidatesWarning,
-    )
-    return batch_initial_conditions
+        >>> with manual_seed(1234):
+        >>>     X = torch.rand(3)
+    """
+    old_state = torch.random.get_rng_state()
+    try:
+        if seed is not None:
+            torch.random.manual_seed(seed)
+        yield
+    finally:
+        if seed is not None:
+            torch.random.set_rng_state(old_state)
 
 
-def gen_one_shot_kg_initial_conditions(
-    acq_function: qKnowledgeGradient,
+def draw_sobol_samples(
     bounds: Tensor,
+    n: int,
     q: int,
-    num_restarts: int,
-    raw_samples: int,
-    fixed_features: Optional[Dict[int, float]] = None,
-    options: Optional[Dict[str, Union[bool, float, int]]] = None,
-    inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-    equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-) -> Optional[Tensor]:
-    r"""Generate a batch of smart initializations for qKnowledgeGradient.
+    batch_shape: Optional[Iterable[int], torch.Size] = None,
+    seed: Optional[int] = None,
+) -> Tensor:
+    r"""Draw qMC samples from the box defined by bounds.
 
-    This function generates initial conditions for optimizing one-shot KG using
-    the maximizer of the posterior objective. Intutively, the maximizer of the
-    fantasized posterior will often be close to a maximizer of the current
-    posterior. This function uses that fact to generate the initital conditions
-    for the fantasy points. Specifically, a fraction of `1 - frac_random` (see
-    options) is generated by sampling from the set of maximizers of the
-    posterior objective (obtained via random restart optimization) according to
-    a softmax transformation of their respective values. This means that this
-    initialization strategy internally solves an acquisition function
-    maximization problem. The remaining `frac_random` fantasy points as well as
-    all `q` candidate points are chosen according to the standard initialization
-    strategy in `gen_batch_initial_conditions`.
-
-    Args:
-        acq_function: The qKnowledgeGradient instance to be optimized.
-        bounds: A `2 x d` tensor of lower and upper bounds for each column of
-            task features.
-        q: The number of candidates to consider.
-        num_restarts: The number of starting points for multistart acquisition
-            function optimization.
-        raw_samples: The number of raw samples to consider in the initialization
-            heuristic.
-        fixed_features: A map `{feature_index: value}` for features that
-            should be fixed to a particular value during generation.
-        options: Options for initial condition generation. These contain all
-            settings for the standard heuristic initialization from
-            `gen_batch_initial_conditions`. In addition, they contain
-            `frac_random` (the fraction of fully random fantasy points),
-            `num_inner_restarts` and `raw_inner_samples` (the number of random
-            restarts and raw samples for solving the posterior objective
-            maximization problem, respectively) and `eta` (temperature parameter
-            for sampling heuristic from posterior objective maximizers).
-        inequality constraints: A list of tuples (indices, coefficients, rhs),
-            with each tuple encoding an inequality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
-        equality constraints: A list of tuples (indices, coefficients, rhs),
-            with each tuple encoding an inequality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+    Args:
+        bounds: A `2 x d` dimensional tensor specifying box constraints on a
+            `d`-dimensional space, where bounds[0, :] and bounds[1, :] correspond
+            to lower and upper bounds, respectively.
+        n: The number of (q-batch) samples. As a best practice, use powers of 2.
+        q: The size of each q-batch.
+        batch_shape: The batch shape of the samples. If given, returns samples
+            of shape `n x batch_shape x q x d`, where each batch is an
+            `n x q x d`-dim tensor of qMC samples.
+        seed: The seed used for initializing Owen scrambling. If None (default),
+            use a random seed.
 
     Returns:
-        A `num_restarts x q' x d` tensor that can be used as initial conditions
-        for `optimize_acqf()`. Here `q' = q + num_fantasies` is the total number
-        of points (candidate points plus fantasy points).
+        A `n x batch_shape x q x d`-dim tensor of qMC samples from the box
+        defined by bounds.
 
     Example:
-        >>> qKG = qKnowledgeGradient(model, num_fantasies=64)
-        >>> bounds = torch.tensor([[0., 0.], [1., 1.]])
-        >>> Xinit = gen_one_shot_kg_initial_conditions(
-        >>>     qKG, bounds, q=3, num_restarts=10, raw_samples=512,
-        >>>     options={"frac_random": 0.25},
-        >>> )
-    """
-    options = options or {}
-    frac_random: float = options.get("frac_random", 0.1)
-    if not 0 < frac_random < 1:
-        raise ValueError(
-            f"frac_random must take on values in (0,1). Value: {frac_random}"
-        )
-    q_aug = acq_function.get_augmented_q_batch_size(q=q)
+        >>> bounds = torch.stack([torch.zeros(3), torch.ones(3)])
+        >>> samples = draw_sobol_samples(bounds, 16, 2)
+    """
+    batch_shape = batch_shape or torch.Size()
+    batch_size = int(torch.prod(torch.tensor(batch_shape)))
+    d = bounds.shape[-1]
+    lower = bounds[0]
+    rng = bounds[1] - bounds[0]
+    sobol_engine = SobolEngine(q * d, scramble=True, seed=seed)
+    samples_raw = sobol_engine.draw(batch_size * n, dtype=lower.dtype)
+    samples_raw = samples_raw.view(*batch_shape, n, q, d).to(device=lower.device)
+    if batch_shape != torch.Size():
+        samples_raw = samples_raw.permute(-3, *range(len(batch_shape)), -2, -1)
+    return lower + rng * samples_raw
+
+
+def draw_sobol_normal_samples(
+    d: int,
+    n: int,
+    device: Optional[torch.device] = None,
+    dtype: Optional[torch.dtype] = None,
+    seed: Optional[int] = None,
+) -> Tensor:
+    r"""Draw qMC samples from a multi-variate standard normal N(0, I_d).
 
-    # TODO: Avoid unnecessary computation by not generating all candidates
-    ics = gen_batch_initial_conditions(
-        acq_function=acq_function,
-        bounds=bounds,
-        q=q_aug,
-        num_restarts=num_restarts,
-        raw_samples=raw_samples,
-        fixed_features=fixed_features,
-        options=options,
-        inequality_constraints=inequality_constraints,
-        equality_constraints=equality_constraints,
-    )
+    A primary use-case for this functionality is to compute an QMC average
+    of f(X) over X where each element of X is drawn N(0, 1).
 
-    # compute maximizer of the value function
-    value_function = _get_value_function(
-        model=acq_function.model,
-        objective=acq_function.objective,
-        posterior_transform=acq_function.posterior_transform,
-        sampler=acq_function.inner_sampler,
-        project=getattr(acq_function, "project", None),
-    )
-    from botorch.optim.optimize import optimize_acqf
+    Args:
+        d: The dimension of the normal distribution.
+        n: The number of samples to return. As a best practice, use powers of 2.
+        device: The torch device.
+        dtype:  The torch dtype.
+        seed: The seed used for initializing Owen scrambling. If None (default),
+            use a random seed.
 
-    fantasy_cands, fantasy_vals = optimize_acqf(
-        acq_function=value_function,
-        bounds=bounds,
-        q=1,
-        num_restarts=options.get("num_inner_restarts", 20),
-        raw_samples=options.get("raw_inner_samples", 1024),
-        fixed_features=fixed_features,
-        return_best_only=False,
-        inequality_constraints=inequality_constraints,
-        equality_constraints=equality_constraints,
-    )
+    Returns:
+        A tensor of qMC standard normal samples with dimension `n x d` with device
+        and dtype specified by the input.
 
-    # sampling from the optimizers
-    n_value = int((1 - frac_random) * (q_aug - q))  # number of non-random ICs
-    eta = options.get("eta", 2.0)
-    weights = torch.exp(eta * standardize(fantasy_vals))
-    idx = torch.multinomial(weights, num_restarts * n_value, replacement=True)
-
-    # set the respective initial conditions to the sampled optimizers
-    ics[..., -n_value:, :] = fantasy_cands[idx, 0].view(num_restarts, n_value, -1)
-    return ics
+    Example:
+        >>> samples = draw_sobol_normal_samples(2, 16)
+    """
+    normal_qmc_engine = NormalQMCEngine(d=d, seed=seed, inv_transform=True)
+    samples = normal_qmc_engine.draw(n, dtype=torch.float if dtype is None else dtype)
+    return samples.to(device=device)
 
 
-def gen_value_function_initial_conditions(
-    acq_function: AcquisitionFunction,
-    bounds: Tensor,
-    num_restarts: int,
-    raw_samples: int,
-    current_model: Model,
-    fixed_features: Optional[Dict[int, float]] = None,
-    options: Optional[Dict[str, Union[bool, float, int]]] = None,
+def sample_hypersphere(
+    d: int,
+    n: int = 1,
+    qmc: bool = False,
+    seed: Optional[int] = None,
+    device: Optional[torch.device] = None,
+    dtype: Optional[torch.dtype] = None,
 ) -> Tensor:
-    r"""Generate a batch of smart initializations for optimizing
-    the value function of qKnowledgeGradient.
+    r"""Sample uniformly from a unit d-sphere.
 
-    This function generates initial conditions for optimizing the inner problem of
-    KG, i.e. its value function, using the maximizer of the posterior objective.
-    Intutively, the maximizer of the fantasized posterior will often be close to a
-    maximizer of the current posterior. This function uses that fact to generate the
-    initital conditions for the fantasy points. Specifically, a fraction of `1 -
-    frac_random` (see options) of raw samples is generated by sampling from the set of
-    maximizers of the posterior objective (obtained via random restart optimization)
-    according to a softmax transformation of their respective values. This means that
-    this initialization strategy internally solves an acquisition function
-    maximization problem. The remaining raw samples are generated using
-    `draw_sobol_samples`. All raw samples are then evaluated, and the initial
-    conditions are selected according to the standard initialization strategy in
-    'initialize_q_batch' individually for each inner problem.
-
-    Args:
-        acq_function: The value function instance to be optimized.
-        bounds: A `2 x d` tensor of lower and upper bounds for each column of
-            task features.
-        num_restarts: The number of starting points for multistart acquisition
-            function optimization.
-        raw_samples: The number of raw samples to consider in the initialization
-            heuristic.
-        current_model: The model of the KG acquisition function that was used to
-            generate the fantasy model of the value function.
-        fixed_features: A map `{feature_index: value}` for features that
-            should be fixed to a particular value during generation.
-        options: Options for initial condition generation. These contain all
-            settings for the standard heuristic initialization from
-            `gen_batch_initial_conditions`. In addition, they contain
-            `frac_random` (the fraction of fully random fantasy points),
-            `num_inner_restarts` and `raw_inner_samples` (the number of random
-            restarts and raw samples for solving the posterior objective
-            maximization problem, respectively) and `eta` (temperature parameter
-            for sampling heuristic from posterior objective maximizers).
-
-    Returns:
-        A `num_restarts x batch_shape x q x d` tensor that can be used as initial
-        conditions for `optimize_acqf()`. Here `batch_shape` is the batch shape
-        of value function model.
+    Args:
+        d: The dimension of the hypersphere.
+        n: The number of samples to return.
+        qmc: If True, use QMC Sobol sampling (instead of i.i.d. uniform).
+        seed: If provided, use as a seed for the RNG.
+        device: The torch device.
+        dtype:  The torch dtype.
+
+    Returns:
+        An  `n x d` tensor of uniform samples from from the d-hypersphere.
 
     Example:
-        >>> fant_X = torch.rand(5, 1, 2)
-        >>> fantasy_model = model.fantasize(fant_X, SobolQMCNormalSampler(16))
-        >>> value_function = PosteriorMean(fantasy_model)
-        >>> bounds = torch.tensor([[0., 0.], [1., 1.]])
-        >>> Xinit = gen_value_function_initial_conditions(
-        >>>     value_function, bounds, num_restarts=10, raw_samples=512,
-        >>>     options={"frac_random": 0.25},
-        >>> )
-    """
-    options = options or {}
-    seed: Optional[int] = options.get("seed")
-    frac_random: float = options.get("frac_random", 0.6)
-    if not 0 < frac_random < 1:
-        raise ValueError(
-            f"frac_random must take on values in (0,1). Value: {frac_random}"
-        )
+        >>> sample_hypersphere(d=5, n=10)
+    """
+    dtype = torch.float if dtype is None else dtype
+    if d == 1:
+        rnd = torch.randint(0, 2, (n, 1), device=device, dtype=dtype)
+        return 2 * rnd - 1
+    if qmc:
+        rnd = draw_sobol_normal_samples(d=d, n=n, device=device, dtype=dtype, seed=seed)
+    else:
+        with manual_seed(seed=seed):
+            rnd = torch.randn(n, d, dtype=dtype)
+    samples = rnd / torch.norm(rnd, dim=-1, keepdim=True)
+    if device is not None:
+        samples = samples.to(device)
+    return samples
 
-    # compute maximizer of the current value function
-    value_function = _get_value_function(
-        model=current_model,
-        objective=getattr(acq_function, "objective", None),
-        posterior_transform=acq_function.posterior_transform,
-        sampler=getattr(acq_function, "sampler", None),
-        project=getattr(acq_function, "project", None),
-    )
-    from botorch.optim.optimize import optimize_acqf
 
-    fantasy_cands, fantasy_vals = optimize_acqf(
-        acq_function=value_function,
-        bounds=bounds,
-        q=1,
-        num_restarts=options.get("num_inner_restarts", 20),
-        raw_samples=options.get("raw_inner_samples", 1024),
-        fixed_features=fixed_features,
-        return_best_only=False,
-        options={
-            k: v
-            for k, v in options.items()
-            if k
-            not in ("frac_random", "num_inner_restarts", "raw_inner_samples", "eta")
-        },
-    )
+def sample_simplex(
+    d: int,
+    n: int = 1,
+    qmc: bool = False,
+    seed: Optional[int] = None,
+    device: Optional[torch.device] = None,
+    dtype: Optional[torch.dtype] = None,
+) -> Tensor:
+    r"""Sample uniformly from a d-simplex.
 
-    batch_shape = acq_function.model.batch_shape
-    # sampling from the optimizers
-    n_value = int((1 - frac_random) * raw_samples)  # number of non-random ICs
-    if n_value > 0:
-        eta = options.get("eta", 2.0)
-        weights = torch.exp(eta * standardize(fantasy_vals))
-        idx = batched_multinomial(
-            weights=weights.expand(*batch_shape, -1),
-            num_samples=n_value,
-            replacement=True,
-        ).permute(-1, *range(len(batch_shape)))
-        resampled = fantasy_cands[idx]
+    Args:
+        d: The dimension of the simplex.
+        n: The number of samples to return.
+        qmc: If True, use QMC Sobol sampling (instead of i.i.d. uniform).
+        seed: If provided, use as a seed for the RNG.
+        device: The torch device.
+        dtype: The torch dtype.
+
+    Returns:
+        An `n x d` tensor of uniform samples from from the d-simplex.
+
+    Example:
+        >>> sample_simplex(d=3, n=10)
+    """
+    dtype = torch.float if dtype is None else dtype
+    if d == 1:
+        return torch.ones(n, 1, device=device, dtype=dtype)
+    if qmc:
+        sobol_engine = SobolEngine(d - 1, scramble=True, seed=seed)
+        rnd = sobol_engine.draw(n, dtype=dtype)
     else:
-        resampled = torch.empty(
-            0,
-            *batch_shape,
-            1,
-            bounds.shape[-1],
-            dtype=fantasy_cands.dtype,
-            device=fantasy_cands.device,
-        )
-    # add qMC samples
-    randomized = draw_sobol_samples(
-        bounds=bounds, n=raw_samples - n_value, q=1, batch_shape=batch_shape, seed=seed
-    ).to(resampled)
-    # full set of raw samples
-    X_rnd = torch.cat([resampled, randomized], dim=0)
-    X_rnd = fix_features(X_rnd, fixed_features=fixed_features)
-
-    # evaluate the raw samples
-    with torch.no_grad():
-        Y_rnd = acq_function(X_rnd)
-
-    # select the restart points using the heuristic
-    return initialize_q_batch(
-        X=X_rnd, Y=Y_rnd, n=num_restarts, eta=options.get("eta", 2.0)
-    )
+        with manual_seed(seed=seed):
+            rnd = torch.rand(n, d - 1, dtype=dtype)
+    srnd, _ = torch.sort(rnd, dim=-1)
+    zeros = torch.zeros(n, 1, dtype=dtype)
+    ones = torch.ones(n, 1, dtype=dtype)
+    srnd = torch.cat([zeros, srnd, ones], dim=-1)
+    if device is not None:
+        srnd = srnd.to(device)
+    return srnd[..., 1:] - srnd[..., :-1]
+
+
+def sample_polytope(
+    A: Tensor,
+    b: Tensor,
+    x0: Tensor,
+    n: int = 10000,
+    n0: int = 100,
+    seed: Optional[int] = None,
+) -> Tensor:
+    r"""
+    Hit and run sampler from uniform sampling points from a polytope,
+    described via inequality constraints A*x<=b.
 
+    Args:
+        A: A Tensor describing inequality constraints
+            so that all samples satisfy Ax<=b.
+        b: A Tensor describing the inequality constraints
+            so that all samples satisfy Ax<=b.
+        x0: A `d`-dim Tensor representing a starting point of the chain
+            satisfying the constraints.
+        n: The number of resulting samples kept in the output.
+        n0: The number of burn-in samples. The chain will produce
+            n+n0 samples but the first n0 samples are not saved.
+        seed: The seed for the sampler. If omitted, use a random seed.
 
-def initialize_q_batch(X: Tensor, Y: Tensor, n: int, eta: float = 1.0) -> Tensor:
-    r"""Heuristic for selecting initial conditions for candidate generation.
+    Returns:
+        (n, d) dim Tensor containing the resulting samples.
+    """
+    n_tot = n + n0
+    seed = seed if seed is not None else torch.randint(0, 1000000, (1,)).item()
+    with manual_seed(seed=seed):
+        rands = torch.rand(n_tot, dtype=A.dtype, device=A.device)
+
+    # pre-sample samples from hypersphere
+    d = x0.size(0)
+    # uniform samples from unit ball in d dims
+    Rs = sample_hypersphere(d=d, n=n_tot, dtype=A.dtype, device=A.device).unsqueeze(-1)
+
+    # compute matprods in batch
+    ARs = (A @ Rs).squeeze(-1)
+    out = torch.empty(n, A.size(-1), dtype=A.dtype, device=A.device)
+    x = x0.clone()
+    for i, (ar, r, rnd) in enumerate(zip(ARs, Rs, rands)):
+        # given x, the next point in the chain is x+alpha*r
+        # it also satisfies A(x+alpha*r)<=b which implies A*alpha*r<=b-Ax
+        # so alpha<=(b-Ax)/ar for ar>0, and alpha>=(b-Ax)/ar for ar<0.
+        # b - A @ x is always >= 0, clamping for numerical tolerances
+        w = (b - A @ x).squeeze().clamp(min=0.0) / ar
+        pos = w >= 0
+        alpha_max = w[pos].min()
+        # important to include equality here in cases x is at the boundary
+        # of the polytope
+        neg = w <= 0
+        alpha_min = w[neg].max()
+        # alpha~Unif[alpha_min, alpha_max]
+        alpha = alpha_min + rnd * (alpha_max - alpha_min)
+        x = x + alpha * r
+        if i >= n0:  # save samples after burn-in period
+            out[i - n0] = x.squeeze()
+    return out
+
+
+def batched_multinomial(
+    weights: Tensor,
+    num_samples: int,
+    replacement: bool = False,
+    generator: Optional[torch.Generator] = None,
+    out: Optional[Tensor] = None,
+) -> LongTensor:
+    r"""Sample from multinomial with an arbitrary number of batch dimensions.
 
-    This heuristic selects points from `X` (without replacement) with probability
-    proportional to `exp(eta * Z)`, where `Z = (Y - mean(Y)) / std(Y)` and `eta`
-    is a temperature parameter.
-
-    When using an acquisiton function that is non-negative and possibly zero
-    over large areas of the feature space (e.g. qEI), you should use
-    `initialize_q_batch_nonneg` instead.
-
-    Args:
-        X: A `b x batch_shape x q x d` tensor of `b` - `batch_shape` samples of
-            `q`-batches from a d`-dim feature space. Typically, these are generated
-            using qMC sampling.
-        Y: A tensor of `b x batch_shape` outcomes associated with the samples.
-            Typically, this is the value of the batch acquisition function to be
-            maximized.
-        n: The number of initial condition to be generated. Must be less than `b`.
-        eta: Temperature parameter for weighting samples.
+    Args:
+        weights: A `batch_shape x num_categories` tensor of weights. For each batch
+            index `i, j, ...`, this functions samples from a multinomial with `input`
+            `weights[i, j, ..., :]`. Note that the weights need not sum to one, but must
+            be non-negative, finite and have a non-zero sum.
+        num_samples: The number of samples to draw for each batch index. Must be smaller
+            than `num_categories` if `replacement=False`.
+        replacement: If True, samples are drawn with replacement.
+        generator: A a pseudorandom number generator for sampling.
+        out: The output tensor (optional). If provided, must be of size
+            `batch_shape x num_samples`.
 
     Returns:
-        A `n x batch_shape x q x d` tensor of `n` - `batch_shape` `q`-batch initial
-        conditions, where each batch of `n x q x d` samples is selected independently.
+        A `batch_shape x num_samples` tensor of samples.
+
+    This is a thin wrapper around `torch.multinomial` that allows weight (`input`)
+    tensors with an arbitrary number of batch dimensions (`torch.multinomial` only
+    allows a single batch dimension). The calling signature is the same as for
+    `torch.multinomial`.
 
     Example:
-        >>> # To get `n=10` starting points of q-batch size `q=3`
-        >>> # for model with `d=6`:
-        >>> qUCB = qUpperConfidenceBound(model, beta=0.1)
-        >>> Xrnd = torch.rand(500, 3, 6)
-        >>> Xinit = initialize_q_batch(Xrnd, qUCB(Xrnd), 10)
-    """
-    n_samples = X.shape[0]
-    batch_shape = X.shape[1:-2] or torch.Size()
-    if n > n_samples:
-        raise RuntimeError(
-            f"n ({n}) cannot be larger than the number of "
-            f"provided samples ({n_samples})"
-        )
-    elif n == n_samples:
-        return X
+        >>> weights = torch.rand(2, 3, 10)
+        >>> samples = batched_multinomial(weights, 4)  # shape is 2 x 3 x 4
+    """
+    batch_shape, n_categories = weights.shape[:-1], weights.size(-1)
+    flat_samples = torch.multinomial(
+        input=weights.view(-1, n_categories),
+        num_samples=num_samples,
+        replacement=replacement,
+        generator=generator,
+        out=None if out is None else out.view(-1, num_samples),
+    )
+    return flat_samples.view(*batch_shape, num_samples)
 
-    Ystd = Y.std(dim=0)
-    if torch.any(Ystd == 0):
-        warnings.warn(
-            "All acquisition values for raw samples points are the same for "
-            "at least one batch. Choosing initial conditions at random.",
-            BadInitialCandidatesWarning,
-        )
-        return X[torch.randperm(n=n_samples, device=X.device)][:n]
 
-    max_val, max_idx = torch.max(Y, dim=0)
-    Z = (Y - Y.mean(dim=0)) / Ystd
-    etaZ = eta * Z
-    weights = torch.exp(etaZ)
-    while torch.isinf(weights).any():
-        etaZ *= 0.5
-        weights = torch.exp(etaZ)
-    if batch_shape == torch.Size():
-        idcs = torch.multinomial(weights, n)
-    else:
-        idcs = batched_multinomial(
-            weights=weights.permute(*range(1, len(batch_shape) + 1), 0), num_samples=n
-        ).permute(-1, *range(len(batch_shape)))
-    # make sure we get the maximum
-    if max_idx not in idcs:
-        idcs[-1] = max_idx
-    if batch_shape == torch.Size():
-        return X[idcs]
-    else:
-        return X.gather(
-            dim=0, index=idcs.view(*idcs.shape, 1, 1).expand(n, *X.shape[1:])
-        )
+def _convert_bounds_to_inequality_constraints(bounds: Tensor) -> Tuple[Tensor, Tensor]:
+    r"""Convert bounds into inequality constraints of the form Ax <= b.
 
+    Args:
+        bounds: A `2 x d`-dim tensor of bounds
 
-def initialize_q_batch_nonneg(
-    X: Tensor, Y: Tensor, n: int, eta: float = 1.0, alpha: float = 1e-4
-) -> Tensor:
-    r"""Heuristic for selecting initial conditions for non-neg. acquisition functions.
+    Returns:
+        A two-element tuple containing
+            - A: A `2d x d`-dim tensor of coefficients
+            - b: A `2d x 1`-dim tensor containing the right hand side
+    """
+    d = bounds.shape[-1]
+    eye = torch.eye(d, dtype=bounds.dtype, device=bounds.device)
+    lower, upper = bounds
+    lower_finite, upper_finite = bounds.isfinite()
+    A = torch.cat([-eye[lower_finite], eye[upper_finite]], dim=0)
+    b = torch.cat([-lower[lower_finite], upper[upper_finite]], dim=0).unsqueeze(-1)
+    return A, b
+
+
+def find_interior_point(
+    A: np.ndarray,
+    b: np.ndarray,
+    A_eq: Optional[np.ndarray] = None,
+    b_eq: Optional[np.ndarray] = None,
+) -> np.ndarray:
+    r"""Find an interior point of a polytope via linear programming.
 
-    This function is similar to `initialize_q_batch`, but designed specifically
-    for acquisition functions that are non-negative and possibly zero over
-    large areas of the feature space (e.g. qEI). All samples for which
-    `Y < alpha * max(Y)` will be ignored (assuming that `Y` contains at least
-    one positive value).
-
-    Args:
-        X: A `b x q x d` tensor of `b` samples of `q`-batches from a `d`-dim.
-            feature space. Typically, these are generated using qMC.
-        Y: A tensor of `b` outcomes associated with the samples. Typically, this
-            is the value of the batch acquisition function to be maximized.
-        n: The number of initial condition to be generated. Must be less than `b`.
-        eta: Temperature parameter for weighting samples.
-        alpha: The threshold (as a fraction of the maximum observed value) under
-            which to ignore samples. All input samples for which
-            `Y < alpha * max(Y)` will be ignored.
+    Args:
+        A: A `n_ineq x d`-dim numpy array containing the coefficients of the
+            constraint inequalities.
+        b: A `n_ineq x 1`-dim numpy array containing the right hand sides of
+            the constraint inequalities.
+        A_eq: A `n_eq x d`-dim numpy array containing the coefficients of the
+            constraint equalities.
+        b_eq: A `n_eq x 1`-dim numpy array containing the right hand sides of
+            the constraint equalities.
 
     Returns:
-        A `n x q x d` tensor of `n` `q`-batch initial conditions.
+        A `d`-dim numpy array containing an interior point of the polytope.
+        This function will raise a ValueError if there is no such point.
 
-    Example:
-        >>> # To get `n=10` starting points of q-batch size `q=3`
-        >>> # for model with `d=6`:
-        >>> qEI = qExpectedImprovement(model, best_f=0.2)
-        >>> Xrnd = torch.rand(500, 3, 6)
-        >>> Xinit = initialize_q_batch(Xrnd, qEI(Xrnd), 10)
-    """
-    n_samples = X.shape[0]
-    if n > n_samples:
-        raise RuntimeError("n cannot be larger than the number of provided samples")
-    elif n == n_samples:
-        return X
-
-    max_val, max_idx = torch.max(Y, dim=0)
-    if torch.any(max_val <= 0):
-        warnings.warn(
-            "All acquisition values for raw sampled points are nonpositive, so "
-            "initial conditions are being selected randomly.",
-            BadInitialCandidatesWarning,
+    This method solves the following Linear Program:
+
+        min -s subject to A @ x <= b - 2 * s, s >= 0, A_eq @ x = b_eq
+
+    In case the polytope is unbounded, then it will also constrain the slack
+    variable `s` to `s<=1`.
+    """
+    # augment inequality constraints: A @ (x, s) <= b
+    d = A.shape[-1]
+    ncon = A.shape[-2] + 1
+    c = np.zeros(d + 1)
+    c[-1] = -1
+    b_ub = np.zeros(ncon)
+    b_ub[:-1] = b.reshape(-1)
+    A_ub = np.zeros((ncon, d + 1))
+    A_ub[:-1, :-1] = A
+    A_ub[:-1, -1] = 2.0
+    A_ub[-1, -1] = -1.0
+
+    result = scipy.optimize.linprog(
+        c=c,
+        A_ub=A_ub,
+        b_ub=b_ub,
+        A_eq=A_eq,
+        b_eq=b_eq,
+        bounds=(None, None),
+        method="highs",
+    )
+
+    if result.status == 3:
+        # problem is unbounded - to find a bounded solution we constrain the
+        # slack variable `s` to `s <= 1.0`.
+        A_s = np.concatenate([np.zeros((1, d)), np.ones((1, 1))], axis=-1)
+        A_ub = np.concatenate([A_ub, A_s], axis=0)
+        b_ub = np.concatenate([b_ub, np.ones(1)], axis=-1)
+        result = scipy.optimize.linprog(
+            c=c,
+            A_ub=A_ub,
+            b_ub=b_ub,
+            A_eq=A_eq,
+            b_eq=b_eq,
+            bounds=(None, None),
+            method="highs",
         )
-        return X[torch.randperm(n=n_samples, device=X.device)][:n]
 
-    # make sure there are at least `n` points with positive acquisition values
-    pos = Y > 0
-    num_pos = pos.sum().item()
-    if num_pos < n:
-        # select all positive points and then fill remaining quota with randomly
-        # selected points
-        remaining_indices = (~pos).nonzero(as_tuple=False).view(-1)
-        rand_indices = torch.randperm(remaining_indices.shape[0], device=Y.device)
-        sampled_remaining_indices = remaining_indices[rand_indices[: n - num_pos]]
-        pos[sampled_remaining_indices] = 1
-        return X[pos]
-    # select points within alpha of max_val, iteratively decreasing alpha by a
-    # factor of 10 as necessary
-    alpha_pos = Y >= alpha * max_val
-    while alpha_pos.sum() < n:
-        alpha = 0.1 * alpha
-        alpha_pos = Y >= alpha * max_val
-    alpha_pos_idcs = torch.arange(len(Y), device=Y.device)[alpha_pos]
-    weights = torch.exp(eta * (Y[alpha_pos] / max_val - 1))
-    idcs = alpha_pos_idcs[torch.multinomial(weights, n)]
-    if max_idx not in idcs:
-        idcs[-1] = max_idx
-    return X[idcs]
-
-
-def sample_points_around_best(
-    acq_function: AcquisitionFunction,
-    n_discrete_points: int,
-    sigma: float,
-    bounds: Tensor,
-    best_pct: float = 5.0,
-    subset_sigma: float = 1e-1,
-    prob_perturb: Optional[float] = None,
-) -> Optional[Tensor]:
-    r"""Find best points and sample nearby points.
-
-    Args:
-        acq_function: The acquisition function.
-        n_discrete_points: The number of points to sample.
-        sigma: The standard deviation of the additive gaussian noise for
-            perturbing the best points.
-        bounds: A `2 x d`-dim tensor containing the bounds.
-        best_pct: The percentage of best points to perturb.
-        subset_sigma: The standard deviation of the additive gaussian
-            noise for perturbing a subset of dimensions of the best points.
-        prob_perturb: The probability of perturbing each dimension.
-
-    Returns:
-        An optional `n_discrete_points x d`-dim tensor containing the
-            sampled points. This is None if no baseline points are found.
-    """
-    X = get_X_baseline(acq_function=acq_function)
-    if X is None:
-        return
-    with torch.no_grad():
-        try:
-            posterior = acq_function.model.posterior(X)
-        except AttributeError:
-            warnings.warn(
-                "Failed to sample around previous best points.",
-                BotorchWarning,
+    if result.status == 2:
+        raise ValueError(
+            "No feasible point found. Constraint polytope appears empty. "
+            + "Check your constraints."
+        )
+    elif result.status > 0:
+        raise ValueError(
+            "Problem checking constraint specification. "
+            + "linprog status: {}".format(result.message)
+        )
+    # the x in the result is really (x, s)
+    return result.x[:-1]
+
+
+class PolytopeSampler(ABC):
+    r"""
+    Base class for samplers that sample points from a polytope.
+
+    :meta private:
+    """
+
+    def __init__(
+        self,
+        inequality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
+        equality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
+        bounds: Optional[Tensor] = None,
+        interior_point: Optional[Tensor] = None,
+    ) -> None:
+        r"""
+        Args:
+            inequality_constraints: Tensors `(A, b)` describing inequality
+                constraints `A @ x <= b`, where `A` is a `n_ineq_con x d`-dim
+                Tensor and `b` is a `n_ineq_con x 1`-dim Tensor, with `n_ineq_con`
+                the number of inequalities and `d` the dimension of the sample space.
+            equality_constraints: Tensors `(C, d)` describing the equality constraints
+                `C @ x = d`, where `C` is a `n_eq_con x d`-dim Tensor and `d` is a
+                `n_eq_con x 1`-dim Tensor with `n_eq_con` the number of equalities.
+            bounds: A `2 x d`-dim tensor of box bounds, where `inf` (`-inf`) means
+                that the respective dimension is unbounded above (below).
+            interior_point: A `d x 1`-dim Tensor presenting a point in the
+                (relative) interior of the polytope. If omitted, determined
+                automatically by solving a Linear Program.
+        """
+        if inequality_constraints is None:
+            if bounds is None:
+                raise BotorchError(
+                    "PolytopeSampler requires either inequality constraints or bounds."
+                )
+            A = torch.empty(
+                0, bounds.shape[-1], dtype=bounds.dtype, device=bounds.device
             )
-            return
-        mean = posterior.mean
-        while mean.ndim > 2:
-            # take average over batch dims
-            mean = mean.mean(dim=0)
-        try:
-            f_pred = acq_function.objective(mean)
-        # Some acquisition functions do not have an objective
-        # and for some acquisition functions the objective is None
-        except (AttributeError, TypeError):
-            f_pred = mean
-        if hasattr(acq_function, "maximize"):
-            # make sure that the optimiztaion direction is set properly
-            if not acq_function.maximize:
-                f_pred = -f_pred
-        try:
-            # handle constraints for EHVI-based acquisition functions
-            constraints = acq_function.constraints
-            if constraints is not None:
-                neg_violation = -torch.stack(
-                    [c(mean).clamp_min(0.0) for c in constraints], dim=-1
-                ).sum(dim=-1)
-                feas = neg_violation == 0
-                if feas.any():
-                    f_pred[~feas] = float("-inf")
-                else:
-                    # set objective equal to negative violation
-                    f_pred = neg_violation
-        except AttributeError:
-            pass
-        if f_pred.ndim == mean.ndim and f_pred.shape[-1] > 1:
-            # multi-objective
-            # find pareto set
-            is_pareto = is_non_dominated(f_pred)
-            best_X = X[is_pareto]
+            b = torch.empty(0, 1, dtype=bounds.dtype, device=bounds.device)
         else:
-            if f_pred.shape[-1] == 1:
-                f_pred = f_pred.squeeze(-1)
-            n_best = max(1, round(X.shape[0] * best_pct / 100))
-            # the view() is to ensure that best_idcs is not a scalar tensor
-            best_idcs = torch.topk(f_pred, n_best).indices.view(-1)
-            best_X = X[best_idcs]
-    use_perturbed_sampling = best_X.shape[-1] >= 20 or prob_perturb is not None
-    n_trunc_normal_points = (
-        n_discrete_points // 2 if use_perturbed_sampling else n_discrete_points
-    )
-    perturbed_X = sample_truncated_normal_perturbations(
-        X=best_X,
-        n_discrete_points=n_trunc_normal_points,
-        sigma=sigma,
-        bounds=bounds,
-    )
-    if use_perturbed_sampling:
-        perturbed_subset_dims_X = sample_perturbed_subset_dims(
-            X=best_X,
+            A, b = inequality_constraints
+        if bounds is not None:
+            # add inequality constraints for bounds
+            # TODO: make sure there are not deduplicate constraints
+            A2, b2 = _convert_bounds_to_inequality_constraints(bounds=bounds)
+            A = torch.cat([A, A2], dim=0)
+            b = torch.cat([b, b2], dim=0)
+        self.A = A
+        self.b = b
+        self.equality_constraints = equality_constraints
+
+        if equality_constraints is not None:
+            self.C, self.d = equality_constraints
+            U, S, Vh = torch.linalg.svd(self.C)
+            r = torch.nonzero(S).size(0)  # rank of matrix C
+            self.nullC = Vh[r:, :].transpose(-1, -2)  # orthonormal null space of C,
+            # satisfying # C @ nullC = 0 and nullC.T @ nullC = I
+            # using the change of variables x=x0+nullC*y,
+            # sample y satisfies A*nullC*y<=b-A*x0.
+            # the linear constraint is automatically satisfied as x0 satisfies it.
+        else:
+            self.C = None
+            self.d = None
+            self.nullC = torch.eye(
+                self.A.size(-1), dtype=self.A.dtype, device=self.A.device
+            )
+
+        self.new_A = self.A @ self.nullC  # doesn't depend on the initial point
+
+        # initial point for the original, not transformed, problem
+        if interior_point is not None:
+            if self.feasible(interior_point):
+                self.x0 = interior_point
+            else:
+                raise ValueError("The given input point is not feasible.")
+        else:
+            self.x0 = self.find_interior_point()
+
+    def feasible(self, x: Tensor) -> bool:
+        r"""Check whether a point is contained in the polytope.
+
+        Args:
+            x: A `d x 1`-dim Tensor.
+
+        Returns:
+            True if `x` is contained inside the polytope (incl. its boundary),
+            False otherwise.
+        """
+        ineq = (self.A @ x - self.b <= 0).all()
+        if self.equality_constraints is not None:
+            eq = (self.C @ x - self.d == 0).all()
+            return ineq & eq
+        return ineq
+
+    def find_interior_point(self) -> Tensor:
+        r"""Find an interior point of the polytope.
+
+        Returns:
+            A `d x 1`-dim Tensor representing a point contained in the polytope.
+            This function will raise a ValueError if there is no such point.
+        """
+        if self.equality_constraints:
+            # equality constraints: A_eq * (x, s) = b_eq
+            A_eq = np.zeros((self.C.size(0), self.C.size(-1) + 1))
+            A_eq[:, :-1] = self.C.cpu().numpy()
+            b_eq = self.d.cpu().numpy()
+        else:
+            A_eq = None
+            b_eq = None
+        x0 = find_interior_point(
+            A=self.A.cpu().numpy(), b=self.b.cpu().numpy(), A_eq=A_eq, b_eq=b_eq
+        )
+        return torch.from_numpy(x0).to(self.A).unsqueeze(-1)
+
+    # -------- Abstract methods to be implemented by subclasses -------- #
+
+    @abstractmethod
+    def draw(self, n: int = 1, seed: Optional[int] = None) -> Tensor:
+        r"""Draw samples from the polytope.
+
+        Args:
+            n: The number of samples.
+            seed: The random seed.
+
+        Returns:
+            A `n x d` Tensor of samples from the polytope.
+        """
+        pass  # pragma: no cover
+
+
+class HitAndRunPolytopeSampler(PolytopeSampler):
+    r"""A sampler for sampling from a polyope using a hit-and-run algorithm."""
+
+    def __init__(
+        self,
+        inequality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
+        equality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
+        bounds: Optional[Tensor] = None,
+        interior_point: Optional[Tensor] = None,
+        n_burnin: int = 0,
+    ) -> None:
+        r"""A sampler for sampling from a polyope using a hit-and-run algorithm.
+
+        Args:
+            inequality_constraints: Tensors `(A, b)` describing inequality
+                constraints `A @ x <= b`, where `A` is a `n_ineq_con x d`-dim
+                Tensor and `b` is a `n_ineq_con x 1`-dim Tensor, with `n_ineq_con`
+                the number of inequalities and `d` the dimension of the sample space.
+            equality_constraints: Tensors `(C, d)` describing the equality constraints
+                `C @ x = d`, where `C` is a `n_eq_con x d`-dim Tensor and `d` is a
+                `n_eq_con x 1`-dim Tensor with `n_eq_con` the number of equalities.
+            bounds: A `2 x d`-dim tensor of box bounds, where `inf` (`-inf`) means
+                that the respective dimension is unbounded from above (below).
+            interior_point: A `d x 1`-dim Tensor representing a point in the
+                (relative) interior of the polytope. If omitted, determined
+                automatically by solving a Linear Program.
+            n_burnin: The number of burn in samples.
+        """
+        super().__init__(
+            inequality_constraints=inequality_constraints,
+            equality_constraints=equality_constraints,
             bounds=bounds,
-            # ensure that we return n_discrete_points
-            n_discrete_points=n_discrete_points - n_trunc_normal_points,
-            sigma=sigma,
-            prob_perturb=prob_perturb,
+            interior_point=interior_point,
         )
-        perturbed_X = torch.cat([perturbed_X, perturbed_subset_dims_X], dim=0)
-        # shuffle points
-        perm = torch.randperm(perturbed_X.shape[0], device=X.device)
-        perturbed_X = perturbed_X[perm]
-    return perturbed_X
+        self.n_burnin = n_burnin
+
+    def draw(self, n: int = 1, seed: Optional[int] = None) -> Tensor:
+        r"""Draw samples from the polytope.
 
+        Args:
+            n: The number of samples.
+            seed: The random seed.
+
+        Returns:
+            A `n x d` Tensor of samples from the polytope.
+        """
+        transformed_samples = sample_polytope(
+            # run this on the cpu
+            A=self.new_A.cpu(),
+            b=(self.b - self.A @ self.x0).cpu(),
+            x0=torch.zeros((self.nullC.size(1), 1), dtype=self.A.dtype),
+            n=n,
+            n0=self.n_burnin,
+            seed=seed,
+        ).to(self.b)
+        init_shift = self.x0.transpose(-1, -2)
+        samples = init_shift + transformed_samples @ self.nullC.transpose(-1, -2)
+        # keep the last element of the resulting chain as
+        # the beginning of the next chain
+        self.x0 = samples[-1].reshape(-1, 1)
+        # reset counter so there is no burn-in for subsequent samples
+        self.n_burnin = 0
+        return samples
+
+
+class DelaunayPolytopeSampler(PolytopeSampler):
+    r"""A polytope sampler using Delaunay triangulation.
+
+    This sampler first enumerates the vertices of the constraint polytope and
+    then uses a Delaunay triangulation to tesselate its convex hull.
+
+    The sampling happens in two stages:
+    1. First, we sample from the set of hypertriangles generated by the
+    Delaunay triangulation (i.e. which hyper-triangle to draw the sample
+    from) with probabilities proportional to the triangle volumes.
+    2. Then, we sample uniformly from the chosen hypertriangle by sampling
+    uniformly from the unit simplex of the appropriate dimension, and
+    then computing the convex combination of the vertices of the
+    hypertriangle according to that draw from the simplex.
+
+    The best reference (not exactly the same, but functionally equivalent) is
+    [Trikalinos2014polytope]_. A simple R implementation is available at
+    https://github.com/gertvv/tesselample.
+    """
 
-def sample_truncated_normal_perturbations(
-    X: Tensor,
-    n_discrete_points: int,
-    sigma: float,
+    def __init__(
+        self,
+        inequality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
+        equality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
+        bounds: Optional[Tensor] = None,
+        interior_point: Optional[Tensor] = None,
+    ) -> None:
+        r"""Initialize DelaunayPolytopeSampler.
+
+        Args:
+            inequality_constraints: Tensors `(A, b)` describing inequality
+                constraints `A @ x <= b`, where `A` is a `n_ineq_con x d`-dim
+                Tensor and `b` is a `n_ineq_con x 1`-dim Tensor, with `n_ineq_con`
+                the number of inequalities and `d` the dimension of the sample space.
+            equality_constraints: Tensors `(C, d)` describing the equality constraints
+                `C @ x = d`, where `C` is a `n_eq_con x d`-dim Tensor and `d` is a
+                `n_eq_con x 1`-dim Tensor with `n_eq_con` the number of equalities.
+            bounds: A `2 x d`-dim tensor of box bounds, where `inf` (`-inf`) means
+                that the respective dimension is unbounded from above (below).
+            interior_point: A `d x 1`-dim Tensor representing a point in the
+                (relative) interior of the polytope. If omitted, determined
+                automatically by solving a Linear Program.
+
+        Warning: The vertex enumeration performed in this algorithm can become
+        extremely costly if there are a large number of inequalities. Similarly,
+        the triangulation can get very expensive in high dimensions. Only use
+        this algorithm for moderate dimensions / moderately complex constraint sets.
+        An alternative is the `HitAndRunPolytopeSampler`.
+        """
+        super().__init__(
+            inequality_constraints=inequality_constraints,
+            equality_constraints=equality_constraints,
+            bounds=bounds,
+            interior_point=interior_point,
+        )
+        # shift coordinate system to be anchored at x0
+        new_b = self.b - self.A @ self.x0
+        if self.new_A.shape[-1] < 2:
+            # if the polytope is in dim 1 (i.e. a line segment) Qhull won't work
+            tshlds = new_b / self.new_A
+            neg = self.new_A < 0
+            self.y_min = tshlds[neg].max()
+            self.y_max = tshlds[~neg].min()
+            self.dim = 1
+        else:
+            # Qhull expects inputs of the form A @ x + b <= 0, so we need to negate here
+            halfspaces = torch.cat([self.new_A, -new_b], dim=-1).cpu().numpy()
+            vertices = HalfspaceIntersection(
+                halfspaces=halfspaces, interior_point=np.zeros(self.new_A.shape[-1])
+            ).intersections
+            self.dim = vertices.shape[-1]
+            try:
+                delaunay = Delaunay(vertices)
+            except ValueError as e:
+                if "Points cannot contain NaN" in str(e):
+                    raise ValueError("Polytope is unbounded.")
+                raise e  # pragma: no cover
+            polytopes = torch.from_numpy(
+                np.array([delaunay.points[s] for s in delaunay.simplices]),
+            ).to(self.A)
+            volumes = torch.stack([torch.det(p[1:] - p[0]).abs() for p in polytopes])
+            self._polytopes = polytopes
+            self._p = volumes / volumes.sum()
+
+    def draw(self, n: int = 1, seed: Optional[int] = None) -> Tensor:
+        r"""Draw samples from the polytope.
+
+        Args:
+            n: The number of samples.
+            seed: The random seed.
+
+        Returns:
+            A `n x d` Tensor of samples from the polytope.
+        """
+        if self.dim == 1:
+            with manual_seed(seed):
+                e = torch.rand(n, 1, device=self.new_A.device, dtype=self.new_A.dtype)
+            transformed_samples = self.y_min + (self.y_max - self.y_min) * e
+        else:
+            if seed is None:
+                generator = None
+            else:
+                generator = torch.Generator(device=self.A.device)
+                generator.manual_seed(seed)
+            index_rvs = torch.multinomial(
+                self._p,
+                num_samples=n,
+                replacement=True,
+                generator=generator,
+            )
+            simplex_rvs = sample_simplex(
+                d=self.dim + 1, n=n, seed=seed, device=self.A.device, dtype=self.A.dtype
+            )
+            transformed_samples = torch.stack(
+                [rv @ self._polytopes[idx] for rv, idx in zip(simplex_rvs, index_rvs)]
+            )
+        init_shift = self.x0.transpose(-1, -2)
+        samples = init_shift + transformed_samples @ self.nullC.transpose(-1, -2)
+        return samples
+
+
+def normalize_linear_constraints(
+    bounds: Tensor, constraints: List[Tuple[Tensor, Tensor, float]]
+) -> List[Tuple[Tensor, Tensor, float]]:
+    r"""Normalize linear constraints to the unit cube.
+
+    Args:
+        bounds (Tensor): A `2 x d`-dim tensor containing the box bounds.
+        constraints (List[Tuple[Tensor, Tensor, float]]): A list of
+            tuples (indices, coefficients, rhs), with each tuple encoding
+            an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs` or
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+    """
+
+    new_constraints = []
+    for index, coefficient, rhs in constraints:
+        lower, upper = bounds[:, index]
+        s = upper - lower
+        new_constraints.append(
+            (index, s * coefficient, (rhs - torch.dot(coefficient, lower)).item())
+        )
+    return new_constraints
+
+
+def get_polytope_samples(
+    n: int,
     bounds: Tensor,
-    qmc: bool = True,
+    inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    seed: Optional[int] = None,
+    thinning: int = 32,
+    n_burnin: int = 10_000,
 ) -> Tensor:
-    r"""Sample points around `X`.
+    r"""Sample from polytope defined by box bounds and (in)equality constraints.
+
+    This uses a hit-and-run Markov chain sampler.
 
-    Sample perturbed points around `X` such that the added perturbations
-    are sampled from N(0, sigma^2 I) and truncated to be within [0,1]^d.
+    TODO: make this method return the sampler object, to avoid doing burn-in
+    every time we draw samples.
 
     Args:
-        X: A `n x d`-dim tensor starting points.
-        n_discrete_points: The number of points to sample.
-        sigma: The standard deviation of the additive gaussian noise for
-            perturbing the points.
-        bounds: A `2 x d`-dim tensor containing the bounds.
-        qmc: A boolean indicating whether to use qmc.
+        n: The number of samples.
+        bounds: A `2 x d`-dim tensor containing the box bounds.
+        inequality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
+        equality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+        seed: The random seed.
+        thinning: The amount of thinning.
+        n_burnin: The number of burn-in samples for the Markov chain sampler.
 
     Returns:
-        A `n_discrete_points x d`-dim tensor containing the sampled points.
+        A `n x d`-dim tensor of samples.
     """
-    X = normalize(X, bounds=bounds)
-    d = X.shape[1]
-    # sample points from N(X_center, sigma^2 I), truncated to be within
-    # [0, 1]^d.
-    if X.shape[0] > 1:
-        rand_indices = torch.randint(X.shape[0], (n_discrete_points,), device=X.device)
-        X = X[rand_indices]
-    if qmc:
-        std_bounds = torch.zeros(2, d, dtype=X.dtype, device=X.device)
-        std_bounds[1] = 1
-        u = draw_sobol_samples(bounds=std_bounds, n=n_discrete_points, q=1).squeeze(1)
+    # create tensors representing linear inequality constraints
+    # of the form Ax >= b.
+    # TODO: remove this error handling functionality in a few releases.
+    # Context: BoTorch inadvertently supported indices with unusual dtypes.
+    # This is now not supported.
+    index_dtype_error = (
+        "Normalizing {var_name} failed. Check that the first "
+        "element of {var_name} is the correct dtype following "
+        "the previous IndexError."
+    )
+    if inequality_constraints:
+        # normalize_linear_constraints is called to solve this issue:
+        # https://github.com/pytorch/botorch/issues/1225
+        try:
+            # non-standard dtypes used to be supported for indices in constraints;
+            # this is no longer true
+            constraints = normalize_linear_constraints(bounds, inequality_constraints)
+        except IndexError as e:
+            msg = index_dtype_error.format(var_name="`inequality_constraints`")
+            raise ValueError(msg) from e
+
+        A, b = sparse_to_dense_constraints(
+            d=bounds.shape[-1],
+            constraints=constraints,
+        )
+        # Note the inequality constraints are of the form Ax >= b,
+        # but PolytopeSampler expects inequality constraints of the
+        # form Ax <= b, so we multiply by -1 below.
+        dense_inequality_constraints = -A, -b
+    else:
+        dense_inequality_constraints = None
+    if equality_constraints:
+        try:
+            # non-standard dtypes used to be supported for indices in constraints;
+            # this is no longer true
+            constraints = normalize_linear_constraints(bounds, equality_constraints)
+        except IndexError as e:
+            msg = index_dtype_error.format(var_name="`equality_constraints`")
+            raise ValueError(msg) from e
+
+        # normalize_linear_constraints is called to solve this issue:
+        # https://github.com/pytorch/botorch/issues/1225
+        dense_equality_constraints = sparse_to_dense_constraints(
+            d=bounds.shape[-1], constraints=constraints
+        )
     else:
-        u = torch.rand((n_discrete_points, d), dtype=X.dtype, device=X.device)
-    # compute bounds to sample from
-    a = -X
-    b = 1 - X
-    # compute z-score of bounds
-    alpha = a / sigma
-    beta = b / sigma
-    normal = Normal(0, 1)
-    cdf_alpha = normal.cdf(alpha)
-    # use inverse transform
-    perturbation = normal.icdf(cdf_alpha + u * (normal.cdf(beta) - cdf_alpha)) * sigma
-    # add perturbation and clip points that are still outside
-    perturbed_X = (X + perturbation).clamp(0.0, 1.0)
-    return unnormalize(perturbed_X, bounds=bounds)
+        dense_equality_constraints = None
+    normalized_bounds = torch.zeros_like(bounds)
+    normalized_bounds[1, :] = 1.0
+    polytope_sampler = HitAndRunPolytopeSampler(
+        bounds=normalized_bounds,
+        inequality_constraints=dense_inequality_constraints,
+        equality_constraints=dense_equality_constraints,
+        n_burnin=n_burnin,
+    )
+    samples = polytope_sampler.draw(n=n * thinning, seed=seed)[::thinning]
+    return bounds[0] + samples * (bounds[1] - bounds[0])
+
+
+def sparse_to_dense_constraints(
+    d: int,
+    constraints: List[Tuple[Tensor, Tensor, float]],
+) -> Tuple[Tensor, Tensor]:
+    r"""Convert parameter constraints from a sparse format into a dense format.
 
+    This method converts sparse triples of the form (indices, coefficients, rhs)
+    to constraints of the form Ax >= b or Ax = b.
 
-def sample_perturbed_subset_dims(
-    X: Tensor,
-    bounds: Tensor,
-    n_discrete_points: int,
-    sigma: float = 1e-1,
-    qmc: bool = True,
-    prob_perturb: Optional[float] = None,
-) -> Tensor:
-    r"""Sample around `X` by perturbing a subset of the dimensions.
+    Args:
+        d: The input dimension.
+        inequality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an (in)equality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs` or
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
 
-    By default, dimensions are perturbed with probability equal to
-    `min(20 / d, 1)`. As shown in [Regis]_, perturbing a small number
-    of dimensions can be beneificial. The perturbations are sampled
-    from N(0, sigma^2 I) and truncated to be within [0,1]^d.
+    Returns:
+        A two-element tuple containing:
+            - A: A `n_constraints x d`-dim tensor of coefficients.
+            - b: A `n_constraints x 1`-dim tensor of right hand sides.
+    """
+    _t = constraints[0][1]
+    A = torch.zeros(len(constraints), d, dtype=_t.dtype, device=_t.device)
+    b = torch.zeros(len(constraints), 1, dtype=_t.dtype, device=_t.device)
+    for i, (indices, coefficients, rhs) in enumerate(constraints):
+        A[i, indices.long()] = coefficients
+        b[i] = rhs
+    return A, b
+
+
+def optimize_posterior_samples(
+    paths: SamplePath,
+    bounds: Tensor,
+    candidates: Optional[Tensor] = None,
+    raw_samples: Optional[int] = 1024,
+    num_restarts: int = 20,
+    maximize: bool = True,
+    **kwargs: Any,
+) -> Tuple[Tensor, Tensor]:
+    r"""Cheaply maximizes posterior samples by random querying followed by vanilla
+    gradient descent on the best num_restarts points.
 
     Args:
-        X: A `n x d`-dim tensor starting points. `X`
-            must be normalized to be within `[0, 1]^d`.
-        bounds: The bounds to sample perturbed values from
-        n_discrete_points: The number of points to sample.
-        sigma: The standard deviation of the additive gaussian noise for
-            perturbing the points.
-        qmc: A boolean indicating whether to use qmc.
-        prob_perturb: The probability of perturbing each dimension. If omitted,
-            defaults to `min(20 / d, 1)`.
+        paths: Random Fourier Feature-based sample paths from the GP
+        bounds: The bounds on the search space.
+        candidates: A priori good candidates (typically previous design points)
+            which acts as extra initial guesses for the optimization routine.
+        raw_samples: The number of samples with which to query the samples initially.
+        num_restarts: The number of points selected for gradient-based optimization.
+        maximize: Boolean indicating whether to maimize or minimize
 
     Returns:
-        A `n_discrete_points x d`-dim tensor containing the sampled points.
-
+        A two-element tuple containing:
+            - X_opt: A `num_optima x [batch_size] x d`-dim tensor of optimal inputs x*.
+            - f_opt: A `num_optima x [batch_size] x 1`-dim tensor of optimal outputs f*.
     """
-    if bounds.ndim != 2:
-        raise BotorchTensorDimensionError("bounds must be a `2 x d`-dim tensor.")
-    elif X.ndim != 2:
-        raise BotorchTensorDimensionError("X must be a `n x d`-dim tensor.")
-    d = bounds.shape[-1]
-    if prob_perturb is None:
-        # Only perturb a subset of the features
-        prob_perturb = min(20.0 / d, 1.0)
+    if maximize:
+
+        def path_func(x):
+            return paths(x)
 
-    if X.shape[0] == 1:
-        X_cand = X.repeat(n_discrete_points, 1)
     else:
-        rand_indices = torch.randint(X.shape[0], (n_discrete_points,), device=X.device)
-        X_cand = X[rand_indices]
-    pert = sample_truncated_normal_perturbations(
-        X=X_cand,
-        n_discrete_points=n_discrete_points,
-        sigma=sigma,
-        bounds=bounds,
-        qmc=qmc,
-    )
 
-    # find cases where we are not perturbing any dimensions
-    mask = (
-        torch.rand(
-            n_discrete_points,
-            d,
-            dtype=bounds.dtype,
-            device=bounds.device,
-        )
-        <= prob_perturb
+        def path_func(x):
+            return -paths(x)
+
+    candidate_set = unnormalize(
+        SobolEngine(dimension=bounds.shape[1], scramble=True).draw(raw_samples), bounds
     )
-    ind = (~mask).all(dim=-1).nonzero()
-    # perturb `n_perturb` of the dimensions
-    n_perturb = ceil(d * prob_perturb)
-    perturb_mask = torch.zeros(d, dtype=mask.dtype, device=mask.device)
-    perturb_mask[:n_perturb].fill_(1)
-    # TODO: use batched `torch.randperm` when available:
-    # https://github.com/pytorch/pytorch/issues/42502
-    for idx in ind:
-        mask[idx] = perturb_mask[torch.randperm(d, device=bounds.device)]
-    # Create candidate points
-    X_cand[mask] = pert[mask]
-    return X_cand
+
+    # queries all samples on all candidates - output shape
+    # raw_samples * num_optima * num_models
+    candidate_queries = path_func(candidate_set)
+    argtop_k = torch.topk(candidate_queries, num_restarts, dim=-1).indices
+    X_top_k = candidate_set[argtop_k, :]
+
+    # to avoid circular import, the import occurs here
+    from botorch.generation.gen import gen_candidates_torch
+
+    X_top_k, f_top_k = gen_candidates_torch(
+        X_top_k, path_func, lower_bounds=bounds[0], upper_bounds=bounds[1], **kwargs
+    )
+    f_opt, arg_opt = f_top_k.max(dim=-1, keepdim=True)
+
+    # For each sample (and possibly for every model in the batch of models), this
+    # retrieves the argmax. We flatten, pick out the indices and then reshape to
+    # the original batch shapes (so instead of pickig out the argmax of a
+    # (3, 7, num_restarts, D)) along the num_restarts dim, we pick it out of a
+    # (21  , num_restarts, D)
+    final_shape = candidate_queries.shape[:-1]
+    X_opt = X_top_k.reshape(final_shape.numel(), num_restarts, -1)[
+        torch.arange(final_shape.numel()), arg_opt.flatten()
+    ].reshape(*final_shape, -1)
+    if not maximize:
+        f_opt = -f_opt
+    return X_opt, f_opt
```

### Comparing `botorch-0.8.3/botorch/optim/numpy_converter.py` & `botorch-0.8.4/botorch/optim/numpy_converter.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/optimize.py` & `botorch-0.8.4/botorch/optim/optimize.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,14 +93,30 @@
         if self.inequality_constraints is None and not (
             self.bounds.ndim == 2 and self.bounds.shape[0] == 2
         ):
             raise ValueError(
                 "bounds should be a `2 x d` tensor, current shape: "
                 f"{list(self.bounds.shape)}."
             )
+        # validate that linear constraints across the q-dim and
+        # self.sequential are not present together
+        if self.inequality_constraints is not None and self.sequential is True:
+            for constraint in self.inequality_constraints:
+                if len(constraint[0].shape) > 1:
+                    raise UnsupportedError(
+                        "Linear inequality constraints across the q-dimension are not "
+                        "supported for sequential optimization."
+                    )
+        if self.equality_constraints is not None and self.sequential is True:
+            for constraint in self.equality_constraints:
+                if len(constraint[0].shape) > 1:
+                    raise UnsupportedError(
+                        "Linear equality constraints across the q-dimension are not "
+                        "supported for sequential optimization."
+                    )
 
         # TODO: Validate constraints if provided:
         # https://github.com/pytorch/botorch/pull/1231
         if self.batch_initial_conditions is not None and self.sequential:
             raise UnsupportedError(
                 "`batch_initial_conditions` is not supported for sequential "
                 "optimization. Either avoid specifying "
@@ -696,17 +712,20 @@
     acq_function_list: List[AcquisitionFunction],
     bounds: Tensor,
     num_restarts: int,
     raw_samples: Optional[int] = None,
     options: Optional[Dict[str, Union[bool, float, int, str]]] = None,
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    nonlinear_inequality_constraints: Optional[List[Callable]] = None,
     fixed_features: Optional[Dict[int, float]] = None,
     fixed_features_list: Optional[List[Dict[int, float]]] = None,
     post_processing_func: Optional[Callable[[Tensor], Tensor]] = None,
+    ic_generator: Optional[TGenInitialConditions] = None,
+    ic_gen_kwargs: Optional[Dict] = None,
 ) -> Tuple[Tensor, Tensor]:
     r"""Generate a list of candidates from a list of acquisition functions.
 
     The acquisition functions are optimized in sequence, with previous candidates
     set as `X_pending`. This is also known as sequential greedy optimization.
 
     Args:
@@ -721,22 +740,37 @@
         options: Options for candidate generation.
         inequality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`
         equality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) = rhs`
+        nonlinear_inequality_constraints: A list of callables with that represent
+            non-linear inequality constraints of the form `callable(x) >= 0`. Each
+            callable is expected to take a `(num_restarts) x q x d`-dim tensor as an
+            input and return a `(num_restarts) x q`-dim tensor with the constraint
+            values. The constraints will later be passed to SLSQP. You need to pass in
+            `batch_initial_conditions` in this case. Using non-linear inequality
+            constraints also requires that `batch_limit` is set to 1, which will be
+            done automatically if not specified in `options`.
         fixed_features: A map `{feature_index: value}` for features that
             should be fixed to a particular value during generation.
         fixed_features_list: A list of maps `{feature_index: value}`. The i-th
             item represents the fixed_feature for the i-th optimization. If
             `fixed_features_list` is provided, `optimize_acqf_mixed` is invoked.
         post_processing_func: A function that post-processes an optimization
             result appropriately (i.e., according to `round-trip`
             transformations).
+        ic_generator: Function for generating initial conditions. Not needed when
+            `batch_initial_conditions` are provided. Defaults to
+            `gen_one_shot_kg_initial_conditions` for `qKnowledgeGradient` acquisition
+            functions and `gen_batch_initial_conditions` otherwise. Must be specified
+            for nonlinear inequality constraints.
+        ic_gen_kwargs: Additional keyword arguments passed to function specified by
+            `ic_generator`
 
     Returns:
         A two-element tuple containing
 
         - a `q x d`-dim tensor of generated candidates.
         - a `q`-dim tensor of expected acquisition values, where the value at
             index `i` is the acquisition value conditional on having observed
@@ -764,31 +798,38 @@
                 bounds=bounds,
                 q=1,
                 num_restarts=num_restarts,
                 raw_samples=raw_samples,
                 options=options or {},
                 inequality_constraints=inequality_constraints,
                 equality_constraints=equality_constraints,
+                nonlinear_inequality_constraints=nonlinear_inequality_constraints,
                 fixed_features_list=fixed_features_list,
                 post_processing_func=post_processing_func,
+                ic_generator=ic_generator,
+                ic_gen_kwargs=ic_gen_kwargs,
             )
         else:
+            ic_gen_kwargs = ic_gen_kwargs or {}
             candidate, acq_value = optimize_acqf(
                 acq_function=acq_function,
                 bounds=bounds,
                 q=1,
                 num_restarts=num_restarts,
                 raw_samples=raw_samples,
                 options=options or {},
                 inequality_constraints=inequality_constraints,
                 equality_constraints=equality_constraints,
+                nonlinear_inequality_constraints=nonlinear_inequality_constraints,
                 fixed_features=fixed_features,
                 post_processing_func=post_processing_func,
                 return_best_only=True,
                 sequential=False,
+                ic_generator=ic_generator,
+                **ic_gen_kwargs,
             )
         candidate_list.append(candidate)
         acq_value_list.append(acq_value)
         candidates = torch.cat(candidate_list, dim=-2)
     return candidates, torch.stack(acq_value_list)
 
 
@@ -798,16 +839,19 @@
     q: int,
     num_restarts: int,
     fixed_features_list: List[Dict[int, float]],
     raw_samples: Optional[int] = None,
     options: Optional[Dict[str, Union[bool, float, int, str]]] = None,
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    nonlinear_inequality_constraints: Optional[List[Callable]] = None,
     post_processing_func: Optional[Callable[[Tensor], Tensor]] = None,
     batch_initial_conditions: Optional[Tensor] = None,
+    ic_generator: Optional[TGenInitialConditions] = None,
+    ic_gen_kwargs: Optional[Dict] = None,
     **kwargs: Any,
 ) -> Tuple[Tensor, Tensor]:
     r"""Optimize over a list of fixed_features and returns the best solution.
 
     This is useful for optimizing over mixed continuous and discrete domains.
     For q > 1 this function always performs sequential greedy optimization (with
     proper conditioning on generated candidates).
@@ -827,19 +871,34 @@
         options: Options for candidate generation.
         inequality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`
         equality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) = rhs`
+        nonlinear_inequality_constraints: A list of callables with that represent
+            non-linear inequality constraints of the form `callable(x) >= 0`. Each
+            callable is expected to take a `(num_restarts) x q x d`-dim tensor as an
+            input and return a `(num_restarts) x q`-dim tensor with the constraint
+            values. The constraints will later be passed to SLSQP. You need to pass in
+            `batch_initial_conditions` in this case. Using non-linear inequality
+            constraints also requires that `batch_limit` is set to 1, which will be
+            done automatically if not specified in `options`.
         post_processing_func: A function that post-processes an optimization
             result appropriately (i.e., according to `round-trip`
             transformations).
         batch_initial_conditions: A tensor to specify the initial conditions. Set
             this if you do not want to use default initialization strategy.
+        ic_generator: Function for generating initial conditions. Not needed when
+            `batch_initial_conditions` are provided. Defaults to
+            `gen_one_shot_kg_initial_conditions` for `qKnowledgeGradient` acquisition
+            functions and `gen_batch_initial_conditions` otherwise. Must be specified
+            for nonlinear inequality constraints.
+        ic_gen_kwargs: Additional keyword arguments passed to function specified by
+            `ic_generator`
         kwargs: kwargs do nothing. This is provided so that the same arguments can
             be passed to different acquisition functions without raising an error.
 
     Returns:
         A two-element tuple containing
 
         - a `q x d`-dim tensor of generated candidates.
@@ -853,30 +912,35 @@
             raise ValueError(
                 "`OneShotAcquisitionFunction`s that do not implement `evaluate` "
                 "are currently not supported when `q > 1`. This is needed to "
                 "compute the joint acquisition value."
             )
     _raise_deprecation_warning_if_kwargs("optimize_acqf_mixed", kwargs)
 
+    ic_gen_kwargs = ic_gen_kwargs or {}
+
     if q == 1:
         ff_candidate_list, ff_acq_value_list = [], []
         for fixed_features in fixed_features_list:
             candidate, acq_value = optimize_acqf(
                 acq_function=acq_function,
                 bounds=bounds,
                 q=q,
                 num_restarts=num_restarts,
                 raw_samples=raw_samples,
                 options=options or {},
                 inequality_constraints=inequality_constraints,
                 equality_constraints=equality_constraints,
+                nonlinear_inequality_constraints=nonlinear_inequality_constraints,
                 fixed_features=fixed_features,
                 post_processing_func=post_processing_func,
                 batch_initial_conditions=batch_initial_conditions,
+                ic_generator=ic_generator,
                 return_best_only=True,
+                **ic_gen_kwargs,
             )
             ff_candidate_list.append(candidate)
             ff_acq_value_list.append(acq_value)
 
         ff_acq_values = torch.stack(ff_acq_value_list)
         best = torch.argmax(ff_acq_values)
         return ff_candidate_list[best], ff_acq_values[best]
@@ -894,16 +958,19 @@
             q=1,
             num_restarts=num_restarts,
             raw_samples=raw_samples,
             fixed_features_list=fixed_features_list,
             options=options or {},
             inequality_constraints=inequality_constraints,
             equality_constraints=equality_constraints,
+            nonlinear_inequality_constraints=nonlinear_inequality_constraints,
             post_processing_func=post_processing_func,
             batch_initial_conditions=batch_initial_conditions,
+            ic_generator=ic_generator,
+            ic_gen_kwargs=ic_gen_kwargs,
         )
         candidates = torch.cat([candidates, candidate], dim=-2)
         acq_function.set_X_pending(
             torch.cat([base_X_pending, candidates], dim=-2)
             if base_X_pending is not None
             else candidates
         )
```

### Comparing `botorch-0.8.3/botorch/optim/parameter_constraints.py` & `botorch-0.8.4/botorch/optim/parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/stopping.py` & `botorch-0.8.4/botorch/optim/stopping.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/utils/__init__.py` & `botorch-0.8.4/botorch/optim/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/utils/acquisition_utils.py` & `botorch-0.8.4/botorch/optim/utils/acquisition_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/utils/common.py` & `botorch-0.8.4/botorch/optim/utils/common.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/utils/model_utils.py` & `botorch-0.8.4/botorch/optim/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/utils/numpy_utils.py` & `botorch-0.8.4/botorch/optim/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/optim/utils/timeout.py` & `botorch-0.8.4/botorch/optim/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/posteriors/__init__.py` & `botorch-0.8.4/botorch/posteriors/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/posteriors/base_samples.py` & `botorch-0.8.4/botorch/posteriors/base_samples.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/posteriors/deterministic.py` & `botorch-0.8.4/botorch/posteriors/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/posteriors/ensemble.py` & `botorch-0.8.4/botorch/posteriors/ensemble.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/posteriors/fully_bayesian.py` & `botorch-0.8.4/botorch/posteriors/fully_bayesian.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,10 +134,10 @@
 
         This is used in samplers to identify the t-batch component of the
         `base_sample_shape`. The base samples are expanded over the t-batches to
         provide consistency in the acquisition values, i.e., to ensure that a
         candidate produces same value regardless of its position on the t-batch.
         """
         if self._is_mt:
-            return (0, -3)
-        else:
             return (0, -2)
+        else:
+            return (0, -1)
```

### Comparing `botorch-0.8.3/botorch/posteriors/gpytorch.py` & `botorch-0.8.4/botorch/posteriors/gpytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,29 +188,14 @@
                 sample_shape=sample_shape, base_samples=base_samples
             )
         # make sure there always is an output dimension
         if not self._is_mt:
             samples = samples.unsqueeze(-1)
         return samples
 
-    def sample(self, sample_shape: Optional[torch.Size] = None) -> Tensor:
-        r"""Sample from the posterior without gradients.
-
-        Args:
-            sample_shape: A `torch.Size` object specifying the sample shape. To
-                draw `n` samples, set to `torch.Size([n])`. To draw `b` batches
-                of `n` samples each, set to `torch.Size([b, n])`.
-
-        Returns:
-            Samples from the posterior, a tensor of shape
-            `self._extended_shape(sample_shape=sample_shape)`.
-        """
-        with torch.no_grad():
-            return self.rsample(sample_shape=sample_shape)
-
     @property
     def mean(self) -> Tensor:
         r"""The posterior mean."""
         mean = self.distribution.mean
         if not self._is_mt:
             mean = mean.unsqueeze(-1)
         return mean
```

### Comparing `botorch-0.8.3/botorch/posteriors/higher_order.py` & `botorch-0.8.4/botorch/posteriors/higher_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         )
 
         # compute y - Y_x
         train_rhs = self.train_targets - train_marginal_samples
 
         # K_{train, train}^{-1} (y - Y_x)
         # internally, this solve is done using Kronecker algebra and is fast.
-        kinv_rhs = self.train_train_covar.inv_matmul(train_rhs)
+        kinv_rhs = self.train_train_covar.solve(train_rhs)
         # multiply by cross-covariance
         test_updated_samples = self.test_train_covar.matmul(kinv_rhs)
 
         # add samples
         test_cond_samples = test_marginal_samples + test_updated_samples
         test_cond_samples = test_cond_samples.permute(
             test_cond_samples.ndim - 1, *range(0, test_cond_samples.ndim - 1)
```

### Comparing `botorch-0.8.3/botorch/posteriors/multitask.py` & `botorch-0.8.4/botorch/posteriors/multitask.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         n_test = joint_samples.shape[-1] - n_obs
         obs_samples, test_samples = torch.split(joint_samples, [n_obs, n_test], dim=-1)
         updated_obs_samples = obs_samples + noise_samples
         obs_minus_samples = (
             train_diff.reshape(*train_diff.shape[:-2], -1) - updated_obs_samples
         )
         train_covar_plus_noise = self.train_train_covar + self.train_noise
-        obs_solve = train_covar_plus_noise.inv_matmul(obs_minus_samples.unsqueeze(-1))
+        obs_solve = train_covar_plus_noise.solve(obs_minus_samples.unsqueeze(-1))
 
         # and multiply the test-observed matrix against the result of the solve
         updated_samples = self.test_train_covar.matmul(obs_solve).squeeze(-1)
 
         # finally, we add the conditioned samples to the prior samples
         final_samples = test_samples + updated_samples
```

### Comparing `botorch-0.8.3/botorch/posteriors/posterior.py` & `botorch-0.8.4/botorch/posteriors/posterior.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,14 +65,29 @@
 
         Returns:
             Samples from the posterior, a tensor of shape
             `self._extended_shape(sample_shape=sample_shape)`.
         """
         pass  # pragma: no cover
 
+    def sample(self, sample_shape: Optional[torch.Size] = None) -> Tensor:
+        r"""Sample from the posterior without gradients.
+
+        Args:
+            sample_shape: A `torch.Size` object specifying the sample shape. To
+                draw `n` samples, set to `torch.Size([n])`. To draw `b` batches
+                of `n` samples each, set to `torch.Size([b, n])`.
+
+        Returns:
+            Samples from the posterior, a tensor of shape
+            `self._extended_shape(sample_shape=sample_shape)`.
+        """
+        with torch.no_grad():
+            return self.rsample(sample_shape=sample_shape)
+
     @property
     def event_shape(self) -> torch.Size:
         r"""The event shape (i.e. the shape of a single sample)."""
         warnings.warn(
             "The `event_shape` attribute of `Posterior` is deprecated. It will default "
             "to the `event_shape` of the underlying distribution in a future version. "
             "Use `_extended_shape` instead.",
```

### Comparing `botorch-0.8.3/botorch/posteriors/posterior_list.py` & `botorch-0.8.4/botorch/posteriors/posterior_list.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/posteriors/torch.py` & `botorch-0.8.4/botorch/posteriors/torch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/posteriors/transformed.py` & `botorch-0.8.4/botorch/posteriors/transformed.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/__init__.py` & `botorch-0.8.4/botorch/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/base.py` & `botorch-0.8.4/botorch/sampling/base.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/deterministic.py` & `botorch-0.8.4/botorch/sampling/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/get_sampler.py` & `botorch-0.8.4/botorch/sampling/get_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/index_sampler.py` & `botorch-0.8.4/botorch/sampling/index_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/list_sampler.py` & `botorch-0.8.4/botorch/sampling/list_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/normal.py` & `botorch-0.8.4/botorch/sampling/normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pairwise_samplers.py` & `botorch-0.8.4/botorch/sampling/pairwise_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/__init__.py` & `botorch-0.8.4/botorch/sampling/pathwise/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/features/__init__.py` & `botorch-0.8.4/botorch/sampling/pathwise/features/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/features/generators.py` & `botorch-0.8.4/botorch/sampling/pathwise/features/generators.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/features/maps.py` & `botorch-0.8.4/botorch/sampling/pathwise/features/maps.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/paths.py` & `botorch-0.8.4/botorch/sampling/pathwise/paths.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/posterior_samplers.py` & `botorch-0.8.4/botorch/sampling/pathwise/posterior_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/prior_samplers.py` & `botorch-0.8.4/botorch/sampling/pathwise/prior_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/update_strategies.py` & `botorch-0.8.4/botorch/sampling/pathwise/update_strategies.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/pathwise/utils.py` & `botorch-0.8.4/botorch/sampling/pathwise/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/qmc.py` & `botorch-0.8.4/botorch/sampling/qmc.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/sampling/stochastic_samplers.py` & `botorch-0.8.4/botorch/sampling/stochastic_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/settings.py` & `botorch-0.8.4/botorch/settings.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/test_functions/__init__.py` & `botorch-0.8.4/botorch/test_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/test_functions/base.py` & `botorch-0.8.4/botorch/test_functions/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple
 
 import torch
+from botorch.exceptions.errors import InputDataError
 from torch import Tensor
 from torch.nn import Module
 
 
 class BaseTestProblem(Module, ABC):
     r"""Base class for test functions."""
 
@@ -31,14 +32,19 @@
         Args:
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
         """
         super().__init__()
         self.noise_std = noise_std
         self.negate = negate
+        if len(self._bounds) != self.dim:
+            raise InputDataError(
+                "Expected the bounds to match the dimensionality of the domain. "
+                f"Got {self.dim=} and {len(self._bounds)=}."
+            )
         self.register_buffer(
             "bounds", torch.tensor(self._bounds, dtype=torch.float).transpose(-1, -2)
         )
 
     def forward(self, X: Tensor, noise: bool = True) -> Tensor:
         r"""Evaluate the function on a set of points.
```

### Comparing `botorch-0.8.3/botorch/test_functions/multi_fidelity.py` & `botorch-0.8.4/botorch/test_functions/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/test_functions/multi_objective.py` & `botorch-0.8.4/botorch/test_functions/multi_objective.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/test_functions/multi_objective_multi_fidelity.py` & `botorch-0.8.4/botorch/test_functions/multi_objective_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/test_functions/sensitivity_analysis.py` & `botorch-0.8.4/botorch/test_functions/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/test_functions/synthetic.py` & `botorch-0.8.4/botorch/test_functions/synthetic.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,20 +34,19 @@
     ) -> None:
         r"""
         Args:
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
+        if bounds is not None:
+            self._bounds = bounds
         super().__init__(noise_std=noise_std, negate=negate)
         if self._optimizers is not None:
             if bounds is not None:
-                if len(bounds) != self.dim:
-                    raise ValueError("Custom bounds does not match function dim.")
-
                 # Ensure at least one optimizer lies within the custom bounds
                 def in_bounds(
                     optimizer: Tuple[float, ...], bounds: List[Tuple[float, float]]
                 ) -> bool:
                     for i, xopt in enumerate(optimizer):
                         lower, upper = bounds[i]
                         if xopt < lower or xopt > upper:
@@ -60,17 +59,14 @@
                     for optimizer in self._optimizers
                 ):
                     raise ValueError(
                         "No global optimum found within custom bounds. Please specify "
                         "bounds which include at least one point in "
                         f"`{self.__class__.__name__}._optimizers`."
                     )
-
-                self._bounds = bounds
-
             self.register_buffer(
                 "optimizers", torch.tensor(self._optimizers, dtype=torch.float)
             )
 
     @property
     def optimal_value(self) -> float:
         r"""The global minimum (maximum if negate=True) of the function."""
@@ -103,15 +99,16 @@
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         self.dim = dim
-        self._bounds = [(-32.768, 32.768) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(-32.768, 32.768) for _ in range(self.dim)]
         self._optimizers = [tuple(0.0 for _ in range(self.dim))]
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
         self.a = 20
         self.b = 0.2
         self.c = 2 * math.pi
 
     def evaluate_true(self, X: Tensor) -> Tensor:
@@ -228,15 +225,16 @@
         r"""
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
         """
         self.dim = dim
-        self._bounds = [(-10.0, 10.0) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(-10.0, 10.0) for _ in range(self.dim)]
         self._optimizers = [
             tuple(
                 math.pow(2.0, -(1.0 - 2.0 ** (-(i - 1))))
                 for i in range(1, self.dim + 1)
             )
         ]
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
@@ -287,15 +285,16 @@
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         self.dim = dim
-        self._bounds = [(-600.0, 600.0) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(-600.0, 600.0) for _ in range(self.dim)]
         self._optimizers = [tuple(0.0 for _ in range(self.dim))]
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
 
     def evaluate_true(self, X: Tensor) -> Tensor:
         part1 = torch.sum(X**2 / 4000.0, dim=-1)
         d = X.shape[-1]
         part2 = -(torch.prod(torch.cos(X / torch.sqrt(X.new(range(1, d + 1)))), dim=-1))
@@ -330,15 +329,16 @@
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         if dim not in (3, 4, 6):
             raise ValueError(f"Hartmann with dim {dim} not defined")
         self.dim = dim
-        self._bounds = [(0.0, 1.0) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(0.0, 1.0) for _ in range(self.dim)]
         # optimizers and optimal values for dim=4 not implemented
         optvals = {3: -3.86278, 6: -3.32237}
         optimizers = {
             3: [(0.114614, 0.555649, 0.852547)],
             6: [(0.20169, 0.150011, 0.476874, 0.275332, 0.311652, 0.6573)],
         }
         self._optimal_value = optvals.get(self.dim)
@@ -463,15 +463,16 @@
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         self.dim = dim
-        self._bounds = [(-10.0, 10.0) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(-10.0, 10.0) for _ in range(self.dim)]
         self._optimizers = [tuple(1.0 for _ in range(self.dim))]
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
 
     def evaluate_true(self, X: Tensor) -> Tensor:
         w = 1.0 + (X - 1.0) / 4.0
         part1 = torch.sin(math.pi * w[..., 0]) ** 2
         part2 = torch.sum(
@@ -504,15 +505,16 @@
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         self.dim = dim
-        self._bounds = [(0.0, math.pi) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(0.0, math.pi) for _ in range(self.dim)]
         optvals = {2: -1.80130341, 5: -4.687658, 10: -9.66015}
         optimizers = {2: [(2.20290552, 1.57079633)]}
         self._optimal_value = optvals.get(self.dim)
         self._optimizers = optimizers.get(self.dim)
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
         self.register_buffer(
             "i", torch.tensor(tuple(range(1, self.dim + 1)), dtype=torch.float)
@@ -549,15 +551,16 @@
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         self.dim = dim
-        self._bounds = [(-4.0, 5.0) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(-4.0, 5.0) for _ in range(self.dim)]
         self._optimizers = [tuple(0.0 for _ in range(self.dim))]
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
 
     def evaluate_true(self, X: Tensor) -> Tensor:
         result = torch.zeros_like(X[..., 0])
         for i in range(self.dim // 4):
             i_ = i + 1
@@ -584,15 +587,16 @@
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         self.dim = dim
-        self._bounds = [(-5.12, 5.12) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(-5.12, 5.12) for _ in range(self.dim)]
         self._optimizers = [tuple(0.0 for _ in range(self.dim))]
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
 
     def evaluate_true(self, X: Tensor) -> Tensor:
         return 10.0 * self.dim + torch.sum(
             X**2 - 10.0 * torch.cos(2.0 * math.pi * X), dim=-1
         )
@@ -622,15 +626,16 @@
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         self.dim = dim
-        self._bounds = [(-5.0, 10.0) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(-5.0, 10.0) for _ in range(self.dim)]
         self._optimizers = [tuple(1.0 for _ in range(self.dim))]
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
 
     def evaluate_true(self, X: Tensor) -> Tensor:
         return torch.sum(
             100.0 * (X[..., 1:] - X[..., :-1] ** 2) ** 2 + (X[..., :-1] - 1) ** 2,
             dim=-1,
@@ -732,15 +737,16 @@
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         self.dim = dim
-        self._bounds = [(-5.0, 5.0) for _ in range(self.dim)]
+        if bounds is None:
+            bounds = [(-5.0, 5.0) for _ in range(self.dim)]
         self._optimal_value = -39.166166 * self.dim
         self._optimizers = [tuple(-2.903534 for _ in range(self.dim))]
         super().__init__(noise_std=noise_std, negate=negate, bounds=bounds)
 
     def evaluate_true(self, X: Tensor) -> Tensor:
         return 0.5 * (X**4 - 16 * X**2 + 5 * X).sum(dim=-1)
```

### Comparing `botorch-0.8.3/botorch/utils/__init__.py` & `botorch-0.8.4/botorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/constants.py` & `botorch-0.8.4/botorch/utils/constants.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/constraints.py` & `botorch-0.8.4/botorch/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/containers.py` & `botorch-0.8.4/botorch/utils/containers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/context_managers.py` & `botorch-0.8.4/botorch/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/datasets.py` & `botorch-0.8.4/botorch/utils/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,38 +33,35 @@
 
 
 class SupervisedDatasetMeta(type):
     def __call__(cls, *args: Any, **kwargs: Any):
         r"""Converts Tensor-valued fields to DenseContainer under the assumption
         that said fields house collections of feature vectors."""
         hints = get_type_hints(cls)
-        f_iter = filter(
-            lambda f: f.init and issubclass(hints[f.name], BotorchContainer),
-            fields(cls),
-        )
+        f_iter = filter(lambda f: f.init, fields(cls))
         f_dict = {}
         for obj, f in chain(
             zip(args, f_iter), ((kwargs.pop(f.name, MISSING), f) for f in f_iter)
         ):
             if obj is MISSING:
                 if f.default is not MISSING:
-
                     obj = f.default
                 elif f.default_factory is not MISSING:
                     obj = f.default_factory()
                 else:
                     raise RuntimeError(f"Missing required field `{f.name}`.")
 
-            if isinstance(obj, Tensor):
-                obj = DenseContainer(obj, event_shape=obj.shape[-1:])
-            elif not isinstance(obj, BotorchContainer):
-                raise TypeError(
-                    f"Expected <BotorchContainer | Tensor> for field `{f.name}` "
-                    f"but was {type(obj)}."
-                )
+            if issubclass(hints[f.name], BotorchContainer):
+                if isinstance(obj, Tensor):
+                    obj = DenseContainer(obj, event_shape=obj.shape[-1:])
+                elif not isinstance(obj, BotorchContainer):
+                    raise TypeError(
+                        f"Expected <BotorchContainer | Tensor> for field `{f.name}` "
+                        f"but was {type(obj)}."
+                    )
             f_dict[f.name] = obj
 
         return super().__call__(**f_dict, **kwargs)
 
 
 @dataclass
 class SupervisedDataset(BotorchDataset, metaclass=SupervisedDatasetMeta):
```

### Comparing `botorch-0.8.3/botorch/utils/dispatcher.py` & `botorch-0.8.4/botorch/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/feasible_volume.py` & `botorch-0.8.4/botorch/utils/feasible_volume.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/gp_sampling.py` & `botorch-0.8.4/botorch/utils/gp_sampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/low_rank.py` & `botorch-0.8.4/botorch/utils/low_rank.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 import torch
 from botorch.exceptions.errors import BotorchError
 from botorch.posteriors.base_samples import _reshape_base_samples_non_interleaved
-from botorch.posteriors.fully_bayesian import FullyBayesianPosterior
 from botorch.posteriors.gpytorch import GPyTorchPosterior
 from gpytorch.distributions.multitask_multivariate_normal import (
     MultitaskMultivariateNormal,
 )
 from linear_operator.operators import BlockDiagLinearOperator, LinearOperator
 
 from linear_operator.utils.cholesky import psd_safe_cholesky
@@ -58,20 +57,17 @@
 
     Returns:
         Reshaped and expanded base samples.
     """
     mvn = posterior.distribution
     loc = mvn.loc
     peshape = posterior._extended_shape()
-    is_fully_b = int(isinstance(posterior, FullyBayesianPosterior))
     base_samples = base_samples.view(
-        sample_shape
-        + torch.Size([1 for _ in range(loc.ndim - 1 - is_fully_b)])
-        + peshape[-2 - is_fully_b :]
-    ).expand(sample_shape + loc.shape[: -1 - is_fully_b] + peshape[-2 - is_fully_b :])
+        sample_shape + torch.Size([1] * (loc.ndim - 1)) + peshape[-2:]
+    ).expand(sample_shape + loc.shape[:-1] + peshape[-2:])
     if posterior._is_mt:
         base_samples = _reshape_base_samples_non_interleaved(
             mvn=posterior.distribution,
             base_samples=base_samples,
             sample_shape=sample_shape,
         )
     base_samples = base_samples.reshape(
```

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/__init__.py` & `botorch-0.8.4/botorch/utils/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/__init__.py` & `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/box_decomposition.py` & `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/box_decomposition.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py` & `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/dominated.py` & `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/dominated.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/non_dominated.py` & `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/non_dominated.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/box_decompositions/utils.py` & `botorch-0.8.4/botorch/utils/multi_objective/box_decompositions/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/hypervolume.py` & `botorch-0.8.4/botorch/utils/multi_objective/hypervolume.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/pareto.py` & `botorch-0.8.4/botorch/utils/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/multi_objective/scalarization.py` & `botorch-0.8.4/botorch/utils/multi_objective/scalarization.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/objective.py` & `botorch-0.8.4/botorch/utils/objective.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/probability/__init__.py` & `botorch-0.8.4/botorch/utils/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/probability/bvn.py` & `botorch-0.8.4/botorch/utils/probability/bvn.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/probability/lin_ess.py` & `botorch-0.8.4/botorch/utils/probability/lin_ess.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/probability/linalg.py` & `botorch-0.8.4/botorch/utils/probability/linalg.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/probability/mvnxpb.py` & `botorch-0.8.4/botorch/utils/probability/mvnxpb.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/probability/truncated_multivariate_normal.py` & `botorch-0.8.4/botorch/utils/probability/truncated_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/probability/unified_skew_normal.py` & `botorch-0.8.4/botorch/utils/probability/unified_skew_normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/probability/utils.py` & `botorch-0.8.4/botorch/utils/probability/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/rounding.py` & `botorch-0.8.4/botorch/utils/rounding.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/safe_math.py` & `botorch-0.8.4/botorch/utils/safe_math.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/sampling.py` & `botorch-0.8.4/botorch/optim/initializers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,875 +1,1041 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 r"""
-Utilities for MC and qMC sampling.
-
 References
 
-.. [Trikalinos2014polytope]
-    T. A. Trikalinos and G. van Valkenhoef. Efficient sampling from uniform
-    density n-polytopes. Technical report, Brown University, 2014.
+.. [Regis]
+    R. G. Regis, C. A. Shoemaker. Combining radial basis function
+    surrogates and dynamic coordinate search in high-dimensional
+    expensive black-box optimization, Engineering Optimization, 2013.
 """
-
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from contextlib import contextmanager
-from typing import Generator, Iterable, List, Optional, Tuple
+import warnings
+from math import ceil
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
-import numpy as np
-import scipy
 import torch
-from botorch.exceptions.errors import BotorchError
-from botorch.sampling.qmc import NormalQMCEngine
-from scipy.spatial import Delaunay, HalfspaceIntersection
-from torch import LongTensor, Tensor
+from botorch import settings
+from botorch.acquisition.acquisition import AcquisitionFunction
+from botorch.acquisition.knowledge_gradient import (
+    _get_value_function,
+    qKnowledgeGradient,
+)
+from botorch.acquisition.utils import is_nonnegative
+from botorch.exceptions.errors import BotorchTensorDimensionError, UnsupportedError
+from botorch.exceptions.warnings import (
+    BadInitialCandidatesWarning,
+    BotorchWarning,
+    SamplingWarning,
+)
+from botorch.models.model import Model
+from botorch.optim.utils import fix_features, get_X_baseline
+from botorch.utils.multi_objective.pareto import is_non_dominated
+from botorch.utils.sampling import (
+    batched_multinomial,
+    draw_sobol_samples,
+    get_polytope_samples,
+    manual_seed,
+)
+from botorch.utils.transforms import normalize, standardize, unnormalize
+from torch import Tensor
+from torch.distributions import Normal
 from torch.quasirandom import SobolEngine
 
+TGenInitialConditions = Callable[
+    [
+        # reasoning behind this annotation: contravariance
+        qKnowledgeGradient,
+        Tensor,
+        int,
+        int,
+        int,
+        Optional[Dict[int, float]],
+        Optional[Dict[str, Union[bool, float, int]]],
+        Optional[List[Tuple[Tensor, Tensor, float]]],
+        Optional[List[Tuple[Tensor, Tensor, float]]],
+    ],
+    Optional[Tensor],
+]
 
-@contextmanager
-def manual_seed(seed: Optional[int] = None) -> Generator[None, None, None]:
-    r"""Contextmanager for manual setting the torch.random seed.
+
+def transform_constraints(
+    constraints: Union[List[Tuple[Tensor, Tensor, float]], None], q: int, d: int
+) -> List[Tuple[Tensor, Tensor, float]]:
+    r"""Transform constraints to sample from a d*q-dimensional space instead of a
+    d-dimensional state.
+
+    This function assumes that constraints are the same for each input batch,
+    and broadcasts the constraints accordingly to the input batch shape.
 
     Args:
-        seed: The seed to set the random number generator to.
+        constraints: A list of tuples (indices, coefficients, rhs), with each tuple
+            encoding an (in-)equality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) (>)= rhs`.
+            If `indices` is a 2-d Tensor, this supports specifying constraints across
+            the points in the `q`-batch (inter-point constraints). If `None`, this
+            function is a nullop and simply returns `None`.
+        q: Size of the `q`-batch.
+        d: Dimensionality of the problem.
 
     Returns:
-        Generator
-
-    Example:
-        >>> with manual_seed(1234):
-        >>>     X = torch.rand(3)
+        List[Tuple[Tensor, Tensor, float]]: List of transformed constraints.
     """
-    old_state = torch.random.get_rng_state()
-    try:
-        if seed is not None:
-            torch.random.manual_seed(seed)
-        yield
-    finally:
-        if seed is not None:
-            torch.random.set_rng_state(old_state)
+    if constraints is None:
+        return None
+    transformed = []
+    for constraint in constraints:
+        if len(constraint[0].shape) == 1:
+            transformed += transform_intra_point_constraint(constraint, d, q)
+        else:
+            transformed.append(transform_inter_point_constraint(constraint, d))
+    return transformed
 
 
-def draw_sobol_samples(
-    bounds: Tensor,
-    n: int,
-    q: int,
-    batch_shape: Optional[Iterable[int], torch.Size] = None,
-    seed: Optional[int] = None,
-) -> Tensor:
-    r"""Draw qMC samples from the box defined by bounds.
+def transform_intra_point_constraint(
+    constraint: Tuple[Tensor, Tensor, float], d: int, q: int
+) -> List[Tuple[Tensor, Tensor, float]]:
+    r"""Transforms an intra-point/pointwise constraint from
+    d-dimensional space to a d*q-dimesional space.
 
     Args:
-        bounds: A `2 x d` dimensional tensor specifying box constraints on a
-            `d`-dimensional space, where bounds[0, :] and bounds[1, :] correspond
-            to lower and upper bounds, respectively.
-        n: The number of (q-batch) samples. As a best practice, use powers of 2.
-        q: The size of each q-batch.
-        batch_shape: The batch shape of the samples. If given, returns samples
-            of shape `n x batch_shape x q x d`, where each batch is an
-            `n x q x d`-dim tensor of qMC samples.
-        seed: The seed used for initializing Owen scrambling. If None (default),
-            use a random seed.
+        constraints: A list of tuples (indices, coefficients, rhs), with each tuple
+            encoding an (in-)equality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) (>)= rhs`. Here `indices` must
+            be one-dimensional, and the constraint is applied to all points within the
+            `q`-batch.
+        d: Dimensionality of the problem.
+
+    Raises:
+        ValueError: If indices in the constraints are larger than the
+            dimensionality d of the problem.
 
     Returns:
-        A `n x batch_shape x q x d`-dim tensor of qMC samples from the box
-        defined by bounds.
-
-    Example:
-        >>> bounds = torch.stack([torch.zeros(3), torch.ones(3)])
-        >>> samples = draw_sobol_samples(bounds, 16, 2)
+        List[Tuple[Tensor, Tensor, float]]: List of transformed constraints.
     """
-    batch_shape = batch_shape or torch.Size()
-    batch_size = int(torch.prod(torch.tensor(batch_shape)))
-    d = bounds.shape[-1]
-    lower = bounds[0]
-    rng = bounds[1] - bounds[0]
-    sobol_engine = SobolEngine(q * d, scramble=True, seed=seed)
-    samples_raw = sobol_engine.draw(batch_size * n, dtype=lower.dtype)
-    samples_raw = samples_raw.view(*batch_shape, n, q, d).to(device=lower.device)
-    if batch_shape != torch.Size():
-        samples_raw = samples_raw.permute(-3, *range(len(batch_shape)), -2, -1)
-    return lower + rng * samples_raw
+    indices, coefficients, rhs = constraint
+    if indices.max() >= d:
+        raise ValueError(
+            f"Constraint indices cannot exceed the problem dimension {d=}."
+        )
+    return [
+        (
+            torch.tensor(
+                [i * d + j for j in indices], dtype=torch.int64, device=indices.device
+            ),
+            coefficients,
+            rhs,
+        )
+        for i in range(q)
+    ]
 
 
-def draw_sobol_normal_samples(
-    d: int,
-    n: int,
-    device: Optional[torch.device] = None,
-    dtype: Optional[torch.dtype] = None,
-    seed: Optional[int] = None,
-) -> Tensor:
-    r"""Draw qMC samples from a multi-variate standard normal N(0, I_d).
-
-    A primary use-case for this functionality is to compute an QMC average
-    of f(X) over X where each element of X is drawn N(0, 1).
+def transform_inter_point_constraint(
+    constraint: Tuple[Tensor, Tensor, float], d: int
+) -> Tuple[Tensor, Tensor, float]:
+    r"""Transforms an inter-point constraint from
+    d-dimensional space to a d*q dimesional space.
 
     Args:
-        d: The dimension of the normal distribution.
-        n: The number of samples to return. As a best practice, use powers of 2.
-        device: The torch device.
-        dtype:  The torch dtype.
-        seed: The seed used for initializing Owen scrambling. If None (default),
-            use a random seed.
+        constraints: A list of tuples (indices, coefficients, rhs), with each tuple
+            encoding an (in-)equality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) (>)= rhs`. `indices` must be a
+            2-d Tensor, where in each row `indices[i] = (k_i, l_i)` the first index
+            `k_i` corresponds to the `k_i`-th element of the `q`-batch and the second
+            index `l_i` corresponds to the `l_i`-th feature of that element.
+
+    Raises:
+        ValueError: If indices in the constraints are larger than the
+            dimensionality d of the problem.
 
     Returns:
-        A tensor of qMC standard normal samples with dimension `n x d` with device
-        and dtype specified by the input.
-
-    Example:
-        >>> samples = draw_sobol_normal_samples(2, 16)
+        List[Tuple[Tensor, Tensor, float]]: Transformed constraint.
     """
-    normal_qmc_engine = NormalQMCEngine(d=d, seed=seed, inv_transform=True)
-    samples = normal_qmc_engine.draw(n, dtype=torch.float if dtype is None else dtype)
-    return samples.to(device=device)
+    indices, coefficients, rhs = constraint
+    if indices[:, 1].max() >= d:
+        raise ValueError(
+            f"Constraint indices cannot exceed the problem dimension {d=}."
+        )
+    return (
+        torch.tensor(
+            [r[0] * d + r[1] for r in indices], dtype=torch.int64, device=indices.device
+        ),
+        coefficients,
+        rhs,
+    )
 
 
-def sample_hypersphere(
-    d: int,
-    n: int = 1,
-    qmc: bool = False,
-    seed: Optional[int] = None,
-    device: Optional[torch.device] = None,
-    dtype: Optional[torch.dtype] = None,
+def sample_q_batches_from_polytope(
+    n: int,
+    q: int,
+    bounds: Tensor,
+    n_burnin: int,
+    thinning: int,
+    seed: int,
+    inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
 ) -> Tensor:
-    r"""Sample uniformly from a unit d-sphere.
+    r"""Samples `n` q-baches from a polytope of dimension `d`.
 
     Args:
-        d: The dimension of the hypersphere.
-        n: The number of samples to return.
-        qmc: If True, use QMC Sobol sampling (instead of i.i.d. uniform).
-        seed: If provided, use as a seed for the RNG.
-        device: The torch device.
-        dtype:  The torch dtype.
+        n: Number of q-batches to sample.
+        q: Number of samples per q-batch
+        bounds: A `2 x d` tensor of lower and upper bounds for each column of `X`.
+        n_burnin: The number of burn-in samples for the Markov chain sampler.
+            thinning: The amount of thinning (number of steps to take between
+            returning samples).
+        seed: The random seed.
+        inequality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
+        equality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
 
     Returns:
-        An  `n x d` tensor of uniform samples from from the d-hypersphere.
-
-    Example:
-        >>> sample_hypersphere(d=5, n=10)
+        A `n x q x d`-dim tensor of samples.
     """
-    dtype = torch.float if dtype is None else dtype
-    if d == 1:
-        rnd = torch.randint(0, 2, (n, 1), device=device, dtype=dtype)
-        return 2 * rnd - 1
-    if qmc:
-        rnd = draw_sobol_normal_samples(d=d, n=n, device=device, dtype=dtype, seed=seed)
+
+    # check if inter-point constraints are present
+    inter_point = any(
+        len(indices.shape) > 1
+        for constraints in (inequality_constraints or [], equality_constraints or [])
+        for indices, _, _ in constraints
+    )
+
+    if inter_point:
+        samples = get_polytope_samples(
+            n=n,
+            bounds=torch.hstack([bounds for _ in range(q)]),
+            inequality_constraints=transform_constraints(
+                constraints=inequality_constraints, q=q, d=bounds.shape[1]
+            ),
+            equality_constraints=transform_constraints(
+                constraints=equality_constraints, q=q, d=bounds.shape[1]
+            ),
+            seed=seed,
+            n_burnin=n_burnin,
+            thinning=thinning * q,
+        )
     else:
-        with manual_seed(seed=seed):
-            rnd = torch.randn(n, d, dtype=dtype)
-    samples = rnd / torch.norm(rnd, dim=-1, keepdim=True)
-    if device is not None:
-        samples = samples.to(device)
-    return samples
+        samples = get_polytope_samples(
+            n=n * q,
+            bounds=bounds,
+            inequality_constraints=inequality_constraints,
+            equality_constraints=equality_constraints,
+            seed=seed,
+            n_burnin=n_burnin,
+            thinning=thinning,
+        )
+    return samples.view(n, q, -1).cpu()
 
 
-def sample_simplex(
-    d: int,
-    n: int = 1,
-    qmc: bool = False,
-    seed: Optional[int] = None,
-    device: Optional[torch.device] = None,
-    dtype: Optional[torch.dtype] = None,
+def gen_batch_initial_conditions(
+    acq_function: AcquisitionFunction,
+    bounds: Tensor,
+    q: int,
+    num_restarts: int,
+    raw_samples: int,
+    fixed_features: Optional[Dict[int, float]] = None,
+    options: Optional[Dict[str, Union[bool, float, int]]] = None,
+    inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    generator: Optional[Callable[[int, int, int], Tensor]] = None,
 ) -> Tensor:
-    r"""Sample uniformly from a d-simplex.
+    r"""Generate a batch of initial conditions for random-restart optimziation.
+
+    TODO: Support t-batches of initial conditions.
 
     Args:
-        d: The dimension of the simplex.
-        n: The number of samples to return.
-        qmc: If True, use QMC Sobol sampling (instead of i.i.d. uniform).
-        seed: If provided, use as a seed for the RNG.
-        device: The torch device.
-        dtype: The torch dtype.
+        acq_function: The acquisition function to be optimized.
+        bounds: A `2 x d` tensor of lower and upper bounds for each column of `X`.
+        q: The number of candidates to consider.
+        num_restarts: The number of starting points for multistart acquisition
+            function optimization.
+        raw_samples: The number of raw samples to consider in the initialization
+            heuristic. Note: if `sample_around_best` is True (the default is False),
+            then `2 * raw_samples` samples are used.
+        fixed_features: A map `{feature_index: value}` for features that
+            should be fixed to a particular value during generation.
+        options: Options for initial condition generation. For valid options see
+            `initialize_q_batch` and `initialize_q_batch_nonneg`. If `options`
+            contains a `nonnegative=True` entry, then `acq_function` is
+            assumed to be non-negative (useful when using custom acquisition
+            functions). In addition, an "init_batch_limit" option can be passed
+            to specify the batch limit for the initialization. This is useful
+            for avoiding memory limits when computing the batch posterior over
+            raw samples.
+        inequality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
+        equality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+        generator: Callable for generating samples that are then further
+            processed. It receives `n`, `q` and `seed` as arguments and
+            returns a tensor of shape `n x q x d`.
 
     Returns:
-        An `n x d` tensor of uniform samples from from the d-simplex.
+        A `num_restarts x q x d` tensor of initial conditions.
 
     Example:
-        >>> sample_simplex(d=3, n=10)
+        >>> qEI = qExpectedImprovement(model, best_f=0.2)
+        >>> bounds = torch.tensor([[0.], [1.]])
+        >>> Xinit = gen_batch_initial_conditions(
+        >>>     qEI, bounds, q=3, num_restarts=25, raw_samples=500
+        >>> )
     """
-    dtype = torch.float if dtype is None else dtype
-    if d == 1:
-        return torch.ones(n, 1, device=device, dtype=dtype)
-    if qmc:
-        sobol_engine = SobolEngine(d - 1, scramble=True, seed=seed)
-        rnd = sobol_engine.draw(n, dtype=dtype)
+    if bounds.isinf().any():
+        raise NotImplementedError(
+            "Currently only finite values in `bounds` are supported "
+            "for generating initial conditions for optimization."
+        )
+    options = options or {}
+    sample_around_best = options.get("sample_around_best", False)
+    if sample_around_best and equality_constraints:
+        raise UnsupportedError(
+            "Option 'sample_around_best' is not supported when equality"
+            "constraints are present."
+        )
+    if sample_around_best and generator:
+        raise UnsupportedError(
+            "Option 'sample_around_best' is not supported when custom "
+            "generator is be used."
+        )
+    seed: Optional[int] = options.get("seed")
+    batch_limit: Optional[int] = options.get(
+        "init_batch_limit", options.get("batch_limit")
+    )
+    factor, max_factor = 1, 5
+    init_kwargs = {}
+    device = bounds.device
+    bounds_cpu = bounds.cpu()
+    if "eta" in options:
+        init_kwargs["eta"] = options.get("eta")
+    if options.get("nonnegative") or is_nonnegative(acq_function):
+        init_func = initialize_q_batch_nonneg
+        if "alpha" in options:
+            init_kwargs["alpha"] = options.get("alpha")
     else:
-        with manual_seed(seed=seed):
-            rnd = torch.rand(n, d - 1, dtype=dtype)
-    srnd, _ = torch.sort(rnd, dim=-1)
-    zeros = torch.zeros(n, 1, dtype=dtype)
-    ones = torch.ones(n, 1, dtype=dtype)
-    srnd = torch.cat([zeros, srnd, ones], dim=-1)
-    if device is not None:
-        srnd = srnd.to(device)
-    return srnd[..., 1:] - srnd[..., :-1]
-
-
-def sample_polytope(
-    A: Tensor,
-    b: Tensor,
-    x0: Tensor,
-    n: int = 10000,
-    n0: int = 100,
-    seed: Optional[int] = None,
-) -> Tensor:
-    r"""
-    Hit and run sampler from uniform sampling points from a polytope,
-    described via inequality constraints A*x<=b.
-
-    Args:
-        A: A Tensor describing inequality constraints
-            so that all samples satisfy Ax<=b.
-        b: A Tensor describing the inequality constraints
-            so that all samples satisfy Ax<=b.
-        x0: A `d`-dim Tensor representing a starting point of the chain
-            satisfying the constraints.
-        n: The number of resulting samples kept in the output.
-        n0: The number of burn-in samples. The chain will produce
-            n+n0 samples but the first n0 samples are not saved.
-        seed: The seed for the sampler. If omitted, use a random seed.
-
-    Returns:
-        (n, d) dim Tensor containing the resulting samples.
-    """
-    n_tot = n + n0
-    seed = seed if seed is not None else torch.randint(0, 1000000, (1,)).item()
-    with manual_seed(seed=seed):
-        rands = torch.rand(n_tot, dtype=A.dtype, device=A.device)
-
-    # pre-sample samples from hypersphere
-    d = x0.size(0)
-    # uniform samples from unit ball in d dims
-    Rs = sample_hypersphere(d=d, n=n_tot, dtype=A.dtype, device=A.device).unsqueeze(-1)
-
-    # compute matprods in batch
-    ARs = (A @ Rs).squeeze(-1)
-    out = torch.empty(n, A.size(-1), dtype=A.dtype, device=A.device)
-    x = x0.clone()
-    for i, (ar, r, rnd) in enumerate(zip(ARs, Rs, rands)):
-        # given x, the next point in the chain is x+alpha*r
-        # it also satisfies A(x+alpha*r)<=b which implies A*alpha*r<=b-Ax
-        # so alpha<=(b-Ax)/ar for ar>0, and alpha>=(b-Ax)/ar for ar<0.
-        # b - A @ x is always >= 0, clamping for numerical tolerances
-        w = (b - A @ x).squeeze().clamp(min=0.0) / ar
-        pos = w >= 0
-        alpha_max = w[pos].min()
-        # important to include equality here in cases x is at the boundary
-        # of the polytope
-        neg = w <= 0
-        alpha_min = w[neg].max()
-        # alpha~Unif[alpha_min, alpha_max]
-        alpha = alpha_min + rnd * (alpha_max - alpha_min)
-        x = x + alpha * r
-        if i >= n0:  # save samples after burn-in period
-            out[i - n0] = x.squeeze()
-    return out
-
-
-def batched_multinomial(
-    weights: Tensor,
-    num_samples: int,
-    replacement: bool = False,
-    generator: Optional[torch.Generator] = None,
-    out: Optional[Tensor] = None,
-) -> LongTensor:
-    r"""Sample from multinomial with an arbitrary number of batch dimensions.
-
-    Args:
-        weights: A `batch_shape x num_categories` tensor of weights. For each batch
-            index `i, j, ...`, this functions samples from a multinomial with `input`
-            `weights[i, j, ..., :]`. Note that the weights need not sum to one, but must
-            be non-negative, finite and have a non-zero sum.
-        num_samples: The number of samples to draw for each batch index. Must be smaller
-            than `num_categories` if `replacement=False`.
-        replacement: If True, samples are drawn with replacement.
-        generator: A a pseudorandom number generator for sampling.
-        out: The output tensor (optional). If provided, must be of size
-            `batch_shape x num_samples`.
-
-    Returns:
-        A `batch_shape x num_samples` tensor of samples.
-
-    This is a thin wrapper around `torch.multinomial` that allows weight (`input`)
-    tensors with an arbitrary number of batch dimensions (`torch.multinomial` only
-    allows a single batch dimension). The calling signature is the same as for
-    `torch.multinomial`.
+        init_func = initialize_q_batch
 
-    Example:
-        >>> weights = torch.rand(2, 3, 10)
-        >>> samples = batched_multinomial(weights, 4)  # shape is 2 x 3 x 4
-    """
-    batch_shape, n_categories = weights.shape[:-1], weights.size(-1)
-    flat_samples = torch.multinomial(
-        input=weights.view(-1, n_categories),
-        num_samples=num_samples,
-        replacement=replacement,
-        generator=generator,
-        out=None if out is None else out.view(-1, num_samples),
+    q = 1 if q is None else q
+    # the dimension the samples are drawn from
+    effective_dim = bounds.shape[-1] * q
+    if effective_dim > SobolEngine.MAXDIM and settings.debug.on():
+        warnings.warn(
+            f"Sample dimension q*d={effective_dim} exceeding Sobol max dimension "
+            f"({SobolEngine.MAXDIM}). Using iid samples instead.",
+            SamplingWarning,
+        )
+
+    while factor < max_factor:
+        with warnings.catch_warnings(record=True) as ws:
+            n = raw_samples * factor
+            if generator is not None:
+                X_rnd = generator(n, q, seed)
+            elif inequality_constraints is None and equality_constraints is None:
+                if effective_dim <= SobolEngine.MAXDIM:
+                    X_rnd = draw_sobol_samples(bounds=bounds_cpu, n=n, q=q, seed=seed)
+                else:
+                    with manual_seed(seed):
+                        # load on cpu
+                        X_rnd_nlzd = torch.rand(
+                            n, q, bounds_cpu.shape[-1], dtype=bounds.dtype
+                        )
+                    X_rnd = bounds_cpu[0] + (bounds_cpu[1] - bounds_cpu[0]) * X_rnd_nlzd
+            else:
+                X_rnd = sample_q_batches_from_polytope(
+                    n=n,
+                    q=q,
+                    bounds=bounds,
+                    n_burnin=options.get("n_burnin", 10000),
+                    thinning=options.get("thinning", 32),
+                    seed=seed,
+                    equality_constraints=equality_constraints,
+                    inequality_constraints=inequality_constraints,
+                )
+            # sample points around best
+            if sample_around_best:
+                X_best_rnd = sample_points_around_best(
+                    acq_function=acq_function,
+                    n_discrete_points=n * q,
+                    sigma=options.get("sample_around_best_sigma", 1e-3),
+                    bounds=bounds,
+                    subset_sigma=options.get("sample_around_best_subset_sigma", 1e-1),
+                    prob_perturb=options.get("sample_around_best_prob_perturb"),
+                )
+                if X_best_rnd is not None:
+                    X_rnd = torch.cat(
+                        [
+                            X_rnd,
+                            X_best_rnd.view(n, q, bounds.shape[-1]).cpu(),
+                        ],
+                        dim=0,
+                    )
+            X_rnd = fix_features(X_rnd, fixed_features=fixed_features)
+            with torch.no_grad():
+                if batch_limit is None:
+                    batch_limit = X_rnd.shape[0]
+                Y_rnd_list = []
+                start_idx = 0
+                while start_idx < X_rnd.shape[0]:
+                    end_idx = min(start_idx + batch_limit, X_rnd.shape[0])
+                    Y_rnd_curr = acq_function(
+                        X_rnd[start_idx:end_idx].to(device=device)
+                    ).cpu()
+                    Y_rnd_list.append(Y_rnd_curr)
+                    start_idx += batch_limit
+                Y_rnd = torch.cat(Y_rnd_list)
+            batch_initial_conditions = init_func(
+                X=X_rnd, Y=Y_rnd, n=num_restarts, **init_kwargs
+            ).to(device=device)
+            if not any(issubclass(w.category, BadInitialCandidatesWarning) for w in ws):
+                return batch_initial_conditions
+            if factor < max_factor:
+                factor += 1
+                if seed is not None:
+                    seed += 1  # make sure to sample different X_rnd
+    warnings.warn(
+        "Unable to find non-zero acquisition function values - initial conditions "
+        "are being selected randomly.",
+        BadInitialCandidatesWarning,
     )
-    return flat_samples.view(*batch_shape, num_samples)
+    return batch_initial_conditions
 
 
-def _convert_bounds_to_inequality_constraints(bounds: Tensor) -> Tuple[Tensor, Tensor]:
-    r"""Convert bounds into inequality constraints of the form Ax <= b.
+def gen_one_shot_kg_initial_conditions(
+    acq_function: qKnowledgeGradient,
+    bounds: Tensor,
+    q: int,
+    num_restarts: int,
+    raw_samples: int,
+    fixed_features: Optional[Dict[int, float]] = None,
+    options: Optional[Dict[str, Union[bool, float, int]]] = None,
+    inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+) -> Optional[Tensor]:
+    r"""Generate a batch of smart initializations for qKnowledgeGradient.
+
+    This function generates initial conditions for optimizing one-shot KG using
+    the maximizer of the posterior objective. Intutively, the maximizer of the
+    fantasized posterior will often be close to a maximizer of the current
+    posterior. This function uses that fact to generate the initital conditions
+    for the fantasy points. Specifically, a fraction of `1 - frac_random` (see
+    options) is generated by sampling from the set of maximizers of the
+    posterior objective (obtained via random restart optimization) according to
+    a softmax transformation of their respective values. This means that this
+    initialization strategy internally solves an acquisition function
+    maximization problem. The remaining `frac_random` fantasy points as well as
+    all `q` candidate points are chosen according to the standard initialization
+    strategy in `gen_batch_initial_conditions`.
 
     Args:
-        bounds: A `2 x d`-dim tensor of bounds
+        acq_function: The qKnowledgeGradient instance to be optimized.
+        bounds: A `2 x d` tensor of lower and upper bounds for each column of
+            task features.
+        q: The number of candidates to consider.
+        num_restarts: The number of starting points for multistart acquisition
+            function optimization.
+        raw_samples: The number of raw samples to consider in the initialization
+            heuristic.
+        fixed_features: A map `{feature_index: value}` for features that
+            should be fixed to a particular value during generation.
+        options: Options for initial condition generation. These contain all
+            settings for the standard heuristic initialization from
+            `gen_batch_initial_conditions`. In addition, they contain
+            `frac_random` (the fraction of fully random fantasy points),
+            `num_inner_restarts` and `raw_inner_samples` (the number of random
+            restarts and raw samples for solving the posterior objective
+            maximization problem, respectively) and `eta` (temperature parameter
+            for sampling heuristic from posterior objective maximizers).
+        inequality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
+        equality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
 
     Returns:
-        A two-element tuple containing
-            - A: A `2d x d`-dim tensor of coefficients
-            - b: A `2d x 1`-dim tensor containing the right hand side
-    """
-    d = bounds.shape[-1]
-    eye = torch.eye(d, dtype=bounds.dtype, device=bounds.device)
-    lower, upper = bounds
-    lower_finite, upper_finite = bounds.isfinite()
-    A = torch.cat([-eye[lower_finite], eye[upper_finite]], dim=0)
-    b = torch.cat([-lower[lower_finite], upper[upper_finite]], dim=0).unsqueeze(-1)
-    return A, b
-
-
-def find_interior_point(
-    A: np.ndarray,
-    b: np.ndarray,
-    A_eq: Optional[np.ndarray] = None,
-    b_eq: Optional[np.ndarray] = None,
-) -> np.ndarray:
-    r"""Find an interior point of a polytope via linear programming.
-
-    Args:
-        A: A `n_ineq x d`-dim numpy array containing the coefficients of the
-            constraint inequalities.
-        b: A `n_ineq x 1`-dim numpy array containing the right hand sides of
-            the constraint inequalities.
-        A_eq: A `n_eq x d`-dim numpy array containing the coefficients of the
-            constraint equalities.
-        b_eq: A `n_eq x 1`-dim numpy array containing the right hand sides of
-            the constraint equalities.
-
-    Returns:
-        A `d`-dim numpy array containing an interior point of the polytope.
-        This function will raise a ValueError if there is no such point.
-
-    This method solves the following Linear Program:
-
-        min -s subject to A @ x <= b - 2 * s, s >= 0, A_eq @ x = b_eq
-
-    In case the polytope is unbounded, then it will also constrain the slack
-    variable `s` to `s<=1`.
-    """
-    # augment inequality constraints: A @ (x, s) <= b
-    d = A.shape[-1]
-    ncon = A.shape[-2] + 1
-    c = np.zeros(d + 1)
-    c[-1] = -1
-    b_ub = np.zeros(ncon)
-    b_ub[:-1] = b.reshape(-1)
-    A_ub = np.zeros((ncon, d + 1))
-    A_ub[:-1, :-1] = A
-    A_ub[:-1, -1] = 2.0
-    A_ub[-1, -1] = -1.0
-
-    result = scipy.optimize.linprog(
-        c=c,
-        A_ub=A_ub,
-        b_ub=b_ub,
-        A_eq=A_eq,
-        b_eq=b_eq,
-        bounds=(None, None),
-        method="highs",
-    )
-
-    if result.status == 3:
-        # problem is unbounded - to find a bounded solution we constrain the
-        # slack variable `s` to `s <= 1.0`.
-        A_s = np.concatenate([np.zeros((1, d)), np.ones((1, 1))], axis=-1)
-        A_ub = np.concatenate([A_ub, A_s], axis=0)
-        b_ub = np.concatenate([b_ub, np.ones(1)], axis=-1)
-        result = scipy.optimize.linprog(
-            c=c,
-            A_ub=A_ub,
-            b_ub=b_ub,
-            A_eq=A_eq,
-            b_eq=b_eq,
-            bounds=(None, None),
-            method="highs",
-        )
+        A `num_restarts x q' x d` tensor that can be used as initial conditions
+        for `optimize_acqf()`. Here `q' = q + num_fantasies` is the total number
+        of points (candidate points plus fantasy points).
 
-    if result.status == 2:
-        raise ValueError(
-            "No feasible point found. Constraint polytope appears empty. "
-            + "Check your constraints."
-        )
-    elif result.status > 0:
+    Example:
+        >>> qKG = qKnowledgeGradient(model, num_fantasies=64)
+        >>> bounds = torch.tensor([[0., 0.], [1., 1.]])
+        >>> Xinit = gen_one_shot_kg_initial_conditions(
+        >>>     qKG, bounds, q=3, num_restarts=10, raw_samples=512,
+        >>>     options={"frac_random": 0.25},
+        >>> )
+    """
+    options = options or {}
+    frac_random: float = options.get("frac_random", 0.1)
+    if not 0 < frac_random < 1:
         raise ValueError(
-            "Problem checking constraint specification. "
-            + "linprog status: {}".format(result.message)
+            f"frac_random must take on values in (0,1). Value: {frac_random}"
         )
-    # the x in the result is really (x, s)
-    return result.x[:-1]
+    q_aug = acq_function.get_augmented_q_batch_size(q=q)
 
+    # TODO: Avoid unnecessary computation by not generating all candidates
+    ics = gen_batch_initial_conditions(
+        acq_function=acq_function,
+        bounds=bounds,
+        q=q_aug,
+        num_restarts=num_restarts,
+        raw_samples=raw_samples,
+        fixed_features=fixed_features,
+        options=options,
+        inequality_constraints=inequality_constraints,
+        equality_constraints=equality_constraints,
+    )
 
-class PolytopeSampler(ABC):
-    r"""
-    Base class for samplers that sample points from a polytope.
-
-    :meta private:
-    """
-
-    def __init__(
-        self,
-        inequality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
-        equality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
-        bounds: Optional[Tensor] = None,
-        interior_point: Optional[Tensor] = None,
-    ) -> None:
-        r"""
-        Args:
-            inequality_constraints: Tensors `(A, b)` describing inequality
-                constraints `A @ x <= b`, where `A` is a `n_ineq_con x d`-dim
-                Tensor and `b` is a `n_ineq_con x 1`-dim Tensor, with `n_ineq_con`
-                the number of inequalities and `d` the dimension of the sample space.
-            equality_constraints: Tensors `(C, d)` describing the equality constraints
-                `C @ x = d`, where `C` is a `n_eq_con x d`-dim Tensor and `d` is a
-                `n_eq_con x 1`-dim Tensor with `n_eq_con` the number of equalities.
-            bounds: A `2 x d`-dim tensor of box bounds, where `inf` (`-inf`) means
-                that the respective dimension is unbounded above (below).
-            interior_point: A `d x 1`-dim Tensor presenting a point in the
-                (relative) interior of the polytope. If omitted, determined
-                automatically by solving a Linear Program.
-        """
-        if inequality_constraints is None:
-            if bounds is None:
-                raise BotorchError(
-                    "PolytopeSampler requires either inequality constraints or bounds."
-                )
-            A = torch.empty(
-                0, bounds.shape[-1], dtype=bounds.dtype, device=bounds.device
-            )
-            b = torch.empty(0, 1, dtype=bounds.dtype, device=bounds.device)
-        else:
-            A, b = inequality_constraints
-        if bounds is not None:
-            # add inequality constraints for bounds
-            # TODO: make sure there are not deduplicate constraints
-            A2, b2 = _convert_bounds_to_inequality_constraints(bounds=bounds)
-            A = torch.cat([A, A2], dim=0)
-            b = torch.cat([b, b2], dim=0)
-        self.A = A
-        self.b = b
-        self.equality_constraints = equality_constraints
-
-        if equality_constraints is not None:
-            self.C, self.d = equality_constraints
-            U, S, Vh = torch.linalg.svd(self.C)
-            r = torch.nonzero(S).size(0)  # rank of matrix C
-            self.nullC = Vh[r:, :].transpose(-1, -2)  # orthonormal null space of C,
-            # satisfying # C @ nullC = 0 and nullC.T @ nullC = I
-            # using the change of variables x=x0+nullC*y,
-            # sample y satisfies A*nullC*y<=b-A*x0.
-            # the linear constraint is automatically satisfied as x0 satisfies it.
-        else:
-            self.C = None
-            self.d = None
-            self.nullC = torch.eye(
-                self.A.size(-1), dtype=self.A.dtype, device=self.A.device
-            )
+    # compute maximizer of the value function
+    value_function = _get_value_function(
+        model=acq_function.model,
+        objective=acq_function.objective,
+        posterior_transform=acq_function.posterior_transform,
+        sampler=acq_function.inner_sampler,
+        project=getattr(acq_function, "project", None),
+    )
+    from botorch.optim.optimize import optimize_acqf
 
-        self.new_A = self.A @ self.nullC  # doesn't depend on the initial point
+    fantasy_cands, fantasy_vals = optimize_acqf(
+        acq_function=value_function,
+        bounds=bounds,
+        q=1,
+        num_restarts=options.get("num_inner_restarts", 20),
+        raw_samples=options.get("raw_inner_samples", 1024),
+        fixed_features=fixed_features,
+        return_best_only=False,
+        inequality_constraints=inequality_constraints,
+        equality_constraints=equality_constraints,
+    )
 
-        # initial point for the original, not transformed, problem
-        if interior_point is not None:
-            if self.feasible(interior_point):
-                self.x0 = interior_point
-            else:
-                raise ValueError("The given input point is not feasible.")
-        else:
-            self.x0 = self.find_interior_point()
+    # sampling from the optimizers
+    n_value = int((1 - frac_random) * (q_aug - q))  # number of non-random ICs
+    eta = options.get("eta", 2.0)
+    weights = torch.exp(eta * standardize(fantasy_vals))
+    idx = torch.multinomial(weights, num_restarts * n_value, replacement=True)
+
+    # set the respective initial conditions to the sampled optimizers
+    ics[..., -n_value:, :] = fantasy_cands[idx, 0].view(num_restarts, n_value, -1)
+    return ics
 
-    def feasible(self, x: Tensor) -> bool:
-        r"""Check whether a point is contained in the polytope.
 
-        Args:
-            x: A `d x 1`-dim Tensor.
+def gen_value_function_initial_conditions(
+    acq_function: AcquisitionFunction,
+    bounds: Tensor,
+    num_restarts: int,
+    raw_samples: int,
+    current_model: Model,
+    fixed_features: Optional[Dict[int, float]] = None,
+    options: Optional[Dict[str, Union[bool, float, int]]] = None,
+) -> Tensor:
+    r"""Generate a batch of smart initializations for optimizing
+    the value function of qKnowledgeGradient.
 
-        Returns:
-            True if `x` is contained inside the polytope (incl. its boundary),
-            False otherwise.
-        """
-        ineq = (self.A @ x - self.b <= 0).all()
-        if self.equality_constraints is not None:
-            eq = (self.C @ x - self.d == 0).all()
-            return ineq & eq
-        return ineq
-
-    def find_interior_point(self) -> Tensor:
-        r"""Find an interior point of the polytope.
-
-        Returns:
-            A `d x 1`-dim Tensor representing a point contained in the polytope.
-            This function will raise a ValueError if there is no such point.
-        """
-        if self.equality_constraints:
-            # equality constraints: A_eq * (x, s) = b_eq
-            A_eq = np.zeros((self.C.size(0), self.C.size(-1) + 1))
-            A_eq[:, :-1] = self.C.cpu().numpy()
-            b_eq = self.d.cpu().numpy()
-        else:
-            A_eq = None
-            b_eq = None
-        x0 = find_interior_point(
-            A=self.A.cpu().numpy(), b=self.b.cpu().numpy(), A_eq=A_eq, b_eq=b_eq
-        )
-        return torch.from_numpy(x0).to(self.A).unsqueeze(-1)
-
-    # -------- Abstract methods to be implemented by subclasses -------- #
-
-    @abstractmethod
-    def draw(self, n: int = 1, seed: Optional[int] = None) -> Tensor:
-        r"""Draw samples from the polytope.
-
-        Args:
-            n: The number of samples.
-            seed: The random seed.
-
-        Returns:
-            A `n x d` Tensor of samples from the polytope.
-        """
-        pass  # pragma: no cover
-
-
-class HitAndRunPolytopeSampler(PolytopeSampler):
-    r"""A sampler for sampling from a polyope using a hit-and-run algorithm."""
-
-    def __init__(
-        self,
-        inequality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
-        equality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
-        bounds: Optional[Tensor] = None,
-        interior_point: Optional[Tensor] = None,
-        n_burnin: int = 0,
-    ) -> None:
-        r"""A sampler for sampling from a polyope using a hit-and-run algorithm.
-
-        Args:
-            inequality_constraints: Tensors `(A, b)` describing inequality
-                constraints `A @ x <= b`, where `A` is a `n_ineq_con x d`-dim
-                Tensor and `b` is a `n_ineq_con x 1`-dim Tensor, with `n_ineq_con`
-                the number of inequalities and `d` the dimension of the sample space.
-            equality_constraints: Tensors `(C, d)` describing the equality constraints
-                `C @ x = d`, where `C` is a `n_eq_con x d`-dim Tensor and `d` is a
-                `n_eq_con x 1`-dim Tensor with `n_eq_con` the number of equalities.
-            bounds: A `2 x d`-dim tensor of box bounds, where `inf` (`-inf`) means
-                that the respective dimension is unbounded from above (below).
-            interior_point: A `d x 1`-dim Tensor representing a point in the
-                (relative) interior of the polytope. If omitted, determined
-                automatically by solving a Linear Program.
-            n_burnin: The number of burn in samples.
-        """
-        super().__init__(
-            inequality_constraints=inequality_constraints,
-            equality_constraints=equality_constraints,
-            bounds=bounds,
-            interior_point=interior_point,
+    This function generates initial conditions for optimizing the inner problem of
+    KG, i.e. its value function, using the maximizer of the posterior objective.
+    Intutively, the maximizer of the fantasized posterior will often be close to a
+    maximizer of the current posterior. This function uses that fact to generate the
+    initital conditions for the fantasy points. Specifically, a fraction of `1 -
+    frac_random` (see options) of raw samples is generated by sampling from the set of
+    maximizers of the posterior objective (obtained via random restart optimization)
+    according to a softmax transformation of their respective values. This means that
+    this initialization strategy internally solves an acquisition function
+    maximization problem. The remaining raw samples are generated using
+    `draw_sobol_samples`. All raw samples are then evaluated, and the initial
+    conditions are selected according to the standard initialization strategy in
+    'initialize_q_batch' individually for each inner problem.
+
+    Args:
+        acq_function: The value function instance to be optimized.
+        bounds: A `2 x d` tensor of lower and upper bounds for each column of
+            task features.
+        num_restarts: The number of starting points for multistart acquisition
+            function optimization.
+        raw_samples: The number of raw samples to consider in the initialization
+            heuristic.
+        current_model: The model of the KG acquisition function that was used to
+            generate the fantasy model of the value function.
+        fixed_features: A map `{feature_index: value}` for features that
+            should be fixed to a particular value during generation.
+        options: Options for initial condition generation. These contain all
+            settings for the standard heuristic initialization from
+            `gen_batch_initial_conditions`. In addition, they contain
+            `frac_random` (the fraction of fully random fantasy points),
+            `num_inner_restarts` and `raw_inner_samples` (the number of random
+            restarts and raw samples for solving the posterior objective
+            maximization problem, respectively) and `eta` (temperature parameter
+            for sampling heuristic from posterior objective maximizers).
+
+    Returns:
+        A `num_restarts x batch_shape x q x d` tensor that can be used as initial
+        conditions for `optimize_acqf()`. Here `batch_shape` is the batch shape
+        of value function model.
+
+    Example:
+        >>> fant_X = torch.rand(5, 1, 2)
+        >>> fantasy_model = model.fantasize(fant_X, SobolQMCNormalSampler(16))
+        >>> value_function = PosteriorMean(fantasy_model)
+        >>> bounds = torch.tensor([[0., 0.], [1., 1.]])
+        >>> Xinit = gen_value_function_initial_conditions(
+        >>>     value_function, bounds, num_restarts=10, raw_samples=512,
+        >>>     options={"frac_random": 0.25},
+        >>> )
+    """
+    options = options or {}
+    seed: Optional[int] = options.get("seed")
+    frac_random: float = options.get("frac_random", 0.6)
+    if not 0 < frac_random < 1:
+        raise ValueError(
+            f"frac_random must take on values in (0,1). Value: {frac_random}"
         )
-        self.n_burnin = n_burnin
 
-    def draw(self, n: int = 1, seed: Optional[int] = None) -> Tensor:
-        r"""Draw samples from the polytope.
+    # compute maximizer of the current value function
+    value_function = _get_value_function(
+        model=current_model,
+        objective=getattr(acq_function, "objective", None),
+        posterior_transform=acq_function.posterior_transform,
+        sampler=getattr(acq_function, "sampler", None),
+        project=getattr(acq_function, "project", None),
+    )
+    from botorch.optim.optimize import optimize_acqf
 
-        Args:
-            n: The number of samples.
-            seed: The random seed.
-
-        Returns:
-            A `n x d` Tensor of samples from the polytope.
-        """
-        transformed_samples = sample_polytope(
-            # run this on the cpu
-            A=self.new_A.cpu(),
-            b=(self.b - self.A @ self.x0).cpu(),
-            x0=torch.zeros((self.nullC.size(1), 1), dtype=self.A.dtype),
-            n=n,
-            n0=self.n_burnin,
-            seed=seed,
-        ).to(self.b)
-        init_shift = self.x0.transpose(-1, -2)
-        samples = init_shift + transformed_samples @ self.nullC.transpose(-1, -2)
-        # keep the last element of the resulting chain as
-        # the beginning of the next chain
-        self.x0 = samples[-1].reshape(-1, 1)
-        # reset counter so there is no burn-in for subsequent samples
-        self.n_burnin = 0
-        return samples
-
-
-class DelaunayPolytopeSampler(PolytopeSampler):
-    r"""A polytope sampler using Delaunay triangulation.
-
-    This sampler first enumerates the vertices of the constraint polytope and
-    then uses a Delaunay triangulation to tesselate its convex hull.
-
-    The sampling happens in two stages:
-    1. First, we sample from the set of hypertriangles generated by the
-    Delaunay triangulation (i.e. which hyper-triangle to draw the sample
-    from) with probabilities proportional to the triangle volumes.
-    2. Then, we sample uniformly from the chosen hypertriangle by sampling
-    uniformly from the unit simplex of the appropriate dimension, and
-    then computing the convex combination of the vertices of the
-    hypertriangle according to that draw from the simplex.
-
-    The best reference (not exactly the same, but functionally equivalent) is
-    [Trikalinos2014polytope]_. A simple R implementation is available at
-    https://github.com/gertvv/tesselample.
-    """
-
-    def __init__(
-        self,
-        inequality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
-        equality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
-        bounds: Optional[Tensor] = None,
-        interior_point: Optional[Tensor] = None,
-    ) -> None:
-        r"""Initialize DelaunayPolytopeSampler.
-
-        Args:
-            inequality_constraints: Tensors `(A, b)` describing inequality
-                constraints `A @ x <= b`, where `A` is a `n_ineq_con x d`-dim
-                Tensor and `b` is a `n_ineq_con x 1`-dim Tensor, with `n_ineq_con`
-                the number of inequalities and `d` the dimension of the sample space.
-            equality_constraints: Tensors `(C, d)` describing the equality constraints
-                `C @ x = d`, where `C` is a `n_eq_con x d`-dim Tensor and `d` is a
-                `n_eq_con x 1`-dim Tensor with `n_eq_con` the number of equalities.
-            bounds: A `2 x d`-dim tensor of box bounds, where `inf` (`-inf`) means
-                that the respective dimension is unbounded from above (below).
-            interior_point: A `d x 1`-dim Tensor representing a point in the
-                (relative) interior of the polytope. If omitted, determined
-                automatically by solving a Linear Program.
-
-        Warning: The vertex enumeration performed in this algorithm can become
-        extremely costly if there are a large number of inequalities. Similarly,
-        the triangulation can get very expensive in high dimensions. Only use
-        this algorithm for moderate dimensions / moderately complex constraint sets.
-        An alternative is the `HitAndRunPolytopeSampler`.
-        """
-        super().__init__(
-            inequality_constraints=inequality_constraints,
-            equality_constraints=equality_constraints,
-            bounds=bounds,
-            interior_point=interior_point,
+    fantasy_cands, fantasy_vals = optimize_acqf(
+        acq_function=value_function,
+        bounds=bounds,
+        q=1,
+        num_restarts=options.get("num_inner_restarts", 20),
+        raw_samples=options.get("raw_inner_samples", 1024),
+        fixed_features=fixed_features,
+        return_best_only=False,
+        options={
+            k: v
+            for k, v in options.items()
+            if k
+            not in ("frac_random", "num_inner_restarts", "raw_inner_samples", "eta")
+        },
+    )
+
+    batch_shape = acq_function.model.batch_shape
+    # sampling from the optimizers
+    n_value = int((1 - frac_random) * raw_samples)  # number of non-random ICs
+    if n_value > 0:
+        eta = options.get("eta", 2.0)
+        weights = torch.exp(eta * standardize(fantasy_vals))
+        idx = batched_multinomial(
+            weights=weights.expand(*batch_shape, -1),
+            num_samples=n_value,
+            replacement=True,
+        ).permute(-1, *range(len(batch_shape)))
+        resampled = fantasy_cands[idx]
+    else:
+        resampled = torch.empty(
+            0,
+            *batch_shape,
+            1,
+            bounds.shape[-1],
+            dtype=fantasy_cands.dtype,
+            device=fantasy_cands.device,
         )
-        # shift coordinate system to be anchored at x0
-        new_b = self.b - self.A @ self.x0
-        if self.new_A.shape[-1] < 2:
-            # if the polytope is in dim 1 (i.e. a line segment) Qhull won't work
-            tshlds = new_b / self.new_A
-            neg = self.new_A < 0
-            self.y_min = tshlds[neg].max()
-            self.y_max = tshlds[~neg].min()
-            self.dim = 1
-        else:
-            # Qhull expects inputs of the form A @ x + b <= 0, so we need to negate here
-            halfspaces = torch.cat([self.new_A, -new_b], dim=-1).cpu().numpy()
-            vertices = HalfspaceIntersection(
-                halfspaces=halfspaces, interior_point=np.zeros(self.new_A.shape[-1])
-            ).intersections
-            self.dim = vertices.shape[-1]
-            try:
-                delaunay = Delaunay(vertices)
-            except ValueError as e:
-                if "Points cannot contain NaN" in str(e):
-                    raise ValueError("Polytope is unbounded.")
-                raise e  # pragma: no cover
-            polytopes = torch.from_numpy(
-                np.array([delaunay.points[s] for s in delaunay.simplices]),
-            ).to(self.A)
-            volumes = torch.stack([torch.det(p[1:] - p[0]).abs() for p in polytopes])
-            self._polytopes = polytopes
-            self._p = volumes / volumes.sum()
-
-    def draw(self, n: int = 1, seed: Optional[int] = None) -> Tensor:
-        r"""Draw samples from the polytope.
-
-        Args:
-            n: The number of samples.
-            seed: The random seed.
-
-        Returns:
-            A `n x d` Tensor of samples from the polytope.
-        """
-        if self.dim == 1:
-            with manual_seed(seed):
-                e = torch.rand(n, 1, device=self.new_A.device, dtype=self.new_A.dtype)
-            transformed_samples = self.y_min + (self.y_max - self.y_min) * e
-        else:
-            if seed is None:
-                generator = None
-            else:
-                generator = torch.Generator(device=self.A.device)
-                generator.manual_seed(seed)
-            index_rvs = torch.multinomial(
-                self._p,
-                num_samples=n,
-                replacement=True,
-                generator=generator,
-            )
-            simplex_rvs = sample_simplex(
-                d=self.dim + 1, n=n, seed=seed, device=self.A.device, dtype=self.A.dtype
-            )
-            transformed_samples = torch.stack(
-                [rv @ self._polytopes[idx] for rv, idx in zip(simplex_rvs, index_rvs)]
-            )
-        init_shift = self.x0.transpose(-1, -2)
-        samples = init_shift + transformed_samples @ self.nullC.transpose(-1, -2)
-        return samples
+    # add qMC samples
+    randomized = draw_sobol_samples(
+        bounds=bounds, n=raw_samples - n_value, q=1, batch_shape=batch_shape, seed=seed
+    ).to(resampled)
+    # full set of raw samples
+    X_rnd = torch.cat([resampled, randomized], dim=0)
+    X_rnd = fix_features(X_rnd, fixed_features=fixed_features)
+
+    # evaluate the raw samples
+    with torch.no_grad():
+        Y_rnd = acq_function(X_rnd)
+
+    # select the restart points using the heuristic
+    return initialize_q_batch(
+        X=X_rnd, Y=Y_rnd, n=num_restarts, eta=options.get("eta", 2.0)
+    )
 
 
-def normalize_linear_constraints(
-    bounds: Tensor, constraints: List[Tuple[Tensor, Tensor, float]]
-) -> List[Tuple[Tensor, Tensor, float]]:
-    r"""Normalize linear constraints to the unit cube.
+def initialize_q_batch(X: Tensor, Y: Tensor, n: int, eta: float = 1.0) -> Tensor:
+    r"""Heuristic for selecting initial conditions for candidate generation.
+
+    This heuristic selects points from `X` (without replacement) with probability
+    proportional to `exp(eta * Z)`, where `Z = (Y - mean(Y)) / std(Y)` and `eta`
+    is a temperature parameter.
+
+    When using an acquisiton function that is non-negative and possibly zero
+    over large areas of the feature space (e.g. qEI), you should use
+    `initialize_q_batch_nonneg` instead.
 
     Args:
-        bounds (Tensor): A `2 x d`-dim tensor containing the box bounds.
-        constraints (List[Tuple[Tensor, Tensor, float]]): A list of
-            tuples (indices, coefficients, rhs), with each tuple encoding
-            an inequality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs` or
-            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+        X: A `b x batch_shape x q x d` tensor of `b` - `batch_shape` samples of
+            `q`-batches from a d`-dim feature space. Typically, these are generated
+            using qMC sampling.
+        Y: A tensor of `b x batch_shape` outcomes associated with the samples.
+            Typically, this is the value of the batch acquisition function to be
+            maximized.
+        n: The number of initial condition to be generated. Must be less than `b`.
+        eta: Temperature parameter for weighting samples.
+
+    Returns:
+        A `n x batch_shape x q x d` tensor of `n` - `batch_shape` `q`-batch initial
+        conditions, where each batch of `n x q x d` samples is selected independently.
+
+    Example:
+        >>> # To get `n=10` starting points of q-batch size `q=3`
+        >>> # for model with `d=6`:
+        >>> qUCB = qUpperConfidenceBound(model, beta=0.1)
+        >>> Xrnd = torch.rand(500, 3, 6)
+        >>> Xinit = initialize_q_batch(Xrnd, qUCB(Xrnd), 10)
     """
+    n_samples = X.shape[0]
+    batch_shape = X.shape[1:-2] or torch.Size()
+    if n > n_samples:
+        raise RuntimeError(
+            f"n ({n}) cannot be larger than the number of "
+            f"provided samples ({n_samples})"
+        )
+    elif n == n_samples:
+        return X
+
+    Ystd = Y.std(dim=0)
+    if torch.any(Ystd == 0):
+        warnings.warn(
+            "All acquisition values for raw samples points are the same for "
+            "at least one batch. Choosing initial conditions at random.",
+            BadInitialCandidatesWarning,
+        )
+        return X[torch.randperm(n=n_samples, device=X.device)][:n]
 
-    new_constraints = []
-    for index, coefficient, rhs in constraints:
-        lower, upper = bounds[:, index]
-        s = upper - lower
-        new_constraints.append(
-            (index, s * coefficient, (rhs - torch.dot(coefficient, lower)).item())
+    max_val, max_idx = torch.max(Y, dim=0)
+    Z = (Y - Y.mean(dim=0)) / Ystd
+    etaZ = eta * Z
+    weights = torch.exp(etaZ)
+    while torch.isinf(weights).any():
+        etaZ *= 0.5
+        weights = torch.exp(etaZ)
+    if batch_shape == torch.Size():
+        idcs = torch.multinomial(weights, n)
+    else:
+        idcs = batched_multinomial(
+            weights=weights.permute(*range(1, len(batch_shape) + 1), 0), num_samples=n
+        ).permute(-1, *range(len(batch_shape)))
+    # make sure we get the maximum
+    if max_idx not in idcs:
+        idcs[-1] = max_idx
+    if batch_shape == torch.Size():
+        return X[idcs]
+    else:
+        return X.gather(
+            dim=0, index=idcs.view(*idcs.shape, 1, 1).expand(n, *X.shape[1:])
         )
-    return new_constraints
 
 
-def get_polytope_samples(
-    n: int,
-    bounds: Tensor,
-    inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-    equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-    seed: Optional[int] = None,
-    thinning: int = 32,
-    n_burnin: int = 10_000,
+def initialize_q_batch_nonneg(
+    X: Tensor, Y: Tensor, n: int, eta: float = 1.0, alpha: float = 1e-4
 ) -> Tensor:
-    r"""Sample from polytope defined by box bounds and (in)equality constraints.
+    r"""Heuristic for selecting initial conditions for non-neg. acquisition functions.
 
-    This uses a hit-and-run Markov chain sampler.
+    This function is similar to `initialize_q_batch`, but designed specifically
+    for acquisition functions that are non-negative and possibly zero over
+    large areas of the feature space (e.g. qEI). All samples for which
+    `Y < alpha * max(Y)` will be ignored (assuming that `Y` contains at least
+    one positive value).
 
-    TODO: make this method return the sampler object, to avoid doing burn-in
-    every time we draw samples.
+    Args:
+        X: A `b x q x d` tensor of `b` samples of `q`-batches from a `d`-dim.
+            feature space. Typically, these are generated using qMC.
+        Y: A tensor of `b` outcomes associated with the samples. Typically, this
+            is the value of the batch acquisition function to be maximized.
+        n: The number of initial condition to be generated. Must be less than `b`.
+        eta: Temperature parameter for weighting samples.
+        alpha: The threshold (as a fraction of the maximum observed value) under
+            which to ignore samples. All input samples for which
+            `Y < alpha * max(Y)` will be ignored.
+
+    Returns:
+        A `n x q x d` tensor of `n` `q`-batch initial conditions.
+
+    Example:
+        >>> # To get `n=10` starting points of q-batch size `q=3`
+        >>> # for model with `d=6`:
+        >>> qEI = qExpectedImprovement(model, best_f=0.2)
+        >>> Xrnd = torch.rand(500, 3, 6)
+        >>> Xinit = initialize_q_batch(Xrnd, qEI(Xrnd), 10)
+    """
+    n_samples = X.shape[0]
+    if n > n_samples:
+        raise RuntimeError("n cannot be larger than the number of provided samples")
+    elif n == n_samples:
+        return X
+
+    max_val, max_idx = torch.max(Y, dim=0)
+    if torch.any(max_val <= 0):
+        warnings.warn(
+            "All acquisition values for raw sampled points are nonpositive, so "
+            "initial conditions are being selected randomly.",
+            BadInitialCandidatesWarning,
+        )
+        return X[torch.randperm(n=n_samples, device=X.device)][:n]
+
+    # make sure there are at least `n` points with positive acquisition values
+    pos = Y > 0
+    num_pos = pos.sum().item()
+    if num_pos < n:
+        # select all positive points and then fill remaining quota with randomly
+        # selected points
+        remaining_indices = (~pos).nonzero(as_tuple=False).view(-1)
+        rand_indices = torch.randperm(remaining_indices.shape[0], device=Y.device)
+        sampled_remaining_indices = remaining_indices[rand_indices[: n - num_pos]]
+        pos[sampled_remaining_indices] = 1
+        return X[pos]
+    # select points within alpha of max_val, iteratively decreasing alpha by a
+    # factor of 10 as necessary
+    alpha_pos = Y >= alpha * max_val
+    while alpha_pos.sum() < n:
+        alpha = 0.1 * alpha
+        alpha_pos = Y >= alpha * max_val
+    alpha_pos_idcs = torch.arange(len(Y), device=Y.device)[alpha_pos]
+    weights = torch.exp(eta * (Y[alpha_pos] / max_val - 1))
+    idcs = alpha_pos_idcs[torch.multinomial(weights, n)]
+    if max_idx not in idcs:
+        idcs[-1] = max_idx
+    return X[idcs]
+
+
+def sample_points_around_best(
+    acq_function: AcquisitionFunction,
+    n_discrete_points: int,
+    sigma: float,
+    bounds: Tensor,
+    best_pct: float = 5.0,
+    subset_sigma: float = 1e-1,
+    prob_perturb: Optional[float] = None,
+) -> Optional[Tensor]:
+    r"""Find best points and sample nearby points.
 
     Args:
-        n: The number of samples.
-        bounds: A `2 x d`-dim tensor containing the box bounds.
-        inequality constraints: A list of tuples (indices, coefficients, rhs),
-            with each tuple encoding an inequality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
-        equality constraints: A list of tuples (indices, coefficients, rhs),
-            with each tuple encoding an inequality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
-        seed: The random seed.
-        thinning: The amount of thinning.
-        n_burnin: The number of burn-in samples for the Markov chain sampler.
+        acq_function: The acquisition function.
+        n_discrete_points: The number of points to sample.
+        sigma: The standard deviation of the additive gaussian noise for
+            perturbing the best points.
+        bounds: A `2 x d`-dim tensor containing the bounds.
+        best_pct: The percentage of best points to perturb.
+        subset_sigma: The standard deviation of the additive gaussian
+            noise for perturbing a subset of dimensions of the best points.
+        prob_perturb: The probability of perturbing each dimension.
 
     Returns:
-        A `n x d`-dim tensor of samples.
+        An optional `n_discrete_points x d`-dim tensor containing the
+            sampled points. This is None if no baseline points are found.
     """
-    # create tensors representing linear inequality constraints
-    # of the form Ax >= b.
-    # TODO: remove this error handling functionality in a few releases.
-    # Context: BoTorch inadvertently supported indices with unusual dtypes.
-    # This is now not supported.
-    index_dtype_error = (
-        "Normalizing {var_name} failed. Check that the first "
-        "element of {var_name} is the correct dtype following "
-        "the previous IndexError."
-    )
-    if inequality_constraints:
-        # normalize_linear_constraints is called to solve this issue:
-        # https://github.com/pytorch/botorch/issues/1225
+    X = get_X_baseline(acq_function=acq_function)
+    if X is None:
+        return
+    with torch.no_grad():
         try:
-            # non-standard dtypes used to be supported for indices in constraints;
-            # this is no longer true
-            constraints = normalize_linear_constraints(bounds, inequality_constraints)
-        except IndexError as e:
-            msg = index_dtype_error.format(var_name="`inequality_constraints`")
-            raise ValueError(msg) from e
-
-        A, b = sparse_to_dense_constraints(
-            d=bounds.shape[-1],
-            constraints=constraints,
-        )
-        # Note the inequality constraints are of the form Ax >= b,
-        # but PolytopeSampler expects inequality constraints of the
-        # form Ax <= b, so we multiply by -1 below.
-        dense_inequality_constraints = -A, -b
-    else:
-        dense_inequality_constraints = None
-    if equality_constraints:
+            posterior = acq_function.model.posterior(X)
+        except AttributeError:
+            warnings.warn(
+                "Failed to sample around previous best points.",
+                BotorchWarning,
+            )
+            return
+        mean = posterior.mean
+        while mean.ndim > 2:
+            # take average over batch dims
+            mean = mean.mean(dim=0)
         try:
-            # non-standard dtypes used to be supported for indices in constraints;
-            # this is no longer true
-            constraints = normalize_linear_constraints(bounds, equality_constraints)
-        except IndexError as e:
-            msg = index_dtype_error.format(var_name="`equality_constraints`")
-            raise ValueError(msg) from e
-
-        # normalize_linear_constraints is called to solve this issue:
-        # https://github.com/pytorch/botorch/issues/1225
-        dense_equality_constraints = sparse_to_dense_constraints(
-            d=bounds.shape[-1], constraints=constraints
+            f_pred = acq_function.objective(mean)
+        # Some acquisition functions do not have an objective
+        # and for some acquisition functions the objective is None
+        except (AttributeError, TypeError):
+            f_pred = mean
+        if hasattr(acq_function, "maximize"):
+            # make sure that the optimiztaion direction is set properly
+            if not acq_function.maximize:
+                f_pred = -f_pred
+        try:
+            # handle constraints for EHVI-based acquisition functions
+            constraints = acq_function.constraints
+            if constraints is not None:
+                neg_violation = -torch.stack(
+                    [c(mean).clamp_min(0.0) for c in constraints], dim=-1
+                ).sum(dim=-1)
+                feas = neg_violation == 0
+                if feas.any():
+                    f_pred[~feas] = float("-inf")
+                else:
+                    # set objective equal to negative violation
+                    f_pred = neg_violation
+        except AttributeError:
+            pass
+        if f_pred.ndim == mean.ndim and f_pred.shape[-1] > 1:
+            # multi-objective
+            # find pareto set
+            is_pareto = is_non_dominated(f_pred)
+            best_X = X[is_pareto]
+        else:
+            if f_pred.shape[-1] == 1:
+                f_pred = f_pred.squeeze(-1)
+            n_best = max(1, round(X.shape[0] * best_pct / 100))
+            # the view() is to ensure that best_idcs is not a scalar tensor
+            best_idcs = torch.topk(f_pred, n_best).indices.view(-1)
+            best_X = X[best_idcs]
+    use_perturbed_sampling = best_X.shape[-1] >= 20 or prob_perturb is not None
+    n_trunc_normal_points = (
+        n_discrete_points // 2 if use_perturbed_sampling else n_discrete_points
+    )
+    perturbed_X = sample_truncated_normal_perturbations(
+        X=best_X,
+        n_discrete_points=n_trunc_normal_points,
+        sigma=sigma,
+        bounds=bounds,
+    )
+    if use_perturbed_sampling:
+        perturbed_subset_dims_X = sample_perturbed_subset_dims(
+            X=best_X,
+            bounds=bounds,
+            # ensure that we return n_discrete_points
+            n_discrete_points=n_discrete_points - n_trunc_normal_points,
+            sigma=sigma,
+            prob_perturb=prob_perturb,
         )
+        perturbed_X = torch.cat([perturbed_X, perturbed_subset_dims_X], dim=0)
+        # shuffle points
+        perm = torch.randperm(perturbed_X.shape[0], device=X.device)
+        perturbed_X = perturbed_X[perm]
+    return perturbed_X
+
+
+def sample_truncated_normal_perturbations(
+    X: Tensor,
+    n_discrete_points: int,
+    sigma: float,
+    bounds: Tensor,
+    qmc: bool = True,
+) -> Tensor:
+    r"""Sample points around `X`.
+
+    Sample perturbed points around `X` such that the added perturbations
+    are sampled from N(0, sigma^2 I) and truncated to be within [0,1]^d.
+
+    Args:
+        X: A `n x d`-dim tensor starting points.
+        n_discrete_points: The number of points to sample.
+        sigma: The standard deviation of the additive gaussian noise for
+            perturbing the points.
+        bounds: A `2 x d`-dim tensor containing the bounds.
+        qmc: A boolean indicating whether to use qmc.
+
+    Returns:
+        A `n_discrete_points x d`-dim tensor containing the sampled points.
+    """
+    X = normalize(X, bounds=bounds)
+    d = X.shape[1]
+    # sample points from N(X_center, sigma^2 I), truncated to be within
+    # [0, 1]^d.
+    if X.shape[0] > 1:
+        rand_indices = torch.randint(X.shape[0], (n_discrete_points,), device=X.device)
+        X = X[rand_indices]
+    if qmc:
+        std_bounds = torch.zeros(2, d, dtype=X.dtype, device=X.device)
+        std_bounds[1] = 1
+        u = draw_sobol_samples(bounds=std_bounds, n=n_discrete_points, q=1).squeeze(1)
     else:
-        dense_equality_constraints = None
-    normalized_bounds = torch.zeros_like(bounds)
-    normalized_bounds[1, :] = 1.0
-    polytope_sampler = HitAndRunPolytopeSampler(
-        bounds=normalized_bounds,
-        inequality_constraints=dense_inequality_constraints,
-        equality_constraints=dense_equality_constraints,
-        n_burnin=n_burnin,
-    )
-    samples = polytope_sampler.draw(n=n * thinning, seed=seed)[::thinning]
-    return bounds[0] + samples * (bounds[1] - bounds[0])
-
-
-def sparse_to_dense_constraints(
-    d: int,
-    constraints: List[Tuple[Tensor, Tensor, float]],
-) -> Tuple[Tensor, Tensor]:
-    r"""Convert parameter constraints from a sparse format into a dense format.
+        u = torch.rand((n_discrete_points, d), dtype=X.dtype, device=X.device)
+    # compute bounds to sample from
+    a = -X
+    b = 1 - X
+    # compute z-score of bounds
+    alpha = a / sigma
+    beta = b / sigma
+    normal = Normal(0, 1)
+    cdf_alpha = normal.cdf(alpha)
+    # use inverse transform
+    perturbation = normal.icdf(cdf_alpha + u * (normal.cdf(beta) - cdf_alpha)) * sigma
+    # add perturbation and clip points that are still outside
+    perturbed_X = (X + perturbation).clamp(0.0, 1.0)
+    return unnormalize(perturbed_X, bounds=bounds)
 
-    This method converts sparse triples of the form (indices, coefficients, rhs)
-    to constraints of the form Ax >= b or Ax = b.
+
+def sample_perturbed_subset_dims(
+    X: Tensor,
+    bounds: Tensor,
+    n_discrete_points: int,
+    sigma: float = 1e-1,
+    qmc: bool = True,
+    prob_perturb: Optional[float] = None,
+) -> Tensor:
+    r"""Sample around `X` by perturbing a subset of the dimensions.
+
+    By default, dimensions are perturbed with probability equal to
+    `min(20 / d, 1)`. As shown in [Regis]_, perturbing a small number
+    of dimensions can be beneificial. The perturbations are sampled
+    from N(0, sigma^2 I) and truncated to be within [0,1]^d.
 
     Args:
-        d: The input dimension.
-        inequality constraints: A list of tuples (indices, coefficients, rhs),
-            with each tuple encoding an (in)equality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs` or
-            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+        X: A `n x d`-dim tensor starting points. `X`
+            must be normalized to be within `[0, 1]^d`.
+        bounds: The bounds to sample perturbed values from
+        n_discrete_points: The number of points to sample.
+        sigma: The standard deviation of the additive gaussian noise for
+            perturbing the points.
+        qmc: A boolean indicating whether to use qmc.
+        prob_perturb: The probability of perturbing each dimension. If omitted,
+            defaults to `min(20 / d, 1)`.
 
     Returns:
-        A two-element tuple containing:
-            - A: A `n_constraints x d`-dim tensor of coefficients.
-            - b: A `n_constraints x 1`-dim tensor of right hand sides.
-    """
-    _t = constraints[0][1]
-    A = torch.zeros(len(constraints), d, dtype=_t.dtype, device=_t.device)
-    b = torch.zeros(len(constraints), 1, dtype=_t.dtype, device=_t.device)
-    for i, (indices, coefficients, rhs) in enumerate(constraints):
-        A[i, indices.long()] = coefficients
-        b[i] = rhs
-    return A, b
+        A `n_discrete_points x d`-dim tensor containing the sampled points.
+
+    """
+    if bounds.ndim != 2:
+        raise BotorchTensorDimensionError("bounds must be a `2 x d`-dim tensor.")
+    elif X.ndim != 2:
+        raise BotorchTensorDimensionError("X must be a `n x d`-dim tensor.")
+    d = bounds.shape[-1]
+    if prob_perturb is None:
+        # Only perturb a subset of the features
+        prob_perturb = min(20.0 / d, 1.0)
+
+    if X.shape[0] == 1:
+        X_cand = X.repeat(n_discrete_points, 1)
+    else:
+        rand_indices = torch.randint(X.shape[0], (n_discrete_points,), device=X.device)
+        X_cand = X[rand_indices]
+    pert = sample_truncated_normal_perturbations(
+        X=X_cand,
+        n_discrete_points=n_discrete_points,
+        sigma=sigma,
+        bounds=bounds,
+        qmc=qmc,
+    )
+
+    # find cases where we are not perturbing any dimensions
+    mask = (
+        torch.rand(
+            n_discrete_points,
+            d,
+            dtype=bounds.dtype,
+            device=bounds.device,
+        )
+        <= prob_perturb
+    )
+    ind = (~mask).all(dim=-1).nonzero()
+    # perturb `n_perturb` of the dimensions
+    n_perturb = ceil(d * prob_perturb)
+    perturb_mask = torch.zeros(d, dtype=mask.dtype, device=mask.device)
+    perturb_mask[:n_perturb].fill_(1)
+    # TODO: use batched `torch.randperm` when available:
+    # https://github.com/pytorch/pytorch/issues/42502
+    for idx in ind:
+        mask[idx] = perturb_mask[torch.randperm(d, device=bounds.device)]
+    # Create candidate points
+    X_cand[mask] = pert[mask]
+    return X_cand
```

### Comparing `botorch-0.8.3/botorch/utils/testing.py` & `botorch-0.8.4/botorch/utils/testing.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/torch.py` & `botorch-0.8.4/botorch/utils/torch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/transforms.py` & `botorch-0.8.4/botorch/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch/utils/types.py` & `botorch-0.8.4/botorch/utils/types.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch.egg-info/PKG-INFO` & `botorch-0.8.4/botorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botorch
-Version: 0.8.3
+Version: 0.8.4
 Summary: Bayesian Optimization in PyTorch
 Home-page: https://botorch.org
 Author: Meta Platforms, Inc.
 License: MIT
 Project-URL: Documentation, https://botorch.org
 Project-URL: Source, https://github.com/pytorch/botorch
 Project-URL: conda, https://anaconda.org/pytorch/botorch
@@ -77,16 +77,16 @@
 
 
 ## Installation
 
 **Installation Requirements**
 - Python >= 3.8
 - PyTorch >= 1.12
-- gpytorch == 1.9.1
-- linear_operator == 0.3.0
+- gpytorch == 1.10
+- linear_operator == 0.4.0
 - pyro-ppl >= 1.8.4
 - scipy
 - multiple-dispatch
 
 ### Prerequisite only for MacOS users with Intel processors:
 Before installing BoTorch, we recommend first manually installing PyTorch, a required dependency of
 BoTorch. Installing it according to the [PyTorch installation instructions](https://pytorch.org/get-started/locally/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botorch Version: 0.8.3 Summary: Bayesian
+Metadata-Version: 2.1 Name: botorch Version: 0.8.4 Summary: Bayesian
 Optimization in PyTorch Home-page: https://botorch.org Author: Meta Platforms,
 Inc. License: MIT Project-URL: Documentation, https://botorch.org Project-URL:
 Source, https://github.com/pytorch/botorch Project-URL: conda, https://
 anaconda.org/pytorch/botorch Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Intended Audience ::
@@ -44,85 +44,84 @@
 recommend using BoTorch as a low-level API for implementing new algorithms for
 [Ax](https://ax.dev). Ax has been designed to be an easy-to-use platform for
 end-users, which at the same time is flexible enough for Bayesian Optimization
 researchers to plug into for handling of feature transformations, (meta-)data
 management, storage, etc. We recommend that end-users who are not actively
 doing research on Bayesian Optimization simply use Ax. ## Installation
 **Installation Requirements** - Python >= 3.8 - PyTorch >= 1.12 - gpytorch ==
-1.9.1 - linear_operator == 0.3.0 - pyro-ppl >= 1.8.4 - scipy - multiple-
-dispatch ### Prerequisite only for MacOS users with Intel processors: Before
-installing BoTorch, we recommend first manually installing PyTorch, a required
-dependency of BoTorch. Installing it according to the [PyTorch installation
-instructions](https://pytorch.org/get-started/locally/) ensures that it is
-properly linked against MKL, a library that optimizes mathematical computation
-for Intel processors. This will result in up to an order-of-magnitude speed-up
-for Bayesian optimization, as at the moment, installing PyTorch from pip does
-not link against MKL. The PyTorch installation instructions currently
-recommend: 1. Install [Anaconda](https://www.anaconda.com/distribution/
-#download-section). Note that there are different installers for Intel and M1
-Macs. 2. Install PyTorch following the [PyTorch installation instructions]
-(https://pytorch.org/get-started/locally/). Currently, this suggests running
-`conda install pytorch torchvision -c pytorch`. If you want to customize your
-installation, please follow the [PyTorch installation instructions](https://
-pytorch.org/get-started/locally/) to build from source. ### Option 1:
-Installing the latest release The latest release of BoTorch is easily installed
-either via [Anaconda](https://www.anaconda.com/distribution/#download-section)
-(recommended) or pip. **To install BoTorch from Anaconda**, run ```bash conda
-install botorch -c pytorch -c gpytorch -c conda-forge ``` The above command
-installs BoTorch and any needed dependencies. ` -c pytorch -c gpytorch -
-c conda-forge` means that the most preferred source to install from is the
-PyTorch channel, the next most preferred is the GPyTorch channel, and the least
-preferred is conda-forge. **Alternatively, to install with `pip`**, do ```bash
-pip install botorch ``` _Note_: Make sure the `pip` being used is actually the
-one from the newly created Conda environment. If you're using a Unix-based OS,
-you can use `which pip` to check. ### Option 2: Installing from latest main
-branch If you would like to try our bleeding edge features (and don't mind
-potentially running into the occasional bug here or there), you can install the
-latest development version directly from GitHub. If you want to also install
-the current `gpytorch` and `linear_operator` development versions, you will
-need to ensure that the `ALLOW_LATEST_GPYTORCH_LINOP` environment variable is
-set: ```bash pip install --upgrade git+https://github.com/cornellius-gp/
-linear_operator.git pip install --upgrade git+https://github.com/cornellius-gp/
-gpytorch.git export ALLOW_LATEST_GPYTORCH_LINOP=true pip install --upgrade
-git+https://github.com/pytorch/botorch.git ``` ### Option 3: Editable/dev
-install If you want to [contribute](CONTRIBUTING.md) to BoTorch, you will want
-to install editably so that you can change files and have the changes reflected
-in your local install. If you want to install the current `gpytorch` and
-`linear_operator` development versions, as in Option 2, do that before
-proceeding. #### Option 3a: Bare-bones editable install ```bash git clone
-https://github.com/pytorch/botorch.git cd botorch pip install -e . ``` ####
-Option 3b: Editable install with development and tutorials dependencies ```bash
-git clone https://github.com/pytorch/botorch.git cd botorch export
-ALLOW_BOTORCH_LATEST=true pip install -e ".[dev, tutorials]" ``` * `dev`:
-Specifies tools necessary for development (testing, linting, docs building; see
-[Contributing](#contributing) below). * `tutorials`: Also installs all packages
-necessary for running the tutorial notebooks. * You can also install either the
-dev or tutorials dependencies without installing both, e.g. by changing the
-last command to `pip install -e ".[dev]"`. ## Getting Started Here's a quick
-run down of the main components of a Bayesian optimization loop. For more
-details see our [Documentation](https://botorch.org/docs/introduction) and the
-[Tutorials](https://botorch.org/tutorials). 1. Fit a Gaussian Process model to
-data ```python import torch from botorch.models import SingleTaskGP from
-botorch.fit import fit_gpytorch_mll from gpytorch.mlls import
-ExactMarginalLogLikelihood train_X = torch.rand(10, 2) Y = 1 - (train_X -
-0.5).norm(dim=-1, keepdim=True) # explicit output dimension Y += 0.1 *
-torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std() gp = SingleTaskGP
-(train_X, train_Y) mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
-fit_gpytorch_mll(mll) ``` 2. Construct an acquisition function ```python from
-botorch.acquisition import UpperConfidenceBound UCB = UpperConfidenceBound(gp,
-beta=0.1) ``` 3. Optimize the acquisition function ```python from botorch.optim
-import optimize_acqf bounds = torch.stack([torch.zeros(2), torch.ones(2)])
-candidate, acq_value = optimize_acqf( UCB, bounds=bounds, q=1, num_restarts=5,
-raw_samples=20, ) ``` ## Citing BoTorch If you use BoTorch, please cite the
-following paper: > [M. Balandat, B. Karrer, D. R. Jiang, S. Daulton, B. Letham,
-A. G. Wilson, and E. Bakshy. BoTorch: A Framework for Efficient Monte-Carlo
-Bayesian Optimization. Advances in Neural Information Processing Systems 33,
-2020.](https://arxiv.org/abs/1910.06403) ``` @inproceedings
-{balandat2020botorch, title={{BoTorch: A Framework for Efficient Monte-Carlo
-Bayesian Optimization}}, author={Balandat, Maximilian and Karrer, Brian and
-Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson, Andrew
-Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
+1.10 - linear_operator == 0.4.0 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
+### Prerequisite only for MacOS users with Intel processors: Before installing
+BoTorch, we recommend first manually installing PyTorch, a required dependency
+of BoTorch. Installing it according to the [PyTorch installation instructions]
+(https://pytorch.org/get-started/locally/) ensures that it is properly linked
+against MKL, a library that optimizes mathematical computation for Intel
+processors. This will result in up to an order-of-magnitude speed-up for
+Bayesian optimization, as at the moment, installing PyTorch from pip does not
+link against MKL. The PyTorch installation instructions currently recommend: 1.
+Install [Anaconda](https://www.anaconda.com/distribution/#download-section).
+Note that there are different installers for Intel and M1 Macs. 2. Install
+PyTorch following the [PyTorch installation instructions](https://pytorch.org/
+get-started/locally/). Currently, this suggests running `conda install pytorch
+torchvision -c pytorch`. If you want to customize your installation, please
+follow the [PyTorch installation instructions](https://pytorch.org/get-started/
+locally/) to build from source. ### Option 1: Installing the latest release The
+latest release of BoTorch is easily installed either via [Anaconda](https://
+www.anaconda.com/distribution/#download-section) (recommended) or pip. **To
+install BoTorch from Anaconda**, run ```bash conda install botorch -c pytorch -
+c gpytorch -c conda-forge ``` The above command installs BoTorch and any needed
+dependencies. ` -c pytorch -c gpytorch -c conda-forge` means that the most
+preferred source to install from is the PyTorch channel, the next most
+preferred is the GPyTorch channel, and the least preferred is conda-forge.
+**Alternatively, to install with `pip`**, do ```bash pip install botorch ```
+_Note_: Make sure the `pip` being used is actually the one from the newly
+created Conda environment. If you're using a Unix-based OS, you can use `which
+pip` to check. ### Option 2: Installing from latest main branch If you would
+like to try our bleeding edge features (and don't mind potentially running into
+the occasional bug here or there), you can install the latest development
+version directly from GitHub. If you want to also install the current
+`gpytorch` and `linear_operator` development versions, you will need to ensure
+that the `ALLOW_LATEST_GPYTORCH_LINOP` environment variable is set: ```bash pip
+install --upgrade git+https://github.com/cornellius-gp/linear_operator.git pip
+install --upgrade git+https://github.com/cornellius-gp/gpytorch.git export
+ALLOW_LATEST_GPYTORCH_LINOP=true pip install --upgrade git+https://github.com/
+pytorch/botorch.git ``` ### Option 3: Editable/dev install If you want to
+[contribute](CONTRIBUTING.md) to BoTorch, you will want to install editably so
+that you can change files and have the changes reflected in your local install.
+If you want to install the current `gpytorch` and `linear_operator` development
+versions, as in Option 2, do that before proceeding. #### Option 3a: Bare-bones
+editable install ```bash git clone https://github.com/pytorch/botorch.git cd
+botorch pip install -e . ``` #### Option 3b: Editable install with development
+and tutorials dependencies ```bash git clone https://github.com/pytorch/
+botorch.git cd botorch export ALLOW_BOTORCH_LATEST=true pip install -e ".[dev,
+tutorials]" ``` * `dev`: Specifies tools necessary for development (testing,
+linting, docs building; see [Contributing](#contributing) below). *
+`tutorials`: Also installs all packages necessary for running the tutorial
+notebooks. * You can also install either the dev or tutorials dependencies
+without installing both, e.g. by changing the last command to `pip install -
+e ".[dev]"`. ## Getting Started Here's a quick run down of the main components
+of a Bayesian optimization loop. For more details see our [Documentation]
+(https://botorch.org/docs/introduction) and the [Tutorials](https://
+botorch.org/tutorials). 1. Fit a Gaussian Process model to data ```python
+import torch from botorch.models import SingleTaskGP from botorch.fit import
+fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood train_X =
+torch.rand(10, 2) Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit
+output dimension Y += 0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std
+() gp = SingleTaskGP(train_X, train_Y) mll = ExactMarginalLogLikelihood
+(gp.likelihood, gp) fit_gpytorch_mll(mll) ``` 2. Construct an acquisition
+function ```python from botorch.acquisition import UpperConfidenceBound UCB =
+UpperConfidenceBound(gp, beta=0.1) ``` 3. Optimize the acquisition function
+```python from botorch.optim import optimize_acqf bounds = torch.stack(
+[torch.zeros(2), torch.ones(2)]) candidate, acq_value = optimize_acqf( UCB,
+bounds=bounds, q=1, num_restarts=5, raw_samples=20, ) ``` ## Citing BoTorch If
+you use BoTorch, please cite the following paper: > [M. Balandat, B. Karrer, D.
+R. Jiang, S. Daulton, B. Letham, A. G. Wilson, and E. Bakshy. BoTorch: A
+Framework for Efficient Monte-Carlo Bayesian Optimization. Advances in Neural
+Information Processing Systems 33, 2020.](https://arxiv.org/abs/1910.06403) ```
+@inproceedings{balandat2020botorch, title={{BoTorch: A Framework for Efficient
+Monte-Carlo Bayesian Optimization}}, author={Balandat, Maximilian and Karrer,
+Brian and Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson,
+Andrew Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
 Processing Systems 33}, year={2020}, url = {http://arxiv.org/abs/1910.06403} }
 ``` See [here](https://botorch.org/docs/papers) for an incomplete selection of
 peer-reviewed papers that build off of BoTorch. ## Contributing See the
 [CONTRIBUTING](CONTRIBUTING.md) file for how to help out. ## License BoTorch is
 MIT licensed, as found in the [LICENSE](LICENSE) file.
```

### Comparing `botorch-0.8.3/botorch.egg-info/SOURCES.txt` & `botorch-0.8.4/botorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch_logo_lockup.png` & `botorch-0.8.4/botorch_logo_lockup.png`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/botorch_logo_lockup.svg` & `botorch-0.8.4/botorch_logo_lockup.svg`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/notebooks/tutorials_performance_tracking.ipynb` & `botorch-0.8.4/notebooks/tutorials_performance_tracking.ipynb`

 * *Files identical despite different names*

### Comparing `botorch-0.8.3/setup.py` & `botorch-0.8.4/setup.py`

 * *Files identical despite different names*


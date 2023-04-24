# Comparing `tmp/servicefoundry-0.8.5rc1.tar.gz` & `tmp/servicefoundry-0.8.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.8.5rc1.tar", max compression
+gzip compressed data, was "servicefoundry-0.8.5rc2.tar", max compression
```

## Comparing `servicefoundry-0.8.5rc1.tar` & `servicefoundry-0.8.5rc2.tar`

### file list

```diff
@@ -1,136 +1,126 @@
--rw-r--r--   0        0        0      672 2023-04-22 14:33:24.758953 servicefoundry-0.8.5rc1/README.md
--rw-r--r--   0        0        0     2284 2023-04-22 14:33:38.183303 servicefoundry-0.8.5rc1/pyproject.toml
--rw-r--r--   0        0        0     1266 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/__init__.py
--rw-r--r--   0        0        0    36721 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4159 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      531 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1364 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1357 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6479 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     6458 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2803 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1890 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2007 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     2852 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     3753 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0     1080 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      591 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     3878 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1077 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     1474 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      228 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     3032 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/io/__init__.py
--rw-r--r--   0        0        0     2289 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/io/cli_input_hook.py
--rw-r--r--   0        0        0     2500 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      347 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      379 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/core/login.py
--rw-r--r--   0        0        0      184 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      313 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/core/util.py
--rw-r--r--   0        0        0      188 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      414 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4224 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0     1801 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/input_hook.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/io/__init__.py
--rw-r--r--   0        0        0     1871 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/io/notebook_callback.py
--rw-r--r--   0        0        0     1041 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/io/notebook_input_hook.py
--rw-r--r--   0        0        0     1010 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/notebook/notebook_util.py
--rw-r--r--   0        0        0      532 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      629 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/parameters.py
--rw-r--r--   0        0        0      825 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    23861 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2232 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-04-22 14:33:24.762953 servicefoundry-0.8.5rc1/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     5568 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1028 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2533 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0     1409 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0     9608 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5191 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/session.py
--rw-r--r--   0        0        0      993 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5276 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8890 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-04-22 14:33:24.766953 servicefoundry-0.8.5rc1/servicefoundry/version.py
--rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 servicefoundry-0.8.5rc1/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-04-24 03:35:24.719930 servicefoundry-0.8.5rc2/README.md
+-rw-r--r--   0        0        0     2119 2023-04-24 03:35:35.595909 servicefoundry-0.8.5rc2/pyproject.toml
+-rw-r--r--   0        0        0     1266 2023-04-24 03:35:24.719930 servicefoundry-0.8.5rc2/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    36721 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4159 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      531 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1364 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1357 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6479 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     6458 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1042 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     2795 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     3875 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     3863 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      228 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     3032 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    23939 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     5624 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1028 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0     9608 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5276 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8890 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/version.py
+-rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 servicefoundry-0.8.5rc2/PKG-INFO
```

### Comparing `servicefoundry-0.8.5rc1/README.md` & `servicefoundry-0.8.5rc2/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/pyproject.toml` & `servicefoundry-0.8.5rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.8.5rc1"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.8.5rc2"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -24,16 +24,14 @@
 PyYAML = "^6.0"
 Mako = "^1.1.6"
 importlib-resources = "^5.2.0"
 requests = ">=2.23.0,<2.29.0"
 importlib-metadata = "^4.2"
 PyJWT = "^2.0.0"
 pydantic = ">=1.9.0,<2.0.0"
-ipywidgets = { version = ">=7.6.0", optional = true }
-ipython = { version = ">=7.10.0", optional = true }
 fastapi = ">=0.56.0,<0.94.0"
 python-socketio = {version = "^5.5.2", extras = ["client"]}
 uvicorn = ">=0.13.0,<0.22.0"
 typing-extensions = ">=3.10.0"
 python-dateutil = "^2.8.2"
 gitignorefile = "^1.1.2"
 GitPython = "^3.1.27"
@@ -41,17 +39,14 @@
 filelock = "^3.8.0"
 cookiecutter = "^2.1.1"
 docker = "^6.0.1"
 chevron = "^0.14.0"
 tqdm = ">=4.0.0,<5.0.0"
 yq = "^3.1.0"
 
-[tool.poetry.extras]
-notebook = ["ipywidgets", "ipython"]
-
 [tool.poetry.dev-dependencies]
 pre-commit = "2.16.0"
 pytest = "7.2.0"
 isort = "^5.10.1"
 black = "^22.3.0"
 absolufy-imports = "^0.3.1"
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/__init__.py` & `servicefoundry-0.8.5rc2/servicefoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/auto_gen/models.py` & `servicefoundry-0.8.5rc2/servicefoundry/auto_gen/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/builder/__init__.py` & `servicefoundry-0.8.5rc2/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.8.5rc2/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.8.5rc2/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.8.5rc2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.8.5rc2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/builder/docker_service.py` & `servicefoundry-0.8.5rc2/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/cli_main.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/build_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
-import logging
 
 import rich_click as click
 
 from servicefoundry import builder
 from servicefoundry.cli.const import GROUP_CLS
 from servicefoundry.cli.util import handle_exception_wrapper
-from servicefoundry.logger import logger
 
 
 @click.group(
     name="build",
     cls=GROUP_CLS,
     invoke_without_command=True,
     help="Build docker image locally from Truefoundry spec",
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/build_logs_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from typing import Optional
 
 import rich_click as click
 
 from servicefoundry.cli.const import COMMAND_CLS
 from servicefoundry.cli.util import handle_exception_wrapper
 from servicefoundry.io.rich_output_callback import RichOutputCallBack
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/create_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import logging
 from typing import Optional
 
 import rich_click as click
 
 from servicefoundry.cli.const import COMMAND_CLS, GROUP_CLS
 from servicefoundry.cli.display_util import print_obj
 from servicefoundry.cli.util import handle_exception_wrapper
 from servicefoundry.lib.dao import workspace as workspace_lib
-from servicefoundry.logger import logger
 
 
 @click.group(name="create", cls=GROUP_CLS)
 def create_command():
     # TODO (chiragjn): Figure out a way to update supported resources based on ENABLE_* flags
     """
     Create Truefoundry resources
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/get_command.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,100 @@
-import logging
-
 import rich_click as click
 
 from servicefoundry.cli.config import CliConfig
 from servicefoundry.cli.const import COMMAND_CLS, GROUP_CLS
-from servicefoundry.cli.display_util import print_json
+from servicefoundry.cli.display_util import print_entity_obj, print_json
 from servicefoundry.cli.util import handle_exception_wrapper
 from servicefoundry.lib.dao import application as application_lib
+from servicefoundry.lib.dao import version as version_lib
 from servicefoundry.lib.dao import workspace as workspace_lib
-from servicefoundry.logger import logger
 
 # TODO (chiragjn): --json should disable all non json console prints
 
 
-@click.group(name="delete", cls=GROUP_CLS)
-def delete_command():
+@click.group(name="get", cls=GROUP_CLS)
+def get_command():
+    # TODO (chiragjn): Figure out a way to update supported resources based on ENABLE_* flags
     """
-    Delete Truefoundry resources
+    Get Truefoundry resources
 
     \b
     Supported resources:
     - Workspace
     - Application
+    - Application Version
     """
     pass
 
 
-@click.command(name="workspace", cls=COMMAND_CLS, help="Delete a Workspace")
+@click.command(name="workspace", cls=COMMAND_CLS, help="Get Workspace details")
 @click.option(
     "-w",
     "--workspace-fqn",
     "--workspace_fqn",
     type=click.STRING,
     default=None,
-    help="FQN of the Workspace to delete",
+    help="FQN of the Workspace",
+    required=True,
+)
+@handle_exception_wrapper
+def get_workspace(workspace_fqn):
+    workspace = workspace_lib.get_workspace_by_fqn(workspace_fqn=workspace_fqn)
+    if CliConfig.get("json"):
+        print_json(data=workspace.dict())
+    else:
+        print_entity_obj("Workspace", workspace)
+
+
+@click.command(name="application", cls=COMMAND_CLS, help="Get Application details")
+@click.option(
+    "--application-fqn",
+    "--application_fqn",
+    type=click.STRING,
+    default=None,
+    help="FQN of the application",
     required=True,
 )
-@click.confirmation_option(prompt="Are you sure you want to delete this workspace?")
 @handle_exception_wrapper
-def delete_workspace(workspace_fqn):
-    deleted_workspace = workspace_lib.delete_workspace(
-        workspace_fqn=workspace_fqn,
-    )
+def get_application(application_fqn):
+    application = application_lib.get_application(application_fqn=application_fqn)
     if CliConfig.get("json"):
-        print_json(data=deleted_workspace.dict())
+        print_json(data=application.dict())
+    else:
+        print_entity_obj(
+            "Application",
+            application,
+        )
 
 
-@click.command(name="application", cls=COMMAND_CLS, help="Delete an Application")
+@click.command(
+    name="application-version", cls=COMMAND_CLS, help="Get Application Version details"
+)
 @click.option(
     "--application-fqn",
     "--application_fqn",
     type=click.STRING,
     default=None,
-    help="FQN of the Application to delete",
+    help="FQN of the application",
+    required=True,
+)
+@click.option(
+    "--version",
+    type=click.STRING,
+    default=None,
+    help="Version number of the application deployment",
     required=True,
 )
-@click.confirmation_option(prompt="Are you sure you want to delete this application?")
 @handle_exception_wrapper
-def delete_application(application_fqn):
-    response = application_lib.delete_application(
-        application_fqn=application_fqn,
-    )
+def get_version(application_fqn, version):
+    version = version_lib.get_version(application_fqn=application_fqn, version=version)
     if CliConfig.get("json"):
-        print_json(data=response)
+        print_json(data=version.dict())
+    else:
+        print_entity_obj("Version", version)
 
 
-def get_delete_command():
-    delete_command.add_command(delete_workspace)
-    delete_command.add_command(delete_application)
-    return delete_command
+def get_get_command():
+    get_command.add_command(get_workspace)
+    get_command.add_command(get_application)
+    get_command.add_command(get_version)
+    return get_command
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/list_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-import logging
-
 import rich_click as click
 
 from servicefoundry.cli.config import CliConfig
-from servicefoundry.cli.console import console
 from servicefoundry.cli.const import COMMAND_CLS, GROUP_CLS
 from servicefoundry.cli.display_util import print_entity_list, print_json
 from servicefoundry.cli.util import handle_exception_wrapper
+from servicefoundry.io.rich_output_callback import RichOutputCallBack
 from servicefoundry.lib.dao import application as application_lib
 from servicefoundry.lib.dao import version as version_lib
 from servicefoundry.lib.dao import workspace as workspace_lib
 from servicefoundry.lib.messages import (
     PROMPT_NO_APPLICATIONS,
     PROMPT_NO_VERSIONS,
     PROMPT_NO_WORKSPACES,
 )
-from servicefoundry.logger import logger
 
 # TODO (chiragjn): --json should disable all non json console prints
 
 
 @click.group(name="list", cls=GROUP_CLS)
 def list_command():
     # TODO (chiragjn): Figure out a way to update supported resources based on ENABLE_* flags
@@ -45,15 +42,16 @@
 )
 @handle_exception_wrapper
 def list_workspaces(cluster_name):
     workspaces = workspace_lib.list_workspaces(
         cluster_name=cluster_name,
     )
     if not workspaces:
-        console.print(PROMPT_NO_WORKSPACES)
+        output_hook = RichOutputCallBack()
+        output_hook.print_line(PROMPT_NO_WORKSPACES)
     else:
         workspaces.sort(key=lambda s: s.createdAt, reverse=True)
 
     if CliConfig.get("json"):
         print_json(data=workspaces)
     else:
         print_entity_list(
@@ -80,15 +78,16 @@
 )
 @handle_exception_wrapper
 def list_applications(workspace_fqn, application_type):
     applications = application_lib.list_applications(
         workspace_fqn=workspace_fqn, application_type=application_type
     )
     if not applications:
-        console.print(PROMPT_NO_APPLICATIONS)
+        output_hook = RichOutputCallBack()
+        output_hook.print_line(PROMPT_NO_APPLICATIONS)
     else:
         applications.sort(key=lambda s: s.createdAt, reverse=True)
     if CliConfig.get("json"):
         print_json(data=applications)
     else:
         # TODO (chiragjn): Display columns here need to show workspace and cluster name!
         print_entity_list(
@@ -110,15 +109,16 @@
 )
 @handle_exception_wrapper
 def list_versions(application_fqn):
     versions = version_lib.list_versions(
         application_fqn=application_fqn,
     )
     if not versions:
-        console.print(PROMPT_NO_VERSIONS)
+        output_hook = RichOutputCallBack()
+        output_hook.print_line(PROMPT_NO_VERSIONS)
     else:
         versions.sort(key=lambda s: s.createdAt, reverse=True)
     if CliConfig.get("json"):
         print_json(data=versions)
     else:
         # TODO (chiragjn): Display columns here need to show workspace and cluster name!
         print_entity_list(
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/login_command.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import rich_click as click
 
-from servicefoundry.cli.console import console
 from servicefoundry.cli.const import COMMAND_CLS
 from servicefoundry.cli.util import (
     _prompt_if_no_value_and_supported,
     handle_exception_wrapper,
 )
 from servicefoundry.io.rich_output_callback import RichOutputCallBack
-from servicefoundry.lib.messages import PROMPT_POST_LOGIN
 from servicefoundry.lib.session import login
 
 
 @click.command(name="login", cls=COMMAND_CLS)
 @click.option("--relogin", type=click.BOOL, is_flag=True, default=False)
 @click.option("--host", type=click.STRING, default=None)
 @click.option(
@@ -24,12 +22,11 @@
 @handle_exception_wrapper
 def login_command(relogin: bool, host: str, api_key: str):
     """
     Login to Truefoundry
     """
     callback = RichOutputCallBack()
     login(api_key=api_key, host=host, relogin=relogin, output_hook=callback)
-    console.print(PROMPT_POST_LOGIN)
 
 
 def get_login_command():
     return login_command
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/logs_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from datetime import datetime
 from typing import Optional
 
 import rich_click as click
 from dateutil.tz import tzlocal
 
 from servicefoundry.cli.const import COMMAND_CLS
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/redeploy_command.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import logging
-
 import rich_click as click
 
 from servicefoundry.cli.const import COMMAND_CLS
 from servicefoundry.cli.util import handle_exception_wrapper
 from servicefoundry.lib.dao import application as application_lib
-from servicefoundry.logger import logger
 
 
 @click.command(name="redeploy", cls=COMMAND_CLS)
 @click.option(
     "--application-fqn",
     type=click.STRING,
     default=None,
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/trigger_command.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,87 @@
 import json
 from typing import Dict, Optional, Sequence
 
 import rich_click as click
+from click import ClickException
 
 from servicefoundry.cli.const import COMMAND_CLS, GROUP_CLS
 from servicefoundry.cli.util import handle_exception_wrapper
 from servicefoundry.lib.dao import application
 
 
 @click.group(name="trigger", cls=GROUP_CLS)
 def trigger_command():
     """
-    Trigger a deployed job asynchronously
+    Trigger a Job asynchronously
     """
     pass
 
 
 @click.command(
     name="job",
     cls=COMMAND_CLS,
-    context_settings=dict(ignore_unknown_options=True),
-    help="Trigger a Job asynchronously",
+    context_settings=dict(ignore_unknown_options=True, allow_extra_args=True),
 )
 @click.option(
     "--application-fqn",
     "--application_fqn",
     type=click.STRING,
     required=True,
     help="FQN of the deployment of the Job. This can be found on the Job details page.",
 )
 @click.option("--command", type=click.STRING, required=False, help="Command to run")
-@click.option(
-    "--params",
-    type=click.UNPROCESSED,
+@click.argument(
+    "params",
+    type=click.STRING,
+    nargs=-1,
     required=False,
-    help="Parameters to pass to the job",
 )
 @handle_exception_wrapper
-def trigger_job(
-    application_fqn: str,
-    command: Optional[Sequence[str]],
-    params: Optional[Dict[str, str]],
-):
+def trigger_job(application_fqn: str, command: Optional[Sequence[str]], params):
+    """
+    Trigger a Job on Truefoundry asynchronously
+
+        [b]sfy trigger job --application-fqn "my-cluster:my-workspace:my-job"[/]
+
+    \n
+    Additionally, you can either pass `--command` or params (if defined in the spec)\n
+
+
+    Passing a command:
+
+        [b]sfy trigger job --application-fqn "my-cluster:my-workspace:my-job" --command "python run.py"[/]
+    \n
+
+    Passing params:
+
+        [b]sfy trigger job --application-fqn "my-cluster:my-workspace:my-job" -- --param1_name param1_value --param2_name param2_value ...[/]
+    """
     if params:
-        try:
-            params = json.loads(params)
-        except json.JSONDecodeError:
-            raise Exception("Invalid JSON passed for `params`")
+        params_dict = {}
+        if len(params) % 2 != 0:
+            raise ClickException(
+                f"Found odd number of argument pairs: {params}. "
+                "Perhaps you forgot to pass a value for one of the params? "
+                "Job params should be passed in the "
+                "format `--param1_name param1_value --param2_name param2_value ...`"
+            )
+        for i in range(0, len(params), 2):
+            key = params[i]
+            value = params[i + 1]
+            if not key.startswith("--"):
+                raise ClickException(
+                    f"Got ambiguous argument {key!r} in params: {params}. "
+                    f"Param names should be prefixed with '--' i.e. "
+                    "Job params should be passed in the "
+                    "format `--param1_name param1_value --param2_name param2_value ...`"
+                )
+            key = key.lstrip("-")
+            params_dict[key] = value
+
     application.trigger_job(
         application_fqn=application_fqn, command=command, params=params
     )
 
 
 def get_trigger_command():
     trigger_command.add_command(trigger_job)
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/display_util.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/cli/util.py` & `servicefoundry-0.8.5rc2/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/__main__.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/app.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/build.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
                 "Please use keyword arguments"
             )
         return self.method.__call__(**kwargs)
 
     def run(self, **kwargs):
         return self.method.run(**kwargs)
 
-    async def run_async(self, *args, **kwargs):
-        return await self.method.run_async(*args, **kwargs)
+    async def run_async(self, **kwargs):
+        return await self.method.run_async(**kwargs)
 
     @property
     def instance(self):
         return self._instance
 
     def get_qual_name(self, method) -> str:
         return get_qual_name(method)
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/route.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/service.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/function_service/utils.py` & `servicefoundry-0.8.5rc2/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/internal/experimental.py` & `servicefoundry-0.8.5rc2/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.8.5rc2/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import functools
 import json
 import os
 import time
 from datetime import datetime, timezone
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 from urllib.parse import urljoin, urlparse
@@ -64,45 +65,49 @@
             )
             http_response = requests.put(metadata["url"], data=wrapped_file)
 
             if http_response.status_code not in [204, 201, 200]:
                 raise RuntimeError(f"Failed to upload code {http_response.content}")
 
 
+def check_min_cli_version(fn):
+    @functools.wraps(fn)
+    def inner(*args, **kwargs):
+        if __version__ != "0.0.0":
+            # "0.0.0" indicates dev version
+            client: "ServiceFoundryServiceClient" = args[0]
+            # noinspection PyProtectedMember
+            min_cli_version = client._get_min_cli_version_requirement()
+            if version.parse(__version__) < version.parse(min_cli_version):
+                raise Exception(
+                    "You are using an outdated version of `servicefoundry`.\n"
+                    f"Run `pip install servicefoundry>={min_cli_version}` to install the supported version.",
+                )
+        else:
+            logger.debug("Ignoring minimum cli version check")
+
+        return fn(*args, **kwargs)
+
+    return inner
+
+
 class ServiceFoundryServiceClient:
     def __init__(self, init_session: bool = True, base_url: Optional[str] = None):
         self._session: Optional[ServiceFoundrySession] = None
         if init_session:
             if base_url:
                 logger.warning("Passed base url %r will be ignored", base_url)
             self._session = ServiceFoundrySession()
             base_url = self._session.base_url
         elif not base_url:
             raise Exception("Neither session, not base_url provided")
 
         self._base_url = base_url.strip("/")
         self._api_server_url = f"{self._base_url}/{API_SERVER_RELATIVE_PATH}"
 
-    def check_min_cli_version(fn):
-        def inner(self, *args, **kwargs):
-            if __version__ != "0.0.0":
-                # "0.0.0" indicates dev version
-                min_cli_version = self._get_min_cli_version_requirement()
-                if version.parse(__version__) < version.parse(min_cli_version):
-                    raise Exception(
-                        "You are using an outdated version of `servicefoundry`.\n"
-                        f"Execute `pip install servicefoundry>={min_cli_version}` to install the supported version.",
-                    )
-            else:
-                logger.debug("Ignoring minimum cli version check")
-
-            return fn(self, *args, **kwargs)
-
-        return inner
-
     @property
     def base_url(self) -> str:
         return self._base_url
 
     def get_tenant_info(self) -> TenantInfo:
         res = requests.get(
             url=f"{self._api_server_url}/v1/tenant-id",
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/config/dict_questionaire.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         for k, v in dicts.items():
             if isinstance(v, dict):
                 dicts[k] = self.__get_all_values(v, tree_path + k, custom_handlers)
             elif isinstance(v, list):
                 if len(v) != 0 and isinstance(v[0], dict):
                     for i, vi in enumerate(v):
                         self.__get_all_values(
-                            vi, tree_path + k + "[" + i + "]", custom_handlers
+                            vi, tree_path + k + "[" + str(i) + "]", custom_handlers
                         )
                 else:
                     dicts[k] = self.__confirm_list_val(
                         v, tree_path + k, custom_handlers
                     )
             else:
                 dicts[k] = self.__confirm_val(v, tree_path + k, custom_handlers)
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/const.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/dao/application.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/dao/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import json
 import shlex
 from typing import Any, Dict, Optional, Sequence, Union
 
 import servicefoundry.lib.dao.version as version_lib
-from servicefoundry.cli.console import console
 from servicefoundry.lib.clients.service_foundry_client import (
     ServiceFoundryServiceClient,
 )
 from servicefoundry.lib.model.entity import Deployment, TriggerJobResult
 from servicefoundry.lib.util import get_application_fqn_from_deployment_fqn
 from servicefoundry.logger import logger
 
@@ -48,16 +46,14 @@
 def delete_application(
     application_fqn: str,
     client: Optional[ServiceFoundryServiceClient] = None,
 ) -> Dict[str, Any]:
     client = client or ServiceFoundryServiceClient()
     application = client.get_id_from_fqn(fqn=application_fqn, fqn_type="app")
     response = client.remove_application(application_id=application["applicationId"])
-
-    console.print("""[yellow]Deleted Application[/]""")
     return response
 
 
 def redeploy_application(
     application_fqn: str,
     version: int,
     wait: bool,
@@ -91,62 +87,62 @@
     Trigger a Job on Truefoundry platform
 
     Args:
         application_fqn: Fully Qualified Name of the Deployed Job (without the version number)
         command: command to run the job with, defaults to `None`. Can be a `str` or `List[str]`
             When `None`, the job is triggered with configured command at the time of deployment.
             When passed as a list, the command will be joined using `shlex.join`
+        params: A dict mapping from parameter names (as defined in the job spec) to string values
 
     Returns:
         TriggerJobResult: metadata returning status of job trigger
     """
-    client = ServiceFoundryServiceClient()
-
     if params and command:
-        raise Exception("Either pass `command` or `params` but not both")
+        raise ValueError(
+            "`command` and `params` arguments are mutually exclusive. Please pass only one of them"
+        )
 
     try:
         # If user is passing in deployment fqn copied from UI, till we change the fqns on UI
         application_fqn = get_application_fqn_from_deployment_fqn(application_fqn)
         logger.warning(
             "Detected version number in `application_fqn`. "
             "Automatically discarding the version number. "
             f"This automatic conversion will be removed in future. "
             f"Please pass {application_fqn!r} as the value."
         )
     except ValueError:
         pass
+    client = ServiceFoundryServiceClient()
     _application_info = client.get_application_info_by_fqn(
         application_fqn=application_fqn
     )
     application_info = client.get_application_info(
         application_id=_application_info.applicationId
     )
-    if command:
+    command_str = ""
+    message = ""
+    if not params and not command:
+        message = "Job triggered with pre-configured command"
+    elif command:
         if not isinstance(command, str):
             command_str = shlex.join(command).strip()
         else:
             command_str = command.strip()
         message = f"Job triggered with command {command_str!r}"
-    elif not params and not command:
-        command_str = ""
-        message = "Job triggered with pre-configured command"
-
-    if params:
-
+    elif params:
         # Check if params has any non string values
         for key, value in params.items():
             if not isinstance(value, str):
-                raise Exception(
+                raise ValueError(
                     f"Invalid value {value!r} for key {key!r}. "
                     "Only string values are allowed for `params`"
                 )
         command_str = ""
         message = f"Job triggered with params {params!r}"
-
     result = client.trigger_job(
         deployment_id=application_info.activeDeploymentId,
         component_name=application_info.name,
         command=command_str if command_str else None,
         params=params if params else None,
     )
     previous_runs_url = f"{client.base_url.strip('/')}/deployments/{application_info.id}?tab=previousRuns"
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/dao/version.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/dao/workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from typing import Optional
 
 from servicefoundry.cli.console import console
 from servicefoundry.lib.clients.service_foundry_client import (
     ServiceFoundryServiceClient,
 )
-from servicefoundry.lib.messages import (
-    PROMPT_CREATING_NEW_WORKSPACE,
-    PROMPT_USING_CLUSTER_CONTEXT,
-)
+from servicefoundry.lib.messages import PROMPT_CREATING_NEW_WORKSPACE
 from servicefoundry.lib.model.entity import Workspace, WorkspaceResources
 from servicefoundry.logger import logger
 
 
 def create_workspace(
     name: str,
     cluster_name: str,
@@ -24,15 +21,14 @@
 
     workspace_resources = WorkspaceResources(
         cpu_limit=cpu_limit,
         memory_limit=memory_limit,
         ephemeral_storage_limit=ephemeral_storage_limit,
     )
 
-    console.print(PROMPT_USING_CLUSTER_CONTEXT.format(cluster_name))
     with console.status(PROMPT_CREATING_NEW_WORKSPACE.format(name), spinner="dots"):
         workspace = client.create_workspace(
             workspace_name=name,
             cluster_name=cluster_name,
             resources=workspace_resources,
         )
 
@@ -68,9 +64,8 @@
 def delete_workspace(
     workspace_fqn: str,
     client: Optional[ServiceFoundryServiceClient] = None,
 ) -> Workspace:
     client = client or ServiceFoundryServiceClient()
     workspace = client.get_id_from_fqn(fqn=workspace_fqn, fqn_type="workspace")
     deleted_workspace = client.remove_workspace(workspace_id=workspace["workspaceId"])
-    console.print(f"[yellow]Deleted workspace {deleted_workspace.fqn!r}[/]")
     return deleted_workspace
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/exceptions.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/messages.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/messages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 SFY = "sfy"
 
 # TODO: probably create another `rich_messages.py` and apply all formatting there
-PROMPT_LOGIN_SUCCESSFUL = f"""[green bold]Login Successful![/]"""
-PROMPT_LOGIN_INFO = (
-    f"""[yellow]You are logged in as {{username!r}} with email {{email!r}}[/]"""
-)
 PROMPT_LOGOUT_SUCCESSFUL = f"""[green bold]Logged Out![/]"""
-PROMPT_POST_LOGIN = ""
 PROMPT_ALREADY_LOGGED_OUT = f"""[yellow]You are already logged out[/]"""
-PROMPT_USING_CLUSTER_CONTEXT = f"""[yellow]Using cluster {{!r}}[/]"""
-PROMPT_USING_WORKSPACE_CONTEXT = f"""[yellow]Using workspace {{!r}}[/]"""
-PROMPT_USING_APPLICATION_CONTEXT = f"""[yellow]Using application {{!r}}[/]"""
 PROMPT_CREATING_NEW_WORKSPACE = f"""[yellow]Creating a new workspace {{!r}}[/]"""
-PROMPT_DELETING_WORKSPACE = f"""[yellow]Deleting workspace {{!r}}[/]"""
 PROMPT_DELETED_WORKSPACE = f"""[green]Deleted workspace {{!r}}[/]"""
-PROMPT_DELETING_SERVICE = f"""[yellow]Deleting service {{!r}}[/]"""
-PROMPT_DELETED_SERVICE = f"""[green]Deleted service {{!r}}[/]"""
+PROMPT_DELETED_APPLICATION = f"""[green]Deleted Application {{!r}}[/]"""
 PROMPT_NO_WORKSPACES = f"""[yellow]No workspaces found. Either cluster name is wrong, or your cluster doesn't contain any workspaces. You can create one with [bold]{SFY} create workspace[/][/]"""
 PROMPT_NO_APPLICATIONS = f"""[yellow]No applications found. You can create one with [bold]{SFY} deploy[/] from within your application folder"""
 PROMPT_NO_VERSIONS = f"""[yellow]No application versions found."""
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/model/entity.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/session.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                     f"Already logged in to {cred_file_content.host!r}\n"
                     f"Do you want to relogin to {host!r}?"
                 ):
                     return login(api_key=api_key, host=host, relogin=True)
 
             user_info = cred_file_content.to_token().to_user_info()
             user_name_display_info = user_info.email or user_info.user_type.value
-            print(
+            output_hook.print_line(
                 f"Already logged in to {cred_file_content.host!r} as "
                 f"{user_info.user_id!r} ({user_name_display_info})\n"
                 "Please use `sfy login --relogin` or `sfy.login(relogin=True)` "
                 "to force relogin"
             )
             return False
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/util.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-from typing import TypeVar, Union
+from typing import Union
 
 from servicefoundry.lib.const import (
     SFY_DEBUG_ENV_KEY,
     SFY_EXPERIMENTAL_ENV_KEY,
     SFY_INTERNAL_ENV_KEY,
 )
 
@@ -31,7 +31,24 @@
     return application_fqn
 
 
 def get_deployment_fqn_from_application_fqn(
     application_fqn: str, version: Union[str, int]
 ) -> str:
     return f"{application_fqn}:{version}"
+
+
+def is_notebook():
+    # https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
+    try:
+        # noinspection PyUnresolvedReferences
+        shell = get_ipython().__class__
+        if shell.__name__ == "ZMQInteractiveShell":
+            return True  # Jupyter notebook or qtconsole
+        elif shell.__name__ == "TerminalInteractiveShell":
+            return False  # Terminal running IPython
+        elif "google.colab" in str(shell):
+            return True  # google colab notebook
+        else:
+            return False  # Other type (?)
+    except NameError:
+        return False  # Probably standard Python interpreter
```

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/lib/win32.py` & `servicefoundry-0.8.5rc2/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/logger.py` & `servicefoundry-0.8.5rc2/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/models.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/servicefoundry/v2/lib/source.py` & `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc1/PKG-INFO` & `servicefoundry-0.8.5rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.8.5rc1
+Version: 0.8.5rc2
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: notebook
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: Mako (>=1.1.6,<2.0.0)
 Requires-Dist: PyJWT (>=2.0.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
 Requires-Dist: click (>=7.0.0,<9.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: docker (>=6.0.1,<7.0.0)
 Requires-Dist: fastapi (>=0.56.0,<0.94.0)
 Requires-Dist: filelock (>=3.8.0,<4.0.0)
 Requires-Dist: gitignorefile (>=1.1.2,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.2,<5.0)
 Requires-Dist: importlib-resources (>=5.2.0,<6.0.0)
-Requires-Dist: ipython (>=7.10.0) ; extra == "notebook"
-Requires-Dist: ipywidgets (>=7.6.0) ; extra == "notebook"
 Requires-Dist: packaging (>=20.0,<24.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: pygments (>=2.12.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-socketio[client] (>=5.5.2,<6.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: requests (>=2.23.0,<2.29.0)
```


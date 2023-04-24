# Comparing `tmp/gitlab-runner-tart-driver-0.1.3.tar.gz` & `tmp/gitlab-runner-tart-driver-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.1.3.tar", last modified: Fri Apr 21 09:03:47 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.1.4.tar", last modified: Mon Apr 24 09:46:19 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.1.3.tar` & `gitlab-runner-tart-driver-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.405937 gitlab-runner-tart-driver-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    15758 2023-04-21 09:03:47.405937 gitlab-runner-tart-driver-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    15237 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.399937 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.403937 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)     9267 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     2145 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.404937 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     7443 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.401937 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15758 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      986 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 09:03:47.405937 gitlab-runner-tart-driver-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.975574 gitlab-runner-tart-driver-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    18383 2023-04-24 09:46:19.975574 gitlab-runner-tart-driver-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    17862 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.968573 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.972574 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10205 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.974574 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8703 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.974574 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2533 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.970574 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18383 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 09:46:19.975574 gitlab-runner-tart-driver-0.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.1.3/LICENSE.txt` & `gitlab-runner-tart-driver-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.3/PKG-INFO` & `gitlab-runner-tart-driver-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,46 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Gitlab Runner Custom Tart Driver
 
+- [Gitlab Runner Custom Tart Driver](#gitlab-runner-custom-tart-driver)
+  - [About](#about)
+  - [Setup](#setup)
+    - [GitLab Runner Configuration](#gitlab-runner-configuration)
+  - [GitLab CI](#gitlab-ci)
+    - [Private OCI Registries](#private-oci-registries)
+    - [Configuring the SSH Credentials](#configuring-the-ssh-credentials)
+  - [Advanced Configuration](#advanced-configuration)
+    - [GitLab Runner Installation](#gitlab-runner-installation)
+    - [Concurrency](#concurrency)
+    - [Host Cache and Builds directories](#host-cache-and-builds-directories)
+    - [Volume Mounts](#volume-mounts)
+    - [Auto Host Resource Distribution](#auto-host-resource-distribution)
+    - [Custom `shell`](#custom-shell)
+    - [Custom `pull_policy`](#custom-pull_policy)
+  - [CLI](#cli)
+    - [CLI Parameters for `config.toml`](#cli-parameters-for-configtoml)
+    - [Command `config`](#command-config)
+    - [Command `prepare`](#command-prepare)
+    - [Command `run`](#command-run)
+    - [Command `cleanup`](#command-cleanup)
+
 ## About
 
 [Tart](https://tart.run) is a virtualization toolset to build, run and manage macOS and Linux virtual machines on Apple Silicon. Tart is using Apple’s native Virtualization.Framework that was developed along with architecting the first M1 chip. This seamless integration between hardware and software ensures smooth performance without any drawbacks.
 
 For storing virtual machine images Tart integrates with **OCI-compatible container registries**. This allows you to work with virtual machines as you used to with Docker containers.
 
 This Custom GitLab Runner Extension integrates [Tart](https://tart.run) semlessly into the GitLabCI ecosystem with similar functionality as the well `docker-runner`
@@ -229,14 +251,28 @@
   artifacts:
     paths:
       - artifact.txt
 ```
 
 ## Advanced Configuration
 
+### GitLab Runner Installation
+
+To have the full GitLabCI functionality in your pipelines like the capabilties to upload artifacts, you will need to *ensure* that the `gitlab-runner` is available within your VM. The `prepare` script can help you to ensure the presence and even install a specific version for you.
+Use `--install-gitlab-runner` to tell the driver to check for a valid runner installation. Per default, if an installation is found that version is used. If you want to ensure that you have always the `latest` or a specific version you can use `--force-install-gitlab-runner` and `--gitlab-runner-version` to indicate your concrete setup.
+
+The installation will follow these simple steps to ensure the proper `gitlab-runner` setup.
+
+1. Check if gitlab-runner is already installed by trying to execute it
+2. If the runner is not present or force install is enabled
+   1. Check if `curl` can be used to download and install the version specified to `/usr/local/bin`
+   2. Check if `wget` can be used to download and install the version specified to `/usr/local/bin`
+   3. Check if `brew` can be used to install the version specified
+   4. Fail if none of the tools is available
+
 ### Concurrency
 
 Currently `tart` only supports two executions of VMs at the same time. This limits the scalability of the solution on a single host. Please ensure you are setting the `concurrent` setting to a maximum of `2` in your `config.toml`.
 
 ```ini
 concurrent = 2 # <-- ATTENTION: ensure not sure go higher than '2'
 check_interval = 0
@@ -310,14 +346,16 @@
 
 ### Custom `pull_policy`
 
 You can use a custom `pull_policy`. The default policy is `if-not-present`
 
 see **Command `prepare`**
 
+## CLI
+
 ### CLI Parameters for `config.toml`
 
 The `gitlab-runner-tart-driver` gives a number of advanced configuration options. Use `gitlab-runner-tart-driver [stage] --help` to get a full list of options that you can pass to the exectuable using your `config.toml` file.
 
 ```
 Usage: gitlab-runner-tart-driver [OPTIONS] COMMAND [ARGS]...
 
@@ -373,16 +411,23 @@
                                   support two concurrent VMs
   --cache-dir TEXT                Caching dir to be used.
   --builds-dir TEXT               Path to the builds directory.
   --timeout INTEGER               Timeout in seconds for the VM to be
                                   reachable via SSH.
   --volume TEXT                   Volume mount definition with docker syntax.
                                   <host_dir>:<vm_dir>[:ro]
+  --install-gitlab-runner         Will install the gitlab-runner if not
+                                  present.
+  --force-install-gitlab-runner   This will force the installation of the
+                                  GitLab Runner independent of a previously
+                                  installed version
+  --gitlab-runner-version TEXT    The version of the GitLab Runner to be
+                                  installed. Example '15.11.0'
   -x, --tart-executable TEXT      Path to the tart executable.
-  --help                          Show this message and exit.                      Show this message and exit.
+  --help                          Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
```

### Comparing `gitlab-runner-tart-driver-0.1.3/README.md` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,46 @@
+Metadata-Version: 2.1
+Name: gitlab-runner-tart-driver
+Version: 0.1.4
+Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
+Author: Matthias Schmieder
+Author-email: schmieder.matthias@gmail.com
+License: BSD
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Version Control
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Gitlab Runner Custom Tart Driver
 
+- [Gitlab Runner Custom Tart Driver](#gitlab-runner-custom-tart-driver)
+  - [About](#about)
+  - [Setup](#setup)
+    - [GitLab Runner Configuration](#gitlab-runner-configuration)
+  - [GitLab CI](#gitlab-ci)
+    - [Private OCI Registries](#private-oci-registries)
+    - [Configuring the SSH Credentials](#configuring-the-ssh-credentials)
+  - [Advanced Configuration](#advanced-configuration)
+    - [GitLab Runner Installation](#gitlab-runner-installation)
+    - [Concurrency](#concurrency)
+    - [Host Cache and Builds directories](#host-cache-and-builds-directories)
+    - [Volume Mounts](#volume-mounts)
+    - [Auto Host Resource Distribution](#auto-host-resource-distribution)
+    - [Custom `shell`](#custom-shell)
+    - [Custom `pull_policy`](#custom-pull_policy)
+  - [CLI](#cli)
+    - [CLI Parameters for `config.toml`](#cli-parameters-for-configtoml)
+    - [Command `config`](#command-config)
+    - [Command `prepare`](#command-prepare)
+    - [Command `run`](#command-run)
+    - [Command `cleanup`](#command-cleanup)
+
 ## About
 
 [Tart](https://tart.run) is a virtualization toolset to build, run and manage macOS and Linux virtual machines on Apple Silicon. Tart is using Apple’s native Virtualization.Framework that was developed along with architecting the first M1 chip. This seamless integration between hardware and software ensures smooth performance without any drawbacks.
 
 For storing virtual machine images Tart integrates with **OCI-compatible container registries**. This allows you to work with virtual machines as you used to with Docker containers.
 
 This Custom GitLab Runner Extension integrates [Tart](https://tart.run) semlessly into the GitLabCI ecosystem with similar functionality as the well `docker-runner`
@@ -214,14 +251,28 @@
   artifacts:
     paths:
       - artifact.txt
 ```
 
 ## Advanced Configuration
 
+### GitLab Runner Installation
+
+To have the full GitLabCI functionality in your pipelines like the capabilties to upload artifacts, you will need to *ensure* that the `gitlab-runner` is available within your VM. The `prepare` script can help you to ensure the presence and even install a specific version for you.
+Use `--install-gitlab-runner` to tell the driver to check for a valid runner installation. Per default, if an installation is found that version is used. If you want to ensure that you have always the `latest` or a specific version you can use `--force-install-gitlab-runner` and `--gitlab-runner-version` to indicate your concrete setup.
+
+The installation will follow these simple steps to ensure the proper `gitlab-runner` setup.
+
+1. Check if gitlab-runner is already installed by trying to execute it
+2. If the runner is not present or force install is enabled
+   1. Check if `curl` can be used to download and install the version specified to `/usr/local/bin`
+   2. Check if `wget` can be used to download and install the version specified to `/usr/local/bin`
+   3. Check if `brew` can be used to install the version specified
+   4. Fail if none of the tools is available
+
 ### Concurrency
 
 Currently `tart` only supports two executions of VMs at the same time. This limits the scalability of the solution on a single host. Please ensure you are setting the `concurrent` setting to a maximum of `2` in your `config.toml`.
 
 ```ini
 concurrent = 2 # <-- ATTENTION: ensure not sure go higher than '2'
 check_interval = 0
@@ -295,14 +346,16 @@
 
 ### Custom `pull_policy`
 
 You can use a custom `pull_policy`. The default policy is `if-not-present`
 
 see **Command `prepare`**
 
+## CLI
+
 ### CLI Parameters for `config.toml`
 
 The `gitlab-runner-tart-driver` gives a number of advanced configuration options. Use `gitlab-runner-tart-driver [stage] --help` to get a full list of options that you can pass to the exectuable using your `config.toml` file.
 
 ```
 Usage: gitlab-runner-tart-driver [OPTIONS] COMMAND [ARGS]...
 
@@ -358,16 +411,23 @@
                                   support two concurrent VMs
   --cache-dir TEXT                Caching dir to be used.
   --builds-dir TEXT               Path to the builds directory.
   --timeout INTEGER               Timeout in seconds for the VM to be
                                   reachable via SSH.
   --volume TEXT                   Volume mount definition with docker syntax.
                                   <host_dir>:<vm_dir>[:ro]
+  --install-gitlab-runner         Will install the gitlab-runner if not
+                                  present.
+  --force-install-gitlab-runner   This will force the installation of the
+                                  GitLab Runner independent of a previously
+                                  installed version
+  --gitlab-runner-version TEXT    The version of the GitLab Runner to be
+                                  installed. Example '15.11.0'
   -x, --tart-executable TEXT      Path to the tart executable.
-  --help                          Show this message and exit.                      Show this message and exit.
+  --help                          Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
@@ -388,8 +448,8 @@
 Usage: gitlab-runner-tart-driver cleanup [OPTIONS]
 
   Command to greet a user.
 
 Options:
   -x, --tart-executable TEXT  Path to the tart executable.
   --help                      Show this message and exit.
-```
+```
```

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,35 @@
     "volumes",
     required=False,
     default=[],
     type=str,
     multiple=True,
     help="Volume mount definition with docker syntax. <host_dir>:<vm_dir>[:ro]",
 )
+@click.option(
+    "--install-gitlab-runner",
+    required=False,
+    type=bool,
+    is_flag=True,
+    help="Will install the gitlab-runner if not present.",
+)
+@click.option(
+    "--force-install-gitlab-runner",
+    required=False,
+    type=str,
+    is_flag=True,
+    help="This will force the installation of the GitLab Runner independent of a previously installed version",
+)
+@click.option(
+    "--gitlab-runner-version",
+    required=False,
+    type=str,
+    default="latest",
+    help="The version of the GitLab Runner to be installed. Example '15.11.0'",
+)
 @click.option("-x", "--tart-executable", required=False, default="tart", type=str, help="Path to the tart executable.")
 def prepare(
     default_ssh_username,
     default_ssh_password,
     registry_username,
     registry_password,
     registry,
@@ -93,14 +114,17 @@
     pull_policy,
     auto_resources,
     concurrency,
     cache_dir,
     builds_dir,
     timeout,
     volumes,
+    install_gitlab_runner,
+    force_install_gitlab_runner,
+    gitlab_runner_version,
     tart_executable,
 ):
     """Prepare the environment and start the tart VM."""
 
     print_host_spec()
 
     p = GitLabCustomCommandConfig()
@@ -234,10 +258,16 @@
         )
 
     if not builds_dir:
         ssh_session.exec_ssh_command(
             f"sudo mkdir -p {remote_build_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_build_dir}",
         )
 
+    if install_gitlab_runner:
+        click.echo(
+            f"[INFO] Installing GitLab Runner '{gitlab_runner_version}' [force: '{force_install_gitlab_runner}']"
+        )
+        tart.install_gitlab_runner(name=tart_vm_name, username=p.tart_ssh_username, password=p.tart_ssh_password)
+
     tart.print_spec(tart_vm_name)
 
     sys.exit(0)
```

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/run.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/tart.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 import re
 import subprocess
+import tempfile
 
 import click
+from jinja2 import Environment
+from jinja2 import FileSystemLoader
 from paramiko import MissingHostKeyPolicy
 from paramiko import SSHClient
 from pydantic import BaseModel
 from pydantic import Field
 from tabulate import tabulate
 
 
@@ -214,7 +217,33 @@
 
     def ssh_session(self, name, username, password) -> TartSshSession:
         ip = self.ip(name=name)
         if not ip:
             raise ValueError("Could not retrievew IP")
 
         return TartSshSession(ip=ip, username=username, password=password)
+
+    def install_gitlab_runner(self, name, username, password, force=False, version="latest"):
+        file_loader = FileSystemLoader(os.path.join(os.path.dirname(__file__), os.path.pardir, "scripts"))
+        env = Environment(loader=file_loader)
+        template = env.get_template("install-gitlab-runner.sh.j2")
+
+        data = {"gitlab_runner_force_install": "true" if force else "false", "gitlab_runner_version": version}
+
+        temp = tempfile.NamedTemporaryFile()
+        with open(temp.name, "w") as f:
+            f.write(template.render(**data))
+        f.close()
+
+        remote_temp_dir = "/tmp"
+        remote_script_path = os.path.join(remote_temp_dir, "install-gitlab-runner.sh")
+
+        ssh_session = self.ssh_session(name=name, username=username, password=password)
+        sftp = ssh_session.ssh_client.open_sftp()
+        sftp.put(temp.name, remote_script_path)
+        sftp.close()
+
+        # ssh_session.exec_ssh_command(f"cd {remote_build_dir}")
+        script_exit_code = ssh_session.exec_ssh_command(f"bash -l {remote_script_path}", get_pty=True)
+
+        if script_exit_code != 0:
+            raise ValueError("Error when installing GitLab Runner")
```

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-Metadata-Version: 2.1
-Name: gitlab-runner-tart-driver
-Version: 0.1.3
-Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
-Author: Matthias Schmieder
-Author-email: schmieder.matthias@gmail.com
-License: BSD
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Version Control
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Gitlab Runner Custom Tart Driver
 
+- [Gitlab Runner Custom Tart Driver](#gitlab-runner-custom-tart-driver)
+  - [About](#about)
+  - [Setup](#setup)
+    - [GitLab Runner Configuration](#gitlab-runner-configuration)
+  - [GitLab CI](#gitlab-ci)
+    - [Private OCI Registries](#private-oci-registries)
+    - [Configuring the SSH Credentials](#configuring-the-ssh-credentials)
+  - [Advanced Configuration](#advanced-configuration)
+    - [GitLab Runner Installation](#gitlab-runner-installation)
+    - [Concurrency](#concurrency)
+    - [Host Cache and Builds directories](#host-cache-and-builds-directories)
+    - [Volume Mounts](#volume-mounts)
+    - [Auto Host Resource Distribution](#auto-host-resource-distribution)
+    - [Custom `shell`](#custom-shell)
+    - [Custom `pull_policy`](#custom-pull_policy)
+  - [CLI](#cli)
+    - [CLI Parameters for `config.toml`](#cli-parameters-for-configtoml)
+    - [Command `config`](#command-config)
+    - [Command `prepare`](#command-prepare)
+    - [Command `run`](#command-run)
+    - [Command `cleanup`](#command-cleanup)
+
 ## About
 
 [Tart](https://tart.run) is a virtualization toolset to build, run and manage macOS and Linux virtual machines on Apple Silicon. Tart is using Apple’s native Virtualization.Framework that was developed along with architecting the first M1 chip. This seamless integration between hardware and software ensures smooth performance without any drawbacks.
 
 For storing virtual machine images Tart integrates with **OCI-compatible container registries**. This allows you to work with virtual machines as you used to with Docker containers.
 
 This Custom GitLab Runner Extension integrates [Tart](https://tart.run) semlessly into the GitLabCI ecosystem with similar functionality as the well `docker-runner`
@@ -229,14 +236,28 @@
   artifacts:
     paths:
       - artifact.txt
 ```
 
 ## Advanced Configuration
 
+### GitLab Runner Installation
+
+To have the full GitLabCI functionality in your pipelines like the capabilties to upload artifacts, you will need to *ensure* that the `gitlab-runner` is available within your VM. The `prepare` script can help you to ensure the presence and even install a specific version for you.
+Use `--install-gitlab-runner` to tell the driver to check for a valid runner installation. Per default, if an installation is found that version is used. If you want to ensure that you have always the `latest` or a specific version you can use `--force-install-gitlab-runner` and `--gitlab-runner-version` to indicate your concrete setup.
+
+The installation will follow these simple steps to ensure the proper `gitlab-runner` setup.
+
+1. Check if gitlab-runner is already installed by trying to execute it
+2. If the runner is not present or force install is enabled
+   1. Check if `curl` can be used to download and install the version specified to `/usr/local/bin`
+   2. Check if `wget` can be used to download and install the version specified to `/usr/local/bin`
+   3. Check if `brew` can be used to install the version specified
+   4. Fail if none of the tools is available
+
 ### Concurrency
 
 Currently `tart` only supports two executions of VMs at the same time. This limits the scalability of the solution on a single host. Please ensure you are setting the `concurrent` setting to a maximum of `2` in your `config.toml`.
 
 ```ini
 concurrent = 2 # <-- ATTENTION: ensure not sure go higher than '2'
 check_interval = 0
@@ -310,14 +331,16 @@
 
 ### Custom `pull_policy`
 
 You can use a custom `pull_policy`. The default policy is `if-not-present`
 
 see **Command `prepare`**
 
+## CLI
+
 ### CLI Parameters for `config.toml`
 
 The `gitlab-runner-tart-driver` gives a number of advanced configuration options. Use `gitlab-runner-tart-driver [stage] --help` to get a full list of options that you can pass to the exectuable using your `config.toml` file.
 
 ```
 Usage: gitlab-runner-tart-driver [OPTIONS] COMMAND [ARGS]...
 
@@ -373,16 +396,23 @@
                                   support two concurrent VMs
   --cache-dir TEXT                Caching dir to be used.
   --builds-dir TEXT               Path to the builds directory.
   --timeout INTEGER               Timeout in seconds for the VM to be
                                   reachable via SSH.
   --volume TEXT                   Volume mount definition with docker syntax.
                                   <host_dir>:<vm_dir>[:ro]
+  --install-gitlab-runner         Will install the gitlab-runner if not
+                                  present.
+  --force-install-gitlab-runner   This will force the installation of the
+                                  GitLab Runner independent of a previously
+                                  installed version
+  --gitlab-runner-version TEXT    The version of the GitLab Runner to be
+                                  installed. Example '15.11.0'
   -x, --tart-executable TEXT      Path to the tart executable.
-  --help                          Show this message and exit.                      Show this message and exit.
+  --help                          Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
@@ -403,8 +433,8 @@
 Usage: gitlab-runner-tart-driver cleanup [OPTIONS]
 
   Command to greet a user.
 
 Options:
   -x, --tart-executable TEXT  Path to the tart executable.
   --help                      Show this message and exit.
-```
+```
```

### Comparing `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.txt
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 gitlab_runner_tart_driver/__init__.py
 gitlab_runner_tart_driver/__main__.py
 gitlab_runner_tart_driver/cli.py
 gitlab_runner_tart_driver.egg-info/PKG-INFO
@@ -17,8 +18,9 @@
 gitlab_runner_tart_driver/commands/config.py
 gitlab_runner_tart_driver/commands/prepare.py
 gitlab_runner_tart_driver/commands/run.py
 gitlab_runner_tart_driver/modules/__init__.py
 gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
 gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
 gitlab_runner_tart_driver/modules/tart.py
-gitlab_runner_tart_driver/modules/utils.py
+gitlab_runner_tart_driver/modules/utils.py
+gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
```

### Comparing `gitlab-runner-tart-driver-0.1.3/setup.py` & `gitlab-runner-tart-driver-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.1.3"
+version = "0.1.4"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```


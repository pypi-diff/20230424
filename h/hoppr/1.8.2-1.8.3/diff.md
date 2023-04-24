# Comparing `tmp/hoppr-1.8.2.tar.gz` & `tmp/hoppr-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.2.tar", max compression
+gzip compressed data, was "hoppr-1.8.3.tar", max compression
```

## Comparing `hoppr-1.8.2.tar` & `hoppr-1.8.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1084 2023-04-18 17:17:59.000000 hoppr-1.8.2/LICENSE
--rw-r--r--   0        0        0     1214 2023-04-18 17:17:59.000000 hoppr-1.8.2/README.md
--rw-r--r--   0        0        0     1035 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    10990 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10732 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12943 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10272 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     3321 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4664 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     3992 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6369 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7978 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4429 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3043 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5403 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4577 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     4810 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/in_toto.py
--rw-r--r--   0        0        0     3074 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/base.py
--rw-r--r--   0        0        0     3778 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17515 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/py.typed
--rw-r--r--   0        0        0     3975 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/transfer.py
--rw-r--r--   0        0        0     4118 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    25427 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/result.py
--rw-r--r--   0        0        0     5305 2023-04-18 17:17:59.000000 hoppr-1.8.2/hoppr/utils.py
--rw-r--r--   0        0        0     3614 2023-04-18 17:17:59.000000 hoppr-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-24 21:09:54.000000 hoppr-1.8.3/LICENSE
+-rw-r--r--   0        0        0     1214 2023-04-24 21:09:54.000000 hoppr-1.8.3/README.md
+-rw-r--r--   0        0        0     1035 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    10990 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10732 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     6256 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/cli/hopctl.py
+-rw-r--r--   0        0        0      563 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12943 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0    10272 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     3321 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4664 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     3992 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6369 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7978 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     4418 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3043 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3739 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5318 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5301 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4577 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     4810 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6847 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3074 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1708 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1409 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    17452 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/py.typed
+-rw-r--r--   0        0        0     3975 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5071 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/net.py
+-rw-r--r--   0        0        0     4323 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    25427 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/resources/hoppr-hippo-large.ansi
+-rw-r--r--   0        0        0    10419 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0     4036 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/result.py
+-rw-r--r--   0        0        0     5791 2023-04-24 21:09:54.000000 hoppr-1.8.3/hoppr/utils.py
+-rw-r--r--   0        0        0     3614 2023-04-24 21:09:54.000000 hoppr-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.3/PKG-INFO
```

### Comparing `hoppr-1.8.2/LICENSE` & `hoppr-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/README.md` & `hoppr-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/__init__.py` & `hoppr-1.8.3/hoppr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.2"
+__version__ = "1.8.3"
```

### Comparing `hoppr-1.8.2/hoppr/base_plugins/collector.py` & `hoppr-1.8.3/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/base_plugins/hoppr.py` & `hoppr-1.8.3/hoppr/base_plugins/hoppr.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/cli/hopctl.py` & `hoppr-1.8.3/hoppr/cli/hopctl.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/constants.py` & `hoppr-1.8.3/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.8.3/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_git_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_nexus_search.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,18 +80,20 @@
         source_url = RepositoryUrl(url=repo_url)
         if not re.match(pattern="^.*simple/?$", string=f"{source_url}"):
             source_url /= "simple"
 
         password_list = []
 
         if creds is not None:
-            source_url.username = creds.username
-            source_url.password = creds.password.get_secret_value()
-            source_url.netloc = f"{source_url.username}:{source_url.password}@{source_url.netloc}"
-            password_list = [source_url.password]
+            source_url = RepositoryUrl(
+                url=source_url.url,
+                username=creds.username,
+                password=creds.password.get_secret_value(),
+            )
+            password_list = [creds.password.get_secret_value()]
 
         target_dir = self.directory_for(purl.type, repo_url, subdir=f"{purl.name}_{purl.version}")
 
         self.get_logger().info(msg=f"Target directory: {target_dir}", indent_level=2)
 
         command = [
             *self.base_command,
```

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.8.3/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/composite_collector.py` & `hoppr-1.8.3/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.8.3/hoppr/core_plugins/delta_sbom.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from hoppr import __version__
 from hoppr.base_plugins.hoppr import HopprPlugin, hoppr_process
 from hoppr.exceptions import HopprError
 from hoppr.models.manifest import Component, Manifest, Sbom
 from hoppr.models.types import BomAccess
 from hoppr.result import Result
-from hoppr.utils import dedup_list, load_string
+from hoppr.utils import dedup_list, get_package_url, load_string
 
 
 class DeltaSbom(HopprPlugin):
     """
     Plugin to remove SBOM components that are specified by a "previous" SBOM
     """
 
@@ -117,16 +117,16 @@
                 return False
 
         return True
 
     @staticmethod
     def _component_match(new_comp: Component, prev_comp: Component) -> bool:
 
-        new_purl: PackageURL = PackageURL.from_string(new_comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
-        prev_purl: PackageURL = PackageURL.from_string(prev_comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
+        new_purl: PackageURL = get_package_url(new_comp.purl)
+        prev_purl: PackageURL = get_package_url(prev_comp.purl)
 
         if not DeltaSbom._purl_match(new_purl, prev_purl):
             return False
 
         hash_matches = 0
 
         for new_hash in new_comp.hashes or []:
```

### Comparing `hoppr-1.8.2/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.8.3/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/oras_registry.py` & `hoppr-1.8.3/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.8.3/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/in_toto.py` & `hoppr-1.8.3/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/main.py` & `hoppr-1.8.3/hoppr/main.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/mem_logger.py` & `hoppr-1.8.3/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/models/__init__.py` & `hoppr-1.8.3/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/models/__main__.py` & `hoppr-1.8.3/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/models/base.py` & `hoppr-1.8.3/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/models/credentials.py` & `hoppr-1.8.3/hoppr/models/credentials.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,27 +29,28 @@
 
     @root_validator(pre=True, allow_reuse=True)
     @classmethod
     def validate_credential_required_service(cls, values: DictStrAny) -> DictStrAny:
         """
         Dynamically parse credentials using specified environment variables
         """
-        user_env = values.get("user_env")
-        if user_env is not None:
-            username = os.environ.get(values["user_env"], "")
-            assert len(username) > 0
-            values["user"] = username
-
-        pass_env = values.get("pass_env", "")
-        assert len(pass_env) > 0
-
-        password = os.environ.get(pass_env, "")
-        assert len(password) > 0
-
-        values["password"] = SecretStr(password)
+        try:
+            if (user_env := values.get("user_env")) is not None:
+                if username := os.environ[user_env]:
+                    values["user"] = username
+                else:
+                    raise ValueError(user_env)
+
+            if (pass_env := values.get("pass_env")) is not None:
+                if password := os.environ[pass_env]:
+                    values["password"] = SecretStr(password)
+                else:
+                    raise ValueError(pass_env)
+        except (KeyError, ValueError) as ex:
+            raise ValueError(f"The environment variable {ex} must be set with a non-empty string") from ex
 
         return values
 
 
 class CredentialsFile(HopprBaseSchemaModel):
     """
     Credentials file data model
```

### Comparing `hoppr-1.8.2/hoppr/models/manifest.py` & `hoppr-1.8.3/hoppr/models/manifest.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,26 +38,19 @@
     """
 
     url: RepositoryUrl
     description: NoneStr = None
 
     @validator("url", pre=True)
     @classmethod
-    def validate_url(cls, url: RepositoryUrl | str) -> RepositoryUrl:
+    def validate_url(cls, url: str | RepositoryUrl) -> RepositoryUrl:
         """
         Validate URL string
         """
         if isinstance(url, str):
-            # Normalize URL scheme (e.g. `file:` to `file://`)
-            if url.endswith(":"):
-                url = f"{url}//"
-
-            if "://" not in url:
-                url = f"http://{url}"
-
             url = RepositoryUrl(url=url)
 
         return url
 
 
 # Dynamic Repositories model with PurlType values as attribute names
 purl_type_repo_mapping = {str(purl_type): (list[Repository], Field([], unique_items=True)) for purl_type in PurlType}
@@ -118,14 +111,15 @@
 
 
 IncludeRef = Annotated[LocalFile | UrlFile, Field(..., description="Reference to a local or remote manifest file")]
 Includes = Annotated[list[IncludeRef], Field(..., description="List of manifest files to load")]
 SbomRef = Annotated[LocalFile | OciFile | UrlFile, Field(..., description="Reference to a local or remote SBOM file")]
 Sboms = Annotated[list[SbomRef], Field(..., description="List of SBOMs to process")]
 SbomRefMap = Annotated[MutableMapping[SbomRef, "Sbom"], Field(...)]
+ComponentPurlMap = Annotated[MutableMapping[str, "Component"], Field(...)]
 
 
 class ExternalReference(HopprBaseModel, ExternalReferenceSpecVersion14):
     """
     ExternalReference data model derived from HopprBaseModel
     """
 
@@ -149,14 +143,30 @@
         "Config for Component model"
         extra = Extra.allow
 
     components: list[Component] | None = Field(None)  # type: ignore[assignment]
     externalReferences: list[ExternalReference] | None = Field(None)  # type: ignore[assignment]
     properties: list[Property] | None = Field(None)  # type: ignore[assignment]
 
+    # Attributes not included in schema
+    component_lookup: ClassVar[ComponentPurlMap] = {}
+
+    @classmethod
+    def find(cls, purl_string: str) -> Component | None:
+        """
+        Look up Component object by package URL string
+
+        Args:
+            purl_string (str): Package URL string to look up
+
+        Returns:
+            Component | None: Component object if found, otherwise None
+        """
+        return cls.component_lookup.get(purl_string)
+
 
 class Sbom(HopprBaseModel, SbomSpecVersion14):
     """
     Sbom data model derived from HopprBaseModel
     """
 
     class Config(HopprBaseModel.Config):  # pylint: disable=too-few-public-methods
@@ -170,15 +180,15 @@
     # Attributes not included in schema
     loaded_sboms: ClassVar[SbomRefMap] = {}
     consolidated_sbom: ClassVar[Sbom]
 
     @classmethod
     def find(cls, ref_type: Literal["local", "oci", "url"], location: str | Path) -> Sbom | None:
         """
-        Lookup SBOM object by reference
+        Look up SBOM object by reference
 
         Args:
             ref_type (Literal["local", "oci", "url"]): Type of SBOM reference
             location (str | Path): Location of SBOM reference
 
         Returns:
             Sbom | None: SBOM object if found, otherwise None
@@ -334,15 +344,15 @@
                 )
 
                 for component in loaded.components or []:
                     purl_str = getattr(component, "purl", None)
                     if purl_str is None:
                         continue
 
-                    purl_type = PackageURL.from_string(purl_str).type
+                    purl_type = hoppr.utils.get_package_url(purl_str).type
 
                     if component.properties is None:
                         component.properties = []
 
                     # Generate the repository search sequence
                     search_sequence = SearchSequence(
                         version="v1", repositories=[str(repo.url) for repo in values["repositories"][purl_type]]
@@ -369,41 +379,34 @@
                 Sbom.loaded_sboms[sbom_ref] = loaded
 
         return sboms
 
     @classmethod
     def _add_component(cls, component: Component) -> None:
         # Remove purl qualifiers for later comparison
-        purl: PackageURL = PackageURL.from_string(component.purl)  # pyright: ignore[reportGeneralTypeIssues]
+        purl: PackageURL = hoppr.utils.get_package_url(component.purl)
         purl.qualifiers.clear()
         purl_str = purl.to_string()
 
-        # Check previously loaded components for component to be added
-        for loaded in Sbom.consolidated_sbom.components:
-            loaded_purl: PackageURL = PackageURL.from_string(loaded.purl)  # pyright: ignore[reportGeneralTypeIssues]
-            loaded_purl.qualifiers.clear()
-            loaded_purl_str = loaded_purl.to_string()
-
-            if loaded.externalReferences is None:
-                loaded.externalReferences = []  # pragma: no cover
+        loaded = Component.find(purl_str)
+        # Merge component into previously loaded component
+        if loaded is not None:
+            loaded.externalReferences = hoppr.utils.dedup_list(
+                [*(loaded.externalReferences or []), *(component.externalReferences or [])]
+            )
 
             if loaded.properties is None:
                 loaded.properties = []  # pragma: no cover
 
-            if purl_str == loaded_purl_str:
-                # Merge component into previously loaded component
-                loaded.externalReferences = list(set(loaded.externalReferences + (component.externalReferences or [])))
-
-                for prop in component.properties or []:
-                    if prop.name not in [loaded_prop.name for loaded_prop in loaded.properties]:
-                        loaded.properties.append(prop)
-
-                return
-
-        Sbom.consolidated_sbom.components.append(Component.parse_obj(component))
+            for prop in component.properties or []:
+                if prop.name not in [loaded_prop.name for loaded_prop in loaded.properties]:
+                    loaded.properties.append(prop)
+        else:
+            Sbom.consolidated_sbom.components.append(component)
+            Component.component_lookup[purl_str] = component
 
     @classmethod
     def _get_ref_url(cls, sbom_ref: SbomRef) -> str | None:
         match sbom_ref:
             case LocalFile():
                 return sbom_ref.local.as_uri()
             case OciFile():
```

### Comparing `hoppr-1.8.2/hoppr/models/transfer.py` & `hoppr-1.8.3/hoppr/models/transfer.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/net.py` & `hoppr-1.8.3/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/oci_artifacts.py` & `hoppr-1.8.3/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/plugin_utils.py` & `hoppr-1.8.3/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/processor.py` & `hoppr-1.8.3/hoppr/processor.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.8.3/hoppr/resources/hoppr-hippo-large.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.8.3/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/result.py` & `hoppr-1.8.3/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.2/hoppr/utils.py` & `hoppr-1.8.3/hoppr/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 """
 from __future__ import annotations
 
 import importlib
 import inspect
 
 from abc import ABCMeta
+from functools import cache
 from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING, Any, Type
 
+from packageurl import PackageURL
 from ruamel.yaml import YAML
 from ruamel.yaml.parser import ParserError as YAMLParserError
 from ruamel.yaml.scanner import ScannerError as YAMLScannerError
 
 from hoppr.exceptions import HopprLoadDataError, HopprPluginError
 
 if TYPE_CHECKING:
@@ -159,7 +161,22 @@
             deleted.update(remove_empty(subdir))
 
     if directory.is_dir() and not any(directory.iterdir()):
         directory.rmdir()
         deleted.add(directory)
 
     return deleted
+
+
+@cache
+def get_package_url(purl_string: str) -> PackageURL:
+    """
+    Get the PackageURL for a given purl_string and store it in a cache for improved performance.
+
+    Args:
+        purl_string (str): The string representation of a Package URL
+
+    Returns:
+        PackageURL: The object representation of a PackageURL
+
+    """
+    return PackageURL.from_string(purl_string)  # pyright: ignore[reportGeneralTypeIssues]
```

### Comparing `hoppr-1.8.2/pyproject.toml` & `hoppr-1.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.8.2"
+version = "1.8.3"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
```

### Comparing `hoppr-1.8.2/PKG-INFO` & `hoppr-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.2
+Version: 1.8.3
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```


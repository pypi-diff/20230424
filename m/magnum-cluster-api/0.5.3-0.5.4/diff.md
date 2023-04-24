# Comparing `tmp/magnum_cluster_api-0.5.3.tar.gz` & `tmp/magnum_cluster_api-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.5.3.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.5.4.tar", max compression
```

## Comparing `magnum_cluster_api-0.5.3.tar` & `magnum_cluster_api-0.5.4.tar`

### file list

```diff
@@ -1,62 +1,65 @@
--rw-r--r--   0        0        0    10142 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/LICENSE
--rw-r--r--   0        0        0     2795 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/README.md
--rw-r--r--   0        0        0        0 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-04-13 21:21:56.335576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-04-13 21:21:56.315576 magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0      843 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     4019 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4182 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     1778 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    10862 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     2155 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3171 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-04-13 21:21:53.687599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4034 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3307 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     1526 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     2880 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    11719 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3616 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    74957 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/service.py
--rw-r--r--   0        0        0     3445 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_helm.py
--rw-r--r--   0        0        0     1731 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_image_utils.py
--rw-r--r--   0        0        0     2759 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_images.py
--rw-r--r--   0        0        0     7554 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1186 2023-04-13 21:21:53.691599 magnum_cluster_api-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 magnum_cluster_api-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2795 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-04-24 16:49:36.448924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-04-24 16:49:36.448924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-04-24 16:49:36.448924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-04-24 16:49:36.548924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-04-24 16:49:36.448924 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-04-24 16:49:36.444923 magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0      843 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     4019 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     4182 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     1778 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    10862 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     2155 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3171 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-04-24 16:49:35.156916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4034 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3307 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     1526 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     2880 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    73565 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-04-24 16:49:35.160916 magnum_cluster_api-0.5.4/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0      942 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/conftest.py
+-rw-r--r--   0        0        0     3445 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_helm.py
+-rw-r--r--   0        0        0     1731 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_image_utils.py
+-rw-r--r--   0        0        0     2759 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_images.py
+-rw-r--r--   0        0        0     1717 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_resources.py
+-rw-r--r--   0        0        0     1192 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_utils.py
+-rw-r--r--   0        0        0     7684 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1186 2023-04-24 16:49:35.164916 magnum_cluster_api-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 magnum_cluster_api-0.5.4/PKG-INFO
```

### Comparing `magnum_cluster_api-0.5.3/LICENSE` & `magnum_cluster_api-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/README.md` & `magnum_cluster_api-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/image_loader.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/driver.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/images.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.5.4/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/structs.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,15 @@
                             repository=repository,
                         )
                     },
                     **{
                         f"storageclass-{vt.name}.yaml": yaml.dump(
                             {
                                 "apiVersion": objects.StorageClass.version,
+                                "allowVolumeExpansion": True,
                                 "kind": objects.StorageClass.kind,
                                 "metadata": {
                                     "annotations": {
                                         "storageclass.kubernetes.io/is-default-class": "true"
                                     }
                                     if default_volume_type.name == vt.name
                                     else {},
@@ -1240,14 +1241,81 @@
     KubeadmControlPlaneTemplate(api).apply()
     KubeadmConfigTemplate(api).apply()
     OpenStackMachineTemplate(api).apply()
     OpenStackClusterTemplate(api).apply()
     ClusterClass(api).apply()
 
 
+def generate_machine_deployments_for_cluster(
+    context: context.RequestContext, cluster: objects.Cluster
+) -> list:
+    auto_scaling_enabled = utils.get_auto_scaling_enabled(cluster)
+    return [
+        {
+            "class": "default-worker",
+            "name": ng.name,
+            "replicas": None if auto_scaling_enabled else ng.node_count,
+            "metadata": {
+                "annotations": {
+                    AUTOSCALE_ANNOTATION_MIN: f"{utils.get_node_group_min_node_count(ng)}",  # noqa: E501
+                    AUTOSCALE_ANNOTATION_MAX: f"{utils.get_node_group_max_node_count(context, ng)}",  # noqa: E501
+                }
+            }
+            if auto_scaling_enabled
+            else {},
+            "failureDomain": utils.get_cluster_label(cluster, "availability_zone", ""),
+            "machineHealthCheck": {
+                "enable": utils.get_cluster_label_as_bool(
+                    cluster, "auto_healing_enabled", True
+                )
+            },
+            "variables": {
+                "overrides": [
+                    {
+                        "name": "bootVolume",
+                        "value": {
+                            "size": utils.get_node_group_label_as_int(
+                                context,
+                                ng,
+                                "boot_volume_size",
+                                CONF.cinder.default_boot_volume_size,
+                            ),
+                            "type": utils.get_node_group_label(
+                                context,
+                                ng,
+                                "boot_volume_type",
+                                cinder.get_default_boot_volume_type(context),
+                            ),
+                        },
+                    },
+                    {
+                        "name": "flavor",
+                        "value": ng.flavor_id,
+                    },
+                    {
+                        "name": "imageRepository",
+                        "value": utils.get_node_group_label(
+                            context,
+                            ng,
+                            "container_infra_prefix",
+                            "quay.io/vexxhost",
+                        ),
+                    },
+                    {
+                        "name": "imageUUID",
+                        "value": ng.image_id,
+                    },
+                ],
+            },
+        }
+        for ng in cluster.nodegroups
+        if ng.role != "master" and not ng.status.startswith("DELETE")
+    ]
+
+
 class Cluster(ClusterBase):
     def __init__(
         self,
         context: context.RequestContext,
         api: pykube.HTTPClient,
         cluster: magnum_objects.Cluster,
     ):
@@ -1277,15 +1345,14 @@
 
     def get_or_none(self) -> objects.Cluster:
         return objects.Cluster.objects(self.api, namespace="magnum-system").get_or_none(
             name=utils.get_or_generate_cluster_api_name(self.api, self.cluster)
         )
 
     def get_object(self) -> objects.Cluster:
-        auto_scaling_enabled = utils.get_auto_scaling_enabled(self.cluster)
         return objects.Cluster(
             self.api,
             {
                 "apiVersion": objects.Cluster.version,
                 "kind": objects.Cluster.kind,
                 "metadata": {
                     "name": utils.get_or_generate_cluster_api_name(
@@ -1328,81 +1395,17 @@
                             "machineHealthCheck": {
                                 "enable": utils.get_cluster_label_as_bool(
                                     self.cluster, "auto_healing_enabled", True
                                 )
                             },
                         },
                         "workers": {
-                            "machineDeployments": [
-                                {
-                                    "class": "default-worker",
-                                    "name": ng.name,
-                                    "replicas": None
-                                    if auto_scaling_enabled
-                                    else ng.node_count,
-                                    "metadata": {
-                                        "annotations": {
-                                            AUTOSCALE_ANNOTATION_MIN: f"{utils.get_node_group_min_node_count(ng)}",  # noqa: E501
-                                            AUTOSCALE_ANNOTATION_MAX: f"{utils.get_node_group_max_node_count(self.context, ng)}",  # noqa: E501
-                                        }
-                                    }
-                                    if auto_scaling_enabled
-                                    else {},
-                                    "failureDomain": utils.get_cluster_label(
-                                        self.cluster, "availability_zone", ""
-                                    ),
-                                    "machineHealthCheck": {
-                                        "enable": utils.get_cluster_label_as_bool(
-                                            self.cluster, "auto_healing_enabled", True
-                                        )
-                                    },
-                                    "variables": {
-                                        "overrides": [
-                                            {
-                                                "name": "bootVolume",
-                                                "value": {
-                                                    "size": utils.get_node_group_label_as_int(
-                                                        self.context,
-                                                        ng,
-                                                        "boot_volume_size",
-                                                        CONF.cinder.default_boot_volume_size,
-                                                    ),
-                                                    "type": utils.get_node_group_label(
-                                                        self.context,
-                                                        ng,
-                                                        "boot_volume_type",
-                                                        cinder.get_default_boot_volume_type(
-                                                            self.context
-                                                        ),
-                                                    ),
-                                                },
-                                            },
-                                            {
-                                                "name": "flavor",
-                                                "value": ng.flavor_id,
-                                            },
-                                            {
-                                                "name": "imageRepository",
-                                                "value": utils.get_node_group_label(
-                                                    self.context,
-                                                    ng,
-                                                    "container_infra_prefix",
-                                                    "quay.io/vexxhost",
-                                                ),
-                                            },
-                                            {
-                                                "name": "imageUUID",
-                                                "value": ng.image_id,
-                                            },
-                                        ],
-                                    },
-                                }
-                                for ng in self.cluster.nodegroups
-                                if ng.role != "master"
-                            ]
+                            "machineDeployments": generate_machine_deployments_for_cluster(
+                                self.context, self.cluster
+                            ),
                         },
                         "variables": [
                             {
                                 "name": "apiServerLoadBalancer",
                                 "value": {
                                     "enabled": self.cluster.master_lb_enabled,
                                 },
```

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/service.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_helm.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_image_utils.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/tests/test_images.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.3/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.5.4/magnum_cluster_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import re
+import string
 import textwrap
 
 import pykube
 import shortuuid
 import yaml
 from magnum import objects as magnum_objects
 from magnum.common import context, exception, octavia
@@ -33,45 +34,48 @@
     return f"{get_or_generate_cluster_api_name(api, cluster)}-cloud-config"
 
 
 def get_or_generate_cluster_api_name(
     api: pykube.HTTPClient, cluster: magnum_objects.Cluster
 ) -> str:
     if cluster.stack_id is None:
-        cluster.stack_id = generate_cluster_api_name(api, cluster)
+        cluster.stack_id = generate_cluster_api_name(api)
         cluster.save()
     return cluster.stack_id
 
 
 @retry(retry=retry_if_exception_type(exception.Conflict))
 def generate_cluster_api_name(
     api: pykube.HTTPClient,
-    cluster: magnum_objects.Cluster,
 ) -> str:
-    name = f"{cluster.name}-{shortuuid.uuid()[:10].lower()}".replace(".", "-")
-    if (
-        objects.Cluster.objects(api)
-        .filter(namespace="magnum-system")
-        .get_or_none(name=name)
-        is not None
-    ):
+    alphabet = string.ascii_lowercase + string.digits
+    su = shortuuid.ShortUUID(alphabet=alphabet)
+
+    name = "kube-%s" % (su.random(length=5))
+    if cluster_exists(api, name):
         raise exception.Conflict("Generated name already exists")
     return name
 
 
+def cluster_exists(api: pykube.HTTPClient, name: str) -> bool:
+    try:
+        objects.Cluster.objects(api, namespace="magnum-system").get(name=name)
+        return True
+    except pykube.exceptions.ObjectDoesNotExist:
+        return False
+
+
 def generate_cloud_controller_manager_config(
     api: pykube.HTTPClient,
     cluster: magnum_objects.Cluster,
 ) -> str:
     """
     Generate coniguration for openstack-cloud-controller-manager if it does
     already exist.
     """
-    api = clients.get_pykube_api()
-
     data = pykube.Secret.objects(api, namespace="magnum-system").get_by_name(
         get_or_generate_cluster_api_cloud_config_secret_name(api, cluster)
     )
     clouds_yaml = base64.decode_as_text(data.obj["data"]["clouds.yaml"])
     cloud_config = yaml.safe_load(clouds_yaml)
 
     return textwrap.dedent(
```

### Comparing `magnum_cluster_api-0.5.3/pyproject.toml` & `magnum_cluster_api-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.5.3"
+version = "0.5.4"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `magnum_cluster_api-0.5.3/PKG-INFO` & `magnum_cluster_api-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.5.3
+Version: 0.5.4
 Summary: Cluster API driver for Magnum
 Author: Mohammed Naser
 Author-email: mnaser@vexxhost.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


# Comparing `tmp/talos_install-0.2.0.dev352.tar.gz` & `tmp/talos_install-0.2.0.dev356.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.0.dev352.tar", last modified: Sun Apr 23 12:53:18 2023, max compression
+gzip compressed data, was "talos_install-0.2.0.dev356.tar", last modified: Mon Apr 24 12:46:37 2023, max compression
```

## Comparing `talos_install-0.2.0.dev352.tar` & `talos_install-0.2.0.dev356.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.468119 talos_install-0.2.0.dev352/
--rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/AUTHORS
--rw-rw-r--   0 installer  (3002) installer  (3002)    11660 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/ChangeLog
--rw-rw-r--   0 installer  (3002) installer  (3002)     3409 2023-04-23 12:53:18.468119 talos_install-0.2.0.dev352/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     2749 2023-04-23 11:45:20.000000 talos_install-0.2.0.dev352/README.md
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.436118 talos_install-0.2.0.dev352/ansible/
--rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-04-23 10:12:10.000000 talos_install-0.2.0.dev352/ansible/ansible.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.436118 talos_install-0.2.0.dev352/ansible/group_vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      702 2023-04-23 12:41:16.000000 talos_install-0.2.0.dev352/ansible/group_vars/all.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.432119 talos_install-0.2.0.dev352/ansible/roles/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.421119 talos_install-0.2.0.dev352/ansible/roles/cli/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.436118 talos_install-0.2.0.dev352/ansible/roles/cli/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-21 16:33:02.000000 talos_install-0.2.0.dev352/ansible/roles/cli/files/FOUNDMEDEVKEY
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.436118 talos_install-0.2.0.dev352/ansible/roles/cli/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/cli/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.438119 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1227 2023-04-21 16:39:14.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/clone.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-19 08:23:48.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/env.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-23 09:25:19.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/logrotate.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-04-21 14:29:02.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-19 14:54:32.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-04-23 08:19:34.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/web.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.440118 talos_install-0.2.0.dev352/ansible/roles/cli/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/agent.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      484 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/app.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/cli.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/env_talos.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-19 14:05:02.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/globals.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/my-httpd.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/passwords.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/talos-logrotate.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-16 16:14:02.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/talos.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/talospass.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.421119 talos_install-0.2.0.dev352/ansible/roles/common/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.440118 talos_install-0.2.0.dev352/ansible/roles/common/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/common/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.441119 talos_install-0.2.0.dev352/ansible/roles/common/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-20 16:08:13.000000 talos_install-0.2.0.dev352/ansible/roles/common/tasks/install_extra_pkgs.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-17 08:59:47.000000 talos_install-0.2.0.dev352/ansible/roles/common/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev352/ansible/roles/common/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.422119 talos_install-0.2.0.dev352/ansible/roles/gather_facts/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.441119 talos_install-0.2.0.dev352/ansible/roles/gather_facts/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-23 10:12:13.000000 talos_install-0.2.0.dev352/ansible/roles/gather_facts/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.442119 talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      930 2023-04-23 08:16:31.000000 talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/RedHat.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      929 2023-04-23 08:19:34.000000 talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/Rocky.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.422119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.422119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.442119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/files/inventory_plugins/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.442119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev352/ansible/roles/install_ansible/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.442119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-04-23 12:42:57.000000 talos_install-0.2.0.dev352/ansible/roles/install_ansible/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.443118 talos_install-0.2.0.dev352/ansible/roles/install_ansible/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-04-23 08:08:27.000000 talos_install-0.2.0.dev352/ansible/roles/install_ansible/templates/ansible.cfg.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.423118 talos_install-0.2.0.dev352/ansible/roles/install_certificates/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.443118 talos_install-0.2.0.dev352/ansible/roles/install_certificates/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/install_certificates/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.443118 talos_install-0.2.0.dev352/ansible/roles/install_certificates/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-19 14:04:55.000000 talos_install-0.2.0.dev352/ansible/roles/install_certificates/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.423118 talos_install-0.2.0.dev352/ansible/roles/install_docker/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.443118 talos_install-0.2.0.dev352/ansible/roles/install_docker/handlers/
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-23 10:25:12.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/handlers/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.444119 talos_install-0.2.0.dev352/ansible/roles/install_docker/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.444119 talos_install-0.2.0.dev352/ansible/roles/install_docker/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-04-23 10:25:12.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.444119 talos_install-0.2.0.dev352/ansible/roles/install_docker/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/templates/daemon.json.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/templates/docker-ce.repo.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.424119 talos_install-0.2.0.dev352/ansible/roles/install_python/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.444119 talos_install-0.2.0.dev352/ansible/roles/install_python/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-04-22 13:21:05.000000 talos_install-0.2.0.dev352/ansible/roles/install_python/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.445119 talos_install-0.2.0.dev352/ansible/roles/install_python/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/install_python/vars/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.428119 talos_install-0.2.0.dev352/ansible/roles/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.445119 talos_install-0.2.0.dev352/ansible/roles/nagios/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-19 14:27:39.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.425119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.425119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.445119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.445119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/conf.d/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.446118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/monitor/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/monitor/.ID
--rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-17 14:32:36.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/resource.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.428119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.446118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.425119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/apache2/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.446118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.426118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.446118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/apache/
--rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/apache/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.447119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/nagios/
--rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.447119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/postfix/
--rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.447119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
--rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.427118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.427118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.447119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.448119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.448119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
--rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
--rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.449118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.449118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
--rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
--rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.427118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.450118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.428119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.428119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/local/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.450118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/local/bin/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.452118 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-20 16:16:42.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.453118 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/cgi.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/contacts.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/localhost.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/nagios.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.431119 talos_install-0.2.0.dev352/ansible/roles/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.453118 talos_install-0.2.0.dev352/ansible/roles/opendcim/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.455119 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/apache2.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/apache2.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-20 12:27:23.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/default.sql
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.429118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.429118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.455119 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/drawings/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.455119 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/pictures/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/mysqld.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.430118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.430118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.430118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.455119 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.456118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
--rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
--rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.456118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-20 13:50:07.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/pre-conf.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-20 15:35:00.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/startup.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.456118 talos_install-0.2.0.dev352/ansible/roles/opendcim/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.457119 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.458119 talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-20 13:12:20.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-20 09:06:15.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/first-run.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/opendcim.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.431119 talos_install-0.2.0.dev352/ansible/roles/os_tune/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.458119 talos_install-0.2.0.dev352/ansible/roles/os_tune/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/ansible/roles/os_tune/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.432119 talos_install-0.2.0.dev352/ansible/roles/talos_users/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/talos_users/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/talos_users/files/talos
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/talos_users/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/talos_users/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/talos_users/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-04-22 13:28:03.000000 talos_install-0.2.0.dev352/ansible/roles/talos_users/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.432119 talos_install-0.2.0.dev352/ansible/roles/uninstall/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/uninstall/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/uninstall/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-22 11:25:57.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.460119 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      660 2023-04-23 08:20:18.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/cli.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-04-22 13:37:20.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/docker.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-04-22 11:29:44.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      345 2023-04-22 12:20:03.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/user.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.461119 talos_install-0.2.0.dev352/ansible/roles/wiki/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.461119 talos_install-0.2.0.dev352/ansible/roles/wiki/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-17 07:46:15.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.461119 talos_install-0.2.0.dev352/ansible/roles/wiki/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/meta/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/requirements.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.465119 talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-17 09:16:59.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/compose.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-17 07:47:31.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-17 07:36:52.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.466118 talos_install-0.2.0.dev352/ansible/roles/wiki/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/templates/docker-compose.yml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/templates/wiki.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/templates/wikidump.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1727 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/ansible/site.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.466118 talos_install-0.2.0.dev352/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      293 2023-04-23 11:14:48.000000 talos_install-0.2.0.dev352/etc/globals.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev352/etc/inventory
--rw-rw-r--   0 installer  (3002) installer  (3002)     1066 2023-04-23 11:16:27.000000 talos_install-0.2.0.dev352/etc/talos.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-04-23 12:53:18.485118 talos_install-0.2.0.dev352/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-21 16:00:17.000000 talos_install-0.2.0.dev352/setup.py
--rwxrwxr-x   0 installer  (3002) installer  (3002)     9008 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/talos_install
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.468119 talos_install-0.2.0.dev352/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3409 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     5583 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev352/talos_install.egg-info/not-zip-safe
--rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/pbr.json
--rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.424332 talos_install-0.2.0.dev356/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11708 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3400 2023-04-24 12:46:37.424332 talos_install-0.2.0.dev356/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2740 2023-04-24 12:02:57.000000 talos_install-0.2.0.dev356/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.395332 talos_install-0.2.0.dev356/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.395332 talos_install-0.2.0.dev356/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      702 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.392332 talos_install-0.2.0.dev356/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.381332 talos_install-0.2.0.dev356/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.395332 talos_install-0.2.0.dev356/ansible/roles/cli/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/files/FOUNDMEDEVKEY
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.396332 talos_install-0.2.0.dev356/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.397332 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1227 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.399332 talos_install-0.2.0.dev356/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      484 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.381332 talos_install-0.2.0.dev356/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.400332 talos_install-0.2.0.dev356/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.400332 talos_install-0.2.0.dev356/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.382332 talos_install-0.2.0.dev356/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.401332 talos_install-0.2.0.dev356/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.401332 talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      930 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      929 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.382332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.382332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.401332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.402332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.402332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.402332 talos_install-0.2.0.dev356/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.383332 talos_install-0.2.0.dev356/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.402332 talos_install-0.2.0.dev356/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.403332 talos_install-0.2.0.dev356/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.383332 talos_install-0.2.0.dev356/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.403332 talos_install-0.2.0.dev356/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.403332 talos_install-0.2.0.dev356/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.403332 talos_install-0.2.0.dev356/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.404332 talos_install-0.2.0.dev356/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.384332 talos_install-0.2.0.dev356/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.404332 talos_install-0.2.0.dev356/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.404332 talos_install-0.2.0.dev356/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.404332 talos_install-0.2.0.dev356/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.385332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.384332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.385332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.405332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.386332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.406332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.406332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.406332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.406332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.387332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.387332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.407332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.407332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.408332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.408332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.409332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.409332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.388332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.409332 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.410332 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.411332 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.391332 talos_install-0.2.0.dev356/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.412332 talos_install-0.2.0.dev356/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.413332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.389332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.389332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.413332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.413332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.390332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.390332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.390332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.414332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.414332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.415332 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.415332 talos_install-0.2.0.dev356/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.416332 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.391332 talos_install-0.2.0.dev356/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-04-24 11:46:13.000000 talos_install-0.2.0.dev356/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.391332 talos_install-0.2.0.dev356/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.417332 talos_install-0.2.0.dev356/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.392332 talos_install-0.2.0.dev356/ansible/roles/uninstall/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.418332 talos_install-0.2.0.dev356/ansible/roles/uninstall/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.418332 talos_install-0.2.0.dev356/ansible/roles/uninstall/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.419332 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      660 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/cli.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/docker.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      345 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/user.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.419332 talos_install-0.2.0.dev356/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.419332 talos_install-0.2.0.dev356/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.420332 talos_install-0.2.0.dev356/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.420332 talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.421332 talos_install-0.2.0.dev356/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1810 2023-04-24 12:01:39.000000 talos_install-0.2.0.dev356/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.422332 talos_install-0.2.0.dev356/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      293 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/etc/globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev356/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1066 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/etc/talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-04-24 12:46:37.425332 talos_install-0.2.0.dev356/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-24 10:47:06.000000 talos_install-0.2.0.dev356/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)    10147 2023-04-24 12:24:19.000000 talos_install-0.2.0.dev356/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-24 12:46:37.423332 talos_install-0.2.0.dev356/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3400 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5583 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev356/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-24 12:46:37.000000 talos_install-0.2.0.dev356/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.0.dev352/ChangeLog` & `talos_install-0.2.0.dev356/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -42,20 +42,22 @@
 * fix ansible-lint config files
 * fix action install
 * remove action install
 * remove action install
 * Update codereview.yaml
 * remove action install
 * remove action install
+* Update codereview.yaml
 * remove action install
 * remove action install
 * add action install
 * Update install\_talos.yaml
 * Update install\_talos.yaml
 * add action install
+* try add ansible-lint
 * all in one Review
 * test
 * all in one
 * all in one
 * all in one
 * all in one
 * all in one
```

### Comparing `talos_install-0.2.0.dev352/PKG-INFO` & `talos_install-0.2.0.dev356/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos_install
-Version: 0.2.0.dev352
+Version: 0.2.0.dev356
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -48,20 +48,20 @@
 pip install talos-install
 ```
 
 ### Installation
 
 The talos_install package can be runned with these options:
 
-- bootstrap: to prepare system with base requirements
+- precheck: to prepare system with base requirements
 - deploy: to install components
 - build: to recreate docker images and pull on docker Hub (only for authorized developper)
-- uninstall: to remove main settings and confurations.
+- remove: to remove main settings and confurations.
 
-> Note that uninstall doesn't remove installed packages (like docker)
+> Note that remove doesn't remove installed packages (like docker)
 and doesn't return to original settings (like selinux or firewalld).
 
 #### inventory
 
 File `<pip_environment>/share/talos_install/etc/inventory` is dinamically create at code level.
 Changes to this file by user are tatally ignored during execution.
 
@@ -79,18 +79,18 @@
 Is not allow to add or delete master and guest configuration
 
 #### global.yaml
 
 Change configuration of config file `<pip_environment>/share/talos_install/etc/global.yaml`
 to change customer configuration.
 
-### Run Installation bootstrap
+### Run Installation precheck
 
 ```bash
-talos_install bootstrap
+talos_install precheck
 ```
 
 A list of change will be shown for user approval. Use `-y` to confirm automatically.
 
 ### Run Installation deploy
 
 ```bash
```

### Comparing `talos_install-0.2.0.dev352/README.md` & `talos_install-0.2.0.dev356/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 pip install talos-install
 ```
 
 ### Installation
 
 The talos_install package can be runned with these options:
 
-- bootstrap: to prepare system with base requirements
+- precheck: to prepare system with base requirements
 - deploy: to install components
 - build: to recreate docker images and pull on docker Hub (only for authorized developper)
-- uninstall: to remove main settings and confurations.
+- remove: to remove main settings and confurations.
 
-> Note that uninstall doesn't remove installed packages (like docker)
+> Note that remove doesn't remove installed packages (like docker)
 and doesn't return to original settings (like selinux or firewalld).
 
 #### inventory
 
 File `<pip_environment>/share/talos_install/etc/inventory` is dinamically create at code level.
 Changes to this file by user are tatally ignored during execution.
 
@@ -61,18 +61,18 @@
 Is not allow to add or delete master and guest configuration
 
 #### global.yaml
 
 Change configuration of config file `<pip_environment>/share/talos_install/etc/global.yaml`
 to change customer configuration.
 
-### Run Installation bootstrap
+### Run Installation precheck
 
 ```bash
-talos_install bootstrap
+talos_install precheck
 ```
 
 A list of change will be shown for user approval. Use `-y` to confirm automatically.
 
 ### Run Installation deploy
 
 ```bash
```

### Comparing `talos_install-0.2.0.dev352/ansible/group_vars/all.yaml` & `talos_install-0.2.0.dev356/ansible/group_vars/all.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/tasks/clone.yaml` & `talos_install-0.2.0.dev356/ansible/roles/cli/tasks/clone.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/tasks/env.yaml` & `talos_install-0.2.0.dev356/ansible/roles/cli/tasks/env.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/tasks/misc.yaml` & `talos_install-0.2.0.dev356/ansible/roles/cli/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/tasks/web.yaml` & `talos_install-0.2.0.dev356/ansible/roles/cli/tasks/web.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/templates/agent.sh.j2` & `talos_install-0.2.0.dev356/ansible/roles/cli/templates/agent.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/templates/cli.conf.j2` & `talos_install-0.2.0.dev356/ansible/roles/cli/templates/cli.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/templates/env_talos.j2` & `talos_install-0.2.0.dev356/ansible/roles/cli/templates/env_talos.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/templates/globals.yaml.j2` & `talos_install-0.2.0.dev356/ansible/roles/cli/templates/globals.yaml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/templates/my-httpd.conf.j2` & `talos_install-0.2.0.dev356/ansible/roles/cli/templates/my-httpd.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/cli/templates/talos.conf.j2` & `talos_install-0.2.0.dev356/ansible/roles/cli/templates/talos.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/common/tasks/misc.yaml` & `talos_install-0.2.0.dev356/ansible/roles/common/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/RedHat.yaml` & `talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/RedHat.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/Rocky.yaml` & `talos_install-0.2.0.dev356/ansible/roles/gather_facts/vars/Rocky.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py` & `talos_install-0.2.0.dev356/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/install_ansible/tasks/main.yaml` & `talos_install-0.2.0.dev356/ansible/roles/install_ansible/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/install_ansible/templates/ansible.cfg.j2` & `talos_install-0.2.0.dev356/ansible/roles/install_ansible/templates/ansible.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/install_certificates/tasks/main.yaml` & `talos_install-0.2.0.dev356/ansible/roles/install_certificates/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/install_docker/tasks/main.yaml` & `talos_install-0.2.0.dev356/ansible/roles/install_docker/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/install_docker/templates/docker-ce.repo.j2` & `talos_install-0.2.0.dev356/ansible/roles/install_docker/templates/docker-ce.repo.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/install_python/tasks/main.yaml` & `talos_install-0.2.0.dev356/ansible/roles/install_python/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/nagios/run` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/nagios/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/postfix/run` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/etc/sv/postfix/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios` & `talos_install-0.2.0.dev356/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/build.yaml` & `talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/misc.yaml` & `talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/run.yaml` & `talos_install-0.2.0.dev356/ansible/roles/nagios/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/templates/Dockerfile.j2` & `talos_install-0.2.0.dev356/ansible/roles/nagios/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/templates/cgi.cfg.j2` & `talos_install-0.2.0.dev356/ansible/roles/nagios/templates/cgi.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/templates/contacts.cfg.j2` & `talos_install-0.2.0.dev356/ansible/roles/nagios/templates/contacts.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/nagios/templates/localhost.cfg.j2` & `talos_install-0.2.0.dev356/ansible/roles/nagios/templates/localhost.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/apache2.conf` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/apache2.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/default.sql` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/default.sql`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/pre-conf.sh` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/pre-conf.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/startup.sh` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/files/startup.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/build.yaml` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/misc.yaml` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/run.yaml` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/Dockerfile.j2` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/first-run.sh.j2` & `talos_install-0.2.0.dev356/ansible/roles/opendcim/templates/first-run.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/os_tune/tasks/main.yaml` & `talos_install-0.2.0.dev356/ansible/roles/os_tune/tasks/main.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,14 @@
     os_tune_stop_firewalld is failed and
     "Could not find the requested service" not in os_tune_stop_firewalld.msg|default('')
 
 - name: Set timezone
   community.general.timezone:
     name: "{{ customer.timezone }}"
 
-- name: Disabling SELinux
-  ansible.posix.selinux:
-    state: disabled
-  register: os_tune_disable_selinux
-
-- name: System will be rebooted for Selinux Changes
-  ansible.builtin.pause:
-    prompt: "!!! System will reboot in 10 seconds. !!!"
-    seconds: 10
-  when: os_tune_disable_selinux is changed
-
-- name: Wait for 5 Second and Reboot
-  ansible.builtin.reboot:
-  when: os_tune_disable_selinux is changed
-
 - name: Change StrictHostKeyChecking
   ansible.builtin.lineinfile:
     dest: /etc/ssh/ssh_config
     state: present
     regexp: 'StrictHostKeyChecking'
     line: 'StrictHostKeyChecking no'
 
@@ -50,7 +35,22 @@
 
 - name: Restart sshd
   ansible.builtin.service:
     name: sshd
     enabled: true
     state: restarted
   when: ssh_strict is changed
+
+- name: Disabling SELinux
+  ansible.posix.selinux:
+    state: disabled
+  register: os_tune_disable_selinux
+
+- name: System will be rebooted for Selinux Changes
+  ansible.builtin.pause:
+    prompt: "!!! System will reboot in 10 seconds. !!!"
+    seconds: 10
+  when: os_tune_disable_selinux is changed
+
+- name: Wait for 5 Second and Reboot
+  ansible.builtin.reboot:
+  when: os_tune_disable_selinux is changed
```

### Comparing `talos_install-0.2.0.dev352/ansible/roles/talos_users/tasks/main.yaml` & `talos_install-0.2.0.dev356/ansible/roles/talos_users/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/cli.yaml` & `talos_install-0.2.0.dev356/ansible/roles/uninstall/tasks/cli.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/wiki/defaults/main.yaml` & `talos_install-0.2.0.dev356/ansible/roles/wiki/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/compose.yaml` & `talos_install-0.2.0.dev356/ansible/roles/wiki/tasks/compose.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/roles/wiki/templates/docker-compose.yml.j2` & `talos_install-0.2.0.dev356/ansible/roles/wiki/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/ansible/site.yaml` & `talos_install-0.2.0.dev356/ansible/site.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,15 @@
 ---
 - hosts: all
-  name: "Bootstrap"
+  name: "Prechecks"
   roles:
-    - role: talos_users
+    - role: os_tune
       become: true
-      tags: talos_users
-      when: cli_action in ['bootstrap']
-
-    - role: install_docker
-      become: true
-      tags: docker
-      when: cli_action in ['bootstrap']
-
-    - role: install_ansible
-      become: true
-      tags: ansible
-      when: cli_action in ['bootstrap']
-
-    - role: install_certificates
-      become: true
-      tags: certificates
-      when: cli_action in ['bootstrap']
+      tags: os_tune
+      when: cli_action in ['precheck']
 
 - hosts: all
   name: "Build container"
   roles:
     - role: install_docker
       become: true
       tags: docker
@@ -49,14 +34,34 @@
       become: true
       tags: opendcim
       when: cli_action in ['build']
 
 - hosts: all
   name: "Deploy"
   roles:
+    - role: talos_users
+      become: true
+      tags: talos_users
+      when: cli_action in ['deploy']
+
+    - role: install_docker
+      become: true
+      tags: docker
+      when: cli_action in ['deploy']
+
+    - role: install_ansible
+      become: true
+      tags: ansible
+      when: cli_action in ['deploy']
+
+    - role: install_certificates
+      become: true
+      tags: certificates
+      when: cli_action in ['deploy']
+  
     - role: common
       become: true
       tags: common
       when: cli_action in ['deploy']
 
     - role: cli
       become: true
@@ -75,13 +80,13 @@
 
     - role: wiki
       become: true
       tags: wiki
       when: cli_action in ['deploy']
 
 - hosts: all
-  name: "Uninstall"
+  name: "Remove"
   roles:
     - role: uninstall
       become: true
       tags: uninstall
-      when: cli_action in ['uninstall']
+      when: cli_action in ['remove']
```

### Comparing `talos_install-0.2.0.dev352/etc/talos.yaml` & `talos_install-0.2.0.dev356/etc/talos.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/setup.cfg` & `talos_install-0.2.0.dev356/setup.cfg`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev352/talos_install` & `talos_install-0.2.0.dev356/talos_install`

 * *Files 18% similar despite different names*

```diff
@@ -31,21 +31,22 @@
 }
 
 check_for_target(){
   echo $hostdef > $inventory
   if [[ -z $target ]]; then target=$(hostname); fi
   target_ip=$(ping $target -4 -c 1 | grep PING | awk '{print $3}' | tr -dc '[:alnum:][.]\n')
   echo "$target   ssh_ip=$target_ip"  >> $inventory
+
   # Try to prevent ssh_pass error copying pub key in authorized_keys file
-  if [[ $(grep -c "$(cat ~/.ssh/id_rsa.pub| awk '{print $2}')" ~/.ssh/authorized_keys) -eq 0 ]]; then
+  if [[ ! -f ~/.ssh/id_rsa ]];  then ssh-keygen -q -t rsa -N ""  ; fi
+  if [[ $(grep -c "$(awk '{print $2}' ~/.ssh/id_rsa.pub)" ~/.ssh/authorized_keys) -eq 0 ]]; then
     cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
   fi
 }
 
-
 check_environment_coherence(){
   if [[ $(rpm -qa | grep -c epel-release) -ne 1 ]]; then
     sudo dnf install epel-release -y &>/dev/null
   fi
   if ! which python3.9 &>/dev/null ; then
     echo "Missing Python 3.9"
     exit 2
@@ -66,38 +67,40 @@
   title_message="$1"
   clear
   # Get Terminal info
   echo "TALOS-CLI | HPC Manager Platform "
   printf "# $title_message\n\n"
 }
 
-confirm_bootstrap(){
-  talos_install_menu "Talos Bootstrap"
+confirm_precheck(){
+  talos_install_menu "Talos Precheck"
   current_selinux=$(grep ^SELINUX= /etc/selinux/config | cut -d= -f2)
 
   echo "These actions will be performed:
-  - Add an user {{ master.user }} with sudo permission.
-  - Install python dependencies
   - Stop firewall service (if present)
   - Set Timezone {{ customer.timezone }}"
   if [[ "$current_selinux" != "disabled" ]]; then
-    echo "- Disable Selinux
-    !!! A REBOOT WILL OCCOUR DURING INSTALLATION !!!"
+    echo "  - Disable Selinux
+    ------------------------------------------------
+    !!! A REBOOT WILL OCCOUR DURING INSTALLATION !!!
+    ------------------------------------------------"
+    force_install=false
   fi
-  echo "  - Install docker and give to {{ master.user }} permission to run containers
-  - Install ansible dependencies
-  - Install CA certificates (if required by {{ ca_idm.enable }})
-  "
   confirm_action
 }
 
 confirm_deploy(){
   talos_install_menu "Talos deploy"
 
   echo "These actions will be performed:
+  - Add an user {{ master.user }} with sudo permission.
+  - Install python dependencies
+  - Install docker and give to {{ master.user }} permission to run containers
+  - Install ansible dependencies
+  - Install CA certificates (if required by {{ ca_idm.enable }})
   - Create Talos environment paths
   - Install Talos-cli dependencies
   - Install Talos-cli source code
   - Install and configure logrotate
   - Install and start Web services
   - Pull Nagios docker
   - Pull OpenDcim docker
@@ -147,20 +150,37 @@
       n|N)
         exit 3 ;;
     esac
   done
 }
 
 process_cmd(){
-    echo "$action : $cmd"
-    $cmd
-    if [[ $? -ne 0 ]]; then
-        echo "Command failed $cmd"
-        exit 1
-    fi
+  echo "$action : $cmd"
+  $cmd
+  if [[ $? -ne 0 ]]; then
+    echo "Command failed $cmd"
+    exit 1
+  elif [[ $f_action == "precheck" ]]; then
+    echo 0 > /tmp/precheck
+  elif [[ $f_action == "remove" ]]; then
+    echo 1 > /tmp/precheck
+  fi
+}
+
+init_step(){
+  if [[ ! -f /tmp/precheck ]]; then
+    echo 1 > /tmp/precheck
+  fi
+}
+
+verify_step(){
+  if [[ $(cat /tmp/precheck) -eq 1 ]]; then
+    echo "ERROR: run talos_install precheck first"
+    exit 2
+  fi
 }
 
 usage(){
     cat <<EOF
 Usage: $0 COMMAND [options]
 
 Options:
@@ -176,43 +196,62 @@
     --vault-password-file <path>       Specify password file for vault decrypt
     --verbose, -v                      Increase verbosity of ansible-playbook
 
 Environment variables:
     extra_opts                         Additional arguments to pass to ansible-playbook
 
 Commands:
-    bootstrap            Bootstrap servers with talos deploy dependencies
+    precheck             Prepare OS for installation
     deploy               Deploy and start main talos containers
     build                Build talos custom containers
-    uninstall            Uninstall Talos-cli
+    remove               Uninstall Talos-cli
 EOF
 }
 
 ### MAIN HERE
 
 # Check Environment
 check_no_root_sudo
 check_environment_coherence
+init_step
 
-# Verifiy if system is able to find shared palybooks
-if [[ -n $TPATH ]]; then
+# Verifiy if system is able to find shared playbooks
+found=false
+# Trying to use User TPATH variable if passed
+if ! $found && [[ -n $TPATH ]]; then
   basedir="${TPATH}/share/talos_install"
-else
+  if [[ -d "$basedir" ]]; then found=true ; fi
+fi
+# Trying to user python --user-base
+if ! $found ; then
+  env_bin=$(python3.9 -m site --user-base)
+  basedir=${env_bin}/share/talos_install
+  if [[ -d "$basedir" ]]; then found=true ; fi
+fi
+# Trying to user sys.executable
+if ! $found ; then
   env_bin=$(pip debug 2>/dev/null | grep sys.executable | awk '{print $2}')
   env_bin="$(dirname $env_bin)"
   env_bin="$(dirname $env_bin)"
   basedir=${env_bin}/share/talos_install
+  if [[ -d "$basedir" ]]; then found=true ; fi
 fi
-if [[ ! -d "$basedir" ]]; then
-  echo "Unable to find $basedir. Please try to pass right path as TPATH=/path/to/..."
+
+if ! $found ; then
+  echo "Unable to find a valid path/to/share/talos_install . Please try to pass right path as TPATH=/path/to/..."
   exit 127
 fi
 
 # Verifify if user have dev_key for GIT
 if [[ -f ~/.ssh/dev_key ]]; then
+  # WA Fix keys
+  sudo chmod 700 ~/.ssh/
+  sudo chmod 600 ~/.ssh/dev_key
+  sudo chmod 644 ~/.ssh/dev_key
+  sudo chmod g-w ~/.ssh/*
   \cp ~/.ssh/dev_key* ${basedir}/ansible/roles/cli/files/
 else
   echo "Missing dev_key in ~/.ssh folder"
   exit 127
 fi
 
 # Start check options
@@ -265,37 +304,42 @@
       force_install=true ; shift ;;
     (*)
       echo "Syntax error" ; usage ; exit 1 ;;
 esac
 done
 
 case "$1" in
-  (bootstrap)
-    confirm_bootstrap
-    action="Bootstrapping servers"
+  (precheck)
+    confirm_precheck
+    f_action=precheck
+    action="Precheck server"
     playbook="${basedir}/ansible/site.yaml"
-    extra_opts="$extra_opts -e cli_action=bootstrap"
+    extra_opts="$extra_opts -e cli_action=precheck"
     hostdef="[talos]" ;;
   (build)
     confirm_build
+    f_action=build
     action="Build Talos containers"
     playbook="${basedir}/ansible/site.yaml"
     extra_opts="$extra_opts -e cli_action=build"
     hostdef="[builder]" ;;
   (deploy)
+    verify_step
     confirm_deploy
+    f_action=deploy
     action="Deploying Playbooks"
     playbook="${basedir}/ansible/site.yaml"
     extra_opts="$extra_opts -e cli_action=deploy"
     hostdef="[talos]" ;;
-  (uninstall)
+  (remove)
     confirm_destroy
+    f_action=deploy
     action="Uninstall talos"
     playbook="${basedir}/ansible/site.yaml"
-    extra_opts="$extra_opts -e cli_action=uninstall"
+    extra_opts="$extra_opts -e cli_action=remove"
     hostdef="[talos]" ;;
   (*)
     usage
     exit 0 ;;
 esac
 
 check_for_target
```

### Comparing `talos_install-0.2.0.dev352/talos_install.egg-info/PKG-INFO` & `talos_install-0.2.0.dev356/talos_install.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos-install
-Version: 0.2.0.dev352
+Version: 0.2.0.dev356
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -48,20 +48,20 @@
 pip install talos-install
 ```
 
 ### Installation
 
 The talos_install package can be runned with these options:
 
-- bootstrap: to prepare system with base requirements
+- precheck: to prepare system with base requirements
 - deploy: to install components
 - build: to recreate docker images and pull on docker Hub (only for authorized developper)
-- uninstall: to remove main settings and confurations.
+- remove: to remove main settings and confurations.
 
-> Note that uninstall doesn't remove installed packages (like docker)
+> Note that remove doesn't remove installed packages (like docker)
 and doesn't return to original settings (like selinux or firewalld).
 
 #### inventory
 
 File `<pip_environment>/share/talos_install/etc/inventory` is dinamically create at code level.
 Changes to this file by user are tatally ignored during execution.
 
@@ -79,18 +79,18 @@
 Is not allow to add or delete master and guest configuration
 
 #### global.yaml
 
 Change configuration of config file `<pip_environment>/share/talos_install/etc/global.yaml`
 to change customer configuration.
 
-### Run Installation bootstrap
+### Run Installation precheck
 
 ```bash
-talos_install bootstrap
+talos_install precheck
 ```
 
 A list of change will be shown for user approval. Use `-y` to confirm automatically.
 
 ### Run Installation deploy
 
 ```bash
```

### Comparing `talos_install-0.2.0.dev352/talos_install.egg-info/SOURCES.txt` & `talos_install-0.2.0.dev356/talos_install.egg-info/SOURCES.txt`

 * *Files identical despite different names*


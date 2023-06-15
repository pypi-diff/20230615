# Comparing `tmp/talos_install-0.2.0.tar.gz` & `tmp/talos_install-0.2.0.dev367.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.0.tar", last modified: Thu Jun 15 16:39:43 2023, max compression
+gzip compressed data, was "talos_install-0.2.0.dev367.tar", last modified: Thu Jun 15 16:56:46 2023, max compression
```

## Comparing `talos_install-0.2.0.tar` & `talos_install-0.2.0.dev367.tar`

### file list

```diff
@@ -1,11 +1,225 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:39:43.021833 talos_install-0.2.0/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3370 2023-06-15 16:39:43.021833 talos_install-0.2.0/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     2740 2023-06-15 07:22:43.000000 talos_install-0.2.0/README.md
--rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-06-15 16:39:43.023833 talos_install-0.2.0/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      323 2023-06-15 16:39:34.000000 talos_install-0.2.0/setup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:39:43.021833 talos_install-0.2.0/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3370 2023-06-15 16:39:42.000000 talos_install-0.2.0/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)      212 2023-06-15 16:39:43.000000 talos_install-0.2.0/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:39:42.000000 talos_install-0.2.0/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-06-15 16:39:42.000000 talos_install-0.2.0/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:39:42.000000 talos_install-0.2.0/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.993787 talos_install-0.2.0.dev367/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    12013 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3378 2023-06-15 16:56:45.993787 talos_install-0.2.0.dev367/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2740 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.965787 talos_install-0.2.0.dev367/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.965787 talos_install-0.2.0.dev367/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      702 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.962787 talos_install-0.2.0.dev367/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.951787 talos_install-0.2.0.dev367/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.965787 talos_install-0.2.0.dev367/ansible/roles/cli/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/files/FOUNDMEDEVKEY
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.965787 talos_install-0.2.0.dev367/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.967787 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1197 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1497 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2718 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.969787 talos_install-0.2.0.dev367/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3814 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      484 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      379 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.951787 talos_install-0.2.0.dev367/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.969787 talos_install-0.2.0.dev367/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.970787 talos_install-0.2.0.dev367/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.951787 talos_install-0.2.0.dev367/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.970787 talos_install-0.2.0.dev367/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.971787 talos_install-0.2.0.dev367/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      930 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      929 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.952787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.952787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.971787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.971787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.971787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.953787 talos_install-0.2.0.dev367/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.953787 talos_install-0.2.0.dev367/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.973787 talos_install-0.2.0.dev367/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.973787 talos_install-0.2.0.dev367/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.954787 talos_install-0.2.0.dev367/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.973787 talos_install-0.2.0.dev367/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.958787 talos_install-0.2.0.dev367/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.955787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.954787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.957787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.975787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.955787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.975787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.956787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.975787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.975787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.976787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.976787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.957787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.957787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.976787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.977787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.977787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1585 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.978787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.978787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.957787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.978787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.958787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.958787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.979787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.979787 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.981787 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2765 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.960787 talos_install-0.2.0.dev367/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.981787 talos_install-0.2.0.dev367/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.982787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.959787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.959787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.983787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.983787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.959787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.959787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.960787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.983787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.984787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53198 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20094 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.984787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.984787 talos_install-0.2.0.dev367/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.985787 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.986787 talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.961787 talos_install-0.2.0.dev367/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.986787 talos_install-0.2.0.dev367/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.961787 talos_install-0.2.0.dev367/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.986787 talos_install-0.2.0.dev367/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.987787 talos_install-0.2.0.dev367/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.987787 talos_install-0.2.0.dev367/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      634 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.962787 talos_install-0.2.0.dev367/ansible/roles/uninstall/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.987787 talos_install-0.2.0.dev367/ansible/roles/uninstall/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.987787 talos_install-0.2.0.dev367/ansible/roles/uninstall/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.988787 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      682 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/cli.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/docker.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      339 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/user.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.988787 talos_install-0.2.0.dev367/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.989787 talos_install-0.2.0.dev367/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      572 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.989787 talos_install-0.2.0.dev367/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.990787 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      161 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/init.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      325 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.990787 talos_install-0.2.0.dev367/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1275 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1835 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.991787 talos_install-0.2.0.dev367/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      293 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/etc/globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev367/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1090 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/etc/talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-06-15 16:56:45.998787 talos_install-0.2.0.dev367/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-06-15 16:56:29.000000 talos_install-0.2.0.dev367/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)    10147 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.993787 talos_install-0.2.0.dev367/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3378 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5618 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.0/PKG-INFO` & `talos_install-0.2.0.dev367/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos_install
-Version: 0.2.0
+Version: 0.2.0.dev367
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -134,7 +134,8 @@
 ```
 
 Check Overall status
 
 ```bash
 talos-config check
 ```
+
```

### Comparing `talos_install-0.2.0/README.md` & `talos_install-0.2.0.dev367/README.md`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0/setup.cfg` & `talos_install-0.2.0.dev367/setup.cfg`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0/talos_install.egg-info/PKG-INFO` & `talos_install-0.2.0.dev367/talos_install.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos-install
-Version: 0.2.0
+Version: 0.2.0.dev367
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -134,7 +134,8 @@
 ```
 
 Check Overall status
 
 ```bash
 talos-config check
 ```
+
```


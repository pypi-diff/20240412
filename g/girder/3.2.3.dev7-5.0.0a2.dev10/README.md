# Comparing `tmp/girder-3.2.3.dev7.tar.gz` & `tmp/girder-5.0.0a2.dev10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-3.2.3.dev7.tar", last modified: Wed Feb 14 18:46:58 2024, max compression
+gzip compressed data, was "girder-5.0.0a2.dev10.tar", last modified: Fri Apr 12 16:12:21 2024, max compression
```

## Comparing `girder-3.2.3.dev7.tar` & `girder-5.0.0a2.dev10.tar`

### file list

```diff
@@ -1,975 +1,487 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.205259 girder-3.2.3.dev7/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/Dockerfile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14387 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/config.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      710 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/create_ansible_subtree.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      316 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/generatePyEnvChecksum.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1118 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/publish_npm.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      360 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.circleci/publish_pypi.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.codecov.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.dockerignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      450 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.editorconfig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      258 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/.readthedocs.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20024 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/CMakeLists.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4925 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/Dockerfile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2721 2024-02-14 18:46:58.205259 girder-3.2.3.dev7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1427 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/Vagrantfile
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.081259 girder-3.2.3.dev7/clients/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/clients/python/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/clients/python/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/clients/python/girder_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    68223 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/clients/python/girder_client/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13535 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/clients/python/girder_client/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/clients/python/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.081259 girder-3.2.3.dev7/devops/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/.yamllint
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/defaults/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/defaults/main.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/handlers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/handlers/main.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/library/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/library/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4135 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/library/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    60712 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/library/girder.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.101259 girder-3.2.3.dev7/devops/ansible-role-girder/meta/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/meta/main.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.081259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/converge.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/data/test1.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/data/test2.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/data/test3.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1278 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/molecule.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/prepare.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/requirements.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22622 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_access.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1154 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_apikey.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3879 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_assetstore.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3895 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_files.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9955 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_hierarchy.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7840 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_resources.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1815 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_setting.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2906 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/ansible-module/test_user.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/converge.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/molecule.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      276 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/prepare.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/pytest.ini
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/molecule/default/tests/test_default.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/tasks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2472 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/tasks/main.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/tasks/nodejs.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.081259 girder-3.2.3.dev7/devops/ansible-role-girder/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/ansible-role-girder/templates/daemon/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/ansible-role-girder/templates/daemon/girder.service.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/deployment-template/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/deployment-template/hosts.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/deployment-template/playbook.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      267 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/deployment-template/provision.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/deployment-template/requirements.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.105259 girder-3.2.3.dev7/devops/vagrant/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/vagrant/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/vagrant/ansible.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2139 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/vagrant/vagrant-playbook.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/devops/vagrant/vagrant-requirements.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docker-compose.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.109259 girder-3.2.3.dev7/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/admin-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5288 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/api-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/build-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/changelog.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2379 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6551 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/configuration.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5131 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/dependencies.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/deployment-alternatives.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/deployment.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/dev-installation.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23262 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/developer-cookbook.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/developer-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18444 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/external-web-clients.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15086 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/favicon.ico
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.109259 girder-3.2.3.dev7/docs/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   803025 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/images/dicom-viewer.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5181 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/license.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26440 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/migration-guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/mount.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38303 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/plugin-development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22537 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/plugins.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10888 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/python-client.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       70 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/requirements-docs.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5707 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/security.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1640 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/sftp.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/user-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14123 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/docs/user-guide.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.109259 girder-3.2.3.dev7/girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11228 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.113259 girder-3.2.3.dev7/girder/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4349 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/access.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/api_docs.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/api_main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33164 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/describe.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5196 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/docs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3483 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/filter_logging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    51261 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7259 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/sftp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.113259 girder-3.2.3.dev7/girder/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13355 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/assetstore.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10847 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19091 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21532 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/folder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15915 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4577 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/notification.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17147 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/resource.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20748 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/system.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2065 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19063 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/api/v1/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.117259 girder-3.2.3.dev7/girder/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      358 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4755 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/build.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24990 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/mount.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/serve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/sftpd.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1618 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/cli/shell.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.117259 girder-3.2.3.dev7/girder/conf/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2337 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/conf/girder.dist.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8332 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10926 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.117259 girder-3.2.3.dev7/girder/mail_templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/_footer.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/_header.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      306 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/accountApproval.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/accountApproved.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/emailVerification.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/groupInvite.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/mail_templates/temporaryAccess.mako
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.117259 girder-3.2.3.dev7/girder/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3265 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4825 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6420 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/assetstore.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16104 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20118 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36301 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/folder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15676 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21408 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    65695 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/model_base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8257 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/notification.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/setting.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4697 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22152 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/upload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24488 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6889 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15380 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.121259 girder-3.2.3.dev7/girder/utility/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6447 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1450 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/_cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/_hash_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17371 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/abstract_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16381 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/acl_mixin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2477 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/assetstore_utilities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2545 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/error.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18720 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/filesystem_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11759 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/gridfs_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6345 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/mail_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2752 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/model_importer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6735 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/path.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4435 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/progress.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27265 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/s3_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2440 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6879 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2946 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/setting_utilities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7267 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/system.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/webroot.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/webroot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8124 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/utility/ziputil.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.121259 girder-3.2.3.dev7/girder/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2332 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/Gruntfile.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.121259 girder-3.2.3.dev7/girder/web_client/eslint-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/.npmignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4715 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/eslint-config/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.125259 girder-3.2.3.dev7/girder/web_client/fontello/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/.npmignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/Gruntfile.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1225 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    58174 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/fontello.config.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45252 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      641 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/fontello/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.125259 girder-3.2.3.dev7/girder/web_client/grunt_tasks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11066 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/build.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1717 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/swagger.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2742 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/test.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6587 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/webpack.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/webpack.paths.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/grunt_tasks/webpack.plugins.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/package.json.template
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.125259 girder-3.2.3.dev7/girder/web_client/pug-lint-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/.npmignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1017 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      432 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/pug-lint-config/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/assets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7590 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/assets/Girder_Mark.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4106 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/auth.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/collections/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/ApiKeyCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/AssetstoreCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10660 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/Collection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/CollectionCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/FileCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      275 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/FolderCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/GroupCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/ItemCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/UserCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/collections/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/constants.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4733 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/dialog.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/events.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6698 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/misc.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2841 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/AccessControlledModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/ApiKeyModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/AssetstoreModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/CollectionCreationPolicyModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10910 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/FileModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      886 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/FolderModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6427 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/GroupModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2284 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/ItemModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2964 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/MetadataMixin.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5688 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/Model.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5467 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/models/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/pluginUtils.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7581 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/rest.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/router.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7109 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.085259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.129259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/apidocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      831 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/apidocs/apidocs.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.133259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      310 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/adminConsole.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      792 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/assetstores.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      697 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/collectionList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/collectionPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      939 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/frontPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/groupList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2127 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/groupPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1370 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/itemPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/plugins.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/searchResultsList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/systemConfig.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userAccount.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userPage.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.133259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/footer.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2843 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/global.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/globalNav.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/header.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/headerUser.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1320 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/layout.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/layoutVars.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      622 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/loading.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/progressArea.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.137259 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1788 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/accessWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/browserWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/markdownWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1662 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/metadataWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/taskProgress.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/timelineWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/uploadWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3818 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.085259 girder-3.2.3.dev7/girder/web_client/src/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.137259 girder-3.2.3.dev7/girder/web_client/src/templates/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/adminConsole.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4103 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/assetstores.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1484 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/collectionList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1307 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/collectionPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1887 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/filesystemImport.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3003 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/frontPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/groupList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3962 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/groupPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1836 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/itemPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      949 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/plugins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/s3Import.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/searchResults.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/searchResultsType.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11102 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/systemConfiguration.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3634 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/userAccount.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/userList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/body/userPage.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.137259 girder-3.2.3.dev7/girder/web_client/src/templates/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/alert.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layout.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutFooter.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutGlobalNav.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutHeader.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      796 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutHeaderUser.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutProgressArea.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/loginDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1719 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/registerDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/layout/resetPasswordDialog.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.145259 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditor.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditorMixins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditorNonModal.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEntry.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1918 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/apiKeyList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1126 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/browserWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/checkedActionsMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1273 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/collectionInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      565 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/confirmDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/dateTimeWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editApiKeyWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editCollectionWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editFileWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editFolderWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editGroupWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editItemWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/fileInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1229 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/fileList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/folderInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/folderList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupAdminList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3129 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupInviteDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupInviteList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupMemberList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupModList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyPaginated.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3835 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      461 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/itemBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1088 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/itemList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/jsonMetadatumView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/loadingAnimation.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/markdownWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadataWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadatumEditWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadatumView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5858 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/newAssetstore.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/paginateWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/pluginConfigBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/rootSelectorWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/searchField.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/searchHelp.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/searchModeSelect.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      469 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/searchResults.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/sortCollectionWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/taskProgress.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/timeline.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/uploadWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1013 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/uploadWidgetNonModal.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      115 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/userOtpBegin.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/userOtpDisable.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/templates/widgets/userOtpEnable.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.149259 girder-3.2.3.dev7/girder/web_client/src/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/EventStream.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/PluginUtils.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9489 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/S3UploadHandler.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.149259 girder-3.2.3.dev7/girder/web_client/src/utilities/jquery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/jquery/girderEnable.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2134 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/utilities/jquery/girderModal.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/version.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.149259 girder-3.2.3.dev7/girder/web_client/src/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/App.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2552 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/View.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.149259 girder-3.2.3.dev7/girder/web_client/src/views/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/AdminView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8160 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/AssetstoresView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6740 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/CollectionView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4353 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/CollectionsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3146 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/FilesystemImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/FolderView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1305 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/FrontPageView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11859 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/GroupView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/GroupsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6011 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/PluginsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/S3ImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5544 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/SearchResultsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7137 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/SystemConfigurationView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6266 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/UserAccountView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5437 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/UserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/UsersView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/body/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.153259 girder-3.2.3.dev7/girder/web_client/src/views/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/FooterView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3163 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/GlobalNavView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/HeaderUserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/HeaderView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3708 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/LoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/ProgressListView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3733 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/RegisterView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2344 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/ResetPasswordView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/layout/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/src/views/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15584 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/AccessWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4632 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/ApiKeyListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14503 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/BrowserWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2441 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/CheckedMenuWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5922 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/DateTimeRangeWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3302 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/DateTimeWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditApiKeyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5940 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3239 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditFileWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4203 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditFolderWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4479 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditGroupWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3797 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditItemWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/FileInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5005 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/FileListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/FolderInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3360 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/FolderListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2901 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupAdminsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1838 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupInvitesWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5965 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupMembersWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2518 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupModsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42297 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/HierarchyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14233 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/ItemListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/LoadingAnimation.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7648 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/MarkdownWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17158 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/MetadataWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3190 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/NewAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1063 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/PaginateWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6455 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/RootSelectorWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13112 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/SearchFieldWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4510 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/SearchPaginateWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1619 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/SortCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3042 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/TaskProgressWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6664 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/TimelineWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13690 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/UploadWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3203 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/UserOtpManagementWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2673 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/src/views/widgets/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/static/.gitignore
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/static/built/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/static/built/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/static/girder-swagger.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/static/img/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/static/img/Girder_Favicon.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.157259 girder-3.2.3.dev7/girder/web_client/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/fake.jpg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.085259 girder-3.2.3.dev7/girder/web_client/test/lib/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4131 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/ConsoleReporter.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/MIT.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6537 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/jasmine.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70934 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/lib/jasmine-1.3.1/jasmine.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8361 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/specRunner.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testEnv.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testFile.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testFile.tsv
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testFile.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testFile2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    46373 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/girder/web_client/test/testUtils.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/girder.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2721 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37817 2024-02-14 18:46:58.000000 girder-3.2.3.dev7/girder.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      327 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-02-14 18:46:57.000000 girder-3.2.3.dev7/girder.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   230120 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3293 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      271 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/.gitignore
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/audit_logs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1963 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      838 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/cleanup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2551 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/audit_logs/girder_audit_logs/report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1710 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/audit_logs/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4605 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/mail_templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1712 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizeUpload.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/authorizedUpload.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/templates/folderActions.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3124 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/authorizedUploadSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/plugin_tests/upload_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1766 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/authorized_upload/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.161259 girder-3.2.3.dev7/plugins/autojoin/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3781 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/girder_autojoin/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/autojoin/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3790 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/plugin_tests/autojoinSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/plugin_tests/autojoin_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1692 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/autojoin/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9428 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/event_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2263 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      765 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1286 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomItem.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13597 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/views/DicomView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      686 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/girder_dicom_viewer/web_client/webpack.helper.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/000000.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/000001.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/000002.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/data/000003.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11077 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/plugin_tests/dicom_viewer_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/dicom_viewer/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.165259 girder-3.2.3.dev7/plugins/download_statistics/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/download_statistics/girder_download_statistics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/girder_download_statistics/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6503 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/download_statistics_test.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/files/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/files/txt1.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/plugin_tests/files/txt2.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/download_statistics/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/lib/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/lib/backbone.analytics.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2186 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/girder_google_analytics/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/google_analytics/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      862 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/plugin_tests/google_analytics_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/google_analytics/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1922 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2103 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/girder_gravatar/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/gravatar/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3106 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/plugin_tests/gravatar_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/gravatar/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.169259 girder-3.2.3.dev7/plugins/hashsum_download/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7455 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/templates/config.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2070 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/girder_hashsum_download/web_client/views/FileInfoWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2371 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/hashsumSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13472 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/plugin_tests/hashsum_download_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/hashsum_download/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2408 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      912 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6270 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1267 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/girder_homepage/web_client/views/FrontPageView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/homepage/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6120 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/plugin_tests/homepageSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/plugin_tests/homepage_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1674 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/homepage/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/item_licenses/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.173259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2831 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2499 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1480 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/EditItemWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/HierarchyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/ItemLicenseWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/SelectLicenseWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1576 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/girder_item_licenses/web_client/views/UploadWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/itemLicensesSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12348 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/plugin_tests/item_licenses_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/item_licenses/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/jobs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2053 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9199 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/job_rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23250 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/models/job.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.177259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2922 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/JobStatus.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/collections/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/collections/JobCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/collections/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/models/JobModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/models/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/stylesheets/jobListWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/adminViewMenuItem.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/headerUserViewMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxContent.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2232 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobDetailsWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobListWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/templates/jobsGraphWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/AdminView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2192 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/CheckBoxMenu.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/HeaderUserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4906 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobDetailsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8414 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobGraphWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12083 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/JobListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/timeChartConfig.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/girder_jobs/web_client/views/timingHistoryChartConfig.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/jobs/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21567 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/plugin_tests/jobsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24932 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/plugin_tests/jobs_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/plugin_tests/local_job_impl.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/jobs/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/ldap/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.181259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6318 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2076 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/editServerMixin.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/templates/newServerTemplate.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4955 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/girder_ldap/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/ldap/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9007 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/plugin_tests/ldap_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1615 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/ldap/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9083 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3526 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/bitbucket.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/box.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/github.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/globus.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2980 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/google.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2951 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/linkedin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3018 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/providers/microsoft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5347 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3127 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      458 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/stylesheets/configView.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2668 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/stylesheets/oauthLoginView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.185259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2762 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/templates/oauthLoginView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/LoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2770 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/OAuthLoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/girder_oauth/web_client/views/RegisterView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/oauth/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    65626 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/plugin_tests/oauth_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1733 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/oauth/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      470 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/stylesheets/readmeWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      101 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/templates/readmeWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/girder_readme/web_client/views/HierarchyWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/plugin_tests/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/readme/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/plugin_tests/data/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/plugin_tests/readmeSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/readme/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/girder_sentry/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1639 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/sentry/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/terms/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/terms/girder_terms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.189259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3270 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3087 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/stylesheets/termsAcceptance.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/templates/collectionInfoWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/templates/editCollectionTermsWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/templates/termsAcceptance.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      717 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/EditCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/girder_terms/web_client/views/TermsAcceptanceView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/terms/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14763 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/plugin_tests/termsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6081 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/plugin_tests/terms_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/terms/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3080 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2346 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/models/ThumbnailModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/stylesheets/flowView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.193259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1510 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/flowView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/templates/itemView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3910 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/CreateThumbnailView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1306 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/FileListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2021 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/FlowView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1171 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/girder_thumbnails/worker.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35946 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/data/sample_dicom.dcm
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13000 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/thumbnail_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2213 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/plugin_tests/thumbnailsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/thumbnails/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      874 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16648 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/quota.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3788 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/models/extendModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      429 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      394 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/stylesheets/userQuota.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3480 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2168 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/utilities/Conversions.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.197259 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/CollectionView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      677 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/UploadWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/UserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/girder_user_quota/web_client/views/extendView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/plugins/user_quota/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16489 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/plugin_tests/userQuotaSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21142 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/plugin_tests/user_quota_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1694 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/user_quota/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/plugins/virtual_folders/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/plugins/virtual_folders/girder_virtual_folders/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8194 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/virtual_folders/girder_virtual_folders/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/plugins/virtual_folders/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/virtual_folders/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6178 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/virtual_folders/plugin_tests/virtual_folders_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/plugins/virtual_folders/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/pytest_girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/MANIFEST.in
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/pytest_girder/pytest_girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/assertions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/fixtures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/plugin_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11468 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/pytest_girder/web_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/pytest_girder/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      746 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/requirements-dev.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/scripts/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:58.201259 girder-3.2.3.dev7/scripts/midas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11413 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/migrate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/walk_girder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1357 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/midas/walk_midas.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/publicNames.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36686 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/publicNames.txt
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      604 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/scripts/test_names.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-02-14 18:46:58.205259 girder-3.2.3.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2614 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2024-02-14 18:46:47.000000 girder-3.2.3.dev7/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.518698 girder-5.0.0a2.dev10/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.410698 girder-5.0.0a2.dev10/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1098 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/Dockerfile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/build_plugins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13158 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/config.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      316 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/generatePyEnvChecksum.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      980 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/publish_npm.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      417 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/publish_pypi.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.codecov.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.editorconfig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.readthedocs.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20024 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      729 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/CMakeLists.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4925 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/Dockerfile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      491 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2724 2024-04-12 16:12:21.518698 girder-5.0.0a2.dev10/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.402697 girder-5.0.0a2.dev10/clients/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.410698 girder-5.0.0a2.dev10/clients/python/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/clients/python/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.410698 girder-5.0.0a2.dev10/clients/python/girder_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    68223 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/clients/python/girder_client/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13535 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/clients/python/girder_client/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/clients/python/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      395 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.414698 girder-5.0.0a2.dev10/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/admin-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5217 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/api-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/build-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/changelog.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2379 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2137 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/configuration.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5131 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/dependencies.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2047 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/deployment.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/dev-installation.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22931 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/developer-cookbook.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/developer-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13030 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15086 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.414698 girder-5.0.0a2.dev10/docs/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   803025 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/images/dicom-viewer.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5181 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/license.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36997 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/migration-guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/mount.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38303 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/plugin-development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21669 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/plugins.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10504 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/python-client.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       70 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/requirements-docs.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5707 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/security.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1640 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/sftp.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/user-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/user-guide.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.418697 girder-5.0.0a2.dev10/girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.418697 girder-5.0.0a2.dev10/girder/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4349 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/access.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1341 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/api_docs.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/api_main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32888 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/describe.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5216 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/docs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3483 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/filter_logging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    51167 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7285 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/sftp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.422697 girder-5.0.0a2.dev10/girder/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12222 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/assetstore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10847 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19091 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21532 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/folder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15915 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4577 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17147 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/resource.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18817 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/system.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2065 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19063 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.422697 girder-5.0.0a2.dev10/girder/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      358 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24760 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/mount.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2452 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/serve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1367 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/sftpd.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1750 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/shell.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7162 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5954 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.422697 girder-5.0.0a2.dev10/girder/mail_templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/_footer.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/_header.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      306 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/accountApproval.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/accountApproved.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/emailVerification.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/groupInvite.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/temporaryAccess.mako
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.426698 girder-5.0.0a2.dev10/girder/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4825 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6054 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/assetstore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16104 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20130 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36301 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/folder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15676 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21461 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    65727 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/model_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8257 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/setting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4697 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22202 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/upload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24605 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6465 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14634 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.426698 girder-5.0.0a2.dev10/girder/utility/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6482 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3111 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/_cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/_hash_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17371 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/abstract_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16381 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/acl_mixin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2310 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/assetstore_utilities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/error.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18688 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/filesystem_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6280 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/mail_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2752 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/model_importer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6735 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/path.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4435 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/progress.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26957 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/s3_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2440 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3589 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2946 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/setting_utilities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6845 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/system.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2857 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/webroot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8124 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/ziputil.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.430698 girder-5.0.0a2.dev10/girder/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/.env.development
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      331 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/.prettierrc.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2069 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.430698 girder-5.0.0a2.dev10/girder/web/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-04-12 16:11:18.000000 girder-5.0.0a2.dev10/girder/web/dist/Girder_Favicon.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7590 2024-04-12 16:11:18.000000 girder-5.0.0a2.dev10/girder/web/dist/Girder_Mark.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.442698 girder-5.0.0a2.dev10/girder/web/dist/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   127292 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-00cea317.ttf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    72868 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-13e61b43.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   183888 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-2d6e9725.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    58716 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-98c6b1f2.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   127460 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-e418b5b2.eot
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20127 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-13634da8.eot
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   108738 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-42f60659.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23424 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-a26394f7.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45404 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-e3950440.ttf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18028 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-fe185d11.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   215659 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/index-269c82d1.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1984729 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/index-41ef1ab1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  5812987 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/index-41ef1ab1.js.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35955 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/jsoneditor-icons-25c04e58.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18668 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300-6e8a28a0.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14932 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300-f677ee2d.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13860 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300italic-453e6eb2.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17668 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300italic-5bb07410.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18100 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400-81f0ec27.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14380 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400-9c50a96c.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17440 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400italic-39ec493a.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13780 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400italic-da407a15.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14880 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600-1491de1b.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18696 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600-57c79375.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13852 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600italic-10879c90.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17492 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600italic-bb878389.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15056 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700-74201a4b.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18900 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700-ea20e5db.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17452 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700italic-1e742589.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13880 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700italic-d8505544.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19072 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800-35eb714d.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15088 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800-75db6959.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13960 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800italic-49512fd4.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17788 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800italic-49b6274b.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/index.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.442698 girder-5.0.0a2.dev10/girder/web/dist/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2938 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/auth.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.446698 girder-5.0.0a2.dev10/girder/web/dist/src/collections/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/ApiKeyCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/AssetstoreCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10660 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/Collection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/CollectionCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/FileCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      275 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/FolderCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/GroupCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/ItemCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/UserCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/constants.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4733 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/dialog.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/events.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/main.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6698 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/misc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.450698 girder-5.0.0a2.dev10/girder/web/dist/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2841 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/AccessControlledModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/ApiKeyModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/AssetstoreModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/CollectionCreationPolicyModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/CollectionModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10910 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/FileModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      882 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/FolderModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6427 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/GroupModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2284 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/ItemModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2964 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/MetadataMixin.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5688 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/Model.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5467 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/UserModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/pluginUtils.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7243 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/rest.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/router.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7074 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.406698 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.450698 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/apidocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      831 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/apidocs/apidocs.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.454697 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      310 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/adminConsole.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      792 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/assetstores.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      697 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/collectionList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/collectionPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      939 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/frontPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/groupList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2127 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/groupPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1370 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/itemPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/plugins.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/searchResultsList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/systemConfig.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userAccount.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userPage.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.458697 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/footer.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2843 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/global.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/globalNav.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/header.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/headerUser.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1320 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/layout.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/layoutVars.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      622 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/loading.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/progressArea.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.462698 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1788 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/accessWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/browserWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/hierarchyWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/markdownWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1662 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/metadataWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/searchFieldWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/taskProgress.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/timelineWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/uploadWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3818 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/userOtpManagementWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.406698 girder-5.0.0a2.dev10/girder/web/dist/src/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.466698 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/adminConsole.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3503 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/assetstores.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1484 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/collectionList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1307 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/collectionPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1887 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/filesystemImport.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2974 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/frontPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/groupList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3962 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/groupPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1836 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/itemPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      949 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/plugins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/s3Import.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/searchResults.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/searchResultsType.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10326 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/systemConfiguration.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3634 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userAccount.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userPage.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.470697 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/alert.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layout.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutFooter.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutGlobalNav.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutHeader.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      796 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutHeaderUser.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutProgressArea.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/loginDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1719 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/registerDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/resetPasswordDialog.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.482698 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditor.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditorMixins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditorNonModal.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEntry.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1918 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/apiKeyList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1126 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/browserWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/checkedActionsMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1273 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/collectionInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      565 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/confirmDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/dateTimeRangeWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/dateTimeWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editApiKeyWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3345 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editAssetstoreWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editCollectionWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editFileWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editFolderWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editGroupWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editItemWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/fileInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1229 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/fileList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/folderInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/folderList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupAdminList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3129 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupInviteDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupInviteList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupMemberList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupModList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyPaginated.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3835 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      461 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/itemBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1088 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/itemList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/jsonMetadatumEditWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/jsonMetadatumView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/loadingAnimation.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/markdownWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadataWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadatumEditWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadatumView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3972 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/newAssetstore.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/paginateWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/pluginConfigBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/rootSelectorWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/searchField.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/searchHelp.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/searchModeSelect.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      469 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/searchResults.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/sortCollectionWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/taskProgress.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/timeline.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/uploadWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1013 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/uploadWidgetMixins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/uploadWidgetNonModal.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      115 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/userOtpBegin.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/userOtpDisable.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/userOtpEnable.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.486698 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/EventStream.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/PluginUtils.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9489 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/S3UploadHandler.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.486698 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/jquery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/jquery/girderEnable.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2134 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/jquery/girderModal.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/version.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.486698 girder-5.0.0a2.dev10/girder/web/dist/src/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/App.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2561 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/View.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.494698 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/AdminView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8160 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/AssetstoresView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6740 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/CollectionView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4353 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/CollectionsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3146 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FilesystemImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FolderView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1305 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FrontPageView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11859 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/GroupView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/GroupsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6011 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/ItemView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/PluginsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/S3ImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5544 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/SearchResultsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6532 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/SystemConfigurationView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6266 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UserAccountView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5437 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UsersView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.498698 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/FooterView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3163 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/GlobalNavView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/HeaderUserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/HeaderView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/LoginView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/ProgressListView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3733 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/RegisterView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2344 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/ResetPasswordView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.510697 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15584 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/AccessWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4631 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ApiKeyListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14503 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/BrowserWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2441 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/CheckedMenuWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/CollectionInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/DateTimeRangeWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3368 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/DateTimeWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditApiKeyWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5411 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3239 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditCollectionWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditFileWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4203 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditFolderWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4479 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditGroupWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3797 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditItemWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FileInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5005 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FileListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FolderInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3360 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FolderListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2901 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupAdminsWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1838 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupInvitesWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5965 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupMembersWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2518 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupModsWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42297 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/HierarchyWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ItemBreadcrumbWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14228 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ItemListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/LoadingAnimation.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7648 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/MarkdownWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17263 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/MetadataWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/NewAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/PaginateWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/PluginConfigBreadcrumbWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6452 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/RootSelectorWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13112 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SearchFieldWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4508 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SearchPaginateWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SortCollectionWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3042 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/TaskProgressWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6664 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/TimelineWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13690 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/UploadWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3203 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/UserOtpManagementWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2673 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/vite-env.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/env.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2259 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/playwright.config.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.510697 girder-5.0.0a2.dev10/girder/web/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2707 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/coverage.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/playwright-setup.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/playwright-teardown.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/server.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.510697 girder-5.0.0a2.dev10/girder/web/tests/spec/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/admin.spec.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/girder/web/tests/spec/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/data/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/data/ten_byte_file.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1514 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_authorized_upload.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1148 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_hashsum_download.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1769 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_homepage.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1161 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_item_licenses.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      861 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_readme.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1567 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_terms.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2225 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_thumbnails.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_user_quota.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3551 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/util.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/wsgi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/girder.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2724 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18574 2024-04-12 16:12:21.000000 girder-5.0.0a2.dev10/girder.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   196254 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3517 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/pytest_girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/MANIFEST.in
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/assertions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6136 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2923 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/plugin_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/web_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      718 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/requirements-dev.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/scripts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/scripts/midas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11413 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/migrate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/walk_girder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1357 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/walk_midas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4118 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/publicNames.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35230 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/publicNames.txt
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      604 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/test_names.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-04-12 16:12:21.518698 girder-5.0.0a2.dev10/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/tox.ini
```

### Comparing `girder-3.2.3.dev7/.circleci/Dockerfile` & `girder-5.0.0a2.dev10/.circleci/Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -9,23 +9,25 @@
   && apt-get install --assume-yes \
     libldap2-dev \
     libsasl2-dev \
     autotools-dev \
     automake \
   && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
 
-RUN curl -sL https://deb.nodesource.com/setup_14.x | bash - \
+RUN curl -sL https://deb.nodesource.com/setup_16.x | bash - \
   && apt-get install -y nodejs \
   && find / -xdev -name __pycache__ -type d -exec rm -r {} \+ \
   && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
 
 # Install Girder development prereqs
 RUN apt-get update \
   && apt-get install --assume-yes \
     cmake \
+    automake \
+    nodejs \
   # Note: universal-ctags is installed for use in the public_names CI job.
   && git clone "https://github.com/universal-ctags/ctags.git" "./ctags" \
   && cd ./ctags \
   && ./autogen.sh \
   && ./configure \
   && make \
   && make install \
```

### Comparing `girder-3.2.3.dev7/.circleci/config.yml` & `girder-5.0.0a2.dev10/.circleci/config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 ---
 version: 2.1
 
 executors:
   py3:
     docker:
       # This image uses the newest version of many dependencies
-      - image: girder/girder_test:py38-node14
+      - image: girder/girder_test:py38-node16
     working_directory: /home/circleci/project
   py3-mongo:
     docker:
-      - image: girder/girder_test:py38-node14
+      - image: girder/girder_test:latest
       # Use the oldest supported MongoDB
       # This is equivalent to the deprecated circleci/mongo:<version>-ram image
       - image: mongo:3.6
         command: bash -c "mkdir /dev/shm/mongo && mongod --storageEngine ephemeralForTest --nojournal --dbpath=/dev/shm/mongo --noauth --bind_ip_all"
     working_directory: /home/circleci/project
   machine:
     machine:
       image: ubuntu-2004:202111-02
     working_directory: /home/circleci/project
 
 commands:
   install-girder:
     description: "Install Girder in a virtualenv and configure CTest"
     steps:
-      - run:
-          name: Generate python environment checksum file
-          command: ./girder/.circleci/generatePyEnvChecksum.sh > girder/py-env-checksum
-      - restore_cache:
-          key: venv-py3.8-{{ arch }}-{{ checksum "girder/py-env-checksum" }}-2
+      #- run:
+      #    name: Generate python environment checksum file
+      #    command: ./girder/.circleci/generatePyEnvChecksum.sh > girder/py-env-checksum
+      #- restore_cache:
+      #    key: venv-py3.8-{{ arch }}-{{ checksum "girder/py-env-checksum" }}
       - run:
           name: Create virtual environment (if necessary)
           command: if [ ! -d girder_env ]; then python3 -m venv girder_env; fi
       - run:
           name: Activate virtual environment
           command: echo ". $CIRCLE_WORKING_DIRECTORY/girder_env/bin/activate" >> $BASH_ENV
       - run:
@@ -45,33 +45,33 @@
             python3 -m pip install
             --upgrade
             --upgrade-strategy eager
             --editable .[sftp,mount]
             --editable clients/python
             --requirement requirements-dev.txt
           working_directory: girder
-      - save_cache:
-          paths:
-            - girder_env
-          key: venv-py3.8-{{ arch }}-{{ checksum "girder/py-env-checksum" }}-2
+      #- save_cache:
+      #    paths:
+      #      - girder_env
+      #    key: venv-py3.8-{{ arch }}-{{ checksum "girder/py-env-checksum" }}
 
 jobs:
   server-lint-test:
     executor: py3
     steps:
       - checkout:
           path: girder
       - run:
           name: Run server linting tests
           command: tox -e lint
           working_directory: girder
-      - run:
-          name: Test public symbols
-          command: tox -e public_names
-          working_directory: girder
+      #- run:
+      #    name: Test public symbols
+      #    command: tox -e public_names
+      #    working_directory: girder
       - run:
           name: Test building docs
           command: tox -e docs
           working_directory: girder
 
   server-pytest-test:
     executor: py3-mongo
@@ -132,53 +132,51 @@
   web-test:
     executor: py3-mongo
     steps:
       - checkout:
           path: girder
       - install-girder
       - run:
-          name: Build Girder web client
-          command: girder build --dev | cat
-      - run:
-          name: Create Girder build directory
-          command: mkdir girder_build
-      - run:
-          name: Run CTest
-          command: >-
-            ctest
-            --extra-verbose
-            --script "$CIRCLE_WORKING_DIRECTORY/girder/.circleci/ci_test.cmake"
-          environment:
-            TEST_GROUP: browser
-            PYTHON_VERSION: 3.8
-            PYTHON_EXECUTABLE: /home/circleci/project/girder_env/bin/python
-            JASMINE_TIMEOUT: 15000
-          working_directory: girder_build
+          name: Install and build @girder/core
+          command: |
+            npm ci
+            npm run build
+          working_directory: girder/girder/web
+      - run:
+          name: Install and build all plugins
+          command: python girder/.circleci/build_plugins.py girder/plugins
+      - run:
+          name: Install playwright browser dependencies
+          command: npm run install-browsers
+          working_directory: girder/girder/web
+      - run:
+          name: Test @girder/core
+          command: npm run test
+          working_directory: girder/girder/web
       - store_artifacts:
-          # Failure screenshots from web tests
-          path: girder/build/test/artifacts
-      - persist_to_workspace:
-          root: /home/circleci/project
-          paths:
-            - girder/build/test/coverage
+          path: girder/girder/web/coverage/report
+          destination: coverage
+      - store_artifacts:
+          path: girder/girder/web/test-results
+          destination: test-results
 
   integration-test:
     executor: machine
     steps:
       - checkout:
           path: girder
       - run:
-          name: Install NodeJS 14
+          name: Install NodeJS 16
           # CircleCI resets the Bash environment between every step, so any steps using node or npm
           # must first:
           #   source $NVM_DIR/nvm.sh
           command: |
             source $NVM_DIR/nvm.sh
-            nvm install v14
-            nvm alias default v14
+            nvm install v16
+            nvm alias default v16
             NODE_DIR=$(dirname $(which node))
             echo "export PATH=$NODE_DIR:\$PATH" >> $BASH_ENV
       - run:
           # Technically, we should add the circleci user to the fuse group, log
           # out, and log back in for it to take effect.  This allows fuse to be
           # available to all users without requiring them to be in the fuse
           # group
@@ -216,19 +214,19 @@
              pyenv install 3.8.12 || true
              pyenv global 3.8.12
       - run:
           name: Install system dependencies for Girder plugins
           command: sudo apt-get install -y libldap2-dev libsasl2-dev
       - install-girder
       - run:
-          name: Build Girder web client
+          name: Install and build @girder/core
           command: |
-            npm --version
-            node --version
-            girder build --dev | cat
+            npm ci
+            npm run build
+          working_directory: girder/girder/web
       - run:
           name: Create Girder build directory
           command: mkdir girder_build
       - run:
           name: CMake
           command: >-
             cmake
@@ -266,120 +264,82 @@
       - attach_workspace:
           at: /home/circleci/project
       - run:
           name: Generate Python coverage report
           command: tox -e coverage
           working_directory: girder
       - run:
-          name: Install Javascript utilities
-          command: npm ci
-          working_directory: girder
-      - run:
-          name: Generate web coverage report
-          command: npm run coverage
-          working_directory: girder
-      - store_artifacts:
-          # Human-readable coverage reports
-          path: girder/build/test/artifacts
-      - run:
           name: Install Codecov client
           command: |
               curl -Os https://uploader.codecov.io/latest/linux/codecov
               chmod +x codecov
           working_directory: girder
       - run:
           name: Upload coverage
           command: ./codecov --disable search pycov gcov --root girder --required --file build/test/coverage/py_coverage.xml build/test/coverage/cobertura-coverage.xml
           working_directory: girder
 
-  ansible-test:
-    docker:
-      - image: cimg/python:3.8
-    working_directory: ~/project
-    steps:
-      - run:
-          name: Install packages needed for ansible
-          command: |
-            sudo apt-get update
-            sudo apt-get install -y rsync
-      - checkout:
-          path: girder
-      - setup_remote_docker:
-          docker_layer_caching: true
-          version: 20.10.12
-      - run:
-          name: Install tox
-          command: pip install tox
-      - run:
-          name: Run Ansible tests
-          command: tox -e ansible
-          working_directory: girder
-
   dockers:
     machine:
         image: ubuntu-2004:202111-02
     steps:
       - checkout
       - run:
           name: Build the Girder docker
           command: |
             docker build --force-rm -t girder/girder .
       - run:
           name: Build the Girder test docker
           command: |
             cd .circleci
-            docker build --force-rm -t girder/girder_test:py38-node14 .
+            docker build --force-rm -t girder/girder_test:py38-node16 .
 
   publish-dockers:
     machine:
         image: ubuntu-2004:202111-02
     steps:
       - checkout
       - run:
           name: Build the Girder docker
           command: |
             docker build --force-rm -t girder/girder .
       - run:
           name: Build the Girder test docker
           command: |
             cd .circleci
-            docker build --force-rm -t girder/girder_test:py38-node14 .
+            docker build --force-rm -t girder/girder_test:py38-node16 .
       - run:
           name: Publish the images to Docker Hub
           command: |
               echo "$DOCKERHUB_PASS" | docker login -u "$DOCKERHUB_USERNAME" --password-stdin
               docker push girder/girder:latest
               docker tag girder/girder:latest girder/girder:latest-py3
               docker push girder/girder:latest-py3
               if [[ $CIRCLE_TAG =~ ^v.*$ ]]; then
               docker tag girder/girder:latest "girder/girder:$CIRCLE_TAG"
               docker push "girder/girder:$CIRCLE_TAG"
               docker tag girder/girder:latest "girder/girder:${CIRCLE_TAG}-py3"
               docker push "girder/girder:${CIRCLE_TAG}-py3"
               fi
-              docker push girder/girder_test:py38-node14
+              docker push girder/girder_test:py38-node16
 
   publish:
     docker:
-      - image: cimg/python:3.8
+      - image: girder/girder_test:py38-node16
     working_directory: ~/project
     steps:
       - checkout:
           path: girder
       - run:
           name: Install tox
           command: pip install tox
       - deploy:
           name: Publish Python packages
           command: tox -e publish
           working_directory: girder
-      # - deploy:
-      #     name: Publish Ansible role
-      #     command: tox -e release_ansible
-      #     working_directory: girder
 
   publish-release:
     executor: py3
     steps:
       - checkout:
           path: girder
       - deploy:
@@ -420,39 +380,35 @@
             - server-pytest-test
             - server-legacy-test
             - web-test
             - integration-test
           filters:
             tags:
               only: /^v[0-9]+.*/
-      # - ansible-test:
-      #     filters:
-      #       tags:
-      #         only: /^v[0-9]+.*/
       - dockers:
           filters:
             tags:
               only: /^v[0-9]+.*/
       - publish:
           requires:
             - server-lint-test
             - web-lint-test
             - coverage
-            # - ansible-test
           filters:
             tags:
               only: /^v[0-9]+.*/
             branches:
-              only: master
+              only:
+                - master
+                - v4-integration
       - publish-release:
           requires:
             - server-lint-test
             - web-lint-test
             - coverage
-            # - ansible-test
           filters:
             tags:
               only: /^v[0-9]+.*/
             branches:
               ignore: /.*/
       - publish-dockers:
           requires:
```

### Comparing `girder-3.2.3.dev7/.circleci/publish_npm.sh` & `girder-5.0.0a2.dev10/.circleci/publish_npm.sh`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 set -e
 # Publish npm packages for selected locations
 # NPM_AUTH_TOKEN must be set by the build environment
 
 readonly GIT_VERSION=$(git describe --tags)
 readonly PUBLISHED_NPM_PACKAGES=(
   # Published Fontello is used by all builds, and is critical to publish
-  girder/web_client/fontello
-  # These lint configs are used by downstream plugins
-  girder/web_client/eslint-config
-  girder/web_client/pug-lint-config
+  girder/web/fontello
   # The raw JS source is used by some downstream 'external builds'
-  girder/web_client/src
+  girder/web/src
   # These plugins were published to support downstream external builds, and should be kept updated
   plugins/jobs/girder_jobs/web_client
   plugins/oauth/girder_oauth/web_client
   plugins/gravatar/girder_gravatar/web_client
 )
 for directory in "${PUBLISHED_NPM_PACKAGES[@]}"; do
   pushd "$directory"
```

### Comparing `girder-3.2.3.dev7/.codecov.yml` & `girder-5.0.0a2.dev10/.codecov.yml`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/CHANGELOG.rst` & `girder-5.0.0a2.dev10/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/CMakeLists.txt` & `girder-5.0.0a2.dev10/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 include(CTest)
 include(CMakeParseArguments)
 
 set(PYTHON_VERSION "3.8" CACHE STRING "Python version used for testing")
 
 find_package(PythonInterp ${PYTHON_VERSION} REQUIRED)
 
-option(BUILD_JAVASCRIPT_TESTS "Build Javascript tests" ON)
 option(RUN_CORE_TESTS "Whether to run the core tests" ON)
 set(TEST_PLUGINS "" CACHE STRING "List of plugins to test. Leave empty to test all plugins")
 
 find_program(PYTHON_COVERAGE_EXECUTABLE NAMES coverage python-coverage)
 
 if(BUILD_TESTING)
   include(tests/TestData.cmake)
   include(tests/TestCommon.cmake)
   include(tests/PythonTests.cmake)
-  include(tests/JavascriptTests.cmake)
   add_subdirectory(tests)
 endif()
```

### Comparing `girder-3.2.3.dev7/CONTRIBUTING.rst` & `girder-5.0.0a2.dev10/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/LICENSE` & `girder-5.0.0a2.dev10/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/PKG-INFO` & `girder-5.0.0a2.dev10/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder
-Version: 3.2.3.dev7
+Version: 5.0.0a2.dev10
 Summary: Web-based data management platform
 Home-page: https://girder.readthedocs.org
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-3.2.3.dev7/README.rst` & `girder-5.0.0a2.dev10/README.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/clients/python/girder_client/__init__.py` & `girder-5.0.0a2.dev10/clients/python/girder_client/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/clients/python/girder_client/cli.py` & `girder-5.0.0a2.dev10/clients/python/girder_client/cli.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/clients/python/setup.py` & `girder-5.0.0a2.dev10/clients/python/setup.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/devops/ansible-role-girder/LICENSE` & `girder-5.0.0a2.dev10/pytest_girder/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
@@ -174,23 +175,23 @@
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
    APPENDIX: How to apply the Apache License to your work.
 
       To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
+      boilerplate notice, with the fields enclosed by brackets "[]"
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {yyyy} {name of copyright owner}
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `girder-3.2.3.dev7/docs/api-docs.rst` & `girder-5.0.0a2.dev10/docs/api-docs.rst`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,14 @@
 
 .. automodule:: girder.utility.config
    :members:
 
 .. automodule:: girder.utility.filesystem_assetstore_adapter
    :members:
 
-.. automodule:: girder.utility.gridfs_assetstore_adapter
-   :members:
-
 .. automodule:: girder.utility.mail_utils
    :members:
 
 .. automodule:: girder.utility.model_importer
    :members:
 
 .. automodule:: girder.utility.path
```

### Comparing `girder-3.2.3.dev7/docs/conf.py` & `girder-5.0.0a2.dev10/docs/conf.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/dependencies.rst` & `girder-5.0.0a2.dev10/docs/dependencies.rst`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 --------------
 Installation of Girder's server has the following system dependencies:
 
 .. note:: Girder only performs continuous integration testing on this particular combination
           of dependencies. The Girder development team can only provide bugfixes and support
           for this environment.
 
-* `Ubuntu <https://releases.ubuntu.com/>`_ 18.04
+* `Ubuntu <https://releases.ubuntu.com/>`_ 20.04
 
   * Girder interacts with some system libraries (particularly
     `OpenSSL <https://packages.ubuntu.com/bionic/openssl>`_) at a very low level, so other
     operating system distributions and versions may not be compatible.
 
 * `Python <https://www.python.org>`_ v3.8
```

### Comparing `girder-3.2.3.dev7/docs/developer-cookbook.rst` & `girder-5.0.0a2.dev10/docs/developer-cookbook.rst`

 * *Files 4% similar despite different names*

```diff
@@ -294,38 +294,31 @@
     mail_utils.sendMailToAdmins(subject='...', text='...')
 
 .. note:: All emails are sent as rich text (``text/html`` MIME type).
 
 Logging a Message
 ^^^^^^^^^^^^^^^^^
 
-Girder application servers maintain an error log and an information log and expose
-a utility module for sending events to them. Any 500 error that occurs during
-execution of a request will automatically be logged in the error log with a
-full stack trace. Also, any 403 error (meaning a user who is logged in but
-requests access to a resource that they don't have permission to access) will also be logged
-automatically. All log messages automatically include a timestamp, so there
-is no need to add your own.
+Girder uses standard Pythonic and 12-factor app logging practices, e.g.::
 
-If you want to log your own custom error or info messages outside of those default
-behaviors, use the following examples:
 
 .. code-block:: python
 
-    from girder import logger
+    import logging
+
+    logger = logging.getLogger(__name__)
 
     try:
         ...
     except Exception:
         # Will log the most recent exception, including a traceback, request URL,
         # and remote IP address. Should only be called from within an exception handler.
         logger.exception('A descriptive message')
 
-    # Will log a message to the info log.
-    logger.info('Test')
+    logger.info('This is an info message')
 
 Adding Automated Tests with CTest
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. note:: Girder is transitioning towards using `pytest <https://pytest.org>`_ for its testing.
           The section below describes how to add automated tests using ``pytest``.
 
@@ -522,31 +515,31 @@
         COVERAGE_PATHS "${PROJECT_SOURCE_DIRECTORY}/plugins/cats/utils"
     )
 
 
 Mounting a custom application
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Normally, the root node (``/``) of the server will serve up the Girder web client.
-A plugin may contain an entire application separate from the default Girder
-web client. This plugin may be written in a way which enables administrators
-to mount the application at a configured endpoint, including the option of
-replacing the root node with the plugin application.
-
-To achieve this, you simply have to register your own root and configure your routes
-as you wish. In your plugin's ``load`` method, you would follow this convention:
+The info object passed to plugins' ``load`` method contains a ``serverRoot`` object that is the
+`CherryPy tree object <https://docs.cherrypy.dev/en/latest/pkg/cherrypy._cptree.html#cherrypy._cptree.Tree>`_
+that will be served by the server, either via ``girder serve`` in development, or via the
+``girder.wsgi:app`` object with your own WSGI server in production. You can mount your own
+applications here using the ``mount`` method, or delete the default Girder application if you wish.
+Note that if you wish to server Girder's default SPA from a place other than the root path ``/``,
+you'll need to rebuild the SPA with a different ``base`` value before it will serve properly. Doing
+this is out of scope of these docs, since there are many different ways to serve static content,
+but the command to build the SPA with a different base looks as follows:
 
-.. code-block:: python
+.. code-block:: bash
 
-    from girder.plugin import registerPluginWebroot
-    registerPluginWebroot(CustomAppRoot(), info['name'])
+    cd <path_to_girder_source_tree>/girder/web
+    npx vite build --base=/new_root/
 
-This will register your ``CustomAppRoot`` with Girder so that it can then be mounted
-wherever an Administrator specifies using the Server Configuration Panel. See
-:ref:`Managing Routes <managing-routes>`.
+That assumes that you've moved the SPA (``info['serverRoot'].apps['']``) to be served out of
+``/new_root`` instead of ``''``.
 
 Supporting web browser operations where custom headers cannot be set
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Some aspects of the web browser make it infeasible to pass the usual
 ``Girder-Token`` authentication header when making a request. For example,
 if using an ``EventSource`` object for SSE, or when you must redirect the user's
```

### Comparing `girder-3.2.3.dev7/docs/development.rst` & `girder-5.0.0a2.dev10/docs/development.rst`

 * *Files 21% similar despite different names*

```diff
@@ -13,57 +13,29 @@
 Next, you should install the Python development dependencies with pip, to
 provide helpful development tools and to allow the test suite to run: ::
 
     pip install -r requirements-dev.txt
 
 Install front-end web client development dependencies and build the web client code: ::
 
-    girder build --dev
+    cd girder/web && yarn && yarn build
 
-For more options for building the web client, run: ::
+This will build the core web client. Any plugins you plan to install that have front-end code
+will need to be built as well. For example, to build the jobs plugin: ::
 
-    girder build --help
+    cd plugins/jobs/girder_jobs/web_client && yarn && yarn build
 
 Finally, you'll want to set your server into development mode. Add the following entry into your
 local config file (see :ref:`Configuration <configuration>` for instructions):
 
 .. code-block:: ini
 
     [server]
     mode="development"
 
-Vagrant
-^^^^^^^
-
-A shortcut to going through the development environment configuration steps is
-to use `Vagrant <https://www.vagrantup.com>`_ to setup the environment on a
-`VirtualBox <https://www.virtualbox.org>`_ virtual machine. For more
-documentation on how to set this up, see `Developer Installation <dev-installation.html>`__
-
-During Development
-------------------
-
-Once Girder is started via ``girder serve``, the server
-will reload itself whenever a Python file is modified.
-
-If you are doing front-end development, it's much faster to use a *watch* process to perform
-automatic fast rebuilds of your code whenever you make changes to source files.
-
-If you are making changes to Girder's core web client, run the following watch command: ::
-
-    girder build --watch
-
-If you are developing a web client of a plugin, run: ::
-
-    girder build --watch-plugin your_plugin_name
-
-With ``watch`` option, *sourcemaps* will be generated, which helps debugging front-end code in browser.
-When you want to end the watch process, press Ctrl+C (or however you would normally terminate a
-process in your terminal).
-
 Girder Shell
 ^^^^^^^^^^^^
 
 To test various functionality in a typical REPL (Python, IPython, etc) some bootstrapping
 is required to configure the Girder server. This sets up an "embedded" server, meaning no TCP ports
 are actually bound but requests can still be performed via Python. Bootstrapping the server
 involves running ``girder.utility.server.configureServer`` with the plugins to be enabled.
@@ -227,128 +199,48 @@
 To run static analysis tests on client side code, run from the top-level Girder directory:
 
 .. code-block:: bash
 
    npm i
    npm run lint
 
-Running the Tests with CTest
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Using the same setup as above for the Server Side Tests, your environment will be set up.
-The client side tests and server side tests are both harnessed with CTest, so use the following commands to run both ::
-
-    cd girder-build
-    ctest
-
-will run all of the tests, which include the client side tests.  Our client tests use the
-Jasmine JS testing framework.
-
-If you encounter errors, there is a chance you missed certain steps for setting up development dependencies.
-You could use ``ccmake`` to change ``CMake`` configuration. Or, it might be easier to recreate the environment from the beginning.
-
-When running client side tests, if you try to SIGINT (ctrl+c) the CTest process, CTest
-won't pass that signal down to the test processes for them to handle.  This can result
-in orphaned python unittest processes and can prevent future runs of client tests.  If you
-run a client side test and see an error message similar to ``IOError: Port 30015 not free on '0.0.0.0'``,
-then look for an existing process similar to ``/usr/bin/python3 -m unittest -v tests.web_client_test``,
-kill the process, and then try your tests again.
-
-Adding a New Client Side Test
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-To add a new client side test, add a new spec file in ``/girder/web_client/test/spec/``, add a line
-referencing your spec file to ``/girder/tests/CMakeLists.txt`` using the ``add_web_client_test`` function,
-and then run in your build directory ::
+Running the client end-to-end tests
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-    cmake ../girder
+Girder's web client test suite are setup as end-to-end tests that make use of an actual server
+and database. To run them, make sure you are within your Girder virtual environment, and make sure
+`mongod` is running locally on port 27017. You'll also need to make sure you've built all the plugin
+web client code, which can be done with:
 
-before running your tests.
-
-An example of a very simple client side test would be as follows ::
-
-    add_web_client_test(some_client_test "someSpec.js" PLUGIN "my_plugin")
+.. code-block:: bash
 
-The ``PLUGIN`` argument indicates that "my_plugin" is the owner of ``some_client_test``, at the time of the test my_plugin and all of its dependencies will be loaded.
+    python .circleci/build_plugins.py ./plugins
 
-If additional plugins are needed for a specific test, that can be achieved using the ``ENABLEDPLUGINS`` argument ::
+Once that is done, then run:
 
-    add_web_client_test(another_client_test "anotherSpec.js" PLUGIN "my_plugin" ENABLEDPLUGINS "my_plugin" "jobs")
+.. code-block:: bash
 
-Here ``ENABLEDPLUGINS`` ensures that my_plugin *and* the jobs plugin are loaded, along with their dependencies at the time of ``another_client_test``.
+    cd girder/web
+    npm i
+    npm run test
 
-.. note:: Core functionality shouldn't depend on plugins being enabled, this test definition is more suitable for a plugin. Information for testing plugins can be found under :doc:`plugin-development`.
 
-You will find many useful methods for client side testing in the ``girderTest`` object
-defined at ``/girder/web_client/test/testUtils.js``.
+Adding a New Client Side Test
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+To add a new client side test, add a new spec file in ``girder/web/test/spec/``. We recommend
+copying an existing test case for setting up the server, and then using VSCode's Playwright plugin
+to record your interactions.
 
 Test Coverage Reporting
 -----------------------
 When Girder's full test suite is run in the CI environment, a test coverage report for both
 server and client code is generated and uploaded to Codecov. This may be
 `viewed online at any time <https://codecov.io/gh/girder/girder>`_.
 
-Initializing the Database for a Test
-------------------------------------
-
-.. note:: This functionality has not yet been ported to our ``pytest`` tests.
-
-When running tests in Girder, the database will initially be empty.  Often times, you want to be able to start the test with the database in a
-particular state.  To avoid repetitive initialization code, Girder provides a way to import a folder hierarchy from the file system
-using a simple initialization file.  This file is in YAML (or JSON) format and provides a list of objects to insert into the database
-before executing your test.  A typical example of this format is as follows
-
-.. code-block:: YAML
-
-    ---
-    users:
-      - login: 'admin'
-        password: 'password'
-        firstName: 'First'
-        lastName: 'Last'
-        email: 'admin@girder.test'
-        admin: true
-        import: 'files/user'
-
-    collections:
-      - name: 'My collection'
-        public: true
-        creator: 'admin'
-        import: 'files/collection'
-
-This will create one admin user and a public collection owned by that user.  Both the generated user and collection objects
-will contain folders imported from the file system.  Relative paths provided by the ``import`` key will be resolved relative
-to the location of the YAML file on disk.  You can also describe the full hierarchy in the YAML file itself for more complicated
-use cases.  See the test spec in ``tests/cases/setup_database_test.yml`` for a more complete example.
-
-.. note::
-
-    When importing from a local path into a user or collection, files directly under that path are ignored because
-    items can be only inserted under folders.
-
-To use the initialization mechanism, you should add the YAML file next to your test file.  For example, if your test
-is defined in ``tests/cases/my_test.py``, then the initialization spec should go in ``tests/cases/my_test.yml``.  This
-file will be automatically detected and loaded before executing your test code.  This is true for both python and
-javascript tests added in core or inside plugins.
-
-The python module ``setup_database.py`` that generates the database can also be run standalone to help in development.  To use it,
-you should point girder to an empty database ::
-
-    GIRDER_MONGO_URI='mongodb://127.0.0.1:27017/mytest' python tests/setup_database.py tests/test_database/spec.yml
-
-You can browse the result in Girder by running ::
-
-    GIRDER_MONGO_URI='mongodb://127.0.0.1:27017/mytest' girder serve
-
-.. note::
-
-    The ``setup_database`` module is meant to provision fixures for tests **only**.  If you want to provision
-    a Girder instance for deployment, see the `Girder ansible client <https://github.com/girder/girder/tree/master/devops/ansible-role-girder/library>`_.
-
-
 Code Review
 -----------
 
 Contributions to Girder are done via pull requests with a core developer
 approving the PR with GitHub review system. At this point, the
 topic branch can be merged to master. This is meant to be a simple,
 low-friction process; however, code review is very important. It should be done
```

### Comparing `girder-3.2.3.dev7/docs/favicon.ico` & `girder-5.0.0a2.dev10/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/images/dicom-viewer.png` & `girder-5.0.0a2.dev10/docs/images/dicom-viewer.png`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/index.rst` & `girder-5.0.0a2.dev10/docs/index.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/license.png` & `girder-5.0.0a2.dev10/docs/license.png`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/migration-guide.rst` & `girder-5.0.0a2.dev10/docs/migration-guide.rst`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,246 @@
 ===============
 
 This document is meant to guide Girder plugin developers in transitioning
 between major versions of Girder. Major version bumps contain breaking changes
 to the Girder core library, which are enumerated in this guide along with
 instructions on how to update your plugin code to work in the newer version.
 
+3.x |ra| 5.x
+------------
+
+Major version 5 contains significant breaking changes on many fronts. The central theme of these
+changes is to bring Girder into compliance with the principles of the
+`12-factor app <https://12factor.net/>`_ to enhance its portability to various managed runtimes,
+and in turn its ease of scalability. We chose to skip major version 4 due to a name collision with
+Kitware's Django-based stack, which we had originally called Girder 4, but now refer to as Resonant
+to distinguish it from this software.
+
+The following are the breaking (or otherwise major) changes, ranked roughly in order of how
+disruptive they are to downstream plugins:
+
+Front-end build system changes
+++++++++++++++++++++++++++++++
+
+The largest change to Girder in version 5 is a complete overhaul of the front-end build system. Most
+notably for users and plugin developers, the ``girder build`` command no longer exists, and Girder
+itself will no longer manage the building of its plugins' web client bundles. Rather, each plugin is
+responsible for building its own web client plugin code and exposing it via the following mechanism:
+
+.. code-block:: python
+
+    from pathlib import Path
+
+    from girder.plugin import GirderPlugin, registerPluginStaticContent
+
+    class Foo(GirderPlugin):
+        DISPLAY_NAME = 'Foo'
+
+        def load(self, info):
+            registerPluginStaticContent(
+                plugin='foo',
+                css=['/style.css'],
+                js=['/girder-plugin-foo.umd.cjs'],
+                staticDir=Path(__file__).parent / 'web_client' / 'dist',
+                tree=info['serverRoot'],
+            )
+
+Whatever files are passed into the ``js`` and ``css`` lists will be included in the core web client
+after it loads. The ``staticDir`` argument should point to the directory containing the built web
+client code, i.e. the filenames passed into the ``js`` and ``css`` lists are relative to this local
+path. The ``tree`` argument should be the ``serverRoot`` object passed into the ``load`` method.
+
+Changes within front-end plugin code
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+There is a mechanical conversion that will need to be performed on all front-end plugin code when
+moving to Girder 5: rather than static ``import`` of symbols from ``@girder/core``
+in your JavaScript/TypeScript code, you will instead rely on the presence of the ``girder`` symbol
+in the global scope (``window.girder``) at runtime. Each import from ``@girder/core`` should be
+changed as in the following examples:
+
+Before:
+
+.. code-block:: javascript
+
+    import router from '@girder/core/router';
+    import events from '@girder/core/events';
+    import { exposePluginConfig } from '@girder/core/utilities/PluginUtils';
+
+    import FrontPageView from '@girder/core/views/body/FrontPageView';
+    import { renderMarkdown } from '@girder/core/misc';
+    import { restRequest, getApiRoot } from '@girder/core/rest';
+    import { wrap } from '@girder/core/utilities/PluginUtils';
+
+After:
+
+.. code-block:: javascript
+
+    const router = girder.router;
+    const events = girder.events;
+    const { exposePluginConfig } = girder.utilities.PluginUtils;
+
+    const FrontPageView = girder.views.body.FrontPageView;
+    const { renderMarkdown } = girder.misc;
+    const { restRequest, getApiRoot } = girder.rest;
+    const { wrap } = girder.utilities.PluginUtils;
+
+
+Static tooling
+^^^^^^^^^^^^^^
+
+If you are using vite as your plugin build tool, you can add the following to your ``vite-env.d.ts``
+file to make TypeScript aware of the ``girder`` symbol, which enables things like IDE
+autocompletion and jump-to-definition for symbols under the ``girder`` namespace.
+
+.. code-block:: typescript
+
+    /// <reference types="vite/client" />
+    import { type Girder } from '@girder/core';
+
+    declare global {
+      const girder: Girder;
+    }
+
+
+Plugins are now also responsible for testing their own web client code. If your plugin was relying
+on any of the old testing infrastructure, those tests will no longer work. We may publish our
+Playwright-based front-end testing utilities as a separate package in the future, but as of 5.0,
+it is not exposed to downstreams.
+
+Removal of the events daemon
+++++++++++++++++++++++++++++
+
+The ``girder.events.daemon`` symbol has been removed, as the use of a background thread violated
+the WSGI contract and tightly coupled Girder to a multi-threaded server model. The main impact of
+this change is that any downstream users listening to the core ``"data.process"`` event,
+which used to be run on the background thread, should now convert their event handlers to be
+celery tasks or otherwise asynchronous methods if there's any risk of the handler taking more
+than 1-2 seconds to complete.
+
+Dynamic route configuration system removed
+++++++++++++++++++++++++++++++++++++++++++
+
+The server-side route table infrastructure that allowed dynamically updating URL paths from which
+webroots would be served has been removed. URL routing should be known at startup time, and not
+changed dynamically. This means that the ``girder.plugin.registerPluginWebroot`` function has been
+removed.
+
+The main challenge this presents is specifically for use cases where downstreams need to serve
+the core Girder front-end application from a base path other than the server root (``/``), since
+with the 5.0 front-end build changes, the front-end application is bundled in and built with a
+static base of ``/``. For this specific use case, one strategy that's supported is to build the
+core front-end application with a different base path, and then configure your server to serve
+the modified front-end client from the desired path on the filesystem.
+
+Example
+^^^^^^^
+
+In your plugin initialization function, add the following:
+
+.. code-block:: python
+
+    core_girder = info['serverRoot'].apps['']
+    core_girder.script_name = '/new_root'
+    info['serverRoot'].mount(core_girder, '/new_root', core_girder.config)
+    del info['serverRoot'].apps['']
+    # Mount your own app under `info['serverRoot']` if you want
+
+Then, build the core front-end application with the desired base path:
+
+.. code-block:: bash
+
+    git clone git@github.com:girder/girder.git
+    cd girder/girder/web
+    npx vite build --base=/new_root/
+    export GIRDER_STATIC_ROOT_DIR=$(pwd)/dist
+
+With that variable set in your environment, the Girder core web client will now be served under
+``/new_root/`` rather than ``/``.
+
+Logging changes
++++++++++++++++
+
+Girder's logging system was overhauled to adhere to
+`12-factor logging principles <https://12factor.net/logs>`_. Use standard idiomatic Python
+logging everywhere now, e.g.:
+
+.. code-block:: python
+
+    import logging
+    logger = logging.getLogger(__name__)
+    logger.info('My message')
+
+The ``girder.logprint`` function was removed, and Girder will no longer write log messages to local
+files on the server's filesystem. Additionally, the API endpoints for fetching logs and log info
+were removed. Instead, logs are now written to standard output and it is up to the deployment
+environment to direct them as needed. There are a huge variety of tools and strategies for log
+management, so precise recommendations on log handlers are out of scope for Girder itself.
+
+Config files removed
+++++++++++++++++++++
+
+The ``girder.local.cfg`` and ``girder.dist.cfg`` files are no longer used. Instead, all settings
+should be passed in through the environment, or as command-line overrides in the case of using
+``girder serve`` in development. Everything that was able to be controlled by the config file can
+now be controlled by environment variables; see the
+:ref:`configuration documentation <configuration_via_env>` for specifics on how to set these.
+
+A notable change here is the configuration of the caching modules, which was previously done
+via the config file alone. Now, the caching modules are configured via environment variables. e.g.
+
+.. code-block:: bash
+
+    GIRDER_SETTING_CORE_CACHE_ENABLED=true
+    GIRDER_SETTING_CORE_CACHE_CONFIG='{"cache.global.backend": "dogpile.cache.redis", "cache.global.expiration_time": 7200}'
+
+Config keys prefixed by ``cache.global.`` are used to configure the global dogpile cache, and
+keys prefixed by ``cache.request.`` are used to configure the request cache.
+
+WSGI app for production deployments
++++++++++++++++++++++++++++++++++++
+
+Through load testing (as well as production usage), we discovered that cherrypy's built-in server
+is not suitable for production use. It is not as performant as a dedicated WSGI server, and some
+fraction of requests fail ungracefully under moderate load. As such, the ``girder serve`` command
+is now only suitable for development and testing.
+
+For production deployments, Girder now exposes a well-behaved WSGI app at ``girder.wsgi:app``.
+Use a WSGI server such as gunicorn or uwsgi to serve in production. See
+the :ref:`deployment documentation <deployment>` for an example gunicorn invocation.
+
+Removal of the GridFS assetstore type
++++++++++++++++++++++++++++++++++++++
+
+When we originally created the GridFS assetstore, it seemed like a reasonable blob storage solution.
+However, in 2024, it is no longer a recommended solution for Girder. We have removed the GridFS
+assetstore adapter type from the core codebase. If you are using GridFS, we recommend migrating your
+data to a Filesystem or S3 assetstore type and deleting your GridFS assetstore prior to upgrading
+to major version 5. There are many offerings in the cloud that support either the S3 or filesystem
+assetstore adapter in a scalable way.
+
+Python version support
+++++++++++++++++++++++
+
+Girder will now only maintain support for CPython versions that have not reached their end-of-life.
+Check `this page <https://devguide.python.org/versions/>`_ to see the current status of upstream
+Python version support. Note that this means we will feel free to use newer language features in
+core as soon as they are available in the oldest supported version.
+
+Switch to HttpOnly cookies in core web client
++++++++++++++++++++++++++++++++++++++++++++++
+
+The ``auth.cookie`` symbol has been removed from the core web client. Cookies sent by the server
+will now be set with the ``HttpOnly`` flag. This means that the cookies will no longer be
+accessible to JavaScript, which is a security best practice. If you were relying on the
+``auth.cookie`` symbol in your plugin, you should now use the ``auth.token`` symbol instead.
+
+Note that cookies will still be sent and will still work for read-only endpoints that have
+set the ``cookie=True`` property on their ``@access`` decorator.
+
 2.x |ra| 3.x
 ------------
 
 Girder 3.0 changed how plugins are installed and loaded into the runtime
 environment.  These changes require that **all** plugins exist as a standalone
 python package.  Automatic loading of plugins from Girder's ``plugins``
 directory is no longer supported.  This also applies to plugins that have no
```

### Comparing `girder-3.2.3.dev7/docs/mount.rst` & `girder-5.0.0a2.dev10/docs/mount.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/plugin-development.rst` & `girder-5.0.0a2.dev10/docs/plugin-development.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/plugins.rst` & `girder-5.0.0a2.dev10/docs/plugins.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,34 +48,14 @@
 When a new user registers, each auto join rule is checked to see if the user's
 email address contains the rule pattern as a substring (case insensitive).
 
 If there is a match, the user is added to the group with the specified access
 level.
 
 
-DICOM Viewer
-------------
-`PyPI package <https://pypi.org/project/girder-dicom-viewer/>`__: ``girder-dicom-viewer``
-
-The DICOM Viewer plugin adds support for previewing DICOM files when viewing
-an item in girder. If multiple DICOM files are present in a single item, they
-are presented as multiple slices. The DICOM image is shown as well as a table
-of DICOM tags. The window center and width can be changed by the user. Controls
-allow the user to step through slices, auto-level the window, auto-zoom, or
-playback the slices at different speeds.
-
-This plugin parses the DICOM tags when files are uploaded and stores them in
-the MongoDB database for quick retrieval. This is mostly used to sort multiple
-images by series and instance.
-
-.. figure:: images/dicom-viewer.png
-
-    DICOM imagery from: https://wiki.cancerimagingarchive.net/display/Public/RIDER+NEURO+MRI
-
-
 Download Statistics
 -------------------
 `PyPI package <https://pypi.org/project/girder-download-statistics/>`__: ``girder-download-statistics``
 
 This plugin tracks and records file download activity. The recorded information
 (downloads started, downloads completed, and total requests made) is stored on the
 file model: ::
```

### Comparing `girder-3.2.3.dev7/docs/python-client.rst` & `girder-5.0.0a2.dev10/docs/python-client.rst`

 * *Files 1% similar despite different names*

```diff
@@ -142,26 +142,20 @@
     girder-client upload 54b6d41a8926486c0cbca367 test_folder --reuse
 
 To include a blacklist of file patterns that will not be uploaded, pass a comma
 separated list to the ``--blacklist`` arg ::
 
     girder-client upload 54b6d41a8926486c0cbca367 test_folder --blacklist .DS_Store
 
-.. note:: The girder_client can upload to an S3 Assetstore when uploading to a Girder server
-   that is version 1.3.0 or later.
+.. note: The girder_client can upload to an S3 Assetstore when uploading to a Girder server
+         that is version 1.3.0 or later.
 
 Download a hierarchy of data into a local folder
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-.. note:: When downloading files, Girder writes them temporarily under the operating system's
-    temporary directory before moving them to their final destination. If you need the
-    temporary files to be stored elsewhere, perhaps due to being on a different volume or
-    device, simply set the ``TMPDIR`` environment variable to the desired location before
-    invoking the download.
-
 Folder
 """"""
 
 To download a Girder Folder hierarchy rooted at Folder id
 ``54b6d40b8926486c0cbca364`` under the local folder ``download_folder`` ::
 
     girder-client download 54b6d40b8926486c0cbca364 download_folder
```

### Comparing `girder-3.2.3.dev7/docs/security.rst` & `girder-5.0.0a2.dev10/docs/security.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/sftp.rst` & `girder-5.0.0a2.dev10/docs/sftp.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/docs/user-guide.rst` & `girder-5.0.0a2.dev10/docs/user-guide.rst`

 * *Files 3% similar despite different names*

```diff
@@ -108,26 +108,14 @@
 the root directory under which files should be stored.
 
 .. note:: If your Girder environment has multiple different application servers
    and you plan to use the Filesystem assetstore type, you must set the
    assetstore root to a location on the filesystem that is shared between all
    of the application servers.
 
-GridFS
-^^^^^^
-
-This ``Assetstore`` type stores files directly within your Mongo database using
-the **GridFS** model. You must specify the database name where files will be
-stored; for now, the same credentials will be used for this database as for the
-main application database.
-
-This database type has the advantage of automatically scaling horizontally with
-your DBMS. However, it is marginally slower than the Filesystem assetstore type
-in a typical single-server use case.
-
 S3
 ^^
 
 This ``Assetstore`` type stores files in an **Amazon S3** bucket. You must
 provide the bucket name, an optional path prefix within the bucket, and
 authentication credentials for the bucket. When using this assetstore type,
 Girder acts as the broker for the data within S3 by authorizing the user agent
```

### Comparing `girder-3.2.3.dev7/girder/api/access.py` & `girder-5.0.0a2.dev10/girder/api/access.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/api_main.py` & `girder-5.0.0a2.dev10/girder/api/api_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
     def GET(self):
         # Since we only have v1 right now, just redirect to the v1 page.
         # If we get more versions, this should show an index of them.
         raise cherrypy.HTTPRedirect(cherrypy.url() + '/v1')
 
 
-def addApiToNode(node):
-    node.api = ApiDocs()
-    _addV1ToNode(node.api)
+def buildApi():
+    api = ApiDocs()
+    _addV1ToNode(api)
 
-    return node
+    return api
 
 
 def _addV1ToNode(node):
     node.v1 = describe.ApiDocs()
     node.v1.describe = describe.Describe()
 
     node.v1.api_key = api_key.ApiKey()
```

### Comparing `girder-3.2.3.dev7/girder/api/describe.py` & `girder-5.0.0a2.dev10/girder/api/describe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 import dateutil.parser
 from functools import wraps
 import inspect
 import jsonschema
 import os
 import cherrypy
 from collections import OrderedDict
+import logging
 
-from girder import constants, logprint
+from girder import constants
 from girder.api.rest import getCurrentUser, getBodyJson
 from girder.constants import SortDir, VERSION
 from girder.exceptions import RestException
 from girder.models.setting import Setting
 from girder.settings import SettingKey
-from girder.utility import config, toBool
+from girder.utility import toBool
 from girder.utility.model_importer import ModelImporter
 from girder.utility.webroot import WebrootBase
 from . import docs, access
 from .rest import Resource, getApiUrl, getUrlParts
 
 from inspect import signature, Parameter
 
 SWAGGER_VERSION = '2.0'
+logger = logging.getLogger(__name__)
 
 
 def _walkTree(node, path=()):
     # This will infinitely recurse if anything mounted under the API root
     # has a cyclical reference. That's bad.
     routeMap = {}
     for k, v in vars(node).items():
@@ -165,25 +167,25 @@
         dataTypeFormat = None
         if dataType in self._dataTypeMap:
             dataType, dataTypeFormat = self._dataTypeMap[dataType]
         # If we are dealing with the body then the dataType might be defined
         # by a schema added using addModel(...), we don't know for sure as we
         # don't know the resource name here to look it up.
         elif paramType != 'body':
-            logprint.warning(
+            logger.warning(
                 'WARNING: Invalid dataType "%s" specified for parameter names "%s"' %
                 (dataType, name))
 
         # Parameter Object spec:
         # Since the parameter is not located at the request body, it is limited
         # to simple types (that is, not an object).
         if paramType != 'body' and dataType not in (
                 'string', 'number', 'integer', 'long', 'boolean', 'array', 'file', 'float',
                 'double', 'date', 'dateTime'):
-            logprint.warning(
+            logger.warning(
                 'WARNING: Invalid dataType "%s" specified for parameter "%s"' % (dataType, name))
 
         if paramType == 'form':
             paramType = 'formData'
 
         return dataType, dataTypeFormat, paramType
 
@@ -443,25 +445,18 @@
 class ApiDocs(WebrootBase):
     """
     This serves up the Swagger page.
     """
 
     def __init__(self, templatePath=None):
         if not templatePath:
-            templatePath = os.path.join(constants.PACKAGE_DIR,
-                                        'api', 'api_docs.mako')
+            templatePath = os.path.join(constants.PACKAGE_DIR, 'api', 'api_docs.mako')
         super().__init__(templatePath)
 
-        curConfig = config.getConfig()
-        self.vars['mode'] = curConfig['server'].get('mode', '')
-
     def _renderHTML(self):
-        from girder.utility import server
-        self.vars['apiRoot'] = server.getApiRoot()
-        self.vars['staticPublicPath'] = server.getStaticPublicPath()
         self.vars['brandName'] = Setting().get(SettingKey.BRAND_NAME)
         return super()._renderHTML()
 
 
 class Describe(Resource):
     def __init__(self):
         super().__init__()
```

### Comparing `girder-3.2.3.dev7/girder/api/docs.py` & `girder-5.0.0a2.dev10/girder/api/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import collections
 import functools
+import logging
 
-from girder import logprint
-
+logger = logging.getLogger(__name__)
 models = collections.defaultdict(dict)
 # routes is dict of dicts of dicts
 # e.g. routes[resource][path][method]
 routes = collections.defaultdict(
     functools.partial(collections.defaultdict, dict))
 
 
@@ -140,11 +140,11 @@
     if resources:
         if isinstance(resources, str):
             resources = (resources,)
         for resource in resources:
             models[resource][name] = model
     else:
         if not silent:
-            logprint.warning(
+            logger.warning(
                 'WARNING: adding swagger models without specifying resources '
-                'to bind to is discouraged (%s).' % name)
+                'to bind to is discouraged (%s).', name)
         models[None][name] = model
```

### Comparing `girder-3.2.3.dev7/girder/api/filter_logging.py` & `girder-5.0.0a2.dev10/girder/api/filter_logging.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/rest.py` & `girder-5.0.0a2.dev10/girder/api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import html
 import cherrypy
 import collections
 import datetime
 from functools import wraps
 import inspect
 import json
+import logging
 import posixpath
 import pymongo
 import sys
 import traceback
 import types
 import unicodedata
 import urllib.parse
 import uuid
 import fnmatch
 
 from dogpile.cache.util import kwarg_function_key_generator
 
 from . import docs
-from girder import auditLogger, events, logger, logprint
+from girder import auditLogger, events
 from girder.constants import TokenScope, SortDir, ServerMode
 from girder.exceptions import AccessException, GirderException, ValidationException, RestException
 from girder.models.setting import Setting
 from girder.models.token import Token
 from girder.models.user import User
 from girder.settings import SettingKey
 from girder.utility import toBool, config, JsonEncoder, optionalArgumentDecorator
@@ -30,14 +31,15 @@
 from girder.utility.model_importer import ModelImporter
 
 
 # Arbitrary buffer length for stream-reading request bodies
 READ_BUFFER_LEN = 65536
 
 _MONGO_CURSOR_TYPES = (pymongo.cursor.Cursor, pymongo.command_cursor.CommandCursor)
+logger = logging.getLogger(__name__)
 
 
 def getUrlParts(url=None):
     """
     Calls `urllib.parse.urlparse`_ on a URL.
 
     :param url: A URL, or None to use the current request's URL.
@@ -62,23 +64,23 @@
 
     :param url: URL from which to extract the base URL. If not specified, uses
         the server root system setting. If that is not specified, uses `cherrypy.url()`
     :param preferReferer: if no url is specified, this is true, and this is in
         a cherrypy request that has a referer header that contains the api
         string, use that referer as the url.
     """
-    apiStr = config.getConfig()['server']['api_root']
+    apiStr = 'api/v1'
 
     if not url:
         if preferReferer and apiStr in cherrypy.request.headers.get('referer', ''):
             url = cherrypy.request.headers['referer']
         else:
             root = Setting().get(SettingKey.SERVER_ROOT)
             if root:
-                return posixpath.join(root, apiStr.lstrip('/'))
+                return posixpath.join(root, apiStr)
 
     url = url or cherrypy.url()
     idx = url.find(apiStr)
 
     if idx < 0:
         raise GirderException('Could not determine API root in %s.' % url)
 
@@ -781,17 +783,17 @@
         do so.
 
         In the past, Resource subclasses were not expected to call their
         superclass constructor.
         """
         if not hasattr(self, '_routes'):
             super().__init__()
-            logprint.warning(
+            logger.warning(
                 'WARNING: Resource subclass "%s" did not call '
-                '"Resource__init__()" from its constructor.' %
+                '"Resource__init__()" from its constructor.',
                 self.__class__.__name__)
 
     def route(self, method, route, handler, nodoc=False, resource=None):
         """
         Define a route for your REST resource.
 
         :param method: The HTTP method, e.g. 'GET', 'POST', 'PUT', 'PATCH'
@@ -832,24 +834,24 @@
         if hasattr(handler, 'description'):
             if handler.description is not None:
                 docs.addRouteDocs(
                     resource=resource, route=route, method=method,
                     info=handler.description.asDict(), handler=handler)
         elif not nodoc:
             routePath = '/'.join([resource] + list(route))
-            logprint.warning(
-                'WARNING: No description docs present for route %s %s' % (
-                    method, routePath))
+            logger.warning(
+                'WARNING: No description docs present for route %s %s',
+                method, routePath)
 
         # Warn if there is no access decorator on the handler function
         if not hasattr(handler, 'accessLevel'):
             routePath = '/'.join([resource] + list(route))
-            logprint.warning(
-                'WARNING: No access level specified for route %s %s' % (
-                    method, routePath))
+            logger.warning(
+                'WARNING: No access level specified for route %s %s',
+                method, routePath)
 
     def removeRoute(self, method, route, resource=None):
         """
         Remove a route from the handler and documentation.
 
         :param method: The HTTP method, e.g. 'GET', 'POST', 'PUT'
         :type method: str
@@ -1184,17 +1186,15 @@
         if token is None:
             token = Token().createToken(user, days=days, scope=scope)
 
         cookie = cherrypy.response.cookie
         cookie['girderToken'] = str(token['_id'])
         cookie['girderToken']['path'] = '/'
         cookie['girderToken']['expires'] = int(days * 3600 * 24)
-
-        if Setting().get(SettingKey.HTTP_ONLY_COOKIES):
-            cookie['girderToken']['httponly'] = True
+        cookie['girderToken']['httponly'] = True
 
         # CherryPy proxy tools modify the request.base, but not request.scheme, when receiving
         # X-Forwarded-Proto headers from a reverse proxy
         if cherrypy.request.scheme == 'https' or cherrypy.request.base.startswith('https'):
             cookie['girderToken']['secure'] = True
 
         return token
```

### Comparing `girder-3.2.3.dev7/girder/api/sftp.py` & `girder-5.0.0a2.dev10/girder/api/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from functools import wraps
+import logging
 import paramiko
 import socketserver
 import stat
 import time
 
-from girder import logger
 from girder.exceptions import AccessException, ValidationException, ResourcePathNotFound
 from girder.models.file import File
 from girder.models.folder import Folder
 from girder.models.item import Item
 from girder.models.user import User
 from girder.utility.path import lookUpPath
 from girder.utility.model_importer import ModelImporter
 
 MAX_BUF_LEN = 10 * 1024 * 1024
+logger = logging.getLogger(__name__)
 
 
 def _handleErrors(fun):
     @wraps(fun)
     def wrapped(*args, **kwargs):
         try:
             return fun(*args, **kwargs)
```

### Comparing `girder-3.2.3.dev7/girder/api/v1/api_key.py` & `girder-5.0.0a2.dev10/girder/api/v1/api_key.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/assetstore.py` & `girder-5.0.0a2.dev10/girder/api/v1/assetstore.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,17 +55,14 @@
         Description('Create a new assetstore.')
         .responseClass('Assetstore')
         .notes('You must be an administrator to call this.')
         .param('name', 'Unique name for the assetstore.')
         .param('type', 'Type of the assetstore.', dataType='integer')
         .param('root', 'Root path on disk (for filesystem type).', required=False)
         .param('perms', 'File creation permissions (for filesystem type).', required=False)
-        .param('db', 'Database name (for GridFS type)', required=False)
-        .param('mongohost', 'Mongo host URI (for GridFS type)', required=False)
-        .param('replicaset', 'Replica set name (for GridFS type)', required=False)
         .param('bucket', 'The S3 bucket to store data in (for S3 type).', required=False)
         .param('prefix', 'Optional path prefix within the bucket under which '
                'files will be stored (for S3 type).', required=False, default='')
         .param('accessKeyId', 'The AWS access key ID to use for authentication '
                '(for S3 type).', required=False)
         .param('secret', 'The AWS secret key to use for authentication (for '
                'S3 type).', required=False)
@@ -81,25 +78,21 @@
                'by Boto rather than explicitly passed. Inferring credentials will '
                'ignore accessKeyId and secret.', dataType='boolean', required=False)
         .param('serverSideEncryption', 'Whether to use S3 SSE to encrypt the objects uploaded to '
                'this bucket (for S3 type).', dataType='boolean', required=False, default=False)
         .errorResponse()
         .errorResponse('You are not an administrator.', 403)
     )
-    def createAssetstore(self, name, type, root, perms, db, mongohost, replicaset, bucket,
+    def createAssetstore(self, name, type, root, perms, bucket,
                          prefix, accessKeyId, secret, service, readOnly, region, inferCredentials,
                          serverSideEncryption):
         if type == AssetstoreType.FILESYSTEM:
             self.requireParams({'root': root})
             return self._model.createFilesystemAssetstore(
                 name=name, root=root, perms=perms)
-        elif type == AssetstoreType.GRIDFS:
-            self.requireParams({'db': db})
-            return self._model.createGridFsAssetstore(
-                name=name, db=db, mongohost=mongohost, replicaset=replicaset)
         elif type == AssetstoreType.S3:
             self.requireParams({'bucket': bucket})
             return self._model.createS3Assetstore(
                 name=name, bucket=bucket, prefix=prefix, secret=secret,
                 accessKeyId=accessKeyId, service=service, readOnly=readOnly, region=region,
                 inferCredentials=inferCredentials, serverSideEncryption=serverSideEncryption)
         else:
@@ -149,17 +142,14 @@
     @autoDescribeRoute(
         Description('Update an existing assetstore.')
         .responseClass('Assetstore')
         .modelParam('id', model=AssetstoreModel)
         .param('name', 'Unique name for the assetstore.', strip=True)
         .param('root', 'Root path on disk (for Filesystem type)', required=False)
         .param('perms', 'File creation permissions (for Filesystem type)', required=False)
-        .param('db', 'Database name (for GridFS type)', required=False)
-        .param('mongohost', 'Mongo host URI (for GridFS type)', required=False)
-        .param('replicaset', 'Replica set name (for GridFS type)', required=False)
         .param('bucket', 'The S3 bucket to store data in (for S3 type).', required=False)
         .param('prefix', 'Optional path prefix within the bucket under which '
                'files will be stored (for S3 type).', required=False, default='')
         .param('accessKeyId', 'The AWS access key ID to use for authentication '
                '(for S3 type).', required=False)
         .param('secret', 'The AWS secret key to use for authentication (for '
                'S3 type).', required=False)
@@ -176,32 +166,25 @@
                'by Boto rather than explicitly passed. Inferring credentials will '
                'ignore accessKeyId and secret.', dataType='boolean', required=False)
         .param('serverSideEncryption', 'Whether to use S3 SSE to encrypt the objects uploaded to '
                'this bucket (for S3 type).', dataType='boolean', required=False, default=False)
         .errorResponse()
         .errorResponse('You are not an administrator.', 403)
     )
-    def updateAssetstore(self, assetstore, name, root, perms, db, mongohost, replicaset,
+    def updateAssetstore(self, assetstore, name, root, perms,
                          bucket, prefix, accessKeyId, secret, service, readOnly, region, current,
                          inferCredentials, serverSideEncryption, params):
         assetstore['name'] = name
         assetstore['current'] = current
 
         if assetstore['type'] == AssetstoreType.FILESYSTEM:
             self.requireParams({'root': root})
             assetstore['root'] = root
             if perms is not None:
                 assetstore['perms'] = perms
-        elif assetstore['type'] == AssetstoreType.GRIDFS:
-            self.requireParams({'db': db})
-            assetstore['db'] = db
-            if mongohost is not None:
-                assetstore['mongohost'] = mongohost
-            if replicaset is not None:
-                assetstore['replicaset'] = replicaset
         elif assetstore['type'] == AssetstoreType.S3:
             self.requireParams({
                 'bucket': bucket
             })
             assetstore['bucket'] = bucket
             assetstore['prefix'] = prefix
             assetstore['accessKeyId'] = accessKeyId
@@ -213,17 +196,16 @@
             if readOnly is not None:
                 assetstore['readOnly'] = readOnly
         else:
             event = events.trigger('assetstore.update', info={
                 'assetstore': assetstore,
                 'params': dict(
                     name=name, current=current, readOnly=readOnly, root=root, perms=perms,
-                    db=db, mongohost=mongohost, replicaset=replicaset, bucket=bucket,
-                    prefix=prefix, accessKeyId=accessKeyId, secret=secret, service=service,
-                    region=region, **params
+                    bucket=bucket, prefix=prefix, accessKeyId=accessKeyId, secret=secret,
+                    service=service, region=region, **params
                 )
             })
             if event.defaultPrevented:
                 return
         return self._model.save(assetstore)
 
     @access.admin
```

### Comparing `girder-3.2.3.dev7/girder/api/v1/collection.py` & `girder-5.0.0a2.dev10/girder/api/v1/collection.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/file.py` & `girder-5.0.0a2.dev10/girder/api/v1/file.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/folder.py` & `girder-5.0.0a2.dev10/girder/api/v1/folder.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/group.py` & `girder-5.0.0a2.dev10/girder/api/v1/group.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/item.py` & `girder-5.0.0a2.dev10/girder/api/v1/item.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/notification.py` & `girder-5.0.0a2.dev10/girder/api/v1/notification.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/resource.py` & `girder-5.0.0a2.dev10/girder/api/v1/resource.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/system.py` & `girder-5.0.0a2.dev10/girder/api/v1/system.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,76 @@
 import cherrypy
 import datetime
 import errno
-import girder
+from functools import lru_cache
+from itertools import chain
 import json
-import os
 import logging
 
 from girder import plugin
 from girder.api import access
 from girder.constants import TokenScope, ACCESS_FLAGS, VERSION
 from girder.exceptions import GirderException, ResourcePathNotFound
 from girder.models.collection import Collection
 from girder.models.file import File
 from girder.models.folder import Folder
 from girder.models.group import Group
 from girder.models.item import Item
 from girder.models.setting import Setting
 from girder.models.upload import Upload
 from girder.models.user import User
+from girder.plugin import getPluginStaticContent
 from girder.settings import SettingKey
 from girder.utility import config, system
 from girder.utility.progress import ProgressContext
 from ..describe import Description, autoDescribeRoute
 from ..rest import Resource
 
 ModuleStartTime = datetime.datetime.utcnow()
 LOG_BUF_SIZE = 65536
+logger = logging.getLogger(__name__)
 
 
 class System(Resource):
     """
     The system endpoints are for querying and managing system-wide properties.
     """
 
     def __init__(self):
         super().__init__()
         self.resourceName = 'system'
         self.route('DELETE', ('setting',), self.unsetSetting)
         self.route('GET', ('version',), self.getVersion)
         self.route('GET', ('configuration',), self.getConfigurationOption)
         self.route('GET', ('setting',), self.getSetting)
+        self.route('GET', ('public_settings',), self.getPublicSettings)
         self.route('GET', ('plugins',), self.getPlugins)
+        self.route('GET', ('plugin_static_files',), self.getPluginStaticFiles)
         self.route('GET', ('access_flag',), self.getAccessFlags)
         self.route('PUT', ('setting',), self.setSetting)
         self.route('GET', ('uploads',), self.getPartialUploads)
         self.route('DELETE', ('uploads',), self.discardPartialUploads)
         self.route('GET', ('check',), self.systemStatus)
         self.route('PUT', ('check',), self.systemConsistencyCheck)
-        self.route('GET', ('log',), self.getLog)
-        self.route('GET', ('log', 'level'), self.getLogLevel)
-        self.route('PUT', ('log', 'level'), self.setLogLevel)
         self.route('GET', ('setting', 'collection_creation_policy', 'access'),
                    self.getCollectionCreationPolicyAccess)
 
+    @access.public
+    @autoDescribeRoute(
+        Description('Get the list of plugin static files to be injected into the Girder app.'),
+        hide=True,
+    )
+    @lru_cache(maxsize=1)  # this serves data that is immutable after server startup
+    def getPluginStaticFiles(self):
+        contentObjects = list(getPluginStaticContent().values())
+        return {
+            'css': list(chain(*[content.css for content in contentObjects])),
+            'js': list(chain(*[content.js for content in contentObjects])),
+        }
+
     @access.admin
     @autoDescribeRoute(
         Description('Set the value for a system setting, or a list of them.')
         .notes('Must be a system administrator to call this. If the value passed is '
                'a valid JSON object, it will be parsed and stored as an object.')
         .param('key', 'The key identifying this setting.', required=False, paramType='formData')
         .param('value', 'The value for this setting.', required=False, paramType='formData')
@@ -116,14 +130,29 @@
     def getSetting(self, key, list):
         if list is not None:
             return {k: Setting().get(k) for k in list}
         else:
             self.requireParams({'key': key})
             return Setting().get(key)
 
+    @access.public()
+    @autoDescribeRoute(
+        Description('Get publicly accessible settings.')
+    )
+    def getPublicSettings(self):
+        publicSettings = [
+            SettingKey.BRAND_NAME,
+            SettingKey.CONTACT_EMAIL_ADDRESS,
+            SettingKey.PRIVACY_NOTICE,
+            SettingKey.BANNER_COLOR,
+            SettingKey.REGISTRATION_POLICY,
+            SettingKey.ENABLE_PASSWORD_LOGIN,
+        ]
+        return {k: Setting().get(k) for k in publicSettings}
+
     @access.admin(scope=TokenScope.PLUGINS_READ)
     @autoDescribeRoute(
         Description('Get the lists of all available and all loaded plugins.')
         .notes('Must be a system administrator to call this.')
         .errorResponse('You are not a system administrator.', 403)
     )
     def getPlugins(self):
@@ -201,16 +230,15 @@
             try:
                 untrackedList = Upload().untrackedUploads('list', assetstoreId)
                 if limit == 0:
                     uploadList += untrackedList
                 elif len(uploadList) < limit:
                     uploadList += untrackedList[:limit - len(uploadList)]
             except Exception:
-                girder.logger.debug(
-                    'Could not get untracked uploads for assetstore %s', assetstoreId)
+                logger.debug('Could not get untracked uploads for assetstore %s', assetstoreId)
         return uploadList
 
     @access.admin(scope=TokenScope.PARTIAL_UPLOAD_CLEAN)
     @autoDescribeRoute(
         Description('Discard uploads that have not been finished.')
         .notes('Must be a system administrator to call this. This frees '
                'resources that were allocated for the uploads and clears the '
@@ -256,16 +284,15 @@
                         'Failed to delete upload.',
                         'girder.api.v1.system.delete-upload-failed')
                 raise
         if includeUntracked:
             try:
                 uploadList += Upload().untrackedUploads('delete', assetstoreId)
             except Exception:
-                girder.logger.debug(
-                    'Could not delete untracked uploads for assetstore %s', assetstoreId)
+                logger.debug('Could not delete untracked uploads for assetstore %s', assetstoreId)
         return uploadList
 
     @access.public
     @autoDescribeRoute(
         Description('Report the current system status.')
         .notes('Must be a system administrator to call this with any mode '
                'other than basic.')
@@ -317,93 +344,18 @@
         # * check that all folders have a valid ancestor tree leading to a
         #   user or collection
         # * check that all folders have the correct baseParentId and
         #   baseParentType
         # * check that all groups contain valid users
         # * check that all resources validate
         # * for filesystem assetstores, find files that are not tracked.
-        # * for gridfs assetstores, find chunks that are not tracked.
         # * for s3 assetstores, find elements that are not tracked.
 
     @access.admin
     @autoDescribeRoute(
-        Description('Show the most recent contents of the server logs.')
-        .notes('Must be a system administrator to call this.')
-        .param('bytes', 'Controls how many bytes (from the end of the log) to show. '
-               'Pass 0 to show the whole log.', dataType='integer', required=False, default=4096)
-        .param('log', 'Which log to tail.', enum=('error', 'info'),
-               required=False, default='error')
-        .errorResponse('You are not a system administrator.', 403)
-    )
-    def getLog(self, bytes, log):
-        path = girder.getLogPaths()[log]
-        filesize = os.path.getsize(path)
-        length = int(bytes) or filesize
-        filesize1 = 0
-        if length > filesize:
-            path1 = path + '.1'
-            if os.path.exists(path1):
-                filesize1 = os.path.getsize(path1)
-
-        def stream():
-            yield '=== Last %d bytes of %s: ===\n\n' % (
-                min(length, filesize + filesize1), path
-            )
-
-            readlength = length
-            if readlength > filesize and filesize1:
-                readlength = length - filesize
-                with open(path1, 'rb') as f:
-                    if readlength < filesize1:
-                        f.seek(-readlength, os.SEEK_END)
-                    while True:
-                        data = f.read(LOG_BUF_SIZE)
-                        if not data:
-                            break
-                        yield data
-                readlength = filesize
-            with open(path, 'rb') as f:
-                if readlength < filesize:
-                    f.seek(-readlength, os.SEEK_END)
-                while True:
-                    data = f.read(LOG_BUF_SIZE)
-                    if not data:
-                        break
-                    yield data
-        return stream
-
-    @access.admin
-    @autoDescribeRoute(
-        Description('Get the current log level.')
-        .notes('Must be a system administrator to call this.')
-        .errorResponse('You are not a system administrator.', 403)
-    )
-    def getLogLevel(self):
-        level = girder.logger.getEffectiveLevel()
-        return logging.getLevelName(level)
-
-    @access.admin
-    @autoDescribeRoute(
-        Description('Set the current log level.')
-        .notes('Must be a system administrator to call this.')
-        .param('level', 'The new level to set.',
-               enum=['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG'],
-               default='INFO')
-        .errorResponse('You are not a system administrator.', 403)
-    )
-    def setLogLevel(self, level):
-        level = logging.getLevelName(level)
-        for logger in (girder.logger, cherrypy.log.access_log, cherrypy.log.error_log):
-            logger.setLevel(level)
-            for handler in logger.handlers:
-                handler.setLevel(level)
-        return logging.getLevelName(level)
-
-    @access.admin
-    @autoDescribeRoute(
         Description('Get access of content creation policy.')
         .notes('Get result in the same structure as the access endpoints '
                'of collection, file, and group')
     )
     def getCollectionCreationPolicyAccess(self):
         cpp = Setting().get(SettingKey.COLLECTION_CREATE_POLICY)
```

### Comparing `girder-3.2.3.dev7/girder/api/v1/token.py` & `girder-5.0.0a2.dev10/girder/api/v1/token.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/api/v1/user.py` & `girder-5.0.0a2.dev10/girder/api/v1/user.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/cli/mount.py` & `girder-5.0.0a2.dev10/girder/cli/mount.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 import time
 
 import cachetools
 import cherrypy
 import click
 import fuse
 
-import girder
-from girder import events, logger, logprint
+from girder import events, plugin
+from girder.constants import ServerMode
 from girder.exceptions import AccessException, FilePathException, ValidationException
 from girder.models.file import File
 from girder.models.folder import Folder
 from girder.models.item import Item
 from girder.models.setting import Setting
 from girder.settings import SettingKey
-from girder.utility import config
 from girder.utility import path as path_util
 from girder.utility.model_importer import ModelImporter
-from girder.utility.server import configureServer
+from girder.utility.server import create_app
+
+logger = logging.getLogger(__name__)
 
 
 class ServerFuse(fuse.Operations):
     """
     This class handles FUSE operations that are non-default.  It exposes the
     Girder resources via the resource path in a read-only manner.  It could be
     extended to expose metadata and other resources by extending the available
@@ -453,23 +454,22 @@
 class FUSELogError(fuse.FUSE):
     def __init__(self, operations, mountpoint, *args, **kwargs):
         """
         This wraps fuse.FUSE so that errors are logged rather than raising a
         RuntimeError exception.
         """
         try:
-            logger.debug('Mounting %s\n' % mountpoint)
+            logger.debug('Mounting %s\n', mountpoint)
             super().__init__(operations, mountpoint, *args, **kwargs)
-            logger.debug('Mounted %s\n' % mountpoint)
+            logger.debug('Mounted %s\n', mountpoint)
         except RuntimeError:
-            logprint.error(
+            logger.error(
                 'Failed to mount FUSE.  Does the mountpoint (%r) exist and is '
                 'it empty?  Does the user have permission to create FUSE '
-                'mounts?  It could be another FUSE mount issue, too.' % (
-                    mountpoint, ))
+                'mounts?  It could be another FUSE mount issue, too.', mountpoint)
             Setting().unset(SettingKey.GIRDER_MOUNT_INFORMATION)
 
 
 def unmountServer(path, lazy=False, quiet=False):
     """
     Unmount a specified path, if possible.
 
@@ -552,28 +552,25 @@
         case insensitive.  For instance, 'foreground' or 'foreground=True' will
         keep this program running until the SIGTERM or unmounted.
     :param quiet: if True, suppress Girder logs.
     :param verbose: if not zero, log to stderr instead of the girder logs.
     :param plugins: an optional list of plugins to enable.  If None, use the
         plugins that are configured.
     """
-    if quiet or verbose:
-        curConfig = config.getConfig()
-        curConfig.setdefault('logging', {})['log_quiet'] = True
-        curConfig.setdefault('logging', {})['log_level'] = 'FATAL'
-        girder._attachFileLogHandlers()
-        if verbose:
-            logger.setLevel(max(1, logging.ERROR - verbose * 10))
-            logger.addHandler(logging.StreamHandler())
+    if verbose:
+        logger.setLevel(max(1, logging.ERROR - verbose * 10))
+    if not quiet:
+        logger.addHandler(logging.StreamHandler())
     if database and '://' in database:
         cherrypy.config['database']['uri'] = database
     if plugins is not None:
         plugins = plugins.split(',')
-    webroot, appconf = configureServer(plugins=plugins)
-    girder._setupCache()
+
+    app_info = create_app(ServerMode.DEVELOPMENT)
+    plugin._loadPlugins(app_info, names=plugins)
 
     options = {
         # By default, we run in the background so the mount command returns
         # immediately.  If we run in the foreground, a SIGTERM will shut it
         # down
         'foreground': False,
         # Cache files if their size and timestamp haven't changed.
@@ -592,15 +589,15 @@
             if '=' in opt:
                 key, value = opt.split('=', 1)
                 value = (False if value.lower() == 'false' else
                          True if value.lower() == 'true' else value)
             else:
                 key, value = opt, True
             if key in ('ro', 'rw') and options.get(key) != value:
-                logprint.warning('Ignoring the %s=%r option' % (key, value))
+                logger.warning('Ignoring the %s=%r option', key, value)
                 continue
             options[key] = value
     opClass = ServerFuse(stat=os.stat(path), options=options)
     Setting().set(SettingKey.GIRDER_MOUNT_INFORMATION,
                   {'path': path, 'mounttime': time.time()})
     FUSELogError(opClass, path, **options)
```

### Comparing `girder-3.2.3.dev7/girder/cli/sftpd.py` & `girder-5.0.0a2.dev10/girder/cli/sftpd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import click
+import logging
 import os
 import paramiko
 import sys
 
-from girder import logprint
 from girder.api.sftp import SftpServer
 
 DEFAULT_PORT = 8022
+logger = logging.getLogger(__name__)
 
 
 @click.command(name='sftpd', short_help='Run the Girder SFTP service.',
                help='Run the Girder SFTP service.')
 @click.option('-i', '--identity-file', show_default=True,
               default=os.path.expanduser(os.path.join('~', '.ssh', 'id_rsa')),
               help='The identity (private key) file to use')
@@ -22,18 +23,17 @@
     """
     This is the entrypoint of the girder sftpd program. It should not be
     called from python code.
     """
     try:
         hostKey = paramiko.RSAKey.from_private_key_file(identity_file)
     except paramiko.ssh_exception.PasswordRequiredException:
-        logprint.error(
-            'Error: encrypted key files are not supported (%s).' % identity_file, file=sys.stderr)
+        logger.error('Error: encrypted key files are not supported (%s).', identity_file)
         sys.exit(1)
 
     server = SftpServer((host, port), hostKey)
-    logprint.info('Girder SFTP service listening on %s:%d.' % (host, port))
+    logger.info('Girder SFTP service listening on %s:%d.', host, port)
 
     try:
         server.serve_forever()
     except (SystemExit, KeyboardInterrupt):
         server.server_close()
```

### Comparing `girder-3.2.3.dev7/girder/cli/shell.py` & `girder-5.0.0a2.dev10/girder/cli/shell.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import click
 import girder
 import sys
 
-from girder.utility.server import configureServer
+from girder import constants, plugin
+from girder.utility.server import create_app
 
 
 def _launchShell(context):
     """
     Launches a Python shell with the given context.
 
     :param context: A dictionary containing key value pairs
@@ -29,20 +30,21 @@
 @click.option('--plugins', default=None, help='Comma separated list of plugins to import.')
 @click.argument('script', type=click.Path(exists=True, dir_okay=False), required=False)
 @click.argument('args', nargs=-1, required=False)
 def main(plugins, script, args):
     if plugins is not None:
         plugins = plugins.split(',')
 
-    webroot, appconf = configureServer(plugins=plugins)
+    app_info = create_app(constants.ServerMode.DEVELOPMENT)
+    plugin._loadPlugins(app_info, plugins)
 
     if script is None:
         _launchShell({
-            'webroot': webroot,
-            'appconf': appconf
+            'webroot': app_info['serverRoot'],
+            'appconf': app_info['config'],
         })
     else:
         globals_ = {k: v for k, v in globals().items() if k not in {'__file__', '__name__'}}
         sys.argv = [script] + list(args)
         exec(open(script, 'rb').read(), dict(
-            webroot=webroot, appconf=appconf, __name__='__main__',
+            webroot=app_info['serverRoot'], appconf=app_info['config'], __name__='__main__',
             __file__=script, **globals_))
```

### Comparing `girder-3.2.3.dev7/girder/constants.py` & `girder-5.0.0a2.dev10/girder/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 """
 Constants should be defined here.
 """
 import os
-import sys
 
 import girder
 
+# TODO turn all these into pathlib.Paths
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 ROOT_DIR = os.path.dirname(PACKAGE_DIR)
-LOG_ROOT = os.path.join(os.path.expanduser('~'), '.girder', 'logs')
-MAX_LOG_SIZE = 1024 * 1024 * 10  # Size in bytes before logs are rotated.
-LOG_BACKUP_COUNT = 5
 ACCESS_FLAGS = {}
 
-# Identifier for Girder's entry in the route table
-GIRDER_ROUTE_ID = 'core_girder'
-
 # Threshold below which text search results will be sorted by their text score.
 # Setting this too high causes mongodb to use too many resources for searches
 # that yield lots of results.
 TEXT_SCORE_SORT_MAX = 200
 VERSION = {
     'release': girder.__version__
 }
 
 #: The local directory containing the static content.
-STATIC_PREFIX = os.path.join(sys.prefix, 'share', 'girder')
-STATIC_ROOT_DIR = os.path.join(STATIC_PREFIX, 'static')
+STATIC_ROOT_DIR = os.path.join(PACKAGE_DIR, 'web', 'dist')
 
 
 def registerAccessFlag(key, name, description=None, admin=False):
     """
     Register a new access flag in the set of ACCESS_FLAGS available
     on data in the hierarchy. These are boolean switches that can be used
     to control access to specific functionality on specific resoruces.
@@ -55,53 +48,20 @@
 
 class ServerMode:
     PRODUCTION = 'production'
     DEVELOPMENT = 'development'
     TESTING = 'testing'
 
 
-class TerminalColor:
-    """
-    Provides a set of values that can be used to color text in the terminal.
-    """
-
-    ERROR = '\033[1;91m'
-    SUCCESS = '\033[32m'
-    WARNING = '\033[1;33m'
-    INFO = '\033[35m'
-    ENDC = '\033[0m'
-
-    @staticmethod
-    def _color(tag, text):
-        return ''.join([tag, text, TerminalColor.ENDC])
-
-    @staticmethod
-    def error(text):
-        return TerminalColor._color(TerminalColor.ERROR, text)
-
-    @staticmethod
-    def success(text):
-        return TerminalColor._color(TerminalColor.SUCCESS, text)
-
-    @staticmethod
-    def warning(text):
-        return TerminalColor._color(TerminalColor.WARNING, text)
-
-    @staticmethod
-    def info(text):
-        return TerminalColor._color(TerminalColor.INFO, text)
-
-
 class AssetstoreType:
     """
     All possible assetstore implementation types.
     """
 
     FILESYSTEM = 0
-    GRIDFS = 1
     S3 = 2
 
 
 class AccessType:
     """
     Represents the level of access granted to a user or group on an
     AccessControlledModel. Having a higher access level on a resource also
@@ -254,10 +214,7 @@
     GROUP_CREATOR_ACCESS = 'core.grantCreatorAccess'
 
     # For creating the default Public and Private folders at user creation time.
     USER_DEFAULT_FOLDERS = 'core.addDefaultFolders'
 
     # For adding a user into its own ACL.
     USER_SELF_ACCESS = 'core.grantSelfAccess'
-
-    # For updating the cached webroot HTML when settings change.
-    WEBROOT_SETTING_CHANGE = 'core.updateWebrootSettings'
```

### Comparing `girder-3.2.3.dev7/girder/exceptions.py` & `girder-5.0.0a2.dev10/girder/exceptions.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/models/__init__.py` & `girder-5.0.0a2.dev10/girder/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import logging
 import pymongo
 import urllib.parse
 
-from girder import logprint
 from girder.utility import config
 
 _dbClients = {}
+logger = logging.getLogger(__name__)
 
 
 def getDbConfig():
     """Get the database configuration values from the cherrypy config."""
     cfg = config.getConfig()
     if 'database' in cfg:
         return cfg['database']
@@ -22,15 +23,15 @@
     We lazy-instantiate a module-level singleton, the MongoClient objects
     manage their own connection pools internally. Any extra kwargs you pass to
     this method will be passed through to the MongoClient.
 
     :param uri: if specified, connect to this mongo db rather than the one in
                 the config.
     :param replicaSet: if uri is specified, use this replica set.
-    :param quiet: if true, don't logprint warnings and success.
+    :param quiet: if true, don't log warnings and success.
     :type quiet: bool
     """
     global _dbClients
 
     origKey = (uri, replicaSet)
     if origKey in _dbClients:
         return _dbClients[origKey]
@@ -69,16 +70,15 @@
     for key in uriParams:
         if key in clientOptions:
             del clientOptions[key]
 
     if uri is None:
         dbUriRedacted = 'mongodb://localhost:27017/girder'
         if not quiet:
-            logprint.warning('WARNING: No MongoDB URI specified, using '
-                             'the default value')
+            logger.warning('WARNING: No MongoDB URI specified, using the default value')
 
         client = pymongo.MongoClient(dbUriRedacted, **clientOptions)
     else:
         parts = uri.split('@')
         if len(parts) == 2:
             dbUriRedacted = 'mongodb://' + parts[1]
         else:
@@ -86,15 +86,15 @@
 
         client = pymongo.MongoClient(uri, **clientOptions)
 
     if not quiet:
         desc = ''
         if replicaSet:
             desc += ', replica set: %s' % replicaSet
-        logprint.info('Connecting to MongoDB: %s%s' % (dbUriRedacted, desc))
+        logger.info('Connecting to MongoDB: %s%s', dbUriRedacted, desc)
 
     # Make sure we can connect to the mongo server at startup
     client.server_info()
 
     _dbClients[origKey] = _dbClients[(uri, replicaSet)] = client
 
     return client
```

### Comparing `girder-3.2.3.dev7/girder/models/api_key.py` & `girder-5.0.0a2.dev10/girder/models/api_key.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/models/assetstore.py` & `girder-5.0.0a2.dev10/girder/models/assetstore.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,25 +115,14 @@
             'type': AssetstoreType.FILESYSTEM,
             'created': datetime.datetime.utcnow(),
             'name': name,
             'root': root,
             'perms': perms
         })
 
-    def createGridFsAssetstore(self, name, db, mongohost=None,
-                               replicaset=None):
-        return self.save({
-            'type': AssetstoreType.GRIDFS,
-            'created': datetime.datetime.utcnow(),
-            'name': name,
-            'db': db,
-            'mongohost': mongohost,
-            'replicaset': replicaset
-        })
-
     def createS3Assetstore(self, name, bucket, accessKeyId, secret, prefix='',
                            service='', readOnly=False, region=None, inferCredentials=False,
                            serverSideEncryption=False):
         return self.save({
             'type': AssetstoreType.S3,
             'created': datetime.datetime.utcnow(),
             'name': name,
```

### Comparing `girder-3.2.3.dev7/girder/models/collection.py` & `girder-5.0.0a2.dev10/girder/models/collection.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/models/file.py` & `girder-5.0.0a2.dev10/girder/models/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import cherrypy
 import datetime
+import logging
 import os
 
 from .model_base import Model, AccessControlledModel
-import girder
 from girder import auditLogger, events
 from girder.constants import AccessType, CoreEventHandler
 from girder.exceptions import FilePathException, ValidationException
 from girder.models.setting import Setting
 from girder.settings import SettingKey
 from girder.utility import acl_mixin, path as path_util
 from girder.utility.model_importer import ModelImporter
 
+logger = logging.getLogger(__name__)
+
 
 class File(acl_mixin.AccessControlMixin, Model):
     """
     This model represents a File, which is stored in an assetstore.
     """
 
     def initialize(self):
@@ -58,16 +60,16 @@
         if file['itemId']:
             item = Item().load(file['itemId'], force=True)
             if item is not None:
                 # files that are linkUrls might not have a size field
                 if file.get('size') is not None:
                     self.propagateSizeChange(item, -file['size'], updateItemSize)
             else:
-                girder.logger.warning('Broken reference in file %s: no item %s exists' %
-                                      (file['_id'], file['itemId']))
+                logger.warning(
+                    'Broken reference in file %s: no item %s exists', file['_id'], file['itemId'])
 
         super().remove(file)
 
     def download(self, file, offset=0, headers=True, endByte=None,
                  contentDisposition=None, extraParameters=None):
         """
         Use the appropriate assetstore adapter for whatever assetstore the
```

### Comparing `girder-3.2.3.dev7/girder/models/folder.py` & `girder-5.0.0a2.dev10/girder/models/folder.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/models/group.py` & `girder-5.0.0a2.dev10/girder/models/group.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/models/item.py` & `girder-5.0.0a2.dev10/girder/models/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import copy
 import datetime
 import json
+import logging
 import os
 
 from bson.objectid import ObjectId
 from .model_base import Model
 from girder import events
-from girder import logger
 from girder.constants import AccessType
 from girder.exceptions import ValidationException, GirderException
 from girder.utility import acl_mixin
 from girder.utility.model_importer import ModelImporter
 
+logger = logging.getLogger(__name__)
+
 
 class Item(acl_mixin.AccessControlMixin, Model):
     """
     Items are leaves in the data hierarchy. They can contain 0 or more
     files within them, and can also contain arbitrary metadata.
     """
 
@@ -178,16 +180,18 @@
         for file in self.childFiles(item):
             # We could add a recalculateSize to the file model, in which case
             # this would be:
             # size += File().recalculateSize(file)
             size += file.get('size', 0)
         delta = size - item.get('size', 0)
         if delta:
-            logger.info('Item %s was wrong size: was %d, is %d' % (
-                item['_id'], item['size'], size))
+            logger.info(
+                'Item %s was wrong size: was %d, is %d',
+                item['_id'], item['size'], size
+            )
             item['size'] = size
             self.update({'_id': item['_id']}, update={'$set': {'size': size}})
             self.propagateSizeChange(item, delta)
         return size
 
     def childFiles(self, item, limit=0, offset=0, sort=None, **kwargs):
         """
```

### Comparing `girder-3.2.3.dev7/girder/models/model_base.py` & `girder-5.0.0a2.dev10/girder/models/model_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import copy
 import functools
 import itertools
+import logging
 import os
 import pymongo
 import re
 
 from bson.objectid import ObjectId
 from bson.errors import InvalidId
 from pymongo.errors import WriteError
-from girder import events, logprint, logger, auditLogger
+from girder import events, auditLogger
 from girder.constants import AccessType, CoreEventHandler, ACCESS_FLAGS, TEXT_SCORE_SORT_MAX
 from girder.models import getDbConnection
 from girder.exceptions import AccessException, ValidationException
 
 # pymongo3 complains about extra kwargs to find(), so we must filter them.
 _allowedFindArgs = ('cursor_type', 'allow_partial_results', 'oplog_replay',
                     'modifiers', 'manipulate')
 # This list is only used for testing, where we must reconnect() all models after
 # the database is dropped between each test case. If we find a cleverer way to do
 # that, we don't need to store these here.
 _modelSingletons = []
+logger = logging.getLogger(__name__)
 
 if 'GIRDER_MAX_CURSOR_TIMEOUT_MS' in os.environ:
     _MAX_CURSOR_TIMEOUT_MS = int(os.environ['GIRDER_MAX_CURSOR_TIMEOUT_MS'])
 else:
     _MAX_CURSOR_TIMEOUT_MS = None
 
 
@@ -123,15 +125,15 @@
         if isinstance(self._textIndex, dict):
             textIdx = [(k, 'text') for k in self._textIndex.keys()]
             try:
                 self.collection.create_index(
                     textIdx, weights=self._textIndex,
                     default_language=self._textLanguage)
             except pymongo.errors.OperationFailure:
-                logprint.warning('WARNING: Text search not enabled.')
+                logger.warning('WARNING: Text search not enabled.')
 
         self._connected = True
 
     def exposeFields(self, level, fields):
         """
         Expose model fields to users with the given access level. Subclasses
         should call this in their initialize method to declare what fields
```

### Comparing `girder-3.2.3.dev7/girder/models/notification.py` & `girder-5.0.0a2.dev10/girder/models/notification.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/models/setting.py` & `girder-5.0.0a2.dev10/girder/models/setting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import json
+import logging
 import os
 
 import pymongo
 
 from .model_base import Model
-from girder import logprint
 from girder.exceptions import ValidationException
 from girder.settings import SettingDefault
 from girder.utility import setting_utilities
 from girder.utility._cache import cache
 
+logger = logging.getLogger(__name__)
+
 
 class Setting(Model):
     """
     This model represents server-wide configuration settings as key/value pairs.
     """
 
     def initialize(self):
@@ -50,17 +52,15 @@
             duplicates = self.collection.aggregate([{
                 '$group': {'_id': '$key',
                            'key': {'$first': '$key'},
                            'ids': {'$addToSet': '$_id'},
                            'count': {'$sum': 1}}}, {
                 '$match': {'count': {'$gt': 1}}}])
             for duplicate in duplicates:
-                logprint.warning(
-                    'Removing duplicate setting with key %s.' % (
-                        duplicate['key']))
+                logger.warning('Removing duplicate setting with key %s.', duplicate['key'])
                 # Remove all of the duplicates.  Keep the item with the lowest
                 # id in Mongo.
                 for duplicateId in sorted(duplicate['ids'])[1:]:
                     self.collection.delete_one({'_id': duplicateId})
             self.collection.create_index('key', unique=True)
 
     def validate(self, doc):
```

### Comparing `girder-3.2.3.dev7/girder/models/token.py` & `girder-5.0.0a2.dev10/girder/models/token.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/models/upload.py` & `girder-5.0.0a2.dev10/girder/models/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import datetime
 import io
+import logging
 from bson.objectid import ObjectId
 
-from girder import events, logger
+from girder import events
 from girder.api import rest
 from .model_base import Model
 from girder.exceptions import GirderException, ValidationException, NoAssetstoreAdapter
 from girder.settings import SettingKey
 from girder.utility import RequestBodyStream
 from girder.utility.model_importer import ModelImporter
 from girder.utility.progress import noProgress
 
+logger = logging.getLogger(__name__)
+
 
 class Upload(Model):
     """
     This model stores temporary records for uploads that have been approved
     but are not yet complete, so that they can be uploaded in chunks of
     arbitrary size. The chunks must be uploaded in order.
     """
@@ -228,27 +231,29 @@
         event_document = {'file': file, 'upload': upload}
         events.trigger('model.file.finalizeUpload.before', event_document)
         file = File().save(file)
         events.trigger('model.file.finalizeUpload.after', event_document)
         if '_id' in upload:
             self.remove(upload)
 
-        logger.info('Upload complete. Upload=%s File=%s User=%s' % (
-            upload['_id'], file['_id'], upload['userId']))
+        logger.info(
+            'Upload complete. Upload=%s File=%s User=%s',
+            upload['_id'], file['_id'], upload['userId']
+        )
 
-        # Add an async event for handlers that wish to process this file.
+        # Add an event for handlers that wish to process this file.
         eventParams = {
             'file': file,
             'assetstore': assetstore,
             'currentToken': rest.getCurrentToken(),
             'currentUser': rest.getCurrentUser()
         }
         if 'reference' in upload:
             eventParams['reference'] = upload['reference']
-        events.daemon.trigger('data.process', eventParams)
+        events.trigger('data.process', eventParams)
 
         return file
 
     def getTargetAssetstore(self, modelType, resource, assetstore=None):
         """
         Get the assetstore for a particular target resource, i.e. where new
         data within the resource should be stored. In Girder core, this is
```

### Comparing `girder-3.2.3.dev7/girder/models/user.py` & `girder-5.0.0a2.dev10/girder/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,22 @@
 
 from .model_base import AccessControlledModel
 from .setting import Setting
 from girder import events
 from girder.constants import AccessType, CoreEventHandler, TokenScope
 from girder.exceptions import AccessException, ValidationException
 from girder.settings import SettingKey
-from girder.utility import config, mail_utils
+from girder.utility import mail_utils
 from girder.utility._cache import rateLimitBuffer
 
+_password_regex = re.compile(os.getenv('GIRDER_PASSWORD_REGEX', r'.{6}.*'))
+_password_valid_description = os.getenv(
+    'GIRDER_VALID_PASSWORD_DESCRIPTION', 'Password must be at least 6 characters long.'
+)
+
 
 class User(AccessControlledModel):
     """
     This model represents the users of the system.
     """
 
     def initialize(self):
@@ -297,19 +302,17 @@
                          be stored for this user. This should be done in cases
                          where an external system is responsible for
                          authenticating the user.
         """
         if password is None:
             user['salt'] = None
         else:
-            cur_config = config.getConfig()
-
             # Normally this would go in validate() but password is a special case.
-            if not re.match(cur_config['users']['password_regex'], password):
-                raise ValidationException(cur_config['users']['password_description'], 'password')
+            if not re.match(_password_regex, password):
+                raise ValidationException(_password_valid_description, 'password')
 
             user['salt'] = self._cryptContext.hash(password)
 
         if save:
             self.save(user)
 
     def initializeOtp(self, user):
```

### Comparing `girder-3.2.3.dev7/girder/plugin.py` & `girder-5.0.0a2.dev10/girder/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,60 @@
 """
 This module defines functions for registering, loading, and querying girder plugins.
 """
 
+from collections import OrderedDict
+from dataclasses import dataclass
 import distutils.dist
 from functools import wraps
 import io
-import json
-import os
-from pkg_resources import iter_entry_points, resource_filename
+import logging
+from pathlib import Path
+from pkg_resources import iter_entry_points
+from typing import List, OrderedDict as OrderedDictType
 
-from girder import logprint
+from girder import __version__
 from girder.exceptions import GirderException
 
+logger = logging.getLogger(__name__)
+
+
+@dataclass
+class PluginStaticContent:
+    css: List[str]
+    js: List[str]
+
 
 _NAMESPACE = 'girder.plugin'
 _pluginRegistry = None
 _pluginLoadOrder = []
-_pluginWebroots = {}
+_pluginStaticContent: OrderedDictType[str, PluginStaticContent] = OrderedDict()
 
 
-def getPluginWebroots():
-    global _pluginWebroots
-    return _pluginWebroots
+def getPluginStaticContent():
+    return _pluginStaticContent
 
 
-def registerPluginWebroot(webroot, name):
-    """
-    Adds a webroot to the global registry for plugins based on
-    the plugin name.
-    """
-    global _pluginWebroots
-
-    _pluginWebroots[name] = webroot
+def registerPluginStaticContent(plugin: str, css: List[str], js: List[str], staticDir: Path, tree):
+    from girder.utility.server import _errorDefault
+
+    if plugin not in _pluginStaticContent:
+        tree.mount(None, f'/plugin_static/{plugin}', {
+            '/': {
+                'tools.staticdir.on': True,
+                'tools.staticdir.dir': str(staticDir),
+                'request.show_tracebacks': False,
+                'response.headers.server': f'Girder {__version__}',
+                'error_page.default': _errorDefault
+            }
+        })
+        _pluginStaticContent[plugin] = PluginStaticContent(
+            css=[f'/plugin_static/{plugin}/{f.lstrip("/")}' for f in css],
+            js=[f'/plugin_static/{plugin}/{f.lstrip("/")}' for f in js],
+        )
 
 
 class _PluginMeta(type):
     """
     This is a metaclass applied to the ``GirderPlugin`` descriptor class.  It
     exists to automatically wrap subclass load methods.
     """
@@ -55,15 +74,15 @@
                 # This block is executed on the first call to the function.
                 # The return value of the call is saved an attribute on the wrapper
                 # for future invocations.
                 self._return = func(self, *args, **kwargs)
 
                 self._loaded = True
                 _pluginLoadOrder.append(self.name)
-                logprint.success('Loaded plugin "%s"' % self.name)
+                logger.info('Loaded plugin "%s"', self.name)
 
             return self._return
 
         return wrapper
 
 
 class GirderPlugin(metaclass=_PluginMeta):
@@ -82,49 +101,20 @@
                 import rest  # register new rest endpoints, etc.
     """
 
     #: This is the named displayed to users on the plugin page.  Unlike the entrypoint name
     #: used internally, this name can be an arbitrary string.
     DISPLAY_NAME = None
 
-    #: The path of the plugin's web client source code.  This path is given relative to the python
-    #: package.  This property is used to link the web client source into the staging area while
-    #: building in development mode.  When this value is `None` it indicates there is no web client
-    #: component.
-    CLIENT_SOURCE_PATH = None
-
     def __init__(self, entrypoint):
         self._name = entrypoint.name
         self._loaded = False
         self._dist = entrypoint.dist
         self._metadata = _readPackageMetadata(self._dist)
 
-    def npmPackages(self):
-        """Return a dictionary of npm packages -> versions for building the plugin client.
-
-        By default, this dictionary will be assembled from the CLIENT_SOURCE_PATH property by
-        inspecting the package.json file in the indicated directory.  Plugins can override this
-        method customize the behaivor for advanced usage.
-        """
-        if self.CLIENT_SOURCE_PATH is None:
-            return {}
-
-        packageJsonFile = resource_filename(
-            self.__module__,
-            os.path.join(self.CLIENT_SOURCE_PATH, 'package.json')
-        )
-        if not os.path.isfile(packageJsonFile):
-            raise Exception('Invalid web client path provided: %s' % packageJsonFile)
-
-        with open(packageJsonFile) as f:
-            packageJson = json.load(f)
-            packageName = packageJson['name']
-
-        return {packageName: 'file:%s' % os.path.dirname(packageJsonFile)}
-
     @property
     def name(self):
         """Return the plugin name defaulting to the entrypoint name."""
         return self._name
 
     @property
     def displayName(self):
```

### Comparing `girder-3.2.3.dev7/girder/settings.py` & `girder-5.0.0a2.dev10/girder/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 from collections import OrderedDict
 
 import cherrypy
 from bson import ObjectId
 import re
 
-from girder.constants import GIRDER_ROUTE_ID
 from girder.exceptions import ValidationException
 from girder.utility import setting_utilities
 
 
 class SettingKey:
     """
     Core settings should be enumerated here by a set of constants corresponding
     to sensible strings.
     """
 
     ADD_TO_GROUP_POLICY = 'core.add_to_group_policy'
     API_KEYS = 'core.api_keys'
     BANNER_COLOR = 'core.banner_color'
     BRAND_NAME = 'core.brand_name'
+    CACHE_ENABLED = 'core.cache.enabled'
+    CACHE_CONFIG = 'core.cache_config'
     COLLECTION_CREATE_POLICY = 'core.collection_create_policy'
     CONTACT_EMAIL_ADDRESS = 'core.contact_email_address'
     COOKIE_LIFETIME = 'core.cookie_lifetime'
     CORS_ALLOW_HEADERS = 'core.cors.allow_headers'
     CORS_ALLOW_METHODS = 'core.cors.allow_methods'
     CORS_ALLOW_ORIGIN = 'core.cors.allow_origin'
     CORS_EXPOSE_HEADERS = 'core.cors.expose_headers'
     EMAIL_FROM_ADDRESS = 'core.email_from_address'
     EMAIL_HOST = 'core.email_host'
     EMAIL_VERIFICATION = 'core.email_verification'
     ENABLE_NOTIFICATION_STREAM = 'core.enable_notification_stream'
     ENABLE_PASSWORD_LOGIN = 'core.enable_password_login'
     GIRDER_MOUNT_INFORMATION = 'core.girder_mount_information'
-    HTTP_ONLY_COOKIES = 'core.http_only_cookies'
     PRIVACY_NOTICE = 'core.privacy_notice'
     REGISTRATION_POLICY = 'core.registration_policy'
-    ROUTE_TABLE = 'core.route_table'
     SERVER_ROOT = 'core.server_root'
     SMTP_ENCRYPTION = 'core.smtp.encryption'
     SMTP_HOST = 'core.smtp_host'
     SMTP_PASSWORD = 'core.smtp.password'
     SMTP_PORT = 'core.smtp.port'
     SMTP_USERNAME = 'core.smtp.username'
     UPLOAD_MINIMUM_CHUNK_SIZE = 'core.upload_minimum_chunk_size'
@@ -53,14 +52,16 @@
     """
 
     defaults = {
         SettingKey.ADD_TO_GROUP_POLICY: 'never',
         SettingKey.API_KEYS: True,
         SettingKey.BANNER_COLOR: '#3F3B3B',
         SettingKey.BRAND_NAME: 'Girder',
+        SettingKey.CACHE_ENABLED: False,
+        SettingKey.CACHE_CONFIG: {},
         SettingKey.COLLECTION_CREATE_POLICY: {
             'open': False,
             'groups': [],
             'users': []
         },
         SettingKey.CONTACT_EMAIL_ADDRESS: 'kitware@kitware.com',
         SettingKey.COOKIE_LIFETIME: 180,
@@ -77,18 +78,16 @@
         #  X-Forwarded-Host, Remote-Addr
         SettingKey.EMAIL_FROM_ADDRESS: 'Girder <no-reply@girder.org>',
         # SettingKey.EMAIL_HOST is provided by a function
         SettingKey.EMAIL_VERIFICATION: 'disabled',
         SettingKey.ENABLE_NOTIFICATION_STREAM: True,
         SettingKey.ENABLE_PASSWORD_LOGIN: True,
         SettingKey.GIRDER_MOUNT_INFORMATION: None,
-        SettingKey.HTTP_ONLY_COOKIES: False,  # TODO This will go away in next major version
         SettingKey.PRIVACY_NOTICE: 'https://www.kitware.com/privacy',
         SettingKey.REGISTRATION_POLICY: 'open',
-        # SettingKey.ROUTE_TABLE is provided by a function
         SettingKey.SERVER_ROOT: '',
         SettingKey.SMTP_ENCRYPTION: 'none',
         SettingKey.SMTP_HOST: 'localhost',
         SettingKey.SMTP_PASSWORD: '',
         SettingKey.SMTP_PORT: 25,
         SettingKey.SMTP_USERNAME: '',
         SettingKey.UPLOAD_MINIMUM_CHUNK_SIZE: 1024 * 1024 * 5,
@@ -100,21 +99,14 @@
     def _defaultEmailHost():
         if cherrypy.request and cherrypy.request.local and cherrypy.request.local.name:
             host = '%s://%s' % (cherrypy.request.scheme, cherrypy.request.local.name)
             if cherrypy.request.local.port != 80:
                 host += ':%d' % cherrypy.request.local.port
             return host
 
-    @staticmethod
-    @setting_utilities.default(SettingKey.ROUTE_TABLE)
-    def _defaultRouteTable():
-        return {
-            GIRDER_ROUTE_ID: '/'
-        }
-
 
 class SettingValidator:
     @staticmethod
     @setting_utilities.validator(SettingKey.ADD_TO_GROUP_POLICY)
     def _validateAddToGroupPolicy(doc):
         doc['value'] = doc['value'].lower()
         if doc['value'] not in ('never', 'noadmin', 'nomod', 'yesadmin', 'yesmod', ''):
@@ -139,14 +131,26 @@
     @staticmethod
     @setting_utilities.validator(SettingKey.BRAND_NAME)
     def _validateBrandName(doc):
         if not doc['value']:
             raise ValidationException('The brand name may not be empty', 'value')
 
     @staticmethod
+    @setting_utilities.validator(SettingKey.CACHE_ENABLED)
+    def _validateCacheEnabled(doc):
+        if not isinstance(doc['value'], bool):
+            raise ValidationException('Cache enabled setting must be boolean.', 'value')
+
+    @staticmethod
+    @setting_utilities.validator(SettingKey.CACHE_CONFIG)
+    def _validateCacheConfig(doc):
+        if not isinstance(doc['value'], dict):
+            raise ValidationException('Cache config must be a JSON object.', 'value')
+
+    @staticmethod
     @setting_utilities.validator(SettingKey.COLLECTION_CREATE_POLICY)
     def _validateCollectionCreatePolicy(doc):
         from girder.models.group import Group
         from girder.models.user import User
 
         value = doc['value']
 
@@ -268,48 +272,28 @@
     def _validateGirderMountInformation(doc):
         value = doc['value']
         if not isinstance(value, dict) or 'path' not in value:
             raise ValidationException(
                 'Girder mount information must be a dict with the "path" key.', 'value')
 
     @staticmethod
-    @setting_utilities.validator(SettingKey.HTTP_ONLY_COOKIES)
-    def _validateHttpOnlyCookies(doc):
-        if not isinstance(doc['value'], bool):
-            raise ValidationException('HTTP only cookies setting must be boolean.', 'value')
-
-    @staticmethod
     @setting_utilities.validator(SettingKey.PRIVACY_NOTICE)
     def _validatePrivacyNotice(doc):
         if not doc['value']:
             raise ValidationException('The privacy notice link may not be empty', 'value')
 
     @staticmethod
     @setting_utilities.validator(SettingKey.REGISTRATION_POLICY)
     def _validateRegistrationPolicy(doc):
         doc['value'] = doc['value'].lower()
         if doc['value'] not in ('open', 'closed', 'approve'):
             raise ValidationException(
                 'Registration policy must be "open", "closed", or "approve".', 'value')
 
     @staticmethod
-    @setting_utilities.validator(SettingKey.ROUTE_TABLE)
-    def _validateRouteTable(doc):
-        nonEmptyRoutes = [route for route in doc['value'].values() if route]
-        if GIRDER_ROUTE_ID not in doc['value'] or not doc['value'][GIRDER_ROUTE_ID]:
-            raise ValidationException('Girder root must be routable.', 'value')
-
-        for key in doc['value']:
-            if (doc['value'][key] and not doc['value'][key].startswith('/')):
-                raise ValidationException('Routes must begin with a forward slash.', 'value')
-
-        if len(nonEmptyRoutes) > len(set(nonEmptyRoutes)):
-            raise ValidationException('Routes must be unique.', 'value')
-
-    @staticmethod
     @setting_utilities.validator(SettingKey.SERVER_ROOT)
     def _validateServerRoot(doc):
         val = doc['value']
         if val and not val.startswith('http://') and not val.startswith('https://'):
             raise ValidationException('Server root must start with http:// or https://.', 'value')
 
     @staticmethod
```

### Comparing `girder-3.2.3.dev7/girder/utility/__init__.py` & `girder-5.0.0a2.dev10/girder/utility/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import cherrypy
 import datetime
 import dateutil.parser
 import errno
 from functools import wraps
 import json
+import logging
 import os
 import pytz
 import re
 import string
 
 import girder
 import girder.events
 
+logger = logging.getLogger(__name__)
+
 try:
     from random import SystemRandom
     random = SystemRandom()
     random.random()  # potentially raises NotImplementedError
 except NotImplementedError:
-    girder.logprint.warning(
-        'WARNING: using non-cryptographically secure PRNG.')
+    logger.warning('WARNING: using non-cryptographically secure PRNG.')
     import random
 
 
 def parseTimestamp(x, naive=True):
     """
     Parse a datetime string using the python-dateutil package.
```

### Comparing `girder-3.2.3.dev7/girder/utility/_hash_state.py` & `girder-5.0.0a2.dev10/girder/utility/_hash_state.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/utility/abstract_assetstore_adapter.py` & `girder-5.0.0a2.dev10/girder/utility/abstract_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/utility/acl_mixin.py` & `girder-5.0.0a2.dev10/girder/utility/acl_mixin.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/utility/assetstore_utilities.py` & `girder-5.0.0a2.dev10/girder/utility/assetstore_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from ..constants import AssetstoreType
 from ..exceptions import NoAssetstoreAdapter
 from .filesystem_assetstore_adapter import FilesystemAssetstoreAdapter
-from .gridfs_assetstore_adapter import GridFsAssetstoreAdapter
 from .s3_assetstore_adapter import S3AssetstoreAdapter
 
 
 _assetstoreTable = {
     AssetstoreType.FILESYSTEM: FilesystemAssetstoreAdapter,
-    AssetstoreType.GRIDFS: GridFsAssetstoreAdapter,
     AssetstoreType.S3: S3AssetstoreAdapter
 }
 
 
 def getAssetstoreAdapter(assetstore, instance=True):
     """
     This is a factory method that will return the appropriate assetstore adapter
@@ -61,10 +59,9 @@
 def fileIndexFields():
     """
     This will return a set of all required index fields from all of the
     different assetstore types.
     """
     return list(set(
         FilesystemAssetstoreAdapter.fileIndexFields()
-        + GridFsAssetstoreAdapter.fileIndexFields()
         + S3AssetstoreAdapter.fileIndexFields()
     ))
```

### Comparing `girder-3.2.3.dev7/girder/utility/filesystem_assetstore_adapter.py` & `girder-5.0.0a2.dev10/girder/utility/filesystem_assetstore_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import filelock
 from hashlib import sha512
 import io
+import logging
 import os
 import psutil
 import shutil
 import stat
 import tempfile
 
-from girder import events, logger
+from girder import events
 from girder.api.rest import setResponseHeader
 from girder.exceptions import ValidationException, GirderException
 from girder.models.file import File
 from girder.models.folder import Folder
 from girder.models.item import Item
 from girder.models.upload import Upload
 from girder.utility import mkdir, progress
@@ -19,14 +20,16 @@
 from .abstract_assetstore_adapter import AbstractAssetstoreAdapter
 
 BUF_SIZE = 65536
 
 # Default permissions for the files written to the filesystem
 DEFAULT_PERMS = stat.S_IRUSR | stat.S_IWUSR
 
+logger = logging.getLogger(__name__)
+
 
 class FilesystemAssetstoreAdapter(AbstractAssetstoreAdapter):
     """
     This assetstore type stores files on the filesystem underneath a root
     directory. Files are named by their SHA-512 hash, which avoids duplication
     of file content.
 
@@ -91,32 +94,29 @@
         # happens to existing assetstores that no longer can access their temp
         # directories.
         self.tempDir = os.path.join(self.assetstore['root'], 'temp')
         try:
             mkdir(self.tempDir)
         except OSError:
             self.unavailable = True
-            logger.exception('Failed to create filesystem assetstore '
-                             'directories %s' % self.tempDir)
+            logger.exception('Failed to create filesystem assetstore directories %s', self.tempDir)
         if not os.access(self.assetstore['root'], os.W_OK):
             self.unavailable = True
-            logger.error('Could not write to assetstore root: %s',
-                         self.assetstore['root'])
+            logger.error('Could not write to assetstore root: %s', self.assetstore['root'])
 
     def capacityInfo(self):
         """
         For filesystem assetstores, we just need to report the free and total
         space on the filesystem where the assetstore lives.
         """
         try:
             usage = psutil.disk_usage(self.assetstore['root'])
             return {'free': usage.free, 'total': usage.total}
         except OSError:
-            logger.exception(
-                'Failed to get disk usage of %s' % self.assetstore['root'])
+            logger.exception('Failed to get disk usage of %s', self.assetstore['root'])
         # If psutil.disk_usage fails or we can't query the assetstore's root
         # directory, just report nothing regarding disk capacity
         return {
             'free': None,
             'total': None
         }
 
@@ -301,15 +301,15 @@
             with filelock.FileLock(path + '.deleteLock'):
                 matching = File().find(q, limit=2, fields=[])
                 matchingUpload = Upload().findOne(q)
                 if matching.count(True) == 1 and matchingUpload is None:
                     try:
                         os.unlink(path)
                     except Exception:
-                        logger.exception('Failed to delete file %s' % path)
+                        logger.exception('Failed to delete file %s', path)
 
     def cancelUpload(self, upload):
         """
         Delete the temporary files associated with a given upload.
         """
         if os.path.exists(upload['tempFile']):
             os.unlink(upload['tempFile'])
```

### Comparing `girder-3.2.3.dev7/girder/utility/mail_utils.py` & `girder-5.0.0a2.dev10/girder/utility/mail_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import logging
 import os
 import re
 import smtplib
 
 from email.mime.text import MIMEText
 from mako.lookup import TemplateLookup
 from girder import events
-from girder import logger
 from girder.constants import PACKAGE_DIR
 from girder.settings import SettingKey
 
+logger = logging.getLogger(__name__)
+
 
 def validateEmailAddress(address):
     """
     Determines whether a string is a valid email address.
 
     This implements the grammar from 4.10.5.1.5 of the HTML Standard.
 
@@ -143,14 +145,19 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.connection.quit()
 
 
 def _submitEmail(msg, recipients):
     from girder.models.setting import Setting
 
+    if os.environ.get('GIRDER_EMAIL_TO_CONSOLE'):
+        print('Redirecting email to console:')
+        print(msg.as_string())
+        return
+
     setting = Setting()
     smtp = _SMTPConnection(
         host=setting.get(SettingKey.SMTP_HOST),
         port=setting.get(SettingKey.SMTP_PORT),
         encryption=setting.get(SettingKey.SMTP_ENCRYPTION),
         username=setting.get(SettingKey.SMTP_USERNAME),
         password=setting.get(SettingKey.SMTP_PASSWORD)
@@ -167,47 +174,40 @@
     recipients = event.info['recipients']
     _submitEmail(msg, recipients)
 
 
 events.bind('_sendmail', 'core.email', _sendmail)
 
 
-def sendMailSync(subject, text, to, bcc=None):
-    """Send an email synchronously."""
-    msg, recipients = _createMessage(subject, text, to, bcc)
-
-    _submitEmail(msg, recipients)
-
-
 def sendMail(subject, text, to, bcc=None):
     """
-    Send an email asynchronously.
+    Send an email.
 
     :param subject: The subject line of the email.
     :type subject: str
     :param text: The body of the email.
     :type text: str
     :param to: The list of recipient email addresses.
     :type to: list
     :param bcc: Recipient email addresses that should be specified using the Bcc header.
     :type bcc: list or None
     """
     msg, recipients = _createMessage(subject, text, to, bcc)
 
-    events.daemon.trigger('_sendmail', info={
+    events.trigger('_sendmail', info={
         'message': msg,
         'recipients': recipients
     })
 
 
 def sendMailToAdmins(subject, text):
-    """Send an email asynchronously to site admins."""
+    """Send an email to site admins."""
     from girder.models.user import User
 
     to = [u['email'] for u in User().getAdmins()]
     sendMail(subject, text, to)
 
 
 def sendMailIndividually(subject, text, to):
-    """Send emails asynchronously to all recipients individually."""
+    """Send emails to all recipients individually."""
     for address in to:
         sendMail(address, subject, text)
```

### Comparing `girder-3.2.3.dev7/girder/utility/model_importer.py` & `girder-5.0.0a2.dev10/girder/utility/model_importer.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/utility/path.py` & `girder-5.0.0a2.dev10/girder/utility/path.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/utility/progress.py` & `girder-5.0.0a2.dev10/girder/utility/progress.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/utility/s3_assetstore_adapter.py` & `girder-5.0.0a2.dev10/girder/utility/s3_assetstore_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import datetime
 import json
+import logging
 import re
 import urllib.parse
 import uuid
 
 import boto3
 import botocore
 import cherrypy
 import requests
 
-from girder import events, logger
+from girder import events
 from girder.api.rest import setContentDisposition
 from girder.exceptions import GirderException, ValidationException
 from girder.models.file import File
 from girder.models.folder import Folder
 from girder.models.item import Item
 
 from .abstract_assetstore_adapter import AbstractAssetstoreAdapter
 
 BUF_LEN = 65536  # Buffer size for download stream
 DEFAULT_REGION = 'us-east-1'
+logger = logging.getLogger(__name__)
 
 
 class S3AssetstoreAdapter(AbstractAssetstoreAdapter):
     """
     This assetstore type stores files on S3. It is responsible for generating
     HMAC-signed messages that authorize the client to communicate directly with
     the S3 server where the files are stored.
@@ -285,31 +287,35 @@
                 'ContentLength': size,
                 'UploadId': upload['s3']['uploadId'],
                 'PartNumber': upload['s3']['partNumber']
             })
 
             resp = requests.request(method='PUT', url=url, data=chunk, headers=headers)
             if resp.status_code not in (200, 201):
-                logger.error('S3 multipart upload failure %d (uploadId=%s):\n%s' % (
-                    resp.status_code, upload['_id'], resp.text))
+                logger.error(
+                    'S3 multipart upload failure %d (uploadId=%s): %s',
+                    resp.status_code, upload['_id'], resp.text
+                )
                 raise GirderException('Upload failed (bad gateway)')
 
             upload['received'] += size
         else:
             size = chunk.getSize()
             if size < upload['size']:
                 raise ValidationException('Uploads of this length must be sent in a single chunk.')
 
             reqInfo = upload['s3']['request']
             resp = requests.request(
                 method=reqInfo['method'], url=reqInfo['url'], data=chunk,
                 headers=dict(reqInfo['headers'], **{'Content-Length': str(size)}))
             if resp.status_code not in (200, 201):
-                logger.error('S3 upload failure %d (uploadId=%s):\n%s' % (
-                    resp.status_code, upload['_id'], resp.text))
+                logger.error(
+                    'S3 upload failure %d (uploadId=%s): %s',
+                    resp.status_code, upload['_id'], resp.text
+                )
                 raise GirderException('Upload failed (bad gateway)')
 
             upload['received'] = size
 
         return upload
 
     def requestOffset(self, upload):
@@ -481,33 +487,27 @@
                 if force_recursive or folder['created'] >= now:
                     self.importData(parent=folder, parentType='folder', params={
                         **params, 'importPath': obj['Prefix']
                     }, progress=progress, user=user, **kwargs)
 
     def deleteFile(self, file):
         """
-        We want to queue up files to be deleted asynchronously since it requires
-        an external HTTP request per file in order to delete them, and we don't
-        want to wait on that.
+        Delete files from S3.
 
         Files that were imported as pre-existing data will not actually be
         deleted from S3, only their references in Girder will be deleted.
         """
         if file['size'] > 0 and 'relpath' in file:
             q = {
                 'relpath': file['relpath'],
                 'assetstoreId': self.assetstore['_id']
             }
             matching = File().find(q, limit=2, fields=[])
             if matching.count(True) == 1:
-                events.daemon.trigger(info={
-                    'client': self.client,
-                    'bucket': self.assetstore['bucket'],
-                    'key': file['s3Key']
-                }, callback=_deleteFileImpl)
+                self.client.delete_object(Bucket=self.assetstore['bucket'], Key=file['s3Key'])
 
     def fileUpdated(self, file):
         """
         On file update, if the name or the MIME type changed, we must update
         them accordingly on the S3 key so that the file downloads with the
         correct name and content type.
         """
@@ -653,11 +653,7 @@
 
     if service:
         if not service.startswith('http://') and not service.startswith('https://'):
             service = 'https://' + service
         params['endpoint_url'] = service
 
     return params
-
-
-def _deleteFileImpl(event):
-    event.info['client'].delete_object(Bucket=event.info['bucket'], Key=event.info['key'])
```

### Comparing `girder-3.2.3.dev7/girder/utility/search.py` & `girder-5.0.0a2.dev10/girder/utility/search.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/utility/setting_utilities.py` & `girder-5.0.0a2.dev10/girder/utility/setting_utilities.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/utility/system.py` & `girder-5.0.0a2.dev10/girder/utility/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import psutil
 import socket
 import threading
 import time
 
 import girder
-from girder import logger
 from girder.models import getDbConnection
 
 
 def _objectToDict(obj):
     """
     Convert an object to a dictionary.  Any non-private attribute that is an
     integer, float, or string is returned in the dictionary.
@@ -36,26 +35,16 @@
     except Exception:
         pass
     # Report on the disk usage where the script is located
     if hasattr(girder, '__file__'):
         status['girderPath'] = os.path.abspath(girder.__file__)
         status['girderDiskUsage'] = _objectToDict(
             psutil.disk_usage(status['girderPath']))
-    # Report where our logs are and how much space is available for them
+    # the "logs" field is vestigial and no longer used as of v4
     status['logs'] = []
-    for handler in logger.handlers:
-        try:
-            logInfo = {'path': handler.baseFilename}
-            logInfo['diskUsage'] = _objectToDict(
-                psutil.disk_usage(logInfo['path']))
-            status['logs'].append(logInfo)
-        except Exception:
-            # If we can't read information about the log, don't throw an
-            # exception
-            pass
     status['mongoDbStats'] = db.command('dbStats')
     try:
         # This can fail when mongo is on a different system.
         status['mongoDbPath'] = getDbConnection().admin.command(
             'getCmdLineOpts')['parsed']['storage']['dbPath']
         status['mongoDbDiskUsage'] = _objectToDict(
             psutil.disk_usage(status['mongoDbPath']))
```

### Comparing `girder-3.2.3.dev7/girder/utility/ziputil.py` & `girder-5.0.0a2.dev10/girder/utility/ziputil.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/assets/Girder_Mark.png` & `girder-5.0.0a2.dev10/girder/web/dist/Girder_Mark.png`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/collections/Collection.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/collections/Collection.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/collections/UserCollection.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/collections/UserCollection.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/collections/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/collections/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/dialog.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/dialog.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/misc.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/misc.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/AccessControlledModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/AccessControlledModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/ApiKeyModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/ApiKeyModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/AssetstoreModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/AssetstoreModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/CollectionCreationPolicyModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/CollectionCreationPolicyModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/FileModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/FileModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/FolderModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/FolderModel.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
     /**
      * Remove the contents of the folder.
      */
     removeContents: function() {
         return restRequest({
             url: `${this.resourceName}/${this.id}/contents`,
             method: 'DELETE'
-        }).done((resp) => {
+        }).done(() => {
             this.trigger('g:success');
         }).fail((err) => {
             this.trigger('g:error', err);
         });
     }
 });
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/GroupModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/GroupModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/ItemModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/ItemModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/MetadataMixin.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/MetadataMixin.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/Model.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/Model.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/UserModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/UserModel.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/models/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/rest.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/rest.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -31,21 +31,14 @@
  * @param {string} root The root path for the API.
  */
 function setApiRoot(root) {
     // Strip trailing slash
     apiRoot = root.replace(/\/$/, '');
 }
 
-// Initialize the API root (at JS load time)
-// This could be overridden when the App is started, but we need sensible defaults so models, etc.
-// can be easily used without having to start an App or explicitly set these values
-setApiRoot(
-    $('#g-global-info-apiroot').text().replace('%HOST%', window.location.origin) || '/api/v1'
-);
-
 /**
  * Make a request to the REST API.
  *
  * This is a wrapper around {@link http://api.jquery.com/jQuery.ajax/ $.ajax}, which also handles
  * authentication and routing to the Girder API, and provides a default for error notification.
  *
  * Most users of this method should attach a "done" handler to the return value. In cases where the
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/router.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/router.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/routes.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/routes.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,7 @@
-/* eslint-disable import/first */
-
 import router from '@girder/core/router';
 import events from '@girder/core/events';
 import eventStream from '@girder/core/utilities/EventStream';
 import {
     getCurrentUser,
     setCurrentUser
 } from '@girder/core/auth';
@@ -11,44 +9,96 @@
     restRequest
 } from '@girder/core/rest';
 
 /**
  * Admin
  */
 import AdminView from '@girder/core/views/body/AdminView';
-router.route('admin', 'admin', function() {
-    events.trigger('g:navigateTo', AdminView);
-});
 
 /**
  * Assetstores
  */
 import AssetstoresView from '@girder/core/views/body/AssetstoresView';
+
+/**
+ * Collections
+ */
+import CollectionsView from '@girder/core/views/body/CollectionsView';
+
+/**
+ * Collection
+ */
+import CollectionView from '@girder/core/views/body/CollectionView';
+
+/**
+ * Folder
+ */
+import FolderView from '@girder/core/views/body/FolderView';
+
+/**
+ * FrontPage
+ */
+import FrontPageView from '@girder/core/views/body/FrontPageView';
+
+/**
+ * Groups
+ */
+import GroupsView from '@girder/core/views/body/GroupsView';
+
+/**
+ * Group
+ */
+import GroupView from '@girder/core/views/body/GroupView';
+
+/**
+ * Item
+ */
+import ItemView from '@girder/core/views/body/ItemView';
+
+/**
+ * Plugins
+ */
+import PluginsView from '@girder/core/views/body/PluginsView';
+import UsersView from '@girder/core/views/body/UsersView';
+
+/**
+ * SystemConfiguration
+ */
+import SystemConfigurationView from '@girder/core/views/body/SystemConfigurationView';
+
+/**
+ * UserAccount
+ */
+import UserAccountView from '@girder/core/views/body/UserAccountView';
+import UserModel from '@girder/core/models/UserModel';
+
+/**
+ * User
+ */
+import UserView from '@girder/core/views/body/UserView';
+
+/**
+ * SearchResults
+ */
+import SearchResultsView from '@girder/core/views/body/SearchResultsView';
+router.route('admin', 'admin', function() {
+    events.trigger('g:navigateTo', AdminView);
+});
 router.route('assetstores', 'assetstores', function(params) {
     events.trigger('g:navigateTo', AssetstoresView, {
         assetstoreEdit: params.dialog === 'assetstoreedit' ? params.dialogid : false
     });
 });
 router.route('assetstore/:id/import', 'assetstoreImport', function(assetstoreId) {
     AssetstoresView.import(assetstoreId);
 });
-
-/**
- * Collections
- */
-import CollectionsView from '@girder/core/views/body/CollectionsView';
 router.route('collections', 'collections', function(params) {
     events.trigger('g:navigateTo', CollectionsView, params || {});
     events.trigger('g:highlightItem', 'CollectionsView');
 });
-
-/**
- * Collection
- */
-import CollectionView from '@girder/core/views/body/CollectionView';
 router.route('collection/:id', 'collectionAccess', function(cid, params) {
     CollectionView.fetchAndInit(cid, {
         access: params.dialog === 'access',
         edit: params.dialog === 'edit',
         folderCreate: params.dialog === 'foldercreate',
         dialog: params.dialog
     });
@@ -61,96 +111,54 @@
         edit: params.dialog === 'edit',
         folderAccess: params.dialog === 'folderaccess',
         folderCreate: params.dialog === 'foldercreate',
         folderEdit: params.dialog === 'folderedit',
         itemCreate: params.dialog === 'itemcreate'
     });
 });
-
-/**
- * Folder
- */
-import FolderView from '@girder/core/views/body/FolderView';
 router.route('folder/:id', 'folder', function(id, params) {
     FolderView.fetchAndInit(id, {
         upload: params.dialog === 'upload',
         folderAccess: params.dialog === 'folderaccess',
         folderCreate: params.dialog === 'foldercreate',
         folderEdit: params.dialog === 'folderedit',
         itemCreate: params.dialog === 'itemcreate'
     });
 });
-
-/**
- * FrontPage
- */
-import FrontPageView from '@girder/core/views/body/FrontPageView';
 router.route('', 'index', function() {
     events.trigger('g:navigateTo', FrontPageView);
 });
-
-/**
- * Groups
- */
-import GroupsView from '@girder/core/views/body/GroupsView';
 router.route('groups', 'groups', function(params) {
     events.trigger('g:navigateTo', GroupsView, params || {});
     events.trigger('g:highlightItem', 'GroupsView');
 });
-
-/**
- * Group
- */
-import GroupView from '@girder/core/views/body/GroupView';
 router.route('group/:id', 'groupView', function(groupId, params) {
     GroupView.fetchAndInit(groupId, {
         edit: params.dialog === 'edit'
     });
 });
 router.route('group/:id/:tab', 'groupView', function(groupId, tab, params) {
     GroupView.fetchAndInit(groupId, {
         edit: params.dialog === 'edit',
         tab: tab
     });
 });
-
-/**
- * Item
- */
-import ItemView from '@girder/core/views/body/ItemView';
 router.route('item/:id', 'item', function(itemId, params) {
     ItemView.fetchAndInit(itemId, {
         edit: params.dialog === 'itemedit',
         fileEdit: params.dialog === 'fileedit' ? params.dialogid : false,
         upload: params.dialog === 'upload' ? params.dialogid : false
     });
 });
-
-/**
- * Plugins
- */
-import PluginsView from '@girder/core/views/body/PluginsView';
-import UsersView from '@girder/core/views/body/UsersView';
 router.route('plugins', 'plugins', function() {
     events.trigger('g:navigateTo', PluginsView);
 });
-
-/**
- * SystemConfiguration
- */
-import SystemConfigurationView from '@girder/core/views/body/SystemConfigurationView';
 router.route('settings', 'settings', function() {
     events.trigger('g:navigateTo', SystemConfigurationView);
 });
-
-/**
- * UserAccount
- */
-import UserAccountView from '@girder/core/views/body/UserAccountView';
-import UserModel from '@girder/core/models/UserModel';
 router.route('useraccount/:id/:tab', 'accountTab', function(id, tab) {
     UserAccountView.fetchAndInit(id, tab);
 });
 router.route('useraccount/:id/token/:token', 'accountToken', function(id, token) {
     UserModel.fromTemporaryToken(id, token)
         .done(() => {
             events.trigger('g:navigateTo', UserAccountView, {
@@ -202,19 +210,14 @@
 /**
  * Users
  */
 router.route('users', 'users', function(params) {
     events.trigger('g:navigateTo', UsersView, params || {});
     events.trigger('g:highlightItem', 'UsersView');
 });
-
-/**
- * User
- */
-import UserView from '@girder/core/views/body/UserView';
 router.route('user/:id', 'user', function(userId, params) {
     UserView.fetchAndInit(userId, {
         folderCreate: params.dialog === 'foldercreate',
         dialog: params.dialog
     });
 });
 router.route('user/:id/folder/:id', 'userFolder', function(userId, folderId, params) {
@@ -223,18 +226,13 @@
         upload: params.dialog === 'upload',
         folderAccess: params.dialog === 'folderaccess',
         folderCreate: params.dialog === 'foldercreate',
         folderEdit: params.dialog === 'folderedit',
         itemCreate: params.dialog === 'itemcreate'
     });
 });
-
-/**
- * SearchResults
- */
-import SearchResultsView from '@girder/core/views/body/SearchResultsView';
 router.route('search/results', 'SearchResults', function(params) {
     events.trigger('g:navigateTo', SearchResultsView, {
         query: params.query,
         mode: params.mode
     });
 });
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/apidocs/apidocs.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/apidocs/apidocs.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/assetstores.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/assetstores.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/collectionList.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/collectionList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/frontPage.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/frontPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/groupList.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/groupList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/groupPage.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/groupPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/itemPage.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/itemPage.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/plugins.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/plugins.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/searchResultsList.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/searchResultsList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/systemConfig.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/systemConfig.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userAccount.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userAccount.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/body/userList.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userList.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/global.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/global.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/globalNav.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/globalNav.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/layout.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/layout.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/layout/loading.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/loading.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/accessWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/accessWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/hierarchyWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/hierarchyWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/markdownWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/markdownWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/metadataWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/metadataWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/searchFieldWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/searchFieldWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/taskProgress.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/taskProgress.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/timelineWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/timelineWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/uploadWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/uploadWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/stylesheets/widgets/userOtpManagementWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/userOtpManagementWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/assetstores.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/assetstores.pug`

 * *Files 4% similar despite different names*

```diff
@@ -27,29 +27,14 @@
               span.g-assetstore-type  Filesystem
             div
               b Root path:
               span.g-assetstore-root  #{assetstore.get('root')}
             div
               b File creation permissions (octal):
               span.g-assetstore-perms  #{(assetstore.get('perms') || 0o600).toString(8)}
-          else if assetstore.get('type') === types.GRIDFS
-            div
-              b Type:
-              span.g-assetstore-type  GridFS
-            div
-              b Database name:
-              span.g-assetstore-root  #{assetstore.get('db')}
-            if assetstore.get('mongohost')
-              div
-                b Mongo Host URI:
-                span.g-assetstore-mongohost  #{assetstore.get('mongohost')}
-              if assetstore.get('replicaset')
-                div
-                  b Replica Set:
-                  span.g-assetstore-replicaset  #{assetstore.get('replicaset')}
           else if assetstore.get('type') === types.S3
             div
               b Type:
               span.g-assetstore-type  S3
             div
               b Bucket:
               span.g-assetstore-bucket  #{assetstore.get('bucket')}
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/collectionList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/collectionList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/collectionPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/collectionPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/filesystemImport.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/filesystemImport.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/frontPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/frontPage.pug`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .g-frontpage-header
   .g-frontpage-logo-container
-    img.g-frontpage-logo(src=require('@girder/core/assets/Girder_Mark.png'))
+    img.g-frontpage-logo(src='Girder_Mark.png')
   .g-frontpage-title-container
     .g-frontpage-title #{brandName}
     .g-frontpage-subtitle Data management platform
 
 .g-frontpage-body
   .g-frontpage-paragraph
     .g-frontpage-welcome-text-content
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/groupList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/groupList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/groupPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/groupPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/itemPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/itemPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/plugins.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/plugins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/s3Import.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/s3Import.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/systemConfiguration.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/systemConfiguration.pug`

 * *Files 9% similar despite different names*

```diff
@@ -135,36 +135,14 @@
           title="The username, if any, used to authenticate to the SMTP server used to send emails.")
     .form-group
       label(for="g-core-smtp-password") SMTP password
       input#g-core-smtp-password.form-control.input-sm(
           type="password", value=settings['core.smtp.password'] || '',
           title="The password, if any, used to authenticate to the SMTP server used to send emails.")
 
-  .g-settings-form-container
-    h4 Routing
-    p.
-      Altering routes requires a restart of the Girder server to take effect.
-    .g-settings-form-container
-      h5 Core Routes
-      label core_girder
-      input.g-core-route-table.form-control.input-sm(
-          type="text",
-          value=routes['core_girder'] || '',
-          data-webroot-name="core_girder",
-          title="The path to place core_girder.")
-    if routeKeys.length > 2
-      .form-group
-        h5 Other Routes
-        each name in routeKeys.slice(2)
-          label= name
-          input.g-core-route-table.form-control.input-sm(
-              type="text",
-              value=routes[name] || '',
-              data-webroot-name=name,
-              title="The path to place ${name}.")
   #g-configuration-accordion.panel-group
     .panel.panel-default
       .panel-heading(data-toggle="collapse",
           data-parent="#g-configuration-accordion",
           data-target="#g-advanced-settings-tab")
         .panel-title
           a
@@ -176,15 +154,15 @@
             label(for="g-core-server-root") Server root URL
             input#g-core-server-root.form-control.input-sm(
                 type="text", value=settings['core.server_root'] || '',
                 placeholder='Detect automatically')
           .form-group
             label(for="g-core-upload-minimum-chunk-size") Upload minimum chunk size (bytes)
             br
-            span This applies to Filesystem and GridFS assetstores.
+            span This applies to Filesystem assetstores.
             input#g-core-upload-minimum-chunk-size.form-control.input-sm(
                 type="text", value=settings['core.upload_minimum_chunk_size'] || '',
                 title="For large files, the minimum size of all but the last chunk.")
           .form-group
             label Server Notification Stream
             br
             span Disabling this may improve server performance with many concurrent web client users.
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/userAccount.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userAccount.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/userList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/body/userPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userPage.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/layout/layoutHeaderUser.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutHeaderUser.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/layout/loginDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/loginDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/layout/registerDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/registerDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/layout/resetPasswordDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/resetPasswordDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditor.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditor.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEditorMixins.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditorMixins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/accessEntry.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEntry.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/apiKeyList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/apiKeyList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/browserWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/browserWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/checkedActionsMenu.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/checkedActionsMenu.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/collectionInfoDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/collectionInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/confirmDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/confirmDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/dateTimeRangeWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/dateTimeRangeWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editApiKeyWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editApiKeyWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editAssetstoreWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editAssetstoreWidget.pug`

 * *Files 13% similar despite different names*

```diff
@@ -13,26 +13,14 @@
           if assetstore.get('type') === types.FILESYSTEM
             .form-group
               label.control-label(for="g-edit-fs-root") Root directory
               input#g-edit-fs-root.input-sm.form-control(type="text", placeholder="Root directory")
             .form-group
               label.control-label(for="g-edit-fs-perms") File creation permissions (octal)
               input#g-edit-fs-perms.input-sm.form-control(type="text", placeholder="600")
-          if assetstore.get('type') === types.GRIDFS
-            .form-group
-              label.control-label(for="g-edit-gridfs-db") Database name
-              input#g-edit-gridfs-db.input-sm.form-control(type="text", placeholder="Database name")
-            .form-group
-              label.control-label(for="g-edit-gridfs-mongohost") Mongo Host URI
-              input#g-edit-gridfs-mongohost.input-sm.form-control(
-                  type="text", placeholder="Mongo host uri (defaults to the main Girder database)",
-                  title="The URI is of the form mongodb://[username:password@]host1[:port1][,host2[:port2],...[,hostN[:portN]]][/[database][?options]]")
-            .form-group
-              label.control-label(for="g-edit-gridfs-replicaset") Replica Set
-              input#g-edit-gridfs-replicaset.input-sm.form-control(type="text", placeholder="Replica set name (blank if not using a replica set)")
           if assetstore.get('type') === types.S3
             .form-group
               label.control-label(for="g-edit-s3-bucket") S3 bucket name
               input#g-edit-s3-bucket.input-sm.form-control(type="text", placeholder="Bucket")
             .form-group
               label.control-label(for="g-edit-s3-prefix") Path prefix (optional)
               input#g-edit-s3-prefix.input-sm.form-control(type="text", placeholder="Prefix")
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editCollectionWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editCollectionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editFileWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editFileWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editFolderWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editFolderWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editGroupWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editGroupWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/editItemWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editItemWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/fileInfoDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/fileInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/fileList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/fileList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/folderInfoDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/folderInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/folderList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/folderList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupAdminList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupAdminList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupInviteDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupInviteDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupMemberList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupMemberList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/groupModList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupModList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyBreadcrumb.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyBreadcrumb.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyPaginated.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyPaginated.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/hierarchyWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/itemList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/itemList.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/jsonMetadatumEditWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/jsonMetadatumEditWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/markdownWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/markdownWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadataWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadataWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/metadatumEditWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadatumEditWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/newAssetstore.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/newAssetstore.pug`

 * *Files 21% similar despite different names*

```diff
@@ -27,49 +27,14 @@
               type="text", placeholder="Root directory")
           p#g-new-fs-error.g-validation-failed-message
           input.g-new-assetstore-submit.btn.btn-sm.btn-primary(type="submit", value="Create")
 
   .panel.panel-default
     .panel-heading(data-toggle="collapse",
         data-parent="#g-assetstore-accordion",
-        data-target="#g-create-gridfs-tab")
-      .panel-title
-        a
-          i.icon-leaf
-          span Create new #[b GridFS] assetstore
-    #g-create-gridfs-tab.panel-collapse.collapse
-      .panel-body
-        p.
-          This type of assetstore uses
-          MongoDB's #[a(target="_blank", href="http://docs.mongodb.org/manual/core/gridfs/") GridFS]
-          storage engine. The files should be stored in a separate database
-          from the rest of the server's information to avoid locking issues.
-        form#g-new-gridfs-form(role="form")
-          .form-group
-            label.control-label(for="g-new-gridfs-name") Assetstore name
-            input#g-new-gridfs-name.input-sm.form-control(type="text", placeholder="Name")
-          .form-group
-            label.control-label(for="g-new-gridfs-db") Database name
-            input#g-new-gridfs-db.input-sm.form-control(
-              type="text", placeholder="Database name")
-          .form-group
-            label.control-label(for="g-new-gridfs-mongohost") Mongo Host URI
-            input#g-new-gridfs-mongohost.input-sm.form-control(
-                type="text", placeholder="Mongo host uri (defaults to the main Girder database)",
-                title="The URI is of the form mongodb://[username:password@]host1[:port1][,host2[:port2],...[,hostN[:portN]]][/[database][?options]]")
-          .form-group
-            label.control-label(for="g-new-gridfs-replicaset") Replica Set
-            input#g-new-gridfs-replicaset.input-sm.form-control(
-                type="text", placeholder="Replica set name (blank if not using a replica set)")
-          p#g-new-gridfs-error.g-validation-failed-message
-          input.g-new-assetstore-submit.btn.btn-sm.btn-primary(type="submit", value="Create")
-
-  .panel.panel-default
-    .panel-heading(data-toggle="collapse",
-        data-parent="#g-assetstore-accordion",
         data-target="#g-create-s3-tab")
       .panel-title
         a
           i.icon-upload-cloud
           span Create new #[b Amazon S3] assetstore
     #g-create-s3-tab.panel-collapse.collapse
       .panel-body
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/rootSelectorWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/rootSelectorWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/sortCollectionWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/sortCollectionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/taskProgress.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/taskProgress.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/timeline.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/timeline.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/uploadWidgetMixins.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/uploadWidgetMixins.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/templates/widgets/userOtpEnable.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/userOtpEnable.pug`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/utilities/EventStream.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/utilities/EventStream.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/utilities/PluginUtils.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/utilities/PluginUtils.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/utilities/S3UploadHandler.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/utilities/S3UploadHandler.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/utilities/jquery/girderModal.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/utilities/jquery/girderModal.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/App.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/App.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/View.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/View.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,16 @@
 import _ from 'underscore';
 import Backbone from 'backbone';
 
 import events from '@girder/core/events';
 import eventStream from '@girder/core/utilities/EventStream';
 
 var View = Backbone.View.extend({
-    constructor: function(opts) { // eslint-disable-line backbone/no-constructor
+    // eslint-disable-next-line backbone/no-constructor
+    constructor: function(opts) {
         if (opts && _.has(opts, 'parentView')) {
             if (opts.parentView) {
                 opts.parentView.registerChildView(this);
                 this.parentView = opts.parentView;
             }
         } else {
             console.error('View created with no parentView property set. ' +
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/AdminView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/AdminView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/AssetstoresView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/AssetstoresView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/CollectionView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/CollectionView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/CollectionsView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/CollectionsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/FilesystemImportView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FilesystemImportView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/FolderView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FolderView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/FrontPageView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FrontPageView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/GroupView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/GroupView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/GroupsView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/GroupsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/ItemView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/PluginsView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/PluginsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/S3ImportView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/S3ImportView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/SearchResultsView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/SearchResultsView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/SystemConfigurationView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/SystemConfigurationView.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,7 @@
-import $ from 'jquery';
 import _ from 'underscore';
 
 import AccessWidget from '@girder/core/views/widgets/AccessWidget';
 import View from '@girder/core/views/View';
 import events from '@girder/core/events';
 import {
     restRequest,
@@ -29,22 +28,15 @@
             this.$('.g-submit-settings').girderEnable(false);
             this.$('#g-settings-error-message').empty();
 
             this.$('#g-core-collection-create-policy').val(JSON.stringify(this._covertCollectionCreationPolicy()));
             var settings = _.map(this.settingsKeys, (key) => {
                 const element = this.$('#g-' + key.replace(/[_.]/g, '-'));
 
-                if (key === 'core.route_table') {
-                    return {
-                        key,
-                        value: _.object(_.map($('.g-core-route-table'), function(el) {
-                            return [$(el).data('webrootName'), $(el).val()];
-                        }))
-                    };
-                } else if (_.contains(
+                if (_.contains(
                         [
                             'core.api_keys',
                             'core.enable_password_login',
                             'core.enable_notification_stream'
                         ],
                         key
                     )) { // booleans via checkboxes
@@ -110,15 +102,14 @@
             'core.enable_notification_stream',
             'core.cors.allow_origin',
             'core.cors.allow_methods',
             'core.cors.allow_headers',
             'core.add_to_group_policy',
             'core.collection_create_policy',
             'core.user_default_folders',
-            'core.route_table'
         ];
         this.settingsKeys = keys;
         restRequest({
             url: 'system/setting',
             method: 'GET',
             data: {
                 list: JSON.stringify(keys)
@@ -128,19 +119,14 @@
             this.render();
         });
     },
 
     render: function() {
         this.$el.html(SystemConfigurationTemplate({
             settings: this.settings,
-            routes: this.settings['core.route_table'],
-            routeKeys: _.sortBy(
-                _.keys(this.settings['core.route_table']),
-                (a) => a.indexOf('core_') === 0 ? -1 : 0
-            ),
             JSON: window.JSON
         }));
 
         var enableCollectionCreationPolicy = this.settings['core.collection_create_policy'] ? this.settings['core.collection_create_policy'].open : false;
 
         this.$('.g-setting-switch')
             .bootstrapSwitch()
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/UserAccountView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UserAccountView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/UserView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UserView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/UsersView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UsersView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/body/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/FooterView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/FooterView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/GlobalNavView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/GlobalNavView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/HeaderUserView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/HeaderUserView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/HeaderView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/LoginView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/LoginView.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
 
             this.$('#g-login-button').girderEnable(false);
             this.$('.g-validation-failed-message').text('');
 
             const loginName = this.$('#g-login').val();
             const password = this.$('#g-password').val();
             const otpToken = this.$('#g-login-otp-group').hasClass('hidden') ? null : this.$('#g-login-otp').val();
-            login(loginName, password, undefined, otpToken)
+            login(loginName, password, otpToken)
                 .done(() => {
                     this.$el.modal('hide');
                 })
                 .fail((err) => {
                     if (err.responseJSON.message.indexOf('Girder-OTP') !== -1 &&
                         this.$('#g-login-otp-group').hasClass('hidden')
                     ) {
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/ProgressListView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/ProgressListView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/RegisterView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/RegisterView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/ResetPasswordView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/ResetPasswordView.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/layout/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/AccessWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/AccessWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/ApiKeyListWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ApiKeyListWidget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -36,15 +36,15 @@
                     confirmCallback: toggleActive
                 });
             } else {
                 toggleActive();
             }
         },
 
-        'click .g-api-key-new': function(e) {
+        'click .g-api-key-new': function() {
             this._renderEditWidget();
         },
 
         'click .g-api-key-edit': function(e) {
             var apiKey = this._getModelFromEvent(e);
             this._renderEditWidget(apiKey);
         },
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/BrowserWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/BrowserWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/CheckedMenuWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/CheckedMenuWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/CollectionInfoWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/CollectionInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/DateTimeRangeWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/DateTimeRangeWidget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,16 @@
 import _ from 'underscore';
 import moment from 'moment';
 
 import View from '@girder/core/views/View';
 
 import dateTimeRangeWidgetTemplate from '@girder/core/templates/widgets/dateTimeRangeWidget.pug';
 
-import 'eonasdan-bootstrap-datetimepicker'; // /src/js/bootstrap-datetimepicker.js'
+// Momentjs is not require()'d in the way this library expects
+// import 'eonasdan-bootstrap-datetimepicker'; // /src/js/bootstrap-datetimepicker.js'
 import 'eonasdan-bootstrap-datetimepicker/build/css/bootstrap-datetimepicker.css';
 
 /**
  * This widget provides text input fields to specify a range of dates/times.
  * That is, the first field specifies "from" and the second field specifies
  * "to." The user chooses each date/time using a popup picker.
  */
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/DateTimeWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/DateTimeWidget.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,16 @@
 import _ from 'underscore';
 import moment from 'moment';
 
 import View from '@girder/core/views/View';
 
 import dateTimeWidgetTemplate from '@girder/core/templates/widgets/dateTimeWidget.pug';
 
-import 'eonasdan-bootstrap-datetimepicker'; // /src/js/bootstrap-datetimepicker.js'
+// Momentjs is not require()'d in the way this library expects
+// import 'eonasdan-bootstrap-datetimepicker'; // /src/js/bootstrap-datetimepicker.js'
 import 'eonasdan-bootstrap-datetimepicker/build/css/bootstrap-datetimepicker.css';
 
 /**
  * This widget provides a text input field to specify a date/time. The user
  * chooses the date/time using a popup picker.
  */
 var DateTimeWidget = View.extend({
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditApiKeyWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditApiKeyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditAssetstoreWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditAssetstoreWidget.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -103,29 +103,14 @@
     set: function() {
         var permStr = this.model.get('perms') ? this.model.get('perms').toString(8) : '600';
         this.$('#g-edit-fs-perms').val(permStr);
         this.$('#g-edit-fs-root').val(this.model.get('root'));
     }
 };
 
-fieldsMap[AssetstoreType.GRIDFS] = {
-    get: function() {
-        return {
-            db: this.$('#g-edit-gridfs-db').val(),
-            mongohost: this.$('#g-edit-gridfs-mongohost').val(),
-            replicaset: this.$('#g-edit-gridfs-replicaset').val()
-        };
-    },
-    set: function() {
-        this.$('#g-edit-gridfs-db').val(this.model.get('db'));
-        this.$('#g-edit-gridfs-mongohost').val(this.model.get('mongohost'));
-        this.$('#g-edit-gridfs-replicaset').val(this.model.get('replicaset'));
-    }
-};
-
 fieldsMap[AssetstoreType.S3] = {
     get: function() {
         return {
             bucket: this.$('#g-edit-s3-bucket').val(),
             prefix: this.$('#g-edit-s3-prefix').val(),
             accessKeyId: this.$('#g-edit-s3-access-key-id').val(),
             secret: this.$('#g-edit-s3-secret').val(),
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditCollectionWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditFileWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditFileWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditFolderWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditFolderWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditGroupWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditGroupWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/EditItemWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditItemWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/FileInfoWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FileInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/FileListWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FileListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/FolderInfoWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FolderInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/FolderListWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FolderListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupAdminsWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupAdminsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupInvitesWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupInvitesWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupMembersWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupMembersWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/GroupModsWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupModsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/HierarchyWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/ItemBreadcrumbWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ItemBreadcrumbWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/ItemListWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ItemListWidget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -279,15 +279,15 @@
             const widgetcontainer = this.$el.parents('.g-hierarchy-widget-container');
             // If the observer already exists disconnect it so it can be recreated
             if (this.observer && this.observer.disconnect) {
                 this.observer.disconnect();
             }
 
             // Event handler for loading images declared once
-            const onLoadImage = (event) => {
+            const onLoadImage = () => {
                 if (this.observer) {
                     this.centerSelected();
                 }
             };
 
             this.observer = new MutationObserver((mutations) => {
                 // for every mutation
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/MarkdownWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/MarkdownWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/MetadataWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/MetadataWidget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -95,15 +95,15 @@
             onMetadataEdited: this.onMetadataEdited,
             onMetadataAdded: this.onMetadataAdded
         }, overrides || {});
 
         this.parentView.modes[newEditorMode].editor(opts).render();
     },
 
-    editMetadata: function(event) {
+    editMetadata: function() {
         this.$el.addClass('editing');
         this.$el.empty();
 
         var opts = {
             item: this.parentView.item,
             key: this.$el.attr('g-key'),
             value: this.$el.attr('g-value'),
@@ -120,15 +120,17 @@
         if (this.mode === 'json') {
             try {
                 var jsonValue = JSON.parse(this.$el.attr('g-value'));
 
                 if (jsonValue !== undefined && !_.isObject(jsonValue)) {
                     opts.value = jsonValue;
                 }
-            } catch (e) {}
+            } catch (e) {
+                // ignore
+            }
         }
 
         this.parentView.modes[this.mode].editor(opts)
             .render()
             .$el.appendTo(this.$el);
     },
 
@@ -414,15 +416,17 @@
             validation: {
                 from: {
                     simple: [
                         function(value) {
                             try {
                                 JSON.parse(value);
                                 return true;
-                            } catch (e) {}
+                            } catch (e) {
+                                // ignore
+                            }
 
                             return false;
                         },
                         'The simple field is not valid JSON and can not be converted.'
                     ]
                 }
             },
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/NewAssetstoreWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/NewAssetstoreWidget.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -21,24 +21,14 @@
             this.createAssetstore(e, this.$('#g-new-fs-error'), {
                 type: AssetstoreType.FILESYSTEM,
                 name: this.$('#g-new-fs-name').val(),
                 root: this.$('#g-new-fs-root').val()
             });
         },
 
-        'submit #g-new-gridfs-form': function(e) {
-            this.createAssetstore(e, this.$('#g-new-gridfs-error'), {
-                type: AssetstoreType.GRIDFS,
-                name: this.$('#g-new-gridfs-name').val(),
-                db: this.$('#g-new-gridfs-db').val(),
-                mongohost: this.$('#g-new-gridfs-mongohost').val(),
-                replicaset: this.$('#g-new-gridfs-replicaset').val()
-            });
-        },
-
         'submit #g-new-s3-form': function(e) {
             this.createAssetstore(e, this.$('#g-new-s3-error'), {
                 type: AssetstoreType.S3,
                 name: this.$('#g-new-s3-name').val(),
                 bucket: this.$('#g-new-s3-bucket').val(),
                 prefix: this.$('#g-new-s3-prefix').val(),
                 accessKeyId: this.$('#g-new-s3-access-key-id').val(),
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/PaginateWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/PaginateWidget.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -4,18 +4,18 @@
 
 /**
  * This widget is used to provide a consistent widget for iterating amongst
  * pages of a Collection.
  */
 var PaginateWidget = View.extend({
     events: {
-        'click .g-page-next:not(.disabled)': function(e) {
+        'click .g-page-next:not(.disabled)': function() {
             this.collection.fetchNextPage();
         },
-        'click .g-page-prev:not(.disabled)': function(e) {
+        'click .g-page-prev:not(.disabled)': function() {
             this.collection.fetchPreviousPage();
         }
     },
 
     initialize: function(settings) {
         this.collection = settings.collection;
     },
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/PluginConfigBreadcrumbWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/PluginConfigBreadcrumbWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/RootSelectorWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/RootSelectorWidget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -133,15 +133,15 @@
         }
     },
 
     /**
      * Called when the user selects a new item.  Resolves the
      * model object from the DOM and triggers the g:selected event.
      */
-    _selectRoot: function(evt) {
+    _selectRoot: function() {
         var sel = this.$(':selected');
         var id = sel.val();
         var group = sel.data('group') || null;
         this.selected = null;
         if (_.has(this.groups, group)) {
             this.selected = this.groups[group].get(id);
         } else if (this._home && this._home.id === id) {
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/SearchFieldWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SearchFieldWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/SearchPaginateWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SearchPaginateWidget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -11,18 +11,18 @@
  * This widget is used to provide a consistent widget for iterating amongst
  * pages of a list of search results (using a search mode, a query, an unique type,
  * and a limit).
  */
 
 var SearchPaginateWidget = View.extend({
     events: {
-        'click .g-page-next:not(.disabled)': function(e) {
+        'click .g-page-next:not(.disabled)': function() {
             this._updateHasNextPage(true);
         },
-        'click .g-page-prev:not(.disabled)': function(e) {
+        'click .g-page-prev:not(.disabled)': function() {
             this._updateHasPreviousPage(true);
         }
     },
 
     initialize: function(settings) {
         this._type = settings.type;
         this._query = settings.query;
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/SortCollectionWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SortCollectionWidget.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
 var SortCollectionWidget = View.extend({
     events: {
         'click a.g-collection-sort-link': function(event) {
             var sortField = $(event.currentTarget).attr('g-sort');
             this.collection.sortField = sortField;
             this.collection.fetch({}, true);
         },
-        'click a.g-sort-order-button': function(event) {
+        'click a.g-sort-order-button': function() {
             if (this.collection.sortDir === SORT_ASC) {
                 this.collection.sortDir = SORT_DESC;
             } else {
                 this.collection.sortDir = SORT_ASC;
             }
             this.collection.fetch({}, true);
         }
```

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/TaskProgressWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/TaskProgressWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/TimelineWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/TimelineWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/UploadWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/UserOtpManagementWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/UserOtpManagementWidget.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/src/views/widgets/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/index.js`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder/web_client/static/img/Girder_Favicon.png` & `girder-5.0.0a2.dev10/girder/web/dist/Girder_Favicon.png`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/girder.egg-info/PKG-INFO` & `girder-5.0.0a2.dev10/girder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder
-Version: 3.2.3.dev7
+Version: 5.0.0a2.dev10
 Summary: Web-based data management platform
 Home-page: https://girder.readthedocs.org
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-3.2.3.dev7/package.json` & `girder-5.0.0a2.dev10/package.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8589368318256578%*

 * *Differences: {"'devDependencies'": "{'@girder/eslint-config': '^3.1.21', '@girder/pug-lint-config': '^3.1.21', "*

 * *                      "'@vue/eslint-config-prettier': '^7.1.0', '@vue/eslint-config-typescript': "*

 * *                      "'^11.0.3', 'esdoc': '^1.1.0', 'esdoc-standard-plugin': '^1.0.0', "*

 * *                      "'eslint-plugin-vue': '^9.11.0', delete: ['nyc', 'phantomjs-prebuilt']}",*

 * * "'esdoc'": "{'source': 'girder/web/src'}",*

 * * "'eslintConfig'": "{'extends': ['@girder', 'plugin:vue/vue3-essential', 'eslint:re […]*

```diff
@@ -1,24 +1,27 @@
 {
     "bugs": {
         "url": "https://github.com/girder/girder/issues"
     },
     "description": "Extensible data management platform",
     "devDependencies": {
-        "@girder/eslint-config": "file:./girder/web_client/eslint-config",
-        "@girder/pug-lint-config": "file:./girder/web_client/pug-lint-config",
+        "@girder/eslint-config": "^3.1.21",
+        "@girder/pug-lint-config": "^3.1.21",
+        "@vue/eslint-config-prettier": "^7.1.0",
+        "@vue/eslint-config-typescript": "^11.0.3",
+        "esdoc": "^1.1.0",
+        "esdoc-standard-plugin": "^1.0.0",
         "eslint": "^8.20.0",
         "eslint-config-semistandard": "^17.0.0",
         "eslint-config-standard": "^17.0.0",
         "eslint-plugin-backbone": "^2.1.1",
         "eslint-plugin-import": "^2.26.0",
         "eslint-plugin-n": "^15.3.0",
         "eslint-plugin-promise": "^6.0.0",
-        "nyc": "^15.1.0",
-        "phantomjs-prebuilt": "^2.1.16",
+        "eslint-plugin-vue": "^9.11.0",
         "pug-lint": "^2.6.0",
         "stylelint": "^15.11.0",
         "stylelint-stylus": "^0.18.0"
     },
     "engines": {
         "node": ">=10.0",
         "npm": ">=5.2"
@@ -36,73 +39,80 @@
                         "image": "girder/web_client/src/assets/Girder_Mark.png",
                         "repository": "https://github.com/girder/girder",
                         "title": "Girder"
                     }
                 }
             }
         ],
-        "source": "girder/web_client/src"
+        "source": "girder/web/src"
     },
     "eslintConfig": {
-        "extends": "@girder",
+        "extends": [
+            "@girder",
+            "plugin:vue/vue3-essential",
+            "eslint:recommended",
+            "@vue/eslint-config-typescript",
+            "@vue/eslint-config-prettier/skip-formatting"
+        ],
         "overrides": [
             {
                 "env": {
                     "jasmine": true,
                     "jquery": true
                 },
                 "files": [
-                    "girder/web_client/test/**",
-                    "plugins/*/plugin_tests/**"
+                    "girder/web/**",
+                    "plugins/*/plugin_tests/**",
+                    "plugins/**/web_client/**"
                 ],
                 "globals": {
                     "Backbone": true,
                     "_": true,
                     "girder": true,
                     "girderTest": true,
                     "moment": true
+                },
+                "parserOptions": {
+                    "ecmaVersion": "latest"
                 }
             }
         ],
-        "root": true
+        "root": true,
+        "rules": {
+            "promise/no-native": 0
+        }
     },
     "eslintIgnore": [
-        "build/",
-        "girder/web_client/test/lib/",
+        "dist/",
+        "dist-lib/",
         "**/node_modules/"
     ],
     "homepage": "https://girder.readthedocs.org",
     "license": "Apache-2.0",
     "name": "@girder/lint",
-    "nyc": {
-        "report-dir": "build/test/artifacts/web_coverage",
-        "reporter": [
-            "cobertura",
-            "html",
-            "text-summary"
-        ],
-        "temp-dir": "build/test/coverage/web_temp"
-    },
     "pugLintConfig": {
         "excludeFiles": [
             "**/node_modules/",
             "**/.tox/"
         ],
         "extends": "@girder/pug-lint-config"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/girder/girder.git"
     },
     "scripts": {
-        "coverage": "nyc report && mv build/test/artifacts/web_coverage/cobertura-coverage.xml build/test/coverage/",
         "docs": "esdoc",
         "lint": "eslint --cache . && pug-lint . && stylelint **/*.styl",
         "publish-all": "./.circleci/publish_npm.sh"
     },
     "stylelint": {
         "extends": [
             "stylelint-stylus/standard"
+        ],
+        "ignoreFiles": [
+            "girder/web/dist/**/*.styl",
+            "girder/web/dist-lib/**/*.styl"
         ]
     },
     "version": "0.0.0"
 }
```

### Comparing `girder-3.2.3.dev7/plugins/autojoin/setup.py` & `girder-5.0.0a2.dev10/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,100 @@
 import os
+import re
 
-from setuptools import find_packages, setup
+from setuptools import setup
 
 
 def prerelease_local_scheme(version):
     """Return local scheme version unless building on master in CircleCI.
     This function returns the local scheme version number
     (e.g. 0.0.0.dev<N>+g<HASH>) unless building on CircleCI for a
     pre-release in which case it ignores the hash and produces a
     PEP440 compliant pre-release version number (e.g. 0.0.0.dev<N>).
     """
     from setuptools_scm.version import get_local_node_and_date
 
-    if os.getenv('CIRCLE_BRANCH') == 'master':
+    # this regex allows us to publish pypi packages from master, our LTS maintenance branches, and
+    # our next major version integration branches
+    pattern = r'master|[0-9]+\.x-maintenance|v[0-9]+-integration'
+
+    if re.match(pattern, os.getenv('CIRCLE_BRANCH', '')):
         return ''
     else:
         return get_local_node_and_date(version)
 
 
-# perform the install
+with open('README.rst') as f:
+    readme = f.read()
+
+installReqs = [
+    'boto3',
+    'botocore',
+    'CherryPy',
+    'click',
+    'click-plugins',
+    'dogpile.cache',
+    'filelock',
+    'jsonschema',
+    'Mako',
+    'passlib [bcrypt,totp]',
+    'pymongo>=3.6,<4',
+    'PyYAML',
+    'psutil',
+    'pyOpenSSL',
+    'python-dateutil',
+    'pytz',
+    'requests',
+]
+
+extrasReqs = {
+    'sftp': [
+        'paramiko'
+    ],
+    'mount': [
+        'cachetools',
+        'diskcache',
+        'fusepy>=3.0'
+    ]
+}
+
 setup(
-    name='girder-autojoin',
-    use_scm_version={'root': '../..', 'local_scheme': prerelease_local_scheme},
+    name='girder',
+    use_scm_version={'local_scheme': prerelease_local_scheme},
     setup_requires=[
         'setuptools-scm',
-        'setuptools-git',
     ],
-    description='Automatically assign new users to groups based on their email domain',
+    description='Web-based data management platform',
+    long_description=readme,
     author='Kitware, Inc.',
     author_email='kitware@kitware.com',
-    url='http://girder.readthedocs.io/en/latest/plugins.html#auto-join',
+    url='https://girder.readthedocs.org',
     license='Apache 2.0',
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
-    include_package_data=True,
     python_requires='>=3.8',
-    packages=find_packages(exclude=['plugin_tests']),
+    packages=['girder'],
+    include_package_data=True,
+    install_requires=installReqs,
+    extras_require=extrasReqs,
     zip_safe=False,
-    install_requires=['girder>=3'],
     entry_points={
-        'girder.plugin': [
-            'autojoin = girder_autojoin:AutojoinPlugin'
+        'console_scripts': [
+            'girder-server = girder.cli.serve:main',
+            'girder-sftpd = girder.cli.sftpd:main',
+            'girder-shell = girder.cli.shell:main',
+            'girder = girder.cli:main'
+        ],
+        'girder.cli_plugins': [
+            'serve = girder.cli.serve:main',
+            'mount = girder.cli.mount:main',
+            'shell = girder.cli.shell:main',
+            'sftpd = girder.cli.sftpd:main',
         ]
     }
 )
```

### Comparing `girder-3.2.3.dev7/plugins/ldap/setup.py` & `girder-5.0.0a2.dev10/pytest_girder/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,38 +14,34 @@
 
     if os.getenv('CIRCLE_BRANCH') == 'master':
         return ''
     else:
         return get_local_node_and_date(version)
 
 
-# perform the install
 setup(
-    name='girder-ldap',
-    use_scm_version={'root': '../..', 'local_scheme': prerelease_local_scheme},
+    name='pytest-girder',
+    use_scm_version={'root': '..', 'local_scheme': prerelease_local_scheme},
     setup_requires=[
         'setuptools-scm',
-        'setuptools-git',
     ],
-    description='Authenticate user credentials against LDAP or Active Directory servers.',
+    description='A set of pytest fixtures for testing Girder applications.',
     author='Kitware, Inc.',
     author_email='kitware@kitware.com',
     license='Apache 2.0',
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Web Environment',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
+        'Framework :: Pytest'
     ],
-    include_package_data=True,
     python_requires='>=3.8',
-    packages=find_packages(exclude=['plugin_tests']),
-    zip_safe=False,
-    install_requires=['girder>=3', 'pyldap'],
+    packages=find_packages(),
+    install_requires=[
+        'girder>=3',
+        'mongomock',
+        'pytest>=3.6',
+        'pytest-cov',
+        'pymongo'
+    ],
     entry_points={
-        'girder.plugin': [
-            'ldap= girder_ldap:LDAPPlugin'
+        'pytest11': [
+            'girder = pytest_girder.plugin'
         ]
-    }
-)
+    })
```

### Comparing `girder-3.2.3.dev7/pytest_girder/pytest_girder/assertions.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/assertions.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/pytest_girder/pytest_girder/fixtures.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,18 +133,14 @@
 
 
 @pytest.fixture
 def smtp(db, server):
     """
     Provides a mock SMTP server for testing.
     """
-    # TODO strictly speaking, this does not depend on the server itself, but does
-    # depend on the events daemon, which is currently managed by the server fixture.
-    # We should sort this out so that the daemon is its own fixture rather than being
-    # started/stopped via the cherrypy server lifecycle.
     from girder.models.setting import Setting
     from girder.settings import SettingKey
 
     receiver = MockSmtpReceiver()
     receiver.start()
 
     host, port = receiver.address
```

### Comparing `girder-3.2.3.dev7/pytest_girder/pytest_girder/plugin.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/plugin.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/pytest_girder/pytest_girder/plugin_registry.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/plugin_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,7 +77,8 @@
         try:
             with unittest.mock.patch.object(
                     plugin, 'iter_entry_points', side_effect=self._iter_entry_points) as mock_:
                 yield mock_
         finally:
             plugin._pluginRegistry = None
             plugin._pluginLoadOrder = []
+            plugin._pluginStaticContent.clear()
```

### Comparing `girder-3.2.3.dev7/pytest_girder/pytest_girder/utils.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import base64
 import cherrypy
 import contextlib
+from dataclasses import dataclass
 import email
 import errno
 import io
 import json
 import os
 import queue
 import socket
 import threading
 import time
+from typing import Optional
 import urllib.parse
 
 _startPort = 31000
 _maxTries = 100
 
 
 class MockSmtpReceiver:
@@ -133,15 +135,15 @@
     return data
 
 
 def request(path='/', method='GET', params=None, user=None,
             prefix='/api/v1', isJson=True, basicAuth=None, body=None,
             type=None, exception=False, cookie=None, token=None,
             additionalHeaders=None, useHttps=False,
-            authHeader='Authorization', appPrefix=''):
+            authHeader='Authorization', appPrefix='/api'):
     """
     Make an HTTP request.
 
     :param path: The path part of the URI.
     :type path: str
     :param method: The HTTP method.
     :type method: str
@@ -290,51 +292,58 @@
 
 def _findFreePort():
     with contextlib.closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
         sock.bind(('', 0))
         return sock.getsockname()[1]
 
 
+@dataclass
+class ServerFixture:
+    request = staticmethod(request)
+    uploadFile = staticmethod(uploadFile)
+    serverRoot: cherrypy._cptree.Tree
+    boundPort: Optional[int] = None
+
+    def __getattr__(self, name):
+        return getattr(self.serverRoot, name)
+
+
 @contextlib.contextmanager
-def serverContext(plugins=None, bindPort=False):
-    # The event daemon cannot be restarted since it is a threading.Thread
-    # object, however all references to girder.events.daemon are a singular
-    # global daemon due to its side effect on import. We have to hack around
-    # this by creating a unique event daemon each time we startup the server
-    # and assigning it to the global.
-    import girder.events
+def serverContext(plugins=None, bindPort=False) -> ServerFixture:
+    from girder import plugin
     from girder.api import docs
-    from girder.utility.server import setup as setupServer
+    from girder.utility.server import create_app
     from girder.constants import ServerMode
 
-    girder.events.daemon = girder.events.AsyncEventsThread()
-
     if plugins is None:
         # By default, pass "[]" to "plugins", disabling any installed plugins
         plugins = []
-    server = setupServer(mode=ServerMode.TESTING, plugins=plugins)
-    server.request = request
-    server.uploadFile = uploadFile
+    app_info = create_app(mode=ServerMode.TESTING)
+    plugin._loadPlugins(app_info, plugins)
+
+    server_fixture = ServerFixture(serverRoot=app_info['serverRoot'])
+
+    cherrypy.tree = app_info['serverRoot']
     cherrypy.server.unsubscribe()
     if bindPort:
         cherrypy.server.subscribe()
         port = _findFreePort()
         cherrypy.config['server.socket_port'] = port
-        server.boundPort = port
+        server_fixture.boundPort = port
         # This is needed if cherrypy started once on another port
         cherrypy.server.socket_port = port
-    cherrypy.config.update({'environment': 'embedded',
-                            'log.screen': False,
-                            'request.throw_errors': True})
+    cherrypy.config.update({
+        'environment': 'embedded',
+        'log.screen': False,
+        'request.throw_errors': True
+    })
     cherrypy.engine.start()
 
     try:
-        yield server
+        yield server_fixture
     finally:
-        cherrypy.engine.unsubscribe('start', girder.events.daemon.start)
-        cherrypy.engine.unsubscribe('stop', girder.events.daemon.stop)
         cherrypy.engine.stop()
         cherrypy.engine.exit()
         cherrypy.tree.apps = {}
         # This is needed to allow cherrypy to restart on another port
         cherrypy.server.httpserver = None
         docs.routes.clear()
```

### Comparing `girder-3.2.3.dev7/pytest_girder/pytest_girder/web_client.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/web_client.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/requirements-dev.txt` & `girder-5.0.0a2.dev10/requirements-dev.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 -e pytest_girder
 -e plugins/jobs
 
 # The following are top level dependencies.
 -e plugins/audit_logs
 -e plugins/authorized_upload
 -e plugins/autojoin
--e plugins/dicom_viewer
 -e plugins/download_statistics
 -e plugins/google_analytics
 -e plugins/gravatar
 -e plugins/hashsum_download
 -e plugins/homepage
 -e plugins/item_licenses
 -e plugins/ldap
@@ -22,16 +21,15 @@
 -e plugins/thumbnails
 -e plugins/user_quota
 -e plugins/virtual_folders
 
 # External dependencies
 configparser
 coverage
-girder-worker
 httmock
 mongomock
 moto[server]<4.2.12
-pytest
-pytest-cov
+pytest>=3.6
+pytest-cov>=2.6
 python-dateutil
 tox
 virtualenv
```

### Comparing `girder-3.2.3.dev7/scripts/midas/README.rst` & `girder-5.0.0a2.dev10/scripts/midas/README.rst`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/scripts/midas/migrate.py` & `girder-5.0.0a2.dev10/scripts/midas/migrate.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/scripts/midas/walk_girder.py` & `girder-5.0.0a2.dev10/scripts/midas/walk_girder.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/scripts/midas/walk_midas.py` & `girder-5.0.0a2.dev10/scripts/midas/walk_midas.py`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/scripts/publicNames.py` & `girder-5.0.0a2.dev10/scripts/publicNames.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 EXCLUDE_DIRS = [
     # Only look in girder, plugins and clients folders i.e. exclude all directories that don't begin
     # with "clients" or "girder" or "plugins"
     '^(?!(clients|girder|plugins|pytest_girder))',
     # Exclude plugin tests
     'plugin_tests',
     '\\.egg/',
+    '\\.eggs/',
     'node_modules/']
 
 IGNORE_FILES = ['setup.py']
 
 excluder = re.compile('|'.join(EXCLUDE_DIRS))
 
 baseTree = Tree()
```

### Comparing `girder-3.2.3.dev7/scripts/publicNames.txt` & `girder-5.0.0a2.dev10/scripts/publicNames.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,21 +72,14 @@
             IncorrectUploadLengthError
             REQ_BUFFER_SIZE
             cli
                 GirderCli
                     sendRestRequest
                 main
 girder
-    LogFormatter
-        format
-        formatException
-    LogLevelFilter
-        filter
-    StreamToLogger
-        write
     api
         access
             admin
             public
             token
             user
         api_main
@@ -297,21 +290,18 @@
                 LOG_BUF_SIZE
                 ModuleStartTime
                 System
                     discardPartialUploads
                     getAccessFlags
                     getCollectionCreationPolicyAccess
                     getConfigurationOption
-                    getLog
-                    getLogLevel
-                    getPartialUploads
                     getPlugins
+                    getPublicSettings
                     getSetting
                     getVersion
-                    setLogLevel
                     setSetting
                     systemConsistencyCheck
                     systemStatus
                     unsetSetting
             token
                 Token
                     currentSession
@@ -377,49 +367,32 @@
             NONE
             READ
             SITE_ADMIN
             WRITE
             validate
         AssetstoreType
             FILESYSTEM
-            GRIDFS
             S3
         CoreEventHandler
             ACCESS_CONTROL_CLEANUP
             FILE_PROPAGATE_SIZE
             GROUP_CREATOR_ACCESS
             USER_DEFAULT_FOLDERS
             USER_SELF_ACCESS
-            WEBROOT_SETTING_CHANGE
-        GIRDER_ROUTE_ID
-        LOG_BACKUP_COUNT
-        LOG_ROOT
-        MAX_LOG_SIZE
         PACKAGE_DIR
         ROOT_DIR
-        STATIC_PREFIX
         STATIC_ROOT_DIR
         ServerMode
             DEVELOPMENT
             PRODUCTION
             TESTING
         SortDir
             ASCENDING
             DESCENDING
         TEXT_SCORE_SORT_MAX
-        TerminalColor
-            ENDC
-            ERROR
-            INFO
-            SUCCESS
-            WARNING
-            error
-            info
-            success
-            warning
         TokenScope
             ANONYMOUS_SESSION
             ASSETSTORES_READ
             DATA_OWN
             DATA_READ
             DATA_WRITE
             EMAIL_VERIFICATION
@@ -440,54 +413,44 @@
             run
             stop
             trigger
         Event
             addResponse
             preventDefault
             stopPropagation
-        ForegroundEventsDaemon
-            start
-            stop
-            trigger
         bind
         bound
-        daemon
-        setupDaemon
         trigger
         unbind
         unbindAll
     exceptions
         AccessException
         FilePathException
             identifier
         GirderBaseException
         GirderException
         NoAssetstoreAdapter
             identifier
         ResourcePathNotFound
         RestException
         ValidationException
-    getLogPaths
-    logStdoutStderr
     logger
-    logprint
     models
         api_key
             ApiKey
                 createApiKey
                 createToken
                 initialize
                 list
                 remove
                 validate
         assetstore
             Assetstore
                 addComputedInfo
                 createFilesystemAssetstore
-                createGridFsAssetstore
                 createS3Assetstore
                 getCurrent
                 importData
                 initialize
                 list
                 remove
                 validate
@@ -719,17 +682,15 @@
             loaded
             name
             npmPackages
             url
             version
         allPlugins
         getPlugin
-        getPluginWebroots
         loadedPlugins
-        registerPluginWebroot
     settings
         SettingDefault
             defaults
         SettingKey
             ADD_TO_GROUP_POLICY
             API_KEYS
             BANNER_COLOR
@@ -743,18 +704,16 @@
             CORS_EXPOSE_HEADERS
             EMAIL_FROM_ADDRESS
             EMAIL_HOST
             EMAIL_VERIFICATION
             ENABLE_NOTIFICATION_STREAM
             ENABLE_PASSWORD_LOGIN
             GIRDER_MOUNT_INFORMATION
-            HTTP_ONLY_COOKIES
             PRIVACY_NOTICE
             REGISTRATION_POLICY
-            ROUTE_TABLE
             SERVER_ROOT
             SMTP_ENCRYPTION
             SMTP_HOST
             SMTP_PASSWORD
             SMTP_PORT
             SMTP_USERNAME
             UPLOAD_MINIMUM_CHUNK_SIZE
@@ -838,35 +797,20 @@
                 importData
                 importFile
                 initUpload
                 requestOffset
                 uploadChunk
                 validateInfo
         genToken
-        gridfs_assetstore_adapter
-            CHUNK_SIZE
-            GridFsAssetstoreAdapter
-                cancelUpload
-                deleteFile
-                downloadFile
-                fileIndexFields
-                finalizeUpload
-                initUpload
-                requestOffset
-                uploadChunk
-                validateInfo
-            RECENT_CONNECTION_CACHE_MAX_SIZE
-            RECENT_CONNECTION_CACHE_TIME
         mail_utils
             addTemplateDirectory
             getEmailUrlPrefix
             renderTemplate
             sendMail
             sendMailIndividually
-            sendMailSync
             sendMailToAdmins
             validateEmailAddress
         mkdir
         model_importer
             ModelImporter
                 model
                 registerModel
@@ -908,19 +852,15 @@
                 validateInfo
             makeBotoConnectParams
         search
             addSearchMode
             getSearchModeHandler
             removeSearchMode
         server
-            configureServer
-            getApiRoot
-            getStaticPublicPath
-            loadRouteTable
-            setup
+            create_app
             staticFile
         setting_utilities
             default
             getDefaultFunction
             getValidator
             registerDefaultFunction
             registerValidator
```

### Comparing `girder-3.2.3.dev7/scripts/test_names.sh` & `girder-5.0.0a2.dev10/scripts/test_names.sh`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/setup.cfg` & `girder-5.0.0a2.dev10/setup.cfg`

 * *Files identical despite different names*

### Comparing `girder-3.2.3.dev7/tox.ini` & `girder-5.0.0a2.dev10/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -37,41 +37,25 @@
 # configuration possible.
 skip_install = true
 skipsdist = true
 # Building docs has a direct dependency on Sphinx. Documentation dependencies are listed in a
 # separate file to allow readthedocs.org to read and install them.
 deps =
     -rdocs/requirements-docs.txt
+setenv =
+    GIRDER_SPHINX_BUILD = true
 commands =
     pip install --no-deps --editable . --editable clients/python
     sphinx-build \
         -W \
         -b html \
         -d {envtmpdir}/doctrees \
         docs \
         build/docs/python
 
-[testenv:ansible]
-skip_install = true
-skipsdist = true
-changedir = devops/ansible-role-girder
-passenv =
-    DOCKER_*
-deps =
-    ansible-lint<5
-    bcrypt
-    rich<11
-    flake8
-    molecule[ansible,docker]
-    pytest
-    pytest-testinfra
-    yamllint
-commands =
-    molecule {posargs: test --all}
-
 [testenv:coverage]
 skip_install = true
 skipsdist = true
 deps =
     coverage
 commands =
     coverage combine
@@ -85,33 +69,21 @@
 skip_install = true
 skipsdist = true
 passenv =
     CIRCLE_BRANCH
     TWINE_USERNAME
     TWINE_PASSWORD
 deps =
+    build
     setuptools-git
     setuptools-scm
     twine
 commands =
     {toxinidir}/.circleci/publish_pypi.sh
 
-[testenv:release_ansible]
-allowlist_externals =
-    {toxinidir}/.circleci/create_ansible_subtree.sh
-skip_install = true
-skipsdist = true
-passenv =
-    ANSIBLE_GALAXY_API_KEY
-deps =
-    ansible
-commands =
-    {toxinidir}/.circleci/create_ansible_subtree.sh
-    ansible-galaxy import --api-key {env:ANSIBLE_GALAXY_API_KEY} girder ansible-role-girder
-
 [testenv:public_names]
 allowlist_externals =
     {toxinidir}/scripts/test_names.sh
 commands =
     {toxinidir}/scripts/test_names.sh
 
 [testenv:pytest_circleci]
@@ -130,21 +102,22 @@
 
 [flake8]
 max-line-length = 100
 show-source = True
 max-complexity = 14
 format = pylint
 exclude =
-    devops/vagrant/roles,
     node_modules,
     .eggs,
     .git,
     __pycache__,
     .tox
 ignore =
+    # B019 - Use of `functools.lru_cache` or `functools.cache` on methods can lead to memory leaks.
+    B019,
     # D10 - Missing docstring (errors D100 - D107)
     D10,
     # D200 - One-line docstrings should fit on one line with quotes.
     D200,
     # D205 - Blank line required between one-line summary and description.
     D205,
     # D400 - First line should end with a period.
```


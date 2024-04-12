# Comparing `tmp/infrahouse-toolkit-2.9.6.tar.gz` & `tmp/infrahouse-toolkit-2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahouse-toolkit-2.9.6.tar", last modified: Sat Dec 30 19:47:03 2023, max compression
+gzip compressed data, was "infrahouse-toolkit-2.9.7.tar", last modified: Sun Dec 31 19:55:34 2023, max compression
```

## Comparing `infrahouse-toolkit-2.9.6.tar` & `infrahouse-toolkit-2.9.7.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.826158 infrahouse-toolkit-2.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2023-12-30 19:47:03.826158 infrahouse-toolkit-2.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.806158 infrahouse-toolkit-2.9.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.ih_plan.cmd_min_permissions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.ih_plan.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.backends.rst
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.backends.tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.tests.status.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.806158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/config/test_aws_home.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/config/test_get_account_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/config/test_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_instance_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_instance_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_launch/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_launch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_launch_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_launch_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_list/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_subnets/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_subnets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_terminate/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_terminate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_download/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.810158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.814158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_load_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_parse_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/test_min_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.814158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_publish/
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.814158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_remove/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.814158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.814158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_puppet/
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_puppet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.814158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_puppet/cmd_apply/
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_puppet/cmd_apply/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.818158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.818158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/tests/test_get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.818158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.818158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/tests/test_system_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.818158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.818158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/s3backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.818158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.822158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/s3backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/githubpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.822158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.822158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/github_pr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/github_pr/test_publish_gist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.822158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/test_parse_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/test_parse_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.822158 infrahouse-toolkit-2.9.6/infrahouse_toolkit/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 19:47:03.822158 infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2023-12-30 19:47:03.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2023-12-30 19:47:03.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-30 19:47:03.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-30 19:47:03.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-30 19:46:44.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-30 19:47:03.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-30 19:47:03.000000 infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-30 19:47:03.826158 infrahouse-toolkit-2.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-30 19:46:17.000000 infrahouse-toolkit-2.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.707095 infrahouse-toolkit-2.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2023-12-31 19:55:34.707095 infrahouse-toolkit-2.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.691095 infrahouse-toolkit-2.9.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_min_permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.ih_plan.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.backends.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.tests.status.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.691095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.691095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.691095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.691095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/config/test_aws_home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/config/test_get_account_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/config/test_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_instance_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_instance_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_launch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_launch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_launch_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_launch_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_list/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_subnets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_subnets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_terminate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_terminate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_download/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_load_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_parse_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/test_min_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_publish/
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_remove/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.695095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.699095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_puppet/
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_puppet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.699095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_puppet/cmd_apply/
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_puppet/cmd_apply/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.699095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.699095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/tests/test_get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.699095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.703095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/tests/test_system_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.703095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.703095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/s3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.703095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.703095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/s3backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/githubpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.703095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.707095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/github_pr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/github_pr/test_publish_gist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.707095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/test_parse_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/test_parse_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.707095 infrahouse-toolkit-2.9.7/infrahouse_toolkit/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 19:55:34.707095 infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2023-12-31 19:55:34.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2023-12-31 19:55:34.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 19:55:34.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-31 19:55:34.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 19:55:17.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-31 19:55:34.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-31 19:55:34.000000 infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-31 19:55:34.707095 infrahouse-toolkit-2.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-31 19:54:53.000000 infrahouse-toolkit-2.9.7/setup.py
```

### Comparing `infrahouse-toolkit-2.9.6/CONTRIBUTING.rst` & `infrahouse-toolkit-2.9.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/LICENSE` & `infrahouse-toolkit-2.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/PKG-INFO` & `infrahouse-toolkit-2.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 2.9.6
+Version: 2.9.7
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-2.9.6/README.rst` & `infrahouse-toolkit-2.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/Makefile` & `infrahouse-toolkit-2.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/conf.py` & `infrahouse-toolkit-2.9.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.cli.tests.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.cli.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.backends.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.backends.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.backends.tests.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.backends.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.tests.github_pr.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.tests.github_pr.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.tests.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/infrahouse_toolkit.terraform.tests.status.rst` & `infrahouse-toolkit-2.9.7/docs/infrahouse_toolkit.terraform.tests.status.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/installation.rst` & `infrahouse-toolkit-2.9.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/docs/usage.rst` & `infrahouse-toolkit-2.9.7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/config.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/config.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/config/test_get_account_id.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/config/test_get_account_id.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/aws/tests/config/test_profiles.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/aws/tests/config/test_profiles.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_instance_types/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_instance_types/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_launch/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_launch/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_launch_templates/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_launch_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_list/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_list/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_subnets/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_subnets/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_ec2/cmd_terminate/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_ec2/cmd_terminate/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,17 +93,33 @@
             "iam:CreateServiceLinkedRole",
             "ec2:CreateTags",
             "ec2:RunInstances",
         ],
         "autoscaling:UpdateAutoScalingGroup": ["iam:PassRole"],
         "elasticloadbalancing:CreateLoadBalancer": ["elasticloadbalancing:AddTags"],
         "iam:AddRoleToInstanceProfile": ["iam:PassRole"],
+        "iam:CreateInstanceProfile": ["iam:TagInstanceProfile"],
         "ec2:CreateLaunchTemplate": ["ec2:CreateTags"],
         "ec2:ImportKeyPair": ["ec2:CreateTags"],
         "ec2:RunInstances": ["ec2:CreateTags"],
+        "logs:CreateLogGroup": ["logs:TagResource"],
+        "lambda:CreateFunction": ["lambda:TagResource"],
+        "s3:CreateBucket": ["s3:PutBucketTagging"],
+        "s3:PutObject": [
+            "kms:Decrypt",
+            "kms:CreateGrant",
+            "kms:DescribeKey",
+            "kms:Encrypt",
+            "s3:AbortMultipartUpload",
+            "s3:GetObject",
+            "s3:ListMultipartUploadParts",
+            "s3:PutObjectTagging",
+        ],
+        "events:PutRule": ["events:TagResource"],
+        "events:PutTargets": ["events:TagResource"],
     }
 
     def __init__(self):
         self._actions = set()
 
     @property
     def actions(self) -> list:
```

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_parse_trace.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/actionlist/test_parse_trace.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,77 @@
 from textwrap import dedent
 
 import pytest
 
 from infrahouse_toolkit.cli.ih_plan.cmd_min_permissions import ActionList
 
 
-def test_parse_trace(tmpdir):
+@pytest.mark.parametrize(
+    "trace, expected_actions",
+    [
+        (
+            '{"aws.operation": "PutScalingPolicy","aws.service": "Auto Scaling"}',
+            [
+                "autoscaling:PutScalingPolicy",
+            ],
+        ),
+        (
+            '{"aws.operation": "DescribePolicies","aws.service": "Auto Scaling"}',
+            [
+                "autoscaling:DescribePolicies",
+            ],
+        ),
+        (
+            '{"rpc.method": "DescribeLogGroups", "rpc.service": "CloudWatch Logs"}',
+            [
+                "logs:DescribeLogGroups",
+            ],
+        ),
+        (
+            '{"rpc.method": "ListTargetsByRule", "rpc.service": "EventBridge"}',
+            [
+                "events:ListTargetsByRule",
+            ],
+        ),
+        (
+            '{"rpc.method": "CompleteMultipartUpload", "rpc.service": "s3"}',
+            [
+                "kms:CreateGrant",
+                "kms:Decrypt",
+                "kms:DescribeKey",
+                "kms:Encrypt",
+                "s3:AbortMultipartUpload",
+                "s3:GetObject",
+                "s3:ListMultipartUploadParts",
+                "s3:PutObject",
+                "s3:PutObjectTagging",
+            ],
+        ),
+        (
+            '{"rpc.method": "UploadPart", "rpc.service": "s3"}',
+            [
+                "kms:CreateGrant",
+                "kms:Decrypt",
+                "kms:DescribeKey",
+                "kms:Encrypt",
+                "s3:AbortMultipartUpload",
+                "s3:GetObject",
+                "s3:ListMultipartUploadParts",
+                "s3:PutObject",
+                "s3:PutObjectTagging",
+            ],
+        ),
+    ],
+)
+def test_parse_trace(trace, expected_actions, tmpdir):
     tracefile = tmpdir.join("trace")
-    tracefile.write(
-        dedent(
-            """
-            {"aws.operation": "PutScalingPolicy","aws.service": "Auto Scaling"}
-            {"aws.operation": "DescribePolicies","aws.service": "Auto Scaling"}
-            {"rpc.method": "DescribeLogGroups", "rpc.service": "CloudWatch Logs"}
-            {"rpc.method": "ListTargetsByRule", "rpc.service": "EventBridge"}
-            {"rpc.method": "CreateMultipartUpload", "rpc.service": "s3"}
-            {"rpc.method": "UploadPart", "rpc.service": "s3"}
-            {"rpc.method": "CompleteMultipartUpload", "rpc.service": "s3"}
-            """
-        )
-    )
+    tracefile.write(trace)
     actions = ActionList()
     actions.parse_trace(str(tracefile))
-    assert actions.actions == [
-        "autoscaling:DescribePolicies",
-        "autoscaling:PutScalingPolicy",
-        "events:ListTargetsByRule",
-        "logs:DescribeLogGroups",
-        "s3:PutObject",
-    ]
+    assert actions.actions == expected_actions
 
 
 @pytest.mark.parametrize(
     "trace_content, expected_permissions",
     [
         (
             dedent(
@@ -61,15 +100,15 @@
         (
             dedent(
                 """
                 {"rpc.method": "CreateBucket", "rpc.service": "S3"}
                 {"rpc.method": "CreateTable", "rpc.service": "DynamoDB"}
                 """
             ),
-            ["s3:CreateBucket", "dynamodb:CreateTable"],
+            ["s3:CreateBucket", "dynamodb:CreateTable", "s3:PutBucketTagging"],
         ),
         (
             dedent(
                 """
                 {"aws.operation": "DeletePublicAccessBlock","aws.service": "S3"}
                 {"aws.operation": "GetPublicAccessBlock","aws.service": "S3"}
                 {"aws.operation": "PutPublicAccessBlock","aws.service": "S3"}
```

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/test_min_permissions.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/tests/test_min_permissions.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_puppet/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_puppet/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_puppet/cmd_apply/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_puppet/cmd_apply/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/lib.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/lib.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/cli/tests/conftest.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/base.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/base.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/system.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/system.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/lock/tests/test_system_lock.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/lock/tests/test_system_lock.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/logging.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/__init__.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/s3backend.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/s3backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/backends/tfbackend.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/backends/tfbackend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/githubpr.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/githubpr.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/status.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/status.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_comment.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_eq.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_eq.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_metadata.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_metadata.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/test_parse_comment.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/test_parse_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/terraform/tests/test_parse_plan.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/terraform/tests/test_parse_plan.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit/timeout.py` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit/timeout.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/PKG-INFO` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 2.9.6
+Version: 2.9.7
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-2.9.6/infrahouse_toolkit.egg-info/SOURCES.txt` & `infrahouse-toolkit-2.9.7/infrahouse_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.9.6/setup.cfg` & `infrahouse-toolkit-2.9.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.9.6
+current_version = 2.9.7
 commit = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
 
 [bumpversion:file(pycode):infrahouse_toolkit/__init__.py]
```

### Comparing `infrahouse-toolkit-2.9.6/setup.py` & `infrahouse-toolkit-2.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,10 +59,10 @@
     include_package_data=True,
     keywords="infrahouse-toolkit",
     name="infrahouse-toolkit",
     packages=find_packages(include=["infrahouse_toolkit", "infrahouse_toolkit.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/infrahouse/infrahouse-toolkit",
-    version="2.9.6",
+    version="2.9.7",
     zip_safe=False,
 )
```


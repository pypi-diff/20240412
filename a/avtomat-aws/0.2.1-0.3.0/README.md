# Comparing `tmp/avtomat_aws-0.2.1.tar.gz` & `tmp/avtomat_aws-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avtomat_aws-0.2.1.tar", max compression
+gzip compressed data, was "avtomat_aws-0.3.0.tar", max compression
```

## Comparing `avtomat_aws-0.2.1.tar` & `avtomat_aws-0.3.0.tar`

### file list

```diff
@@ -1,125 +1,130 @@
--rw-r--r--   0        0        0     1733 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0    18091 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/LICENSE
--rw-r--r--   0        0        0     3838 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/README.md
--rw-r--r--   0        0        0       69 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/backup/create_backups.py
--rw-r--r--   0        0        0      864 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/backup/delete_backups.py
--rw-r--r--   0        0        0      928 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     1156 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     1145 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1300 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/copy_snapshots.py
--rw-r--r--   0        0        0      874 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/create_images.py
--rw-r--r--   0        0        0      711 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/create_snapshots.py
--rw-r--r--   0        0        0      855 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_images.py
--rw-r--r--   0        0        0     1265 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_instances.py
--rw-r--r--   0        0        0      718 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_security_groups.py
--rw-r--r--   0        0        0      688 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_snapshots.py
--rw-r--r--   0        0        0      834 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_volumes.py
--rw-r--r--   0        0        0      513 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_active_regions.py
--rw-r--r--   0        0        0      522 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     1244 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_images.py
--rw-r--r--   0        0        0     1410 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_instances.py
--rw-r--r--   0        0        0      675 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     1442 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     1203 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_tags.py
--rw-r--r--   0        0        0      522 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     1389 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_volumes.py
--rw-r--r--   0        0        0      960 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0      884 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1175 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     1251 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_tags.py
--rw-r--r--   0        0        0     1131 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_volumes.py
--rw-r--r--   0        0        0      824 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/ec2/share_snapshots.py
--rw-r--r--   0        0        0      887 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/general/get_date.py
--rw-r--r--   0        0        0      791 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0      781 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_inactive_users.py
--rw-r--r--   0        0        0      509 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0      732 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0      763 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_old_password_users.py
--rw-r--r--   0        0        0      766 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0      746 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     1262 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/modify_access_keys.py
--rw-r--r--   0        0        0     1364 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/modify_users_console_access.py
--rw-r--r--   0        0        0      583 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/iam/quarantine_user.py
--rw-r--r--   0        0        0     4829 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/main.py
--rw-r--r--   0        0        0     1242 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/s3/create_objects.py
--rw-r--r--   0        0        0      895 2024-04-10 20:09:13.226189 avtomat_aws-0.2.1/avtomat_aws/cli/s3/delete_objects.py
--rw-r--r--   0        0        0     1225 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/cli/s3/discover_objects.py
--rw-r--r--   0        0        0     1418 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/cli/services.py
--rw-r--r--   0        0        0     1375 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/cli/sts/create_session.py
--rw-r--r--   0        0        0      462 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/cli/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/decorators/__init__.py
--rw-r--r--   0        0        0      789 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/decorators/authenticate.py
--rw-r--r--   0        0        0      615 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/decorators/set_logger.py
--rw-r--r--   0        0        0      724 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/decorators/validate.py
--rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/cli/__init__.py
--rw-r--r--   0        0        0      203 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/cli/set_output.py
--rw-r--r--   0        0        0     2083 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/cli/table.py
--rw-r--r--   0        0        0      858 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/format_tags.py
--rw-r--r--   0        0        0      288 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/set_defaults.py
--rw-r--r--   0        0        0      805 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/set_region.py
--rw-r--r--   0        0        0     2636 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/set_session.py
--rw-r--r--   0        0        0      728 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/helpers/set_session_objects.py
--rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/loggers/__init__.py
--rw-r--r--   0        0        0      457 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/loggers/config.py
--rw-r--r--   0        0        0      138 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/loggers/set_logging.py
--rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/__init__.py
--rw-r--r--   0        0        0       86 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/backup/__init__.py
--rw-r--r--   0        0        0     3810 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/backup/create_backups.py
--rw-r--r--   0        0        0     1629 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/backup/delete_backups.py
--rw-r--r--   0        0        0      163 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0     2821 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     3420 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     3289 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1187 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/__init__.py
--rw-r--r--   0        0        0     2625 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/copy_snapshots.py
--rw-r--r--   0        0        0     2512 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/create_images.py
--rw-r--r--   0        0        0     1988 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/create_snapshots.py
--rw-r--r--   0        0        0     2264 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_images.py
--rw-r--r--   0        0        0    12176 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_instances.py
--rw-r--r--   0        0        0     1532 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_security_groups.py
--rw-r--r--   0        0        0     1430 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_snapshots.py
--rw-r--r--   0        0        0     2663 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_volumes.py
--rw-r--r--   0        0        0      902 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_active_regions.py
--rw-r--r--   0        0        0     1346 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     3012 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_images.py
--rw-r--r--   0        0        0     3599 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_instances.py
--rw-r--r--   0        0        0     1800 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     3330 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     5204 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_tags.py
--rw-r--r--   0        0        0    16665 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     3322 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_volumes.py
--rw-r--r--   0        0        0     4757 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0     3973 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1853 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     4403 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_tags.py
--rw-r--r--   0        0        0     2983 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_volumes.py
--rw-r--r--   0        0        0     1819 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/ec2/share_snapshots.py
--rw-r--r--   0        0        0       31 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/general/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/general/get_date.py
--rw-r--r--   0        0        0      618 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/__init__.py
--rw-r--r--   0        0        0     2674 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0     3228 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_inactive_users.py
--rw-r--r--   0        0        0     1538 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0     2138 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0     2026 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_old_password_users.py
--rw-r--r--   0        0        0     2808 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0     1945 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     2081 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/modify_access_keys.py
--rw-r--r--   0        0        0     3175 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/modify_users_console_access.py
--rw-r--r--   0        0        0     1719 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/iam/quarantine_user.py
--rw-r--r--   0        0        0      133 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/s3/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/s3/create_objects.py
--rw-r--r--   0        0        0     2141 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/s3/delete_objects.py
--rw-r--r--   0        0        0     2517 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/s3/discover_objects.py
--rw-r--r--   0        0        0       70 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/sts/__init__.py
--rw-r--r--   0        0        0      750 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/sts/create_session.py
--rw-r--r--   0        0        0      717 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/services/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/validations/__init__.py
--rw-r--r--   0        0        0      291 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/validations/config.py
--rw-r--r--   0        0        0     3514 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/validations/rules.py
--rw-r--r--   0        0        0      497 2024-04-10 20:09:13.230189 avtomat_aws-0.2.1/avtomat_aws/validations/validate.py
--rw-r--r--   0        0        0     1743 2024-04-10 20:09:13.234189 avtomat_aws-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1823 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    18091 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3838 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/README.md
+-rw-r--r--   0        0        0       69 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/backup/create_backups.py
+-rw-r--r--   0        0        0      864 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/backup/delete_backups.py
+-rw-r--r--   0        0        0      928 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     1156 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     1145 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1300 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0      874 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/create_images.py
+-rw-r--r--   0        0        0      711 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/create_snapshots.py
+-rw-r--r--   0        0        0      855 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_images.py
+-rw-r--r--   0        0        0     1265 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_instances.py
+-rw-r--r--   0        0        0      718 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0      688 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0      834 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      513 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0      522 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1244 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_images.py
+-rw-r--r--   0        0        0     1410 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_instances.py
+-rw-r--r--   0        0        0      675 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     1442 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     1203 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_tags.py
+-rw-r--r--   0        0        0      522 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     1389 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_volumes.py
+-rw-r--r--   0        0        0      960 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0      884 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1175 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1251 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/modify_tags.py
+-rw-r--r--   0        0        0     1131 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/modify_volumes.py
+-rw-r--r--   0        0        0      824 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/ec2/share_snapshots.py
+-rw-r--r--   0        0        0      887 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/general/get_date.py
+-rw-r--r--   0        0        0      791 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0      781 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0      509 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0      732 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0      763 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0      964 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_permissive_inline_policies.py
+-rw-r--r--   0        0        0      786 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_permissive_policies.py
+-rw-r--r--   0        0        0      766 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0      746 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     1262 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     1364 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0      583 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/iam/quarantine_user.py
+-rw-r--r--   0        0        0     4829 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/main.py
+-rw-r--r--   0        0        0     1242 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/s3/create_objects.py
+-rw-r--r--   0        0        0      895 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/s3/delete_objects.py
+-rw-r--r--   0        0        0     1225 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/s3/discover_objects.py
+-rw-r--r--   0        0        0     1522 2024-04-12 19:42:21.831400 avtomat_aws-0.3.0/avtomat_aws/cli/services.py
+-rw-r--r--   0        0        0      909 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/cli/sts/clear_session.py
+-rw-r--r--   0        0        0     2480 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/cli/sts/create_session.py
+-rw-r--r--   0        0        0      462 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/cli/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      789 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/decorators/authenticate.py
+-rw-r--r--   0        0        0      615 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/decorators/set_logger.py
+-rw-r--r--   0        0        0      724 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/decorators/validate.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/cli/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/cli/set_output.py
+-rw-r--r--   0        0        0     2083 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/cli/table.py
+-rw-r--r--   0        0        0      858 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/format_tags.py
+-rw-r--r--   0        0        0      288 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/set_defaults.py
+-rw-r--r--   0        0        0      805 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/set_region.py
+-rw-r--r--   0        0        0     2636 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/set_session.py
+-rw-r--r--   0        0        0      728 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/helpers/set_session_objects.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/loggers/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/loggers/config.py
+-rw-r--r--   0        0        0      138 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/loggers/set_logging.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/backup/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/backup/create_backups.py
+-rw-r--r--   0        0        0     1629 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/backup/delete_backups.py
+-rw-r--r--   0        0        0      163 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0     2821 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     3420 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     3289 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1187 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0     2625 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0     2512 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/create_images.py
+-rw-r--r--   0        0        0     1988 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/create_snapshots.py
+-rw-r--r--   0        0        0     2264 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_images.py
+-rw-r--r--   0        0        0    12176 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_instances.py
+-rw-r--r--   0        0        0     1532 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0     1430 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0     2663 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      902 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0     1346 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     3012 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_images.py
+-rw-r--r--   0        0        0     3599 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_instances.py
+-rw-r--r--   0        0        0     1800 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     3330 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     5204 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_tags.py
+-rw-r--r--   0        0        0    16665 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     3322 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_volumes.py
+-rw-r--r--   0        0        0     4757 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0     3973 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1853 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     4403 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/modify_tags.py
+-rw-r--r--   0        0        0     2983 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/modify_volumes.py
+-rw-r--r--   0        0        0     1819 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/ec2/share_snapshots.py
+-rw-r--r--   0        0        0       31 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/general/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/general/get_date.py
+-rw-r--r--   0        0        0      774 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/__init__.py
+-rw-r--r--   0        0        0     2674 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0     3228 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0     1538 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0     2138 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0     2026 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0     5434 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_permissive_inline_policies.py
+-rw-r--r--   0        0        0     3073 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_permissive_policies.py
+-rw-r--r--   0        0        0     2808 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0     1945 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     2081 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     3175 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0     1719 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/iam/quarantine_user.py
+-rw-r--r--   0        0        0      133 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/s3/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/s3/create_objects.py
+-rw-r--r--   0        0        0     2141 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/s3/delete_objects.py
+-rw-r--r--   0        0        0     2517 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/s3/discover_objects.py
+-rw-r--r--   0        0        0       70 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/sts/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/sts/create_session.py
+-rw-r--r--   0        0        0      717 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/services/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/validations/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/validations/config.py
+-rw-r--r--   0        0        0     3514 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/validations/rules.py
+-rw-r--r--   0        0        0      497 2024-04-12 19:42:21.835400 avtomat_aws-0.3.0/avtomat_aws/validations/validate.py
+-rw-r--r--   0        0        0     1743 2024-04-12 19:42:21.839400 avtomat_aws-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.3.0/PKG-INFO
```

### Comparing `avtomat_aws-0.2.1/CHANGELOG.md` & `avtomat_aws-0.3.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.3.0 (2024-04-12)
+
+### Feat
+
+- **iam.discover_permissive_policies**: Add new actions
+
 ## 0.2.1 (2024-04-10)
 
 ### Fix
 
 - **ec2.delete_instances.discover_image_snapshots.exception**: Change image.image_id to image.id
 - **ec2.delete_instances.cli**: Revert the original cli interface
 - **ec2.delete_instances.discover_image_snapshots**: Skip snapshot retrieval for images not in 'available' state
```

### Comparing `avtomat_aws-0.2.1/LICENSE` & `avtomat_aws-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/README.md` & `avtomat_aws-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/backup/create_backups.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/backup/delete_backups.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_events.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/cloudtrail/discover_user_events.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/copy_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/create_images.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/create_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/create_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_images.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_instances.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_security_groups.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/delete_volumes.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_active_regions.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_images.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_instances.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_tags.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/discover_volumes.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/encrypt_volume.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_tags.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/modify_volumes.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/ec2/share_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/general/get_date.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_inactive_console_users.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_inactive_users.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_old_access_keys.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_old_password_users.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_unused_access_keys.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/discover_unused_roles.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/modify_access_keys.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/modify_users_console_access.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/iam/quarantine_user.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/main.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/main.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/s3/create_objects.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/s3/delete_objects.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/s3/discover_objects.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/cli/services.py` & `avtomat_aws-0.3.0/avtomat_aws/cli/services.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,16 +33,18 @@
     "general": ["get_date"],
     "iam": [
         "discover_inactive_console_users",
         "discover_inactive_users",
         "discover_no_mfa_users",
         "discover_old_access_keys",
         "discover_old_password_users",
+        "discover_permissive_inline_policies",
+        "discover_permissive_policies",
         "discover_unused_access_keys",
         "discover_unused_roles",
         "modify_access_keys",
         "modify_users_console_access",
         "quarantine_user",
     ],
-    "sts": ["create_session", "whoami"],
+    "sts": ["clear_session", "create_session", "whoami"],
     "s3": ["create_objects", "delete_objects", "discover_objects"],
 }
```

### Comparing `avtomat_aws-0.2.1/avtomat_aws/decorators/authenticate.py` & `avtomat_aws-0.3.0/avtomat_aws/decorators/authenticate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/decorators/set_logger.py` & `avtomat_aws-0.3.0/avtomat_aws/decorators/set_logger.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/decorators/validate.py` & `avtomat_aws-0.3.0/avtomat_aws/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/helpers/cli/table.py` & `avtomat_aws-0.3.0/avtomat_aws/helpers/cli/table.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/helpers/format_tags.py` & `avtomat_aws-0.3.0/avtomat_aws/helpers/format_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/helpers/set_region.py` & `avtomat_aws-0.3.0/avtomat_aws/helpers/set_region.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/helpers/set_session.py` & `avtomat_aws-0.3.0/avtomat_aws/helpers/set_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/helpers/set_session_objects.py` & `avtomat_aws-0.3.0/avtomat_aws/helpers/set_session_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/backup/create_backups.py` & `avtomat_aws-0.3.0/avtomat_aws/services/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/backup/delete_backups.py` & `avtomat_aws-0.3.0/avtomat_aws/services/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_events.py` & `avtomat_aws-0.3.0/avtomat_aws/services/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.3.0/avtomat_aws/services/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/cloudtrail/discover_user_events.py` & `avtomat_aws-0.3.0/avtomat_aws/services/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/__init__.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/copy_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/create_images.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/create_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/create_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_images.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_instances.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_security_groups.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/delete_volumes.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_active_regions.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_images.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_instances.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_tags.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/discover_volumes.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/encrypt_volume.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_tags.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/modify_volumes.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/ec2/share_snapshots.py` & `avtomat_aws-0.3.0/avtomat_aws/services/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/general/get_date.py` & `avtomat_aws-0.3.0/avtomat_aws/services/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/__init__.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .discover_inactive_console_users import discover_inactive_console_users
 from .discover_inactive_users import discover_inactive_users
 from .discover_no_mfa_users import discover_no_mfa_users
 from .discover_old_access_keys import discover_old_access_keys
 from .discover_old_password_users import discover_old_password_users
+from .discover_permissive_inline_policies import discover_permissive_inline_policies
+from .discover_permissive_policies import discover_permissive_policies
 from .discover_unused_access_keys import discover_unused_access_keys
 from .discover_unused_roles import discover_unused_roles
 from .modify_access_keys import modify_access_keys
 from .modify_users_console_access import modify_users_console_access
 from .quarantine_user import quarantine_user
```

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_inactive_console_users.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_inactive_users.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_no_mfa_users.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_no_mfa_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_old_access_keys.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_old_password_users.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_unused_access_keys.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/discover_unused_roles.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/modify_access_keys.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/modify_users_console_access.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/iam/quarantine_user.py` & `avtomat_aws-0.3.0/avtomat_aws/services/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/s3/create_objects.py` & `avtomat_aws-0.3.0/avtomat_aws/services/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/s3/delete_objects.py` & `avtomat_aws-0.3.0/avtomat_aws/services/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/s3/discover_objects.py` & `avtomat_aws-0.3.0/avtomat_aws/services/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/sts/create_session.py` & `avtomat_aws-0.3.0/avtomat_aws/services/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/services/sts/whoami.py` & `avtomat_aws-0.3.0/avtomat_aws/services/sts/whoami.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/avtomat_aws/validations/rules.py` & `avtomat_aws-0.3.0/avtomat_aws/validations/rules.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.2.1/pyproject.toml` & `avtomat_aws-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avtomat-aws"
-version = "0.2.1"
+version = "0.3.0"
 description = "A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations."
 authors = ["Dimitar Atanasov <dimitar@avtomat.io>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://avtomat.io"
 documentation = "https://docs.avtomat.io/aws/get_started"
 keywords = ["aws", "cloud", "automation", "cli", "python", "boto3"]
```

### Comparing `avtomat_aws-0.2.1/PKG-INFO` & `avtomat_aws-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avtomat-aws
-Version: 0.2.1
+Version: 0.3.0
 Summary: A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations.
 Home-page: https://avtomat.io
 License: GPL-2.0-only
 Keywords: aws,cloud,automation,cli,python,boto3
 Author: Dimitar Atanasov
 Author-email: dimitar@avtomat.io
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: avtomat-aws Version: 0.2.1 Summary: A collection of
+Metadata-Version: 2.1 Name: avtomat-aws Version: 0.3.0 Summary: A collection of
 reusable Amazon Web Services actions, bringing speed and certainty to cloud
 operations. Home-page: https://avtomat.io License: GPL-2.0-only Keywords:
 aws,cloud,automation,cli,python,boto3 Author: Dimitar Atanasov Author-email:
 dimitar@avtomat.io Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```


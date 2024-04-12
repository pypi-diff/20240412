# Comparing `tmp/edumfa-1.5.1.tar.gz` & `tmp/edumfa-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edumfa-1.5.1.tar", last modified: Tue Apr  9 12:49:27 2024, max compression
+gzip compressed data, was "edumfa-2.0.0.tar", last modified: Fri Apr 12 08:48:31 2024, max compression
```

## Comparing `edumfa-1.5.1.tar` & `edumfa-2.0.0.tar`

### file list

```diff
@@ -1,989 +1,1013 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.428377 edumfa-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-09 12:49:21.000000 edumfa-1.5.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-09 12:49:21.000000 edumfa-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 12:49:21.000000 edumfa-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-09 12:49:27.428377 edumfa-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-09 12:49:21.000000 edumfa-1.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/apache/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/apache/edumfaapp.wsgi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/apache/sites-available/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/apache/sites-available/edumfa-venv.conf
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/apache/sites-available/edumfa.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.252379 edumfa-1.5.1/deploy/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/config/freeradius2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/config/freeradius2/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/config/freeradius2/mods-perl-edumfa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/config/freeradius3/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/config/freeradius3/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/config/freeradius3/mods-perl-edumfa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/crontab/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/crontab/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/docker-compose-example.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/docker-example/
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/docker-example/edumfa-policy.conf
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/docker-example/edumfa-setup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/docker-example/edumfa.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/docker-setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/edumfa/
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/edumfa/dictionary
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/edumfa/edumfa.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/edumfa_radius.pm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/gunicorn/edumfaapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/logging.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/nginx/edumfaapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.276378 edumfa-1.5.1/deploy/nginx/sites-available/
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/nginx/sites-available/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/rlm_perl.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.280378 edumfa-1.5.1/deploy/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu/changelog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu/clean
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu/compat
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu/control
--rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu/copyright
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu/rules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.284378 edumfa-1.5.1/deploy/ubuntu/source/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu/source/format
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu/source/options
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.280378 edumfa-1.5.1/deploy/ubuntu-radius/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/changelog
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/compat
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/control
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/copyright
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/edumfa-radius.install
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/edumfa-radius.postinst
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/edumfa-radius.postrm
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/rules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.280378 edumfa-1.5.1/deploy/ubuntu-radius/source/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-radius/source/format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.280378 edumfa-1.5.1/deploy/ubuntu-server/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/changelog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/clean
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/compat
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/control
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/edumfa-apache2.install
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/edumfa-apache2.postinst
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/edumfa-apache2.postrm
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/edumfa-nginx.install
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/edumfa-nginx.postinst
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/edumfa-nginx.postrm
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/rules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.284378 edumfa-1.5.1/deploy/ubuntu-server/source/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/source/format
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/ubuntu-server/source/options
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.256379 edumfa-1.5.1/deploy/uwsgi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.284378 edumfa-1.5.1/deploy/uwsgi/apps-available/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 12:49:21.000000 edumfa-1.5.1/deploy/uwsgi/apps-available/edumfa.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.284378 edumfa-1.5.1/edumfa/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.288378 edumfa-1.5.1/edumfa/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/before_after.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/clienttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.292378 edumfa-1.5.1/edumfa/api/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/lib/policyhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    41925 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/lib/postpolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)   101628 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/lib/prepolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/machineresolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/recover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/smsgateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    55749 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/ttype.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    29126 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/api/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/babel.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.300378 edumfa-1.5.1/edumfa/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.300378 edumfa-1.5.1/edumfa/lib/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/applications/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/applications/luks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/applications/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/applications/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/audit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.300378 edumfa-1.5.1/edumfa/lib/auditmodules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/auditmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/auditmodules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/auditmodules/containeraudit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/auditmodules/loggeraudit.py
--rw-r--r--   0 runner    (1001) docker     (127)    26334 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/auditmodules/sqlaudit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/authcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.300378 edumfa-1.5.1/edumfa/lib/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/caconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.300378 edumfa-1.5.1/edumfa/lib/caconnectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/caconnectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/caconnectors/baseca.py
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/caconnectors/caservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/caconnectors/caservice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/caconnectors/localca.py
--rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/caconnectors/msca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/challengeresponsedecorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/clientapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    37215 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28674 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.304378 edumfa-1.5.1/edumfa/lib/eventhandler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/counterhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/customuserattributeshandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/federationhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/logginghandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/requestmangler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/responsemangler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/scripthandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    30653 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/tokenhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/usernotification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/eventhandler/webhookeventhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    29337 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/importotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    19552 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/machineresolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.304378 edumfa-1.5.1/edumfa/lib/machines/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/machines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/machines/hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/machines/ldap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.304378 edumfa-1.5.1/edumfa/lib/monitoringmodules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/monitoringmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/monitoringmodules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/monitoringmodules/sqlstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/monitoringstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/passwordreset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/periodictask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.304378 edumfa-1.5.1/edumfa/lib/pinhandling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/pinhandling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/pinhandling/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   146757 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    28842 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/policydecorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.304378 edumfa-1.5.1/edumfa/lib/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/queues/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/queues/huey_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.308378 edumfa-1.5.1/edumfa/lib/resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/resolvers/HTTPResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    56725 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/resolvers/LDAPIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/resolvers/PasswdIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/resolvers/SCIMIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    28267 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/resolvers/SQLIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/resolvers/UserIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/resolvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.308378 edumfa-1.5.1/edumfa/lib/security/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/security/aeshsm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/security/default.py
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/security/encryptkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.308378 edumfa-1.5.1/edumfa/lib/security/password/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/security/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/serviceid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.308378 edumfa-1.5.1/edumfa/lib/smsprovider/
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/FirebaseProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/HttpMessageToUidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/HttpSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/SMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/ScriptSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/SipgateSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/SmppSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/SmtpSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smsprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/sqlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.308378 edumfa-1.5.1/edumfa/lib/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/task/eventcounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/task/simplestats.py
--rw-r--r--   0 runner    (1001) docker     (127)    96866 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    68419 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokenclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokengroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/lib/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/HMAC.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/applicationspecificpasswordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25837 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/certificatetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/daplugtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/daypasswordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/emailtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    18983 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/foureyestoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    33207 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/hotptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/indexedsecrettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/mOTP.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/motptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/ocra.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/ocratoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/papertoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/passwordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    46777 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/pushtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/questionnairetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/radiustoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/registrationtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/remotetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/smstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/spasstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/sshkeytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/tantoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/tiqrtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    27633 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/totptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    23127 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/u2ftoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/vasco.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/vascotoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    89138 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)    66656 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/webauthntoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/yubicotoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/tokens/yubikeytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/usercache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    55043 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/lib/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    71279 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)   121289 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.264378 edumfa-1.5.1/edumfa/static/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.260378 edumfa-1.5.1/edumfa/static/components/audit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/static/components/audit/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/audit/controllers/auditControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/static/components/audit/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/audit/factories/audit.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/static/components/audit/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/audit/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/static/components/audit/views/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/audit/views/audit.html
--rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/audit/views/audit.log.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.260378 edumfa-1.5.1/edumfa/static/components/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/static/components/components/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/components/controllers/componentControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/static/components/components/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/components/factories/component.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.316378 edumfa-1.5.1/edumfa/static/components/components/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/components/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.320378 edumfa-1.5.1/edumfa/static/components/components/views/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/components/views/component.clienttype.html
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/components/views/component.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.260378 edumfa-1.5.1/edumfa/static/components/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.320378 edumfa-1.5.1/edumfa/static/components/config/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    50570 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/configControllers.js
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/eduMfaServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/eventController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/ldapMachineResolverController.js
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/periodicTaskController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/radiusServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/serviceidController.js
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/smsgatewayController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/smtpServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/controllers/tokengroupController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.320378 edumfa-1.5.1/edumfa/static/components/config/factories/
--rw-r--r--   0 runner    (1001) docker     (127)    32353 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/factories/config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.320378 edumfa-1.5.1/edumfa/static/components/config/states/
--rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/config/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.caconnectors.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.caconnectors.local.html
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.caconnectors.microsoft.html
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.edumfaserver.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.edumfaserver.list.html
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.events.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.events.html
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.events.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.machineresolvers.html
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.mresolvers.hosts.html
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.mresolvers.ldap.html
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.mresolvers.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.periodictasks.details.html
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.periodictasks.html
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.periodictasks.list.html
--rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.policies.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.policies.html
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.policies.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.radius.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.radius.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.realms.html
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.realms.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.html
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.http.html
--rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.ldap.html
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.passwd.html
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.scim.html
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.sql.html
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.serviceid.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.serviceid.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.smsgateway.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.smsgateway.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.smtp.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.smtp.list.html
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.system.doc.html
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.system.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.system.html
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.email.html
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.question.html
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.radius.html
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.remote.html
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.sms.html
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.yubico.html
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.token.yubikey.html
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.tokengroup.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.tokengroup.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/config.tokens.html
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/config/views/dialog.confirm_delete.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.260378 edumfa-1.5.1/edumfa/static/components/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/dashboard/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/dashboard/controllers/dashboardControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/dashboard/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/dashboard/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/dashboard/views/
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/dashboard/views/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.260378 edumfa-1.5.1/edumfa/static/components/dialogs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/dialogs/views/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.about.html
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.lock.html
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.no.token.html
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.welcome.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.260378 edumfa-1.5.1/edumfa/static/components/directives/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/directives/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    19746 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/controllers/directives.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/directives/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/views/directive.assigntoken.html
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/views/directive.assignuser.html
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/views/directive.attachmachine.html
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/views/directive.attachtoken.html
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/views/directive.csvdownload.html
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/views/directive.filter.table.html
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/views/directive.policyconditions.html
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/directives/views/directive.tokendata.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/filters/filters.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.260378 edumfa-1.5.1/edumfa/static/components/login/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/login/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    30344 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/controllers/loginControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.332378 edumfa-1.5.1/edumfa/static/components/login/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/factories/auth.js
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/factories/u2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/factories/webauthn.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/login/states/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/login/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/views/enter-response.html
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/views/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/views/offline.html
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/login/views/pinchange.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.264378 edumfa-1.5.1/edumfa/static/components/machine/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/machine/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/machine/controllers/machineController.js
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/machine/controllers/machineDetailsController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/machine/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/machine/factories/machine.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/machine/states/
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/machine/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/machine/views/
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/machine/views/machine.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/machine/views/machine.html
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/machine/views/machine.list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.264378 edumfa-1.5.1/edumfa/static/components/recovery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/recovery/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/recovery/controllers/recoveryControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/recovery/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/recovery/factories/recoveryFactory.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/recovery/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/recovery/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/recovery/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/recovery/views/recovery.html
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/recovery/views/recovery.reset.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.264378 edumfa-1.5.1/edumfa/static/components/register/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/register/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/register/controllers/registerControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/register/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/register/factories/registerFactory.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/register/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/register/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.336377 edumfa-1.5.1/edumfa/static/components/register/views/
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/register/views/register.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.264378 edumfa-1.5.1/edumfa/static/components/token/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.340377 edumfa-1.5.1/edumfa/static/components/token/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/controllers/tokenApplicationsController.js
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/controllers/tokenChallengesController.js
--rw-r--r--   0 runner    (1001) docker     (127)    29864 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/controllers/tokenControllers.js
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/controllers/tokenDetailController.js
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/controllers/tokenGetSerialController.js
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/controllers/tokenLostController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.340377 edumfa-1.5.1/edumfa/static/components/token/factories/
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/factories/token.js
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/factories/validate.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.340377 edumfa-1.5.1/edumfa/static/components/token/states/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.348377 edumfa-1.5.1/edumfa/static/components/token/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/dialog.ask_token_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.applications.html
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.applications.offline.html
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.applications.ssh.html
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.assign.html
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.challenges.html
--rw-r--r--   0 runner    (1001) docker     (127)    32395 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.details.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.display.apps.html
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.4eyes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.applspec.html
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.certificate.html
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.email.html
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.html
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.indexedsecret.html
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.motp.html
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.paper.html
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.push.html
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.question.html
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.radius.html
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.registration.html
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.remote.html
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.sms.html
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.spass.html
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.sshkey.html
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.tan.html
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.vasco.html
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.yubico.html
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.yubikey.html
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.applspec.html
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.certificate.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.motp.html
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.paper.html
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.push.html
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.registration.html
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.tan.html
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.getserial.html
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.html
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.import.html
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/token/views/token.lost.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.348377 edumfa-1.5.1/edumfa/static/components/translation/
--rw-r--r--   0 runner    (1001) docker     (127)   557560 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/translation/translations.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.264378 edumfa-1.5.1/edumfa/static/components/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.348377 edumfa-1.5.1/edumfa/static/components/user/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    19169 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/controllers/userControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.348377 edumfa-1.5.1/edumfa/static/components/user/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/factories/user.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.348377 edumfa-1.5.1/edumfa/static/components/user/states/
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.352377 edumfa-1.5.1/edumfa/static/components/user/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/views/dialog.ask_user_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/views/user.add.dynamic.form.fields.html
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/views/user.add.html
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/views/user.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/views/user.html
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/views/user.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/components/user/views/user.password.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.264378 edumfa-1.5.1/edumfa/static/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.352377 edumfa-1.5.1/edumfa/static/contrib/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/css/angular-inform.css
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/css/angular-inform.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    25682 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    48005 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   145933 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   390887 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/css/hotkeys.css
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/css/isteven-multi-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.356377 edumfa-1.5.1/edumfa/static/contrib/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.356377 edumfa-1.5.1/edumfa/static/contrib/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/angular-inform.js
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/angular-inform.js.map
--rw-r--r--   0 runner    (1001) docker     (127)  1377909 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/angular.js
--rw-r--r--   0 runner    (1001) docker     (127)    75484 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    53486 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/hotkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.360377 edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/
--rw-r--r--   0 runner    (1001) docker     (127)    32388 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-gettext.js
--rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-idle.js
--rw-r--r--   0 runner    (1001) docker     (127)    33197 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-sanitize.js
--rw-r--r--   0 runner    (1001) docker     (127)   487964 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-ui-router.js
--rw-r--r--   0 runner    (1001) docker     (127)   760134 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js
--rw-r--r--   0 runner    (1001) docker     (127)    81683 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/ng-file-upload.js
--rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/u2f-api.js
--rw-r--r--   0 runner    (1001) docker     (127)   276562 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/ui-bootstrap-tpls.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.360377 edumfa-1.5.1/edumfa/static/contrib/js/webauthn-client/
--rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.364377 edumfa-1.5.1/edumfa/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/css/baseline.css
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/css/content.css
--rw-r--r--   0 runner    (1001) docker     (127)    24602 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/css/eduMFA-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/css/highlight.css
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/css/menu.css
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/css/papertoken.css
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/css/signin.css
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/css/table-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.364377 edumfa-1.5.1/edumfa/static/customize/
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/customize/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.364377 edumfa-1.5.1/edumfa/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png
--rw-r--r--   0 runner    (1001) docker     (127)    47610 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/img/plugup.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   336777 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/img/solokeys.png
--rw-r--r--   0 runner    (1001) docker     (127)   107999 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/img/u2fzero.png
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.364377 edumfa-1.5.1/edumfa/static/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/providers/errorMessageProvider.js
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/providers/versioningProvider.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.364377 edumfa-1.5.1/edumfa/static/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/baseline.html
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/cert_request_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/deactivated.html
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/templates/token_enrolled.html
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/static/update_contrib.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.364377 edumfa-1.5.1/edumfa/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23376 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    84098 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.368377 edumfa-1.5.1/edumfa/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    95309 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   127521 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.368377 edumfa-1.5.1/edumfa/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    81449 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   118619 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.368377 edumfa-1.5.1/edumfa/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    53719 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104451 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.368377 edumfa-1.5.1/edumfa/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    87343 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.368377 edumfa-1.5.1/edumfa/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    85965 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   120848 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.368377 edumfa-1.5.1/edumfa/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.368377 edumfa-1.5.1/edumfa/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    78400 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   115604 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.368377 edumfa-1.5.1/edumfa/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    79882 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.372377 edumfa-1.5.1/edumfa/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    33313 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    96048 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/si/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.372377 edumfa-1.5.1/edumfa/translations/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/si/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    73291 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/si/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.372377 edumfa-1.5.1/edumfa/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    82030 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   117846 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.268378 edumfa-1.5.1/edumfa/translations/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.372377 edumfa-1.5.1/edumfa/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    68507 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104457 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.272378 edumfa-1.5.1/edumfa/translations/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.372377 edumfa-1.5.1/edumfa/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70327 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   105843 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.372377 edumfa-1.5.1/edumfa/webui/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/webui/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa/webui/login.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    62952 2024-04-09 12:49:21.000000 edumfa-1.5.1/edumfa-manage
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.424377 edumfa-1.5.1/edumfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-09 12:49:27.000000 edumfa-1.5.1/edumfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32602 2024-04-09 12:49:27.000000 edumfa-1.5.1/edumfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:49:27.000000 edumfa-1.5.1/edumfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:49:27.000000 edumfa-1.5.1/edumfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-09 12:49:27.000000 edumfa-1.5.1/edumfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 12:49:27.000000 edumfa-1.5.1/edumfa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.372377 edumfa-1.5.1/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.384377 edumfa-1.5.1/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/006d4747f858_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/00762b3f7a60_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/0c7123345224_.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/0d011e94a8e8_.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/140ba0ca4f07_.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/145ce80decd_.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/14a1bcb10018_.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/19f727d285e2_.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/1a0710df148b_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/1a69e5e5e2ac_.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/1edda52b619f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/204d8d4f351e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/205bda834127_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/20969b4cbf06_.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/2118e566df16_.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/2181294eed0b_.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/22558d9f3178_.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/239995464c48_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/2551ee982544_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/2ac117d0a6f5_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/2c9430cfc66b_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/307a4fbe8a05_.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/3236a1abf1c6_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/3429d523e51f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/36428afb2457_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/37e6b49fc686_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/3ae3c668f444_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/3ba618f6b820_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/3c6e9dd7fbac_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/3d7f8b29cbb1_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/3f7e8583ea2_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/4023571658f8_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/4238eac8ccab_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/449903fb6e35_.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/48ee74b8a7c8_.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/49a04e560d96_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/4a0aec37e7cf_.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/4d9178fa8336_.py
--rw-r--r--   0 runner    (1001) docker     (127)    19377 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/4f32a4e1bf33_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/50adc980d625_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/5402fd96fbca_.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/58e4f7ebb705_.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/59ef3e03bc62_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/5cb310101a1f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/631ec59e1ca6_.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/849170064430_.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/86f40f535d7c_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/888b56ed5dcb_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/89e57ed16379_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/8d40dbcfda25_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/9155f0d3d028_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/a28f2733897b_.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/a63df077051a_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/a7e91b18a460_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/b9131d0686eb_.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/cb6d7b7bae63_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/d2ae8e54b628_.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/d3c0f0403a84_.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/d415d490eb05_.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/d5870fd2f2a4_.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/d6b40a745e5_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/d756b34061ff_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/dceb6cd3c41e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/e360c56bcf8c_.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/e5cbeb7c177_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/ef29ba43e290_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/fa07bd604a75.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/fabcf24d9304_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 12:49:21.000000 edumfa-1.5.1/migrations/versions/ff26585932ec_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-09 12:49:21.000000 edumfa-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:49:27.428377 edumfa-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-09 12:49:21.000000 edumfa-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.408377 edumfa-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/ldap3mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/mscamock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/pkcs11mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/queuemock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/radiusmock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/redismock.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/smppmock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/smtpmock.py
--rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_2stepinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    20710 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    48917 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_clienttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    35517 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_events.py
--rw-r--r--   0 runner    (1001) docker     (127)   193396 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_lib_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_machineresolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    38769 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    16166 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_machines_serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_offline_no_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    36128 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    26177 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_push_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_register.py
--rw-r--r--   0 runner    (1001) docker     (127)    76125 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_serviceids.py
--rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_smsgateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    62186 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_system.py
--rw-r--r--   0 runner    (1001) docker     (127)   195170 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_ttype.py
--rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    33114 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_users.py
--rw-r--r--   0 runner    (1001) docker     (127)   302927 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    45689 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_db_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_authcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_challenges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_clientapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    35302 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_eventhandler_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_eventhandler_usernotification.py
--rw-r--r--   0 runner    (1001) docker     (127)   113340 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    29545 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_importotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_machine_resolver_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_machinetokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_monitoringstats.py
--rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    75326 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    36401 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_policydecorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)   123815 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)    32074 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_smsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_sqlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_task_eventcounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_task_simplestats.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    97908 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokenclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    36699 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25260 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_daplug.py
--rw-r--r--   0 runner    (1001) docker     (127)    27651 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_daypassword.py
--rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_foureyes.py
--rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_hotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_indexedsecret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_motp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_paper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_passwordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    75419 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_spass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_tan.py
--rw-r--r--   0 runner    (1001) docker     (127)    31214 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_tiqr.py
--rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_vasco.py
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_yubico.py
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_tokens_yubikey.py
--rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_usercache.py
--rw-r--r--   0 runner    (1001) docker     (127)    45888 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_lib_utils_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)    38033 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_mock_ldap3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_resolver_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_ui_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/test_ui_login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.416377 edumfa-1.5.1/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/FIDO-U2F-Security-Key-444x444.png
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/NetKnights.pem
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.272378 edumfa-1.5.1/tests/testdata/altstatic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.416377 edumfa-1.5.1/tests/testdata/altstatic/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/altstatic/templates/testui.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.416377 edumfa-1.5.1/tests/testdata/attestation/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/attestation/yubico.pem
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/audit.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.416377 edumfa-1.5.1/tests/testdata/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/ca/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/ca/cakey.pem
--rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/ca/index.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/ca/index.txt.attr
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/ca/openssl.cnf
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/ca/serial
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/ca/templates.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/dictionary
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/does_not_exist
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/emailtemplate.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/empty.oath
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/enckey
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/enckey.enc
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/fancytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/firebase-test.json
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/google-services.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.416377 edumfa-1.5.1/tests/testdata/gpg/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/gpg/public.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/gpg/pubring.gpg
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/gpg/random_seed
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/gpg/secring.gpg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/gpg/trustdb.gpg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/hosts
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/import.oath
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/import.oath.asc
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/jwt_sign.key
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/logging.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/logging_broken.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.416377 edumfa-1.5.1/tests/testdata/msca-connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/msca-connector/ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/msca-connector/privacyidea-encrypted.key
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/msca-connector/privacyidea.key
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/msca-connector/privacyidea.pem
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/ocra.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/passwd
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/passwd-duplicate-name
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/passwords
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/policy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/policy_empty_file.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/private.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/pskc-aes.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/pskc-password.xml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/public.pem
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/pw-2nd-resolver
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.416377 edumfa-1.5.1/tests/testdata/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/scripts/fail.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/scripts/ls.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/scripts/success.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/test.sub
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/test2.sub
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/testuser-api.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/testuser.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/testusercache.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.420377 edumfa-1.5.1/tests/testdata/trusted_attestation_roots/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/yubico-oath-long.csv
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/yubico-oath.csv
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-09 12:49:21.000000 edumfa-1.5.1/tests/testdata/yubico.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:49:27.424377 edumfa-1.5.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/creategoogleauthenticator-file
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-authorizedkeys
--rwxr-xr-x   0 runner    (1001) docker     (127)     1766 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-convert-base32.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-convert-token
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-convert-token.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-convert-xml-to-csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-ad-users
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-ad-users.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-certificate
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-certificate.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1985 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-pwidresolver-user
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-pwidresolver-user.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-sqlidresolver-user
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-sqlidresolver-user.1
--rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-userdb
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-create-userdb.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     6703 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-cron
--rwxr-xr-x   0 runner    (1001) docker     (127)     7030 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-diag
--rwxr-xr-x   0 runner    (1001) docker     (127)     6991 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-expired-users
--rwxr-xr-x   0 runner    (1001) docker     (127)     1354 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-export-edumfa-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4514 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-export-linotp-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3719 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-fetchssh
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-fetchssh.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     2500 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-fix-access-rights
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-fix-access-rights.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     3541 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-get-serial
--rwxr-xr-x   0 runner    (1001) docker     (127)     4940 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-get-unused-tokens
--rwxr-xr-x   0 runner    (1001) docker     (127)    25361 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-migrate-linotp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2525 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-pip-update
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-pip-update.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-queue-huey
--rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-schema-upgrade
--rwxr-xr-x   0 runner    (1001) docker     (127)    11397 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-standalone
--rwxr-xr-x   0 runner    (1001) docker     (127)     8176 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-sync-owncloud.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31889 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-token-janitor
--rwxr-xr-x   0 runner    (1001) docker     (127)     3746 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-update-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5391 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-update-linotp-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5471 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-user-action
--rwxr-xr-x   0 runner    (1001) docker     (127)     3674 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/edumfa-usercache-cleanup
--rwxr-xr-x   0 runner    (1001) docker     (127)     1476 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/getgooglecodes
--rwxr-xr-x   0 runner    (1001) docker     (127)     3049 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/reset-edumfa
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-09 12:49:21.000000 edumfa-1.5.1/tools/ssha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.457755 edumfa-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-12 08:48:25.000000 edumfa-2.0.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-12 08:48:25.000000 edumfa-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-12 08:48:25.000000 edumfa-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-12 08:48:31.457755 edumfa-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-12 08:48:25.000000 edumfa-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.293755 edumfa-2.0.0/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.293755 edumfa-2.0.0/deploy/apache/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/apache/edumfaapp.wsgi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.293755 edumfa-2.0.0/deploy/apache/sites-available/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/apache/sites-available/edumfa-venv.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/apache/sites-available/edumfa.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.273755 edumfa-2.0.0/deploy/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.293755 edumfa-2.0.0/deploy/config/freeradius2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/config/freeradius2/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/config/freeradius2/mods-perl-edumfa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.293755 edumfa-2.0.0/deploy/config/freeradius3/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/config/freeradius3/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/config/freeradius3/mods-perl-edumfa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.293755 edumfa-2.0.0/deploy/crontab/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/crontab/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/docker-compose-example.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.293755 edumfa-2.0.0/deploy/docker-example/
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/docker-example/edumfa-policy.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/docker-example/edumfa-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/docker-example/edumfa.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/docker-setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.297755 edumfa-2.0.0/deploy/edumfa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/edumfa/dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/edumfa/edumfa.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/edumfa_radius.pm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.297755 edumfa-2.0.0/deploy/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/gunicorn/edumfaapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/logging.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.297755 edumfa-2.0.0/deploy/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/nginx/edumfaapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.297755 edumfa-2.0.0/deploy/nginx/sites-available/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/nginx/sites-available/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/rlm_perl.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.297755 edumfa-2.0.0/deploy/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu/clean
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu/control
+-rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.301755 edumfa-2.0.0/deploy/ubuntu/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu/source/format
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu/source/options
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.297755 edumfa-2.0.0/deploy/ubuntu-radius/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/compat
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/control
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/edumfa-radius.install
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/edumfa-radius.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/edumfa-radius.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.297755 edumfa-2.0.0/deploy/ubuntu-radius/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-radius/source/format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.301755 edumfa-2.0.0/deploy/ubuntu-server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/clean
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/control
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/edumfa-apache2.install
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/edumfa-apache2.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/edumfa-apache2.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/edumfa-nginx.install
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/edumfa-nginx.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/edumfa-nginx.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.301755 edumfa-2.0.0/deploy/ubuntu-server/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/source/format
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/ubuntu-server/source/options
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.273755 edumfa-2.0.0/deploy/uwsgi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.301755 edumfa-2.0.0/deploy/uwsgi/apps-available/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 08:48:25.000000 edumfa-2.0.0/deploy/uwsgi/apps-available/edumfa.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.301755 edumfa-2.0.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-04-12 08:48:25.000000 edumfa-2.0.0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.301755 edumfa-2.0.0/edumfa/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.309755 edumfa-2.0.0/edumfa/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/before_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/clienttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.309755 edumfa-2.0.0/edumfa/api/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/lib/policyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41925 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/lib/postpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101628 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/lib/prepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/machineresolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/smsgateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55749 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/ttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29126 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/api/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/babel.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.309755 edumfa-2.0.0/edumfa/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.313755 edumfa-2.0.0/edumfa/commands/manage/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/authcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/hsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/commands/manage/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.321755 edumfa-2.0.0/edumfa/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.321755 edumfa-2.0.0/edumfa/lib/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/applications/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/applications/luks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/applications/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/applications/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/audit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.321755 edumfa-2.0.0/edumfa/lib/auditmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/auditmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/auditmodules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/auditmodules/containeraudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/auditmodules/loggeraudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26334 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/auditmodules/sqlaudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/authcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.321755 edumfa-2.0.0/edumfa/lib/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/caconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.325755 edumfa-2.0.0/edumfa/lib/caconnectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/caconnectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/caconnectors/baseca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/caconnectors/caservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/caconnectors/caservice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/caconnectors/localca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/caconnectors/msca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/challengeresponsedecorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/clientapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37215 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28674 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.325755 edumfa-2.0.0/edumfa/lib/eventhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/counterhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/customuserattributeshandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/federationhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/logginghandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/requestmangler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/responsemangler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/scripthandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30653 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/tokenhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/usernotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/eventhandler/webhookeventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29337 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/importotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19552 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/machineresolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.325755 edumfa-2.0.0/edumfa/lib/machines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/machines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/machines/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/machines/ldap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.329755 edumfa-2.0.0/edumfa/lib/monitoringmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/monitoringmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/monitoringmodules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/monitoringmodules/sqlstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/monitoringstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/passwordreset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/periodictask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.329755 edumfa-2.0.0/edumfa/lib/pinhandling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/pinhandling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/pinhandling/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146757 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28842 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/policydecorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.329755 edumfa-2.0.0/edumfa/lib/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/queues/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/queues/huey_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.329755 edumfa-2.0.0/edumfa/lib/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/resolvers/HTTPResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56725 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/resolvers/LDAPIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/resolvers/PasswdIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/resolvers/SCIMIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28267 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/resolvers/SQLIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/resolvers/UserIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/resolvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.329755 edumfa-2.0.0/edumfa/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/security/aeshsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/security/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/security/encryptkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.329755 edumfa-2.0.0/edumfa/lib/security/password/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/security/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/serviceid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.333755 edumfa-2.0.0/edumfa/lib/smsprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/FirebaseProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/HttpMessageToUidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/HttpSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/SMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/ScriptSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/SipgateSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/SmppSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/SmtpSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smsprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/sqlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.333755 edumfa-2.0.0/edumfa/lib/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/task/eventcounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/task/simplestats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96840 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68419 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokenclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokengroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.337755 edumfa-2.0.0/edumfa/lib/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/HMAC.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/applicationspecificpasswordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25837 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/certificatetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/daplugtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/daypasswordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/emailtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18983 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/foureyestoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33207 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/hotptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/indexedsecrettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/mOTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/motptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/ocra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/ocratoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/papertoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/passwordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46777 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/pushtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/questionnairetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/radiustoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/registrationtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/remotetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/smstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/spasstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/sshkeytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/tantoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/tiqrtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27633 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/totptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23127 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/u2ftoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/vasco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/vascotoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89138 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66757 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/webauthntoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/yubicotoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/tokens/yubikeytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/usercache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    55043 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/lib/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71279 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)   121289 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/static/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.277755 edumfa-2.0.0/edumfa/static/components/audit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/components/audit/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/audit/controllers/auditControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/components/audit/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/audit/factories/audit.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/components/audit/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/audit/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/components/audit/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/audit/views/audit.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/audit/views/audit.log.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.277755 edumfa-2.0.0/edumfa/static/components/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/components/components/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/components/controllers/componentControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/components/components/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/components/factories/component.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/components/components/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/components/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.341755 edumfa-2.0.0/edumfa/static/components/components/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/components/views/component.clienttype.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/components/views/component.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.281755 edumfa-2.0.0/edumfa/static/components/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.345755 edumfa-2.0.0/edumfa/static/components/config/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    50570 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/configControllers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/eduMfaServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/eventController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/ldapMachineResolverController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/periodicTaskController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/radiusServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/serviceidController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/smsgatewayController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/smtpServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/controllers/tokengroupController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.345755 edumfa-2.0.0/edumfa/static/components/config/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)    32353 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/factories/config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.345755 edumfa-2.0.0/edumfa/static/components/config/states/
+-rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.353755 edumfa-2.0.0/edumfa/static/components/config/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.caconnectors.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.caconnectors.local.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.caconnectors.microsoft.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.edumfaserver.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.edumfaserver.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.events.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.events.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.events.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.machineresolvers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.mresolvers.hosts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.mresolvers.ldap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.mresolvers.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.periodictasks.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.periodictasks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.periodictasks.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.policies.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.policies.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.policies.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.radius.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.radius.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.realms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.realms.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.http.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.ldap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.passwd.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.scim.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.sql.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.serviceid.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.serviceid.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.smsgateway.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.smsgateway.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.smtp.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.smtp.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.system.doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.system.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.system.html
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.email.html
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.question.html
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.radius.html
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.remote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.sms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.yubico.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.token.yubikey.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.tokengroup.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.tokengroup.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/config.tokens.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/config/views/dialog.confirm_delete.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.281755 edumfa-2.0.0/edumfa/static/components/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.353755 edumfa-2.0.0/edumfa/static/components/dashboard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/dashboard/controllers/dashboardControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.353755 edumfa-2.0.0/edumfa/static/components/dashboard/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/dashboard/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.353755 edumfa-2.0.0/edumfa/static/components/dashboard/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/dashboard/views/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.281755 edumfa-2.0.0/edumfa/static/components/dialogs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.357755 edumfa-2.0.0/edumfa/static/components/dialogs/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.about.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.lock.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.no.token.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.welcome.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.281755 edumfa-2.0.0/edumfa/static/components/directives/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.357755 edumfa-2.0.0/edumfa/static/components/directives/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19746 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/controllers/directives.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.357755 edumfa-2.0.0/edumfa/static/components/directives/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/views/directive.assigntoken.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/views/directive.assignuser.html
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/views/directive.attachmachine.html
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/views/directive.attachtoken.html
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/views/directive.csvdownload.html
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/views/directive.filter.table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/views/directive.policyconditions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/directives/views/directive.tokendata.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.357755 edumfa-2.0.0/edumfa/static/components/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/filters/filters.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.281755 edumfa-2.0.0/edumfa/static/components/login/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.357755 edumfa-2.0.0/edumfa/static/components/login/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    30344 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/controllers/loginControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.357755 edumfa-2.0.0/edumfa/static/components/login/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/factories/auth.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/factories/u2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/factories/webauthn.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.357755 edumfa-2.0.0/edumfa/static/components/login/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/login/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/views/enter-response.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/views/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/views/offline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/login/views/pinchange.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.281755 edumfa-2.0.0/edumfa/static/components/machine/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/machine/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/machine/controllers/machineController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/machine/controllers/machineDetailsController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/machine/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/machine/factories/machine.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/machine/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/machine/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/machine/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/machine/views/machine.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/machine/views/machine.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/machine/views/machine.list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.281755 edumfa-2.0.0/edumfa/static/components/recovery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/recovery/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/recovery/controllers/recoveryControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/recovery/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/recovery/factories/recoveryFactory.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/recovery/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/recovery/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/recovery/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/recovery/views/recovery.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/recovery/views/recovery.reset.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.281755 edumfa-2.0.0/edumfa/static/components/register/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/register/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/register/controllers/registerControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/register/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/register/factories/registerFactory.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/register/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/register/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/register/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/register/views/register.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/static/components/token/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.361755 edumfa-2.0.0/edumfa/static/components/token/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/controllers/tokenApplicationsController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/controllers/tokenChallengesController.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29864 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/controllers/tokenControllers.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/controllers/tokenDetailController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/controllers/tokenGetSerialController.js
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/controllers/tokenLostController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.365755 edumfa-2.0.0/edumfa/static/components/token/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/factories/token.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/factories/validate.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.365755 edumfa-2.0.0/edumfa/static/components/token/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.373755 edumfa-2.0.0/edumfa/static/components/token/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/dialog.ask_token_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.applications.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.applications.offline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.applications.ssh.html
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.assign.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.challenges.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32395 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.display.apps.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.4eyes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.applspec.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.certificate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.html
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.indexedsecret.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.motp.html
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.paper.html
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.push.html
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.question.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.radius.html
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.registration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.remote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.sms.html
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.spass.html
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.sshkey.html
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.tan.html
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.vasco.html
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.yubico.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.yubikey.html
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.applspec.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.certificate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.motp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.paper.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.push.html
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.registration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.tan.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.getserial.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.import.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/token/views/token.lost.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.373755 edumfa-2.0.0/edumfa/static/components/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)   557560 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/translation/translations.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/static/components/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.373755 edumfa-2.0.0/edumfa/static/components/user/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19169 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/controllers/userControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.373755 edumfa-2.0.0/edumfa/static/components/user/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/factories/user.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.373755 edumfa-2.0.0/edumfa/static/components/user/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.377755 edumfa-2.0.0/edumfa/static/components/user/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/views/dialog.ask_user_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/views/user.add.dynamic.form.fields.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/views/user.add.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/views/user.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/views/user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/views/user.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/components/user/views/user.password.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/static/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.377755 edumfa-2.0.0/edumfa/static/contrib/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/css/angular-inform.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/css/angular-inform.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    25682 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    48005 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145933 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   390887 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/css/hotkeys.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/css/isteven-multi-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.377755 edumfa-2.0.0/edumfa/static/contrib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.381755 edumfa-2.0.0/edumfa/static/contrib/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/angular-inform.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/angular-inform.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)  1377909 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/angular.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75484 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    53486 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/hotkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.385755 edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)    32388 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-gettext.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-idle.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33197 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-sanitize.js
+-rw-r--r--   0 runner    (1001) docker     (127)   487964 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js
+-rw-r--r--   0 runner    (1001) docker     (127)   760134 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js
+-rw-r--r--   0 runner    (1001) docker     (127)    81683 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/ng-file-upload.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/u2f-api.js
+-rw-r--r--   0 runner    (1001) docker     (127)   276562 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/ui-bootstrap-tpls.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.385755 edumfa-2.0.0/edumfa/static/contrib/js/webauthn-client/
+-rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.385755 edumfa-2.0.0/edumfa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/css/baseline.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/css/content.css
+-rw-r--r--   0 runner    (1001) docker     (127)    24602 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/css/eduMFA-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/css/highlight.css
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/css/menu.css
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/css/papertoken.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/css/signin.css
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/css/table-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.385755 edumfa-2.0.0/edumfa/static/customize/
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/customize/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.389755 edumfa-2.0.0/edumfa/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47610 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/img/plugup.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   336777 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/img/solokeys.png
+-rw-r--r--   0 runner    (1001) docker     (127)   107999 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/img/u2fzero.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.389755 edumfa-2.0.0/edumfa/static/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/providers/errorMessageProvider.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/providers/versioningProvider.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.389755 edumfa-2.0.0/edumfa/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/baseline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/cert_request_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/deactivated.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/templates/token_enrolled.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/static/update_contrib.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.389755 edumfa-2.0.0/edumfa/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23376 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    84098 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.393755 edumfa-2.0.0/edumfa/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    95309 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   127521 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.393755 edumfa-2.0.0/edumfa/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    81449 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   118619 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.393755 edumfa-2.0.0/edumfa/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    53719 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104451 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.285755 edumfa-2.0.0/edumfa/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.393755 edumfa-2.0.0/edumfa/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    87343 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.393755 edumfa-2.0.0/edumfa/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    85965 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   120848 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.393755 edumfa-2.0.0/edumfa/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.393755 edumfa-2.0.0/edumfa/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    78400 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   115604 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.393755 edumfa-2.0.0/edumfa/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    79882 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.397755 edumfa-2.0.0/edumfa/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    33313 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    96048 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/si/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.397755 edumfa-2.0.0/edumfa/translations/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/si/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    73291 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/si/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.397755 edumfa-2.0.0/edumfa/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    82030 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   117846 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.397755 edumfa-2.0.0/edumfa/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    68507 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104457 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/edumfa/translations/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.397755 edumfa-2.0.0/edumfa/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70327 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   105843 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.397755 edumfa-2.0.0/edumfa/webui/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/webui/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-12 08:48:25.000000 edumfa-2.0.0/edumfa/webui/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.453755 edumfa-2.0.0/edumfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-12 08:48:31.000000 edumfa-2.0.0/edumfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33263 2024-04-12 08:48:31.000000 edumfa-2.0.0/edumfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:48:31.000000 edumfa-2.0.0/edumfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 08:48:31.000000 edumfa-2.0.0/edumfa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:48:30.000000 edumfa-2.0.0/edumfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 08:48:31.000000 edumfa-2.0.0/edumfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 08:48:31.000000 edumfa-2.0.0/edumfa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.397755 edumfa-2.0.0/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.409755 edumfa-2.0.0/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/006d4747f858_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/00762b3f7a60_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/0c7123345224_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/0d011e94a8e8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/140ba0ca4f07_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/145ce80decd_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/14a1bcb10018_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/19f727d285e2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/1a0710df148b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/1a69e5e5e2ac_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/1edda52b619f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/204d8d4f351e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/205bda834127_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/20969b4cbf06_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/2118e566df16_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/2181294eed0b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/22558d9f3178_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/239995464c48_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/2551ee982544_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/2ac117d0a6f5_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/2c9430cfc66b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/307a4fbe8a05_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/3236a1abf1c6_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/3429d523e51f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/36428afb2457_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/37e6b49fc686_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/3ae3c668f444_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/3ba618f6b820_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/3c6e9dd7fbac_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/3d7f8b29cbb1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/3f7e8583ea2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/4023571658f8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/4238eac8ccab_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/449903fb6e35_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/48ee74b8a7c8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/49a04e560d96_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/4a0aec37e7cf_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/4d9178fa8336_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19377 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/4f32a4e1bf33_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/50adc980d625_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/5402fd96fbca_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/58e4f7ebb705_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/59ef3e03bc62_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/5cb310101a1f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/631ec59e1ca6_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/849170064430_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/86f40f535d7c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/888b56ed5dcb_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/89e57ed16379_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/8d40dbcfda25_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/9155f0d3d028_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/a28f2733897b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/a63df077051a_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/a7e91b18a460_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/b9131d0686eb_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/cb6d7b7bae63_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/d2ae8e54b628_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/d3c0f0403a84_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/d415d490eb05_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/d5870fd2f2a4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/d6b40a745e5_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/d756b34061ff_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/dceb6cd3c41e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/e360c56bcf8c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/e5cbeb7c177_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/ef29ba43e290_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/fa07bd604a75.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/fabcf24d9304_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 08:48:25.000000 edumfa-2.0.0/migrations/versions/ff26585932ec_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-12 08:48:25.000000 edumfa-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:48:31.457755 edumfa-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-12 08:48:25.000000 edumfa-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.433755 edumfa-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/ldap3mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/mscamock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/pkcs11mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/queuemock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/radiusmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/redismock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/smppmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/smtpmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_2stepinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20710 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48907 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_clienttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35517 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193396 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_lib_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_machineresolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38769 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16166 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_machines_serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_offline_no_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36128 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26177 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_push_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76125 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_serviceids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_smsgateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62186 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195170 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_ttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33099 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)   302927 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45689 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_db_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_authcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_challenges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_clientapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35302 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_eventhandler_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_eventhandler_usernotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113340 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29545 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_importotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_machine_resolver_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_machinetokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_monitoringstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75326 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36401 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_policydecorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123815 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32074 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_smsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_sqlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_task_eventcounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_task_simplestats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97908 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokenclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36699 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25260 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_daplug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27651 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_daypassword.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_foureyes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_hotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_indexedsecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_motp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_passwordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75419 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_spass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_tan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31214 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_tiqr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_vasco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_yubico.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_tokens_yubikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_usercache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45888 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_lib_utils_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38033 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_mock_ldap3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_resolver_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_ui_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/test_ui_login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.441755 edumfa-2.0.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/FIDO-U2F-Security-Key-444x444.png
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/NetKnights.pem
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.289755 edumfa-2.0.0/tests/testdata/altstatic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.441755 edumfa-2.0.0/tests/testdata/altstatic/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/altstatic/templates/testui.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.441755 edumfa-2.0.0/tests/testdata/attestation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/attestation/yubico.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/audit.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.445755 edumfa-2.0.0/tests/testdata/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/ca/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/ca/cakey.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/ca/index.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/ca/index.txt.attr
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/ca/openssl.cnf
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/ca/serial
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/ca/templates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/does_not_exist
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/emailtemplate.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/empty.oath
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/enckey
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/enckey.enc
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/event.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/fancytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/firebase-test.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/google-services.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.445755 edumfa-2.0.0/tests/testdata/gpg/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/gpg/public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/gpg/pubring.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/gpg/random_seed
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/gpg/secring.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/gpg/trustdb.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/hosts
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/import.oath
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/import.oath.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/jwt_sign.key
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/logging.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/logging_broken.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.445755 edumfa-2.0.0/tests/testdata/msca-connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/msca-connector/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/msca-connector/privacyidea-encrypted.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/msca-connector/privacyidea.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/msca-connector/privacyidea.pem
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/ocra.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/passwd
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/passwd-duplicate-name
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/passwords
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/policy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/policy.conf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/policy_empty_file.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/pskc-aes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/pskc-password.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/pw-2nd-resolver
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.445755 edumfa-2.0.0/tests/testdata/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/scripts/fail.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/scripts/ls.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/scripts/success.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/test.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/test2.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/testuser-api.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/testuser.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/testusercache.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.445755 edumfa-2.0.0/tests/testdata/trusted_attestation_roots/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/yubico-oath-long.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/yubico-oath.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 08:48:25.000000 edumfa-2.0.0/tests/testdata/yubico.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:48:31.453755 edumfa-2.0.0/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/creategoogleauthenticator-file
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-authorizedkeys
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1766 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-convert-base32.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-convert-token
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-convert-token.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-convert-xml-to-csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-ad-users
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-ad-users.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-certificate
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-certificate.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1985 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-pwidresolver-user
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-pwidresolver-user.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-sqlidresolver-user
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-sqlidresolver-user.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-userdb
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-create-userdb.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6795 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-cron
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7030 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-diag
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7372 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-expired-users
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1354 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-export-edumfa-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4514 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-export-linotp-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3719 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-fetchssh
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-fetchssh.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2500 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-fix-access-rights
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-fix-access-rights.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4303 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-get-serial
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5191 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-get-unused-tokens
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25361 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-migrate-linotp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2525 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-pip-update
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-pip-update.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-queue-huey
+-rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-schema-upgrade
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12070 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-standalone
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8176 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-sync-owncloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31000 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-token-janitor
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3746 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-update-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5391 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-update-linotp-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5471 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-user-action
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4203 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/edumfa-usercache-cleanup
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1476 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/getgooglecodes
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3049 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/reset-edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-12 08:48:25.000000 edumfa-2.0.0/tools/ssha.py
```

### Comparing `edumfa-1.5.1/AUTHORS.md` & `edumfa-2.0.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/LICENSE` & `edumfa-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/PKG-INFO` & `edumfa-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edumfa
-Version: 1.5.1
+Version: 2.0.0
 Summary: eduMFA: identity, multifactor authentication (OTP), authorization, audit
 Home-page: https://www.edumfa.io
 Author: edumfa.io
 Author-email: edumfa@listserv.dfn.de
 License: AGPLv3
 Keywords: OTP,two factor authentication,management,security
 Classifier: Framework :: Flask
@@ -12,68 +12,69 @@
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: beautifulsoup4[lxml]>=4.3.2
+Requires-Dist: Flask-Babel>=4.0.0
+Requires-Dist: Flask-Migrate>=3.2.0
+Requires-Dist: Flask-SQLAlchemy>=3.0
+Requires-Dist: Flask-Versioned>=0.9.4
+Requires-Dist: Flask>=3.0
+Requires-Dist: PyJWT>=1.3.0
+Requires-Dist: PyMySQL>=0.6.6
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: SQLAlchemy>=1.4.0
+Requires-Dist: argon2_cffi>=20.1.0
+Requires-Dist: beautifulsoup4[lxml]>=4.12.3
 Requires-Dist: cbor2>=5.0.1
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: croniter>=0.3.8
-Requires-Dist: cryptography>=2.4.2
+Requires-Dist: cryptography>=42.0.5
 Requires-Dist: defusedxml>=0.4.1
-Requires-Dist: Flask<2.0,>=0.10.1
-Requires-Dist: Flask-Babel>=0.9
-Requires-Dist: Flask-Migrate<3.0,>=1.2.0
-Requires-Dist: Flask-Script>=2.0.5
-Requires-Dist: Flask-SQLAlchemy>=2.0
-Requires-Dist: Flask-Versioned>=0.9.4
 Requires-Dist: google-auth>=1.23.0
+Requires-Dist: grpcio>=1.62.1
 Requires-Dist: huey[redis]>=1.11.0
 Requires-Dist: importlib_metadata>=2.1.1
 Requires-Dist: ldap3>=2.6
+Requires-Dist: lxml>=5.0.0
 Requires-Dist: netaddr>=0.7.12
 Requires-Dist: passlib[bcrypt]>=1.7.0
-Requires-Dist: argon2_cffi>=20.1.0
+Requires-Dist: psycopg2-binary>=2.9.9
+Requires-Dist: pyOpenSSL>=24
 Requires-Dist: pydash>=4.7.4
-Requires-Dist: PyJWT>=1.3.0
-Requires-Dist: PyMySQL>=0.6.6
-Requires-Dist: pyOpenSSL>=17.5
 Requires-Dist: pyrad>=2.0
 Requires-Dist: python-dateutil>=2.7.3
 Requires-Dist: python-gnupg>=0.4.4
-Requires-Dist: PyYAML>=5.1
-Requires-Dist: requests>=2.7.0
+Requires-Dist: requests>=2.31.0
 Requires-Dist: segno>=1.5
 Requires-Dist: smpplib>=2.0
-Requires-Dist: SQLAlchemy<2.0,>=1.4.0
-Requires-Dist: MarkupSafe<2.1
+Requires-Dist: typing-extensions>=4.6.0
+Requires-Dist: urllib3>=2.2.1
 Provides-Extra: doc
 Requires-Dist: Pallets-Sphinx-Themes>=1.2.3; extra == "doc"
 Requires-Dist: Sphinx>=1.3.1; extra == "doc"
 Requires-Dist: sphinxcontrib-httpdomain>=1.3.0; extra == "doc"
 Requires-Dist: sphinxcontrib-plantuml>=0.18; extra == "doc"
 Requires-Dist: sphinxcontrib-spelling>=7.0.0; extra == "doc"
 Provides-Extra: test
 Requires-Dist: mock>=2.0.0; extra == "test"
 Requires-Dist: pytest>=3.6.0; extra == "test"
 Requires-Dist: pytest-cov>=2.5.1; extra == "test"
 Requires-Dist: responses>=0.9.0; extra == "test"
 Requires-Dist: testfixtures>=6.14.2; extra == "test"
-Provides-Extra: postgres
-Requires-Dist: psycopg2>=2.8.3; extra == "postgres"
 Provides-Extra: hsm
 Requires-Dist: PyKCS11>=1.5.10; extra == "hsm"
 Provides-Extra: kerberos
 Requires-Dist: gssapi>=1.7.0; extra == "kerberos"
 
 eduMFA
 ===========
```

### Comparing `edumfa-1.5.1/README.rst` & `edumfa-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/apache/sites-available/edumfa.conf` & `edumfa-2.0.0/deploy/apache/sites-available/edumfa.conf`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/docker-compose-example.yml` & `edumfa-2.0.0/deploy/docker-compose-example.yml`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/docker-example/edumfa-policy.conf` & `edumfa-2.0.0/deploy/docker-example/edumfa-policy.conf`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/docker-example/edumfa.cfg` & `edumfa-2.0.0/deploy/docker-example/edumfa.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/docker-setup.sh` & `edumfa-2.0.0/deploy/docker-setup.sh`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/edumfa/dictionary` & `edumfa-2.0.0/deploy/edumfa/dictionary`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/edumfa/edumfa.cfg` & `edumfa-2.0.0/deploy/edumfa/edumfa.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/edumfa_radius.pm` & `edumfa-2.0.0/deploy/edumfa_radius.pm`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/logging.cfg` & `edumfa-2.0.0/deploy/logging.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/nginx/sites-available/edumfa` & `edumfa-2.0.0/deploy/nginx/sites-available/edumfa`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/rlm_perl.ini` & `edumfa-2.0.0/deploy/rlm_perl.ini`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/ubuntu/changelog` & `edumfa-2.0.0/deploy/ubuntu/changelog`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+edumfa (2.0.0{{CODENAME}}) {{CODENAME}}; urgency=medium
+ 
+ * chore: Several (major) dependency upgrades
+ * chore: Rework CLI tools and drop `Flask-Script` 
+
+ -- eduMFA <edumfa-dev@listserv.dfn.de>  Fri, 12 Apr 2024 12:00:00 +0200
+
 edumfa (1.5.1{{CODENAME}}) {{CODENAME}}; urgency=medium
 
   * fix: correct location of venv for ubuntu packages 
   * fix: ignore revoked, disabled webauthn tokens for passkey auth 
   * fix: correct handling of login mode 
 
  -- eduMFA <edumfa-dev@listserv.dfn.de>  Fri, 05 Apr 2024 12:00:00 +0200
@@ -25,23 +32,23 @@
   * feat: new API endpoint POST /info/<serial> to bulk modify tokeninfo
   * feat: token janitor find by user
   * fix: make ldap connections persistent and restartable
   * fix: wrong indentation caused false "Action .. requires serial number" line
   * fix: improve handling of resident keys
   * fix: rename provider module names in DB on migration
 
- -- eduMFA <edumfa-dev@listserv.dfn.de>  Tue, 19 Mar 2024 38:57:00 +0100
+ -- eduMFA <edumfa-dev@listserv.dfn.de>  Tue, 19 Mar 2024 12:00:00 +0100
 
 edumfa (1.3.0{{CODENAME}}) {{CODENAME}}; urgency=medium
 
   * Corrected ASCII art spacing
   * Handled Windows credProtect flag
   * Drop support for CentOS and Red Hat
 
- -- eduMFA <edumfa-dev@listserv.dfn.de>  Mon, 4 Mar 2024 38:34:00 +0100
+ -- eduMFA <edumfa-dev@listserv.dfn.de>  Mon, 4 Mar 2024 12:00:00 +0100
 
 edumfa (1.2.0{{CODENAME}}) {{CODENAME}}; urgency=medium
 
   * Bugfix Release for CI Actions
 
  -- eduMFA <edumfa-dev@listserv.dfn.de>  Fri, 1 Mar 2024 13:46:00 +0100
```

### Comparing `edumfa-1.5.1/deploy/ubuntu/control` & `edumfa-2.0.0/deploy/ubuntu/control`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/ubuntu/copyright` & `edumfa-2.0.0/deploy/ubuntu/copyright`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/ubuntu-radius/control` & `edumfa-2.0.0/deploy/ubuntu-radius/control`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/ubuntu-radius/copyright` & `edumfa-2.0.0/deploy/ubuntu-radius/copyright`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/ubuntu-radius/edumfa-radius.postinst` & `edumfa-2.0.0/deploy/ubuntu-radius/edumfa-radius.postinst`

 * *Files 13% similar despite different names*

```diff
@@ -12,44 +12,44 @@
 fi
 
 activate_perl() {
   ln -sf /etc/freeradius/3.0/mods-available/mods-perl-edumfa /etc/freeradius/3.0/mods-enabled/
 }
 
 activate_site() {
-	rm -f /etc/freeradius/3.0/sites-enabled/* || true
-	ln -s /etc/freeradius/3.0/sites-available/edumfa /etc/freeradius/3.0/sites-enabled/
+  rm -f /etc/freeradius/3.0/sites-enabled/* || true
+  ln -s /etc/freeradius/3.0/sites-available/edumfa /etc/freeradius/3.0/sites-enabled/
 }
 
 deactivate_eap() {
   # EAP will not run with perl
   if [ -L /etc/freeradius/3.0/mods-enabled/eap ]; then
     rm /etc/freeradius/3.0/mods-enabled/eap
   fi
 }
 
 case "$1" in
-
+  
   configure)
-  activate_perl
-	activate_site
-  deactivate_eap
-  systemctl enable freeradius
-  systemctl restart freeradius
+    activate_perl
+    activate_site
+    deactivate_eap
+    systemctl enable freeradius
+    systemctl restart freeradius
   ;;
-
+  
   abort-upgrade|abort-remove|abort-deconfigure)
     exit 0
   ;;
-
+  
   *)
     echo "postinst called with unknown argument \`$1'" >&2
     exit 1
   ;;
-
+  
 esac
 
 
 #DEBHELPER#
 
 db_stop
```

### Comparing `edumfa-1.5.1/deploy/ubuntu-server/control` & `edumfa-2.0.0/deploy/ubuntu-server/control`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/deploy/ubuntu-server/edumfa-apache2.postinst` & `edumfa-2.0.0/deploy/ubuntu-server/edumfa-apache2.postinst`

 * *Files 10% similar despite different names*

```diff
@@ -11,187 +11,182 @@
 if [ -f /usr/share/dbconfig-common/dpkg/postinst.pgsql  ]; then
   . /usr/share/dbconfig-common/dpkg/postinst.pgsql
 fi
 
 USERNAME=edumfa
 CERTDAYS=1095
 CERTKEYSIZE=4096
+MIGRATIONSDIR=/opt/edumfa/lib/edumfa/migrations/
 MYSQLFIX=/etc/mysql/conf.d/edumfa-maxkeylengthfix.cnf
+DB_CREATED=0
 
 if test -f /etc/default/edumfa; then
-    . /etc/default/edumfa
-    # If the daemon user was changed,
-    # we set other access rights
-    USERNAME=$USER
+  . /etc/default/edumfa
+  # If the daemon user was changed,
+  # we set other access rights
+  USERNAME=$USER
 fi
 
 
 create_user() {
-        useradd -r $USERNAME -m || true
+  useradd -r "$USERNAME" -m || true
 }
 
 create_files() {
-        mkdir -p /var/log/edumfa
-        mkdir -p /var/lib/edumfa
-	mkdir -p /etc/edumfa/scripts
-        touch /var/log/edumfa/edumfa.log
-        /opt/edumfa/bin/edumfa-manage create_enckey || true > /dev/null
-        /opt/edumfa/bin/edumfa-manage create_tables || true > /dev/null
-	#/opt/edumfa/bin/edumfa-manage createdb || true > /dev/null
-        /opt/edumfa/bin/edumfa-manage create_audit_keys || true > /dev/null
-        chown -R $USERNAME /var/log/edumfa
-        chown -R $USERNAME /var/lib/edumfa
-        chown -R $USERNAME /etc/edumfa
-        chmod 600 /etc/edumfa/enckey
-        chmod 600 /etc/edumfa/private.pem
-	# we need to change access right, otherwise each local user could call
-	# edumfa-manage
-	chgrp root /etc/edumfa/edumfa.cfg
-	chmod 640 /etc/edumfa/edumfa.cfg
+  mkdir -p /var/log/edumfa
+  mkdir -p /var/lib/edumfa
+  mkdir -p /etc/edumfa/scripts
+  touch /var/log/edumfa/edumfa.log
+  /opt/edumfa/bin/edumfa-manage create_enckey || true
+  /opt/edumfa/bin/edumfa-manage create_audit_keys || true
+  chown -R "$USERNAME" /var/log/edumfa
+  chown -R "$USERNAME" /var/lib/edumfa
+  chown -R "$USERNAME" /etc/edumfa
+  chmod 600 /etc/edumfa/enckey
+  chmod 600 /etc/edumfa/private.pem
+  # we need to change access right, otherwise each local user could call edumfa-manage
+  chgrp root /etc/edumfa/edumfa.cfg
+  chmod 640 /etc/edumfa/edumfa.cfg
 }
 
 create_certificate() {
-if [ ! -e /etc/edumfa/server.pem ]; then
-        # This is the certificate when running with paster...
-        cd /etc/edumfa
-        openssl genrsa -out server.key $CERTKEYSIZE
-        openssl req -new -key server.key -out server.csr -subj "/CN=edumfa"
-        openssl x509 -req -days $CERTDAYS -in server.csr -signkey server.key -out server.crt
-        cat server.crt server.key > server.pem
-        rm -f server.crt server.key
-        chown edumfa server.pem
-        chmod 400 server.pem
-fi
-
-if [ ! -e /etc/ssl/certs/edumfaserver.pem ]; then
-        # This is the certificate when running with apache or nginx
-        KEY=/etc/ssl/private/edumfaserver.key
-        CSR=`mktemp`
-        CERT=/etc/ssl/certs/edumfaserver.pem
-        openssl genrsa -out $KEY $CERTKEYSIZE
-        openssl req -new -key $KEY -out $CSR -subj "/CN=`hostname`"
-        openssl x509 -req -days $CERTDAYS -in $CSR -signkey $KEY -out $CERT
-        rm -f $CSR
-        chmod 400 $KEY
-fi
+  if [ ! -e /etc/edumfa/server.pem ]; then
+    # This is the certificate when running with paster...
+    cd /etc/edumfa
+    openssl genrsa -out server.key $CERTKEYSIZE
+    openssl req -new -key server.key -out server.csr -subj "/CN=edumfa"
+    openssl x509 -req -days $CERTDAYS -in server.csr -signkey server.key -out server.crt
+    cat server.crt server.key > server.pem
+    rm -f server.crt server.key
+    chown edumfa server.pem
+    chmod 400 server.pem
+  fi
+  
+  if [ ! -e /etc/ssl/certs/edumfaserver.pem ]; then
+    # This is the certificate when running with apache or nginx
+    KEY=/etc/ssl/private/edumfaserver.key
+    CSR=$(mktemp)
+    CERT=/etc/ssl/certs/edumfaserver.pem
+    openssl genrsa -out $KEY $CERTKEYSIZE
+    openssl req -new -key $KEY -out "$CSR" -subj "/CN=$(hostname)"
+    openssl x509 -req -days $CERTDAYS -in "$CSR" -signkey $KEY -out $CERT
+    rm -f "$CSR"
+    chmod 400 $KEY
+  fi
 }
 
 adapt_edumfa_cfg() {
-	if [ -z "$(grep '^EDUMFA_PEPPER' /etc/edumfa/edumfa.cfg)" ]; then
-	    # PEPPER does not exist, yet
-	    PEPPER="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c24)"
-	    echo "EDUMFA_PEPPER = '$PEPPER'" >> /etc/edumfa/edumfa.cfg
-	fi
-	if [ -z "$(grep '^SECRET_KEY' /etc/edumfa/edumfa.cfg)" ]; then
-	    # SECRET_KEY does not exist, yet
-	    SECRET="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c24)"
-	    echo "SECRET_KEY = '$SECRET'" >> /etc/edumfa/edumfa.cfg
-	fi
-	if [ -n "$(grep '^SQLALCHEMY_DATABASE_URI\s*=\s*.mysql:.*$' /etc/edumfa/edumfa.cfg)" ]; then
-	    #  We found an old mysql config file
-	    sed -i -e s/"\(^SQLALCHEMY_DATABASE_URI\s*=\s*.\)mysql:\(.*\)$"/"\1mysql+pymysql:\2"/g /etc/edumfa/edumfa.cfg
-	    echo "# The SQLALCHEMY_DATABASE_URI was updated during the update to eduMFA 3.2" >> /etc/edumfa/edumfa.cfg
-	fi
-
+  if ! grep -q '^EDUMFA_PEPPER' /etc/edumfa/edumfa.cfg; then
+    # PEPPER does not exist, yet
+    PEPPER="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c24)"
+    echo "EDUMFA_PEPPER = '$PEPPER'" >> /etc/edumfa/edumfa.cfg
+  fi
+  if ! grep -q '^SECRET_KEY' /etc/edumfa/edumfa.cfg; then
+    # SECRET_KEY does not exist, yet
+    SECRET="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c24)"
+    echo "SECRET_KEY = '$SECRET'" >> /etc/edumfa/edumfa.cfg
+  fi
+  if ! grep -q '^SQLALCHEMY_DATABASE_URI\s*=\s*.mysql:.*$' /etc/edumfa/edumfa.cfg; then
+    #  We found an old mysql config file
+    sed -i -e 's/\(^SQLALCHEMY_DATABASE_URI\s*=\s*.\)mysql:\(.*\)$/\1mysql+pymysql:\2/g' /etc/edumfa/edumfa.cfg
+    echo "# The SQLALCHEMY_DATABASE_URI was updated during the update to eduMFA 3.2" >> /etc/edumfa/edumfa.cfg
+  fi
 }
 
 create_database() {
   # Create the file with the MySQL Barracuda fix, if it does not exist
   if [ ! -f $MYSQLFIX ]; then
-    printf "[mariadb]\ninnodb_large_prefix=on\ninnodb_file_format=Barracuda\n" > /etc/mysql/conf.d/edumfa-maxkeylengthfix.cnf
+    printf "[mariadb]\ninnodb_large_prefix=on\ninnodb_file_format=Barracuda\n" > $MYSQLFIX
     systemctl restart mysql
   fi
-
-	# create the MYSQL database
-	if [ !$(grep "^SQLALCHEMY_DATABASE_URI" /etc/edumfa/edumfa.cfg || true) ]; then
-	    USER=$(grep "^user" /etc/mysql/debian.cnf | sort -u | awk '{print $3}')
-	    PASSWORD=$(grep "^password" /etc/mysql/debian.cnf | sort -u | awk '{print $3}')
-	    NPW="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c12)"
-	    mysql -u $USER --password=$PASSWORD -e "create database edumfa;" || true
-            mysql -u $USER --password=$PASSWORD -e "create user 'edumfa'@'localhost' IDENTIFIED BY '$NPW';"
-            mysql -u $USER --password=$PASSWORD -e "grant all privileges on edumfa.* to 'edumfa'@'localhost';"
-            echo "SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://edumfa:$NPW@localhost/edumfa?charset=utf8'" >> /etc/edumfa/edumfa.cfg
-            echo "DB created"
-        fi
+  # create the MYSQL database
+  if [ ! "$(grep "^SQLALCHEMY_DATABASE_URI" /etc/edumfa/edumfa.cfg || true)" ]; then
+    USER=$(grep "^user" /etc/mysql/debian.cnf | sort -u | awk '{print $3}')
+    PASSWORD=$(grep "^password" /etc/mysql/debian.cnf | sort -u | awk '{print $3}')
+    NPW="$(tr -dc A-Za-z0-9_ < /dev/urandom | head -c12)"
+    mysql -u "$USER" --password="$PASSWORD" -e "create database edumfa;" || true
+    mysql -u "$USER" --password="$PASSWORD" -e "create user 'edumfa'@'localhost' IDENTIFIED BY '$NPW';"
+    mysql -u "$USER" --password="$PASSWORD" -e "grant all privileges on edumfa.* to 'edumfa'@'localhost';"
+    echo "SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://edumfa:$NPW@localhost/edumfa?charset=utf8'" >> /etc/edumfa/edumfa.cfg
+    echo "DB created"
+    /opt/edumfa/bin/edumfa-manage create_tables || true
+    DB_CREATED=1
+  fi
 }
 
 enable_apache() {
-    a2enmod wsgi headers ssl rewrite
-    if [ ! -h /etc/apache2/sites-enabled/edumfa.conf ]; then
-        rm -f /etc/apache2/sites-enabled/*
-        a2ensite edumfa
-        ln -s /etc/ssl/certs/edumfaserver.pem /etc/ssl/certs/edumfa-bundle.crt || true
-        ln -s /etc/ssl/private/edumfaserver.key /etc/ssl/private/edumfa.key || true
-    fi
-    if [ ! -h /etc/apache2/sites-enabled/edumfa-venv.conf ]; then
-	a2ensite edumfa-venv
-    fi
+  a2enmod wsgi headers ssl rewrite
+  if [ ! -h /etc/apache2/sites-enabled/edumfa.conf ]; then
+    rm -f /etc/apache2/sites-enabled/*
+    a2ensite edumfa
+    ln -s /etc/ssl/certs/edumfaserver.pem /etc/ssl/certs/edumfa-bundle.crt || true
+    ln -s /etc/ssl/private/edumfaserver.key /etc/ssl/private/edumfa.key || true
+  fi
+  if [ ! -h /etc/apache2/sites-enabled/edumfa-venv.conf ]; then
+    a2ensite edumfa-venv
+  fi
 }
 
 update_db() {
-	# Upgrade the database
-	/opt/edumfa/bin/edumfa-schema-upgrade /opt/edumfa/lib/edumfa/migrations > /dev/null
+  # Upgrade the database
+  /opt/edumfa/bin/edumfa-schema-upgrade $MIGRATIONSDIR
 }
 
 create_gpg() {
-    if [ "jammy" = $(lsb_release -cs) ] && [ -n $(pgrep rngd) ]; then
-        echo "killing rngd process..."
-        killall -9 rngd || true
-    fi
-	mkdir -p /etc/edumfa/gpg
-	rngd -r /dev/urandom
-	/opt/edumfa/bin/edumfa-manage create_pgp_keys || true
-	chown -R $USERNAME /etc/edumfa/gpg
-	killall -9 rngd
+  if [ "jammy" = "$(lsb_release -cs)" ] && [ -n "$(pgrep rngd)" ]; then
+    echo "killing rngd process..."
+    killall -9 rngd || true
+  fi
+  mkdir -p /etc/edumfa/gpg
+  rngd -r /dev/urandom
+  /opt/edumfa/bin/edumfa-manage create_pgp_keys || true
+  chown -R "$USERNAME" /etc/edumfa/gpg
+  killall -9 rngd
 }
 
 
 set_path() {
-	# Allow edumfa-manage to be called from everywhere
-	ln -sf /opt/edumfa/bin/edumfa-manage /usr/bin/
-	ln -sf /opt/edumfa/bin/edumfa-diag /usr/bin/
-	ln -sf /opt/edumfa/bin/edumfa-token-janitor /usr/bin/
+  # Allow edumfa-manage to be called from everywhere
+  ln -sf /opt/edumfa/bin/edumfa-manage /usr/bin/
+  ln -sf /opt/edumfa/bin/edumfa-diag /usr/bin/
+  ln -sf /opt/edumfa/bin/edumfa-token-janitor /usr/bin/
 }
 
 case "$1" in
-
   configure)
-	export PATH=$PATH:/opt/edumfa/bin
-	create_user
-	adapt_edumfa_cfg
-	create_database	
-	enable_apache
-	create_files
-	create_certificate
-	#update-rc.d apache2 defaults
-	service apache2 restart
-	if [ -z "$2" ]; then
-		# We are in the install step
-		# So we stamp the DB
-		touch /tmp/edumfa-install
-		/opt/edumfa/bin/edumfa-manage db stamp -d /opt/edumfa/lib/edumfa/migrations/ head
-	else
-		# We are in an update step
-		touch /tmp/edumfa-upgrade
-		update_db
-	fi
-	create_gpg
-	set_path
+    export PATH=$PATH:/opt/edumfa/bin
+    create_user
+    adapt_edumfa_cfg
+    create_files
+    create_database
+    enable_apache
+    create_certificate
+    #update-rc.d apache2 defaults
+    service apache2 restart
+    if [ "$DB_CREATED" ]; then
+      # We've created the DB, so we stamp the DB
+      touch /tmp/edumfa-install
+      /opt/edumfa/bin/edumfa-manage db stamp -d $MIGRATIONSDIR head
+    else
+      # The DB was already created, so a update might be necessary
+      touch /tmp/edumfa-upgrade
+      update_db
+    fi
+    create_gpg
+    set_path
   ;;
-
+  
   abort-upgrade|abort-remove|abort-deconfigure)
     exit 0
   ;;
-
+  
   *)
     echo "postinst called with unknown argument \`$1'" >&2
     exit 1
   ;;
-
 esac
 
-
 #DEBHELPER#
 
 db_stop
 
 exit 0
```

### Comparing `edumfa-1.5.1/deploy/ubuntu-server/edumfa-apache2.postrm` & `edumfa-2.0.0/deploy/ubuntu-server/edumfa-apache2.postrm`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 # Source dbconfig-common functions
 if [ -f /usr/share/dbconfig-common/dpkg/postinst.pgsql  ]; then
   . /usr/share/dbconfig-common/dpkg/postinst.pgsql
 fi
 
 unset_sites () {
-    if [ ! "upgrade" = "$1" ]; then
-        rm -f /etc/apache2/sites-enabled/edumfa.conf
-        rm -f /etc/apache2/sites-enabled/edumfa-venv.conf
-    fi
+  if [ ! "upgrade" = "$1" ]; then
+    rm -f /etc/apache2/sites-enabled/edumfa.conf
+    rm -f /etc/apache2/sites-enabled/edumfa-venv.conf
+  fi
 }
 
-unset_sites $1
+unset_sites "$1"
 
 # Remove the symbolic link to edumfa-manage
 if [ -L /usr/local/bin/edumfa-manage ]; then
-    rm -f /usr/local/bin/edumfa-manage
-    rm -f /usr/bin/edumfa-manage
-    rm -f /usr/bin/edumfa-diag
-    rm -f /usr/bin/edumfa-token-janitor
+  rm -f /usr/local/bin/edumfa-manage
+  rm -f /usr/bin/edumfa-manage
+  rm -f /usr/bin/edumfa-diag
+  rm -f /usr/bin/edumfa-token-janitor
 fi
 
 #DEBHELPER#
 exit 0
```

### Comparing `edumfa-1.5.1/deploy/ubuntu-server/edumfa-nginx.postinst` & `edumfa-2.0.0/deploy/ubuntu-server/edumfa-nginx.postinst`

 * *Files 12% similar despite different names*

```diff
@@ -11,168 +11,166 @@
   . /usr/share/dbconfig-common/dpkg/postinst.pgsql
 fi
 
 USERNAME=edumfa
 CERTDAYS=1095
 CERTKEYSIZE=4096
 MIGRATIONSDIR=/opt/edumfa/lib/edumfa/migrations/
-MYSQLFIX=/etc/mysql/conf.d/edumfa-maxkeylengthfix.cnfh
+MYSQLFIX=/etc/mysql/conf.d/edumfa-maxkeylengthfix.cnf
+DB_CREATED=0
 
 
 if test -f /etc/default/edumfa; then
-    . /etc/default/edumfa
-    # If the daemon user was changed,
-    # we set other access rights
-    USERNAME=$USER
+  . /etc/default/edumfa
+  # If the daemon user was changed,
+  # we set other access rights
+  USERNAME=$USER
 fi
 
 
 create_user() {
-        useradd -r $USERNAME -m || true
+  useradd -r "$USERNAME" -m || true
 }
 
 create_files() {
-        mkdir -p /var/log/edumfa
-        mkdir -p /var/lib/edumfa
-	mkdir -p /etc/edumfa/scripts
-        touch /var/log/edumfa/edumfa.log
-	/opt/edumfa/bin/edumfa-manage create_enckey || true
-	/opt/edumfa/bin/edumfa-manage create_tables || true
-	#/opt/edumfa/bin/edumfa-manage createdb || true
-	/opt/edumfa/bin/edumfa-manage create_audit_keys || true
-        chown -R $USERNAME /var/log/edumfa
-        chown -R $USERNAME /var/lib/edumfa
-        chown -R $USERNAME /etc/edumfa
-        chmod 600 /etc/edumfa/enckey
-        chmod 600 /etc/edumfa/private.pem
-        # we need to change access right, otherwise each local user could call
-        # edumfa-manage
-        chgrp root /etc/edumfa/edumfa.cfg
-        chmod 640 /etc/edumfa/edumfa.cfg
+  mkdir -p /var/log/edumfa
+  mkdir -p /var/lib/edumfa
+  mkdir -p /etc/edumfa/scripts
+  touch /var/log/edumfa/edumfa.log
+  /opt/edumfa/bin/edumfa-manage create_enckey || true
+  /opt/edumfa/bin/edumfa-manage create_audit_keys || true
+  chown -R "$USERNAME" /var/log/edumfa
+  chown -R "$USERNAME" /var/lib/edumfa
+  chown -R "$USERNAME" /etc/edumfa
+  chmod 600 /etc/edumfa/enckey
+  chmod 600 /etc/edumfa/private.pem
+  # we need to change access right, otherwise each local user could call
+  # edumfa-manage
+  chgrp root /etc/edumfa/edumfa.cfg
+  chmod 640 /etc/edumfa/edumfa.cfg
 }
 
 create_certificate() {
-if [ ! -e /etc/edumfa/server.pem ]; then
-        # This is the certificate when running with paster...
-        cd /etc/edumfa
-        openssl genrsa -out server.key $CERTKEYSIZE
-        openssl req -new -key server.key -out server.csr -subj "/CN=edumfa"
-        openssl x509 -req -days $CERTDAYS -in server.csr -signkey server.key -out server.crt
-        cat server.crt server.key > server.pem
-        rm -f server.crt server.key
-        chown edumfa server.pem
-        chmod 400 server.pem
-fi
-
-if [ ! -e /etc/ssl/certs/edumfaserver.pem ]; then
-        # This is the certificate when running with apache or nginx
-        KEY=/etc/ssl/private/edumfaserver.key
-        CSR=`mktemp`
-        CERT=/etc/ssl/certs/edumfaserver.pem
-        openssl genrsa -out $KEY $CERTKEYSIZE
-        openssl req -new -key $KEY -out $CSR -subj "/CN=`hostname`"
-        openssl x509 -req -days $CERTDAYS -in $CSR -signkey $KEY -out $CERT
-        rm -f $CSR
-        chmod 400 $KEY
-fi
+  if [ ! -e /etc/edumfa/server.pem ]; then
+    # This is the certificate when running with paster...
+    cd /etc/edumfa
+    openssl genrsa -out server.key $CERTKEYSIZE
+    openssl req -new -key server.key -out server.csr -subj "/CN=edumfa"
+    openssl x509 -req -days $CERTDAYS -in server.csr -signkey server.key -out server.crt
+    cat server.crt server.key > server.pem
+    rm -f server.crt server.key
+    chown edumfa server.pem
+    chmod 400 server.pem
+  fi
+  
+  if [ ! -e /etc/ssl/certs/edumfaserver.pem ]; then
+    # This is the certificate when running with apache or nginx
+    KEY=/etc/ssl/private/edumfaserver.key
+    CSR=$(mktemp)
+    CERT=/etc/ssl/certs/edumfaserver.pem
+    openssl genrsa -out $KEY $CERTKEYSIZE
+    openssl req -new -key $KEY -out "$CSR" -subj "/CN=$(hostname)"
+    openssl x509 -req -days $CERTDAYS -in "$CSR" -signkey $KEY -out $CERT
+    rm -f "$CSR"
+    chmod 400 $KEY
+  fi
 }
 
 adapt_edumfa_cfg() {
-	if [ !$(grep "^EDUMFA_PEPPER" /etc/edumfa/edumfa.cfg) ]; then
-	    # PEPPER does not exist, yet
-	    PEPPER="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c24)"
-	    echo "EDUMFA_PEPPER = '$PEPPER'" >> /etc/edumfa/edumfa.cfg
-	fi
-	if [ !$(grep "^SECRET_KEY" /etc/edumfa/edumfa.cfg || true) ]; then
-	    # SECRET_KEY does not exist, yet
-	    SECRET="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c24)"
-	    echo "SECRET_KEY = '$SECRET'" >> /etc/edumfa/edumfa.cfg
-	fi
-        if [ -n "$(grep '^SQLALCHEMY_DATABASE_URI\s*=\s*.mysql:.*$' /etc/edumfa/edumfa.cfg)" ]; then
-	    #  We found an old mysql config file
-	    sed -i -e s/"\(^SQLALCHEMY_DATABASE_URI\s*=\s*.\)mysql:\(.*\)$"/"\1mysql+pymysql:\2"/g /etc/edumfa/edumfa.cfg
-	    echo "# The SQLALCHEMY_DATABASE_URI was updated during the update to eduMFA 3.2" >> /etc/edumfa/edumfa.cfg
-	fi
+  if ! grep -q '^EDUMFA_PEPPER' /etc/edumfa/edumfa.cfg; then
+    # PEPPER does not exist, yet
+    PEPPER="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c24)"
+    echo "EDUMFA_PEPPER = '$PEPPER'" >> /etc/edumfa/edumfa.cfg
+  fi
+  if ! grep -q '^SECRET_KEY' /etc/edumfa/edumfa.cfg; then
+    # SECRET_KEY does not exist, yet
+    SECRET="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c24)"
+    echo "SECRET_KEY = '$SECRET'" >> /etc/edumfa/edumfa.cfg
+  fi
+  if ! grep -q '^SQLALCHEMY_DATABASE_URI\s*=\s*.mysql:.*$' /etc/edumfa/edumfa.cfg; then
+    #  We found an old mysql config file
+    sed -i -e 's/\(^SQLALCHEMY_DATABASE_URI\s*=\s*.\)mysql:\(.*\)$/\1mysql+pymysql:\2/g' /etc/edumfa/edumfa.cfg
+    echo "# The SQLALCHEMY_DATABASE_URI was updated during the update to eduMFA 3.2" >> /etc/edumfa/edumfa.cfg
+  fi
 }
 
 create_database() {
-        # Create the file with the MySQL Barracuda fix, if it does not exist
-        if [ ! -f $MYSQLFIX ]; then
-                printf "[mariadb]\ninnodb_large_prefix=on\ninnodb_file_format=Barracuda\n" > $MYSQLFIX
-                systemctl restart mysql
-        fi
-	# create the MYSQL database
-	if [ !$(grep "^SQLALCHEMY_DATABASE_URI" /etc/edumfa/edumfa.cfg || true) ]; then
-	    USER="debian-sys-maint"
-	    PASSWORD=$(grep "^password" /etc/mysql/debian.cnf | sort -u | cut -d " " -f3)
-	    NPW="$(tr -dc A-Za-z0-9_ </dev/urandom | head -c12)"
-	    mysql -u $USER --password=$PASSWORD -e "create database edumfa;" || true
-	    mysql -u $USER --password=$PASSWORD -e "create user 'edumfa'@'localhost' IDENTIFIED BY '$NPW';"
-	    mysql -u $USER --password=$PASSWORD -e "grant all privileges on edumfa.* to 'edumfa'@'localhost';"
-	    echo "SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://edumfa:$NPW@localhost/edumfa?charset=utf8'" >> /etc/edumfa/edumfa.cfg
-	fi
+  # Create the file with the MySQL Barracuda fix, if it does not exist
+  if [ ! -f $MYSQLFIX ]; then
+    printf "[mariadb]\ninnodb_large_prefix=on\ninnodb_file_format=Barracuda\n" > $MYSQLFIX
+    systemctl restart mysql
+  fi
+  # create the MYSQL database
+  if [ ! "$(grep "^SQLALCHEMY_DATABASE_URI" /etc/edumfa/edumfa.cfg || true)" ]; then
+    USER=$(grep "^user" /etc/mysql/debian.cnf | sort -u | awk '{print $3}')
+    PASSWORD=$(grep "^password" /etc/mysql/debian.cnf | sort -u | awk '{print $3}')
+    NPW="$(tr -dc A-Za-z0-9_ < /dev/urandom | head -c12)"
+    mysql -u "$USER" --password="$PASSWORD" -e "create database edumfa;" || true
+    mysql -u "$USER" --password="$PASSWORD" -e "create user 'edumfa'@'localhost' IDENTIFIED BY '$NPW';"
+    mysql -u "$USER" --password="$PASSWORD" -e "grant all privileges on edumfa.* to 'edumfa'@'localhost';"
+    echo "SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://edumfa:$NPW@localhost/edumfa?charset=utf8'" >> /etc/edumfa/edumfa.cfg
+    echo "DB created"
+    /opt/edumfa/bin/edumfa-manage create_tables || true
+    DB_CREATED=1
+  fi
 }
 
 enable_nginx_uwsgi() {
-        rm -f /etc/nginx/sites-enabled/*
-        rm -f /etc/uwsgi/apps-enabled/*
-        ln -sf /etc/nginx/sites-available/edumfa /etc/nginx/sites-enabled/
-	ln -sf /etc/uwsgi/apps-available/edumfa.xml /etc/uwsgi/apps-enabled/
-
-	ln -s /etc/ssl/certs/edumfaserver.pem /etc/ssl/certs/edumfa-bundle.crt || true
-	ln -s /etc/ssl/private/edumfaserver.key /etc/ssl/private/edumfa.key || true
+  rm -f /etc/nginx/sites-enabled/*
+  rm -f /etc/uwsgi/apps-enabled/*
+  ln -sf /etc/nginx/sites-available/edumfa /etc/nginx/sites-enabled/
+  ln -sf /etc/uwsgi/apps-available/edumfa.xml /etc/uwsgi/apps-enabled/
+  
+  ln -s /etc/ssl/certs/edumfaserver.pem /etc/ssl/certs/edumfa-bundle.crt || true
+  ln -s /etc/ssl/private/edumfaserver.key /etc/ssl/private/edumfa.key || true
 }
 
 update_db() {
-        # Upgrade the database
-	/opt/edumfa/bin/edumfa-schema-upgrade $MIGRATIONSDIR > /dev/null
+  # Upgrade the database
+  /opt/edumfa/bin/edumfa-schema-upgrade $MIGRATIONSDIR
 }
 
-
 set_path() {
-	# Allow edumfa-manage to be called
-	ln -sf /opt/edumfa/bin/edumfa-manage /usr/bin/
-	ln -sf /opt/edumfa/bin/edumfa-diag /usr/bin/
-	ln -sf /opt/edumfa/bin/edumfa-token-janitor /usr/bin/
+  # Allow edumfa-manage to be called
+  ln -sf /opt/edumfa/bin/edumfa-manage /usr/bin/
+  ln -sf /opt/edumfa/bin/edumfa-diag /usr/bin/
+  ln -sf /opt/edumfa/bin/edumfa-token-janitor /usr/bin/
 }
 
 case "$1" in
-
+  
   configure)
-        set_path
-	create_user
-	adapt_edumfa_cfg
-        create_database     
-	enable_nginx_uwsgi
-	create_files
-	create_certificate
-        if [ -z "$2" ]; then
-		# We are in the install step
-		# So we stamp the DB
-		/opt/edumfa/bin/edumfa-manage db stamp -d $MIGRATIONSDIR head
-	else
-		# We are in an update step
-		update_db
-	fi
-	#update-rc.d nginx defaults
-	#update-rc.d uwsgi defaults
-	service uwsgi restart
-	service nginx restart
+    set_path
+    create_user
+    adapt_edumfa_cfg
+    create_files
+    create_database
+    enable_nginx_uwsgi
+    create_certificate
+    if [ "$DB_CREATED" ]; then
+      # We've created the DB, so we stamp the DB
+      /opt/edumfa/bin/edumfa-manage db stamp -d $MIGRATIONSDIR head
+    else
+      # The DB was already created, so a update might be necessary
+      update_db
+    fi
+    #update-rc.d nginx defaults
+    #update-rc.d uwsgi defaults
+    service uwsgi restart
+    service nginx restart
   ;;
-
+  
   abort-upgrade|abort-remove|abort-deconfigure)
     exit 0
   ;;
-
+  
   *)
     echo "postinst called with unknown argument \`$1'" >&2
     exit 1
   ;;
-
 esac
 
-
 #DEBHELPER#
 
 db_stop
 
 exit 0
```

### Comparing `edumfa-1.5.1/deploy/ubuntu-server/edumfa-nginx.postrm` & `edumfa-2.0.0/deploy/ubuntu-server/edumfa-nginx.postrm`

 * *Files 16% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 
 # Source dbconfig-common functions
 if [ -f /usr/share/dbconfig-common/dpkg/postinst.pgsql  ]; then
   . /usr/share/dbconfig-common/dpkg/postinst.pgsql
 fi
 
 unset_sites () {
-	rm -f /etc/nginx/sites-enabled/edumfa
-	rm -f /etc/uwsgi/apps-enabled/edumfa.xml
+  rm -f /etc/nginx/sites-enabled/edumfa
+  rm -f /etc/uwsgi/apps-enabled/edumfa.xml
 }
 
-
 unset_sites
 
 # Remove the symbolic link to edumfa-manage
 if [ -L /usr/local/bin/edumfa-manage ]; then
-    rm /usr/local/bin/edumfa-manage
+  rm -f /usr/local/bin/edumfa-manage
+  rm -f /usr/bin/edumfa-manage
+  rm -f /usr/bin/edumfa-diag
+  rm -f /usr/bin/edumfa-token-janitor
 fi
 
 #DEBHELPER#
 exit 0
```

### Comparing `edumfa-1.5.1/deploy/uwsgi/apps-available/edumfa.xml` & `edumfa-2.0.0/deploy/uwsgi/apps-available/edumfa.xml`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/__init__.py` & `edumfa-2.0.0/edumfa/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/__init__.py` & `edumfa-2.0.0/edumfa/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/application.py` & `edumfa-2.0.0/edumfa/api/application.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/audit.py` & `edumfa-2.0.0/edumfa/api/audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/auth.py` & `edumfa-2.0.0/edumfa/api/auth.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/before_after.py` & `edumfa-2.0.0/edumfa/api/before_after.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/caconnector.py` & `edumfa-2.0.0/edumfa/api/caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/clienttype.py` & `edumfa-2.0.0/edumfa/api/clienttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/edumfaserver.py` & `edumfa-2.0.0/edumfa/api/edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/event.py` & `edumfa-2.0.0/edumfa/api/event.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/lib/decorators.py` & `edumfa-2.0.0/edumfa/api/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/lib/policyhelper.py` & `edumfa-2.0.0/edumfa/api/lib/policyhelper.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/lib/postpolicy.py` & `edumfa-2.0.0/edumfa/api/lib/postpolicy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/lib/prepolicy.py` & `edumfa-2.0.0/edumfa/api/lib/prepolicy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/lib/utils.py` & `edumfa-2.0.0/edumfa/api/lib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,17 @@
     return_param = {}
     if param:
         log.debug("Update params in request {0!s} {1!s} with values.".format(request.method,
                                                                              request.base_url))
         # Add the unquoted HTML and form parameters
         return_param = check_unquote(request, request.values)
 
+    if request.method == "GET" and request.form:
+        return_param.update(check_unquote(request, request.form))
+
     if request.is_json:
         log.debug("Update params in request {0!s} {1!s} with JSON data.".format(request.method,
                                                                                 request.base_url))
         # Add the original JSON data
         return_param.update(request.json)
     elif body:
         # In case of serialized JSON data in the body, add these to the values.
```

### Comparing `edumfa-1.5.1/edumfa/api/machine.py` & `edumfa-2.0.0/edumfa/api/machine.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/machineresolver.py` & `edumfa-2.0.0/edumfa/api/machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/monitoring.py` & `edumfa-2.0.0/edumfa/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/periodictask.py` & `edumfa-2.0.0/edumfa/api/periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/policy.py` & `edumfa-2.0.0/edumfa/api/policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/radiusserver.py` & `edumfa-2.0.0/edumfa/api/radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/realm.py` & `edumfa-2.0.0/edumfa/api/realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/recover.py` & `edumfa-2.0.0/edumfa/api/recover.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/register.py` & `edumfa-2.0.0/edumfa/api/register.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/resolver.py` & `edumfa-2.0.0/edumfa/api/resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/serviceid.py` & `edumfa-2.0.0/edumfa/api/serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/smsgateway.py` & `edumfa-2.0.0/edumfa/api/smsgateway.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/smtpserver.py` & `edumfa-2.0.0/edumfa/api/smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/system.py` & `edumfa-2.0.0/edumfa/api/system.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/token.py` & `edumfa-2.0.0/edumfa/api/token.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/tokengroup.py` & `edumfa-2.0.0/edumfa/api/tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/ttype.py` & `edumfa-2.0.0/edumfa/api/ttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/user.py` & `edumfa-2.0.0/edumfa/api/user.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/api/validate.py` & `edumfa-2.0.0/edumfa/api/validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/app.py` & `edumfa-2.0.0/edumfa/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,38 +66,42 @@
 from edumfa.api.serviceid import serviceid_blueprint
 from edumfa.lib import queue
 from edumfa.lib.log import DEFAULT_LOGGING_CONFIG
 from edumfa.config import config
 from edumfa.models import db
 from edumfa.lib.crypto import init_hsm
 
-
 ENV_KEY = "EDUMFA_CONFIGFILE"
 
 
 class PiResponseClass(Response):
     """Custom Response class overwriting the flask.Response.
     To avoid caching problems with the json property in the Response class,
     the property is overwritten using a non-caching approach.
     """
+
     @property
     def json(self):
         """This will contain the parsed JSON data if the mimetype indicates
         JSON (:mimetype:`application/json`, see :meth:`is_json`), otherwise it
         will be ``None``.
         Caching of the json data is disabled.
         """
-        return self.get_json(cache=False)
+        return self.get_json()
 
     default_mimetype = 'application/json'
 
 
+def get_locale():
+    return get_accepted_language(request)
+
+
 def create_app(config_name="development",
                config_file='/etc/edumfa/edumfa.cfg',
-               silent=False, init_hsm=False):
+               silent=False, init_hsm=False, script=False):
     """
     First the configuration from the config.py is loaded depending on the
     config type like "production" or "development" or "testing".
 
     Then the environment variable EDUMFA_CONFIGFILE is checked for a
     config file, that contains additional settings, that will overwrite the
     default settings from config.py
@@ -175,15 +179,16 @@
     app.register_blueprint(eventhandling_blueprint, url_prefix='/event')
     app.register_blueprint(smsgateway_blueprint, url_prefix='/smsgateway')
     app.register_blueprint(client_blueprint, url_prefix='/client')
     app.register_blueprint(monitoring_blueprint, url_prefix='/monitoring')
     app.register_blueprint(tokengroup_blueprint, url_prefix='/tokengroup')
     app.register_blueprint(serviceid_blueprint, url_prefix='/serviceid')
     db.init_app(app)
-    migrate = Migrate(app, db)
+    if not script:
+        migrate = Migrate(app, db)
 
     app.response_class = PiResponseClass
 
     # Setup logging
     log_read_func = {
         'yaml': lambda x: logging.config.dictConfig(yaml.safe_load(open(x, 'r').read())),
         'cfg': lambda x: logging.config.fileConfig(x)
@@ -214,19 +219,15 @@
             sys.stderr.write("Using EDUMFA_LOGLEVEL {0!s}.\n".format(level))
             sys.stderr.write("Using EDUMFA_LOGFILE {0!s}.\n".format(logfile))
         DEFAULT_LOGGING_CONFIG["handlers"]["file"]["filename"] = logfile
         DEFAULT_LOGGING_CONFIG["handlers"]["file"]["level"] = level
         DEFAULT_LOGGING_CONFIG["loggers"]["edumfa"]["level"] = level
         logging.config.dictConfig(DEFAULT_LOGGING_CONFIG)
 
-    babel = Babel(app)
-
-    @babel.localeselector
-    def get_locale():
-        return get_accepted_language(request)
+    babel = Babel(app, locale_selector=get_locale)
 
     queue.register_app(app)
 
     if init_hsm:
         with app.app_context():
             init_hsm()
```

### Comparing `edumfa-1.5.1/edumfa/config.py` & `edumfa-2.0.0/edumfa/config.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/__init__.py` & `edumfa-2.0.0/edumfa/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/applications/__init__.py` & `edumfa-2.0.0/edumfa/lib/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/applications/base.py` & `edumfa-2.0.0/edumfa/lib/applications/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/applications/luks.py` & `edumfa-2.0.0/edumfa/lib/applications/luks.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/applications/offline.py` & `edumfa-2.0.0/edumfa/lib/applications/offline.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/applications/ssh.py` & `edumfa-2.0.0/edumfa/lib/applications/ssh.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/apps.py` & `edumfa-2.0.0/edumfa/lib/apps.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/audit.py` & `edumfa-2.0.0/edumfa/lib/audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/auditmodules/base.py` & `edumfa-2.0.0/edumfa/lib/auditmodules/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/auditmodules/containeraudit.py` & `edumfa-2.0.0/edumfa/lib/auditmodules/containeraudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/auditmodules/loggeraudit.py` & `edumfa-2.0.0/edumfa/lib/auditmodules/loggeraudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/auditmodules/sqlaudit.py` & `edumfa-2.0.0/edumfa/lib/auditmodules/sqlaudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/auth.py` & `edumfa-2.0.0/edumfa/lib/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from edumfa.lib.crypto import hash_with_pepper, verify_with_pepper
 from edumfa.lib.utils import fetch_one_resource
 import logging
 
 log = logging.getLogger(__name__)
 
 
-
 class ROLE(object):
     ADMIN = "admin"
     USER = "user"
     VALIDATE = "validate"
 
 
 def verify_db_admin(username, password):
@@ -63,30 +62,22 @@
 
     :param username: The username of the admin
     :return: True, if exist
     """
     return bool(get_db_admin(username))
 
 
-def create_db_admin(app, username, email=None, password=None):
+def create_db_admin(username: str, email: str = None, password=None):
     pw_dig = None
     if password:
         pw_dig = hash_with_pepper(password)
     user = Admin(email=email, username=username, password=pw_dig)
     user.save()
 
 
-def list_db_admin():
-    admins = Admin.query.all()
-    print("Name \t email")
-    print(30*"=")
-    for admin in admins:
-        print("{0!s} \t {1!s}".format(admin.username, admin.email))
-
-
 def get_db_admins():
     admins = Admin.query.all()
     return admins
 
 
 def get_db_admin(username):
     return Admin.query.filter(Admin.username == username).first()
@@ -115,16 +106,15 @@
     :param user_obj: The user who tries to authenticate
     :type user_obj: User Object
     :param password: Password, static and or OTP
     :param options: additional options like g and clientip
     :type options: dict
     :param superuser_realms: list of realms, that contain admins
     :type superuser_realms: list
-    :param check_otp: If set, the user is not authenticated against the
-         userstore but against eduMFA
+    :param check_otp: If set, the user is not authenticated against the userstore but against eduMFA
     :return: tuple of bool, string and dict/None
     """
     options = options or {}
     superuser_realms = superuser_realms or []
     user_auth = False
     role = ROLE.USER
     details = None
```

### Comparing `edumfa-1.5.1/edumfa/lib/authcache.py` & `edumfa-2.0.0/edumfa/lib/authcache.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/caconnector.py` & `edumfa-2.0.0/edumfa/lib/caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/caconnectors/baseca.py` & `edumfa-2.0.0/edumfa/lib/caconnectors/baseca.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/caconnectors/caservice_pb2.py` & `edumfa-2.0.0/edumfa/lib/caconnectors/caservice_pb2.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/caconnectors/caservice_pb2_grpc.py` & `edumfa-2.0.0/edumfa/lib/caconnectors/caservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/caconnectors/localca.py` & `edumfa-2.0.0/edumfa/lib/caconnectors/localca.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/caconnectors/msca.py` & `edumfa-2.0.0/edumfa/lib/caconnectors/msca.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/challenge.py` & `edumfa-2.0.0/edumfa/lib/challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         sortby = cols.get(sortby)
 
     if sortdir == "desc":
         sql_query = sql_query.order_by(sortby.desc())
     else:
         sql_query = sql_query.order_by(sortby.asc())
 
-    pagination = sql_query.paginate(page, per_page=psize,
+    pagination = sql_query.paginate(page=page, per_page=psize,
                                     error_out=False)
     challenges = pagination.items
     prev = None
     if pagination.has_prev:
         prev = page-1
     next = None
     if pagination.has_next:
```

### Comparing `edumfa-1.5.1/edumfa/lib/challengeresponsedecorators.py` & `edumfa-2.0.0/edumfa/lib/challengeresponsedecorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/clientapplication.py` & `edumfa-2.0.0/edumfa/lib/clientapplication.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/config.py` & `edumfa-2.0.0/edumfa/lib/config.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/counter.py` & `edumfa-2.0.0/edumfa/lib/counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/crypto.py` & `edumfa-2.0.0/edumfa/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/decorators.py` & `edumfa-2.0.0/edumfa/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/edumfaserver.py` & `edumfa-2.0.0/edumfa/lib/edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/error.py` & `edumfa-2.0.0/edumfa/lib/error.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/event.py` & `edumfa-2.0.0/edumfa/lib/event.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/base.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/counterhandler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/counterhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/customuserattributeshandler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/customuserattributeshandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/federationhandler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/federationhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/logginghandler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/logginghandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/requestmangler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/requestmangler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/responsemangler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/responsemangler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/scripthandler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/scripthandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/tokenhandler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/tokenhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/usernotification.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/usernotification.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/eventhandler/webhookeventhandler.py` & `edumfa-2.0.0/edumfa/lib/eventhandler/webhookeventhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/framework.py` & `edumfa-2.0.0/edumfa/lib/framework.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/importotp.py` & `edumfa-2.0.0/edumfa/lib/importotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/lifecycle.py` & `edumfa-2.0.0/edumfa/lib/lifecycle.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/log.py` & `edumfa-2.0.0/edumfa/lib/log.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/machine.py` & `edumfa-2.0.0/edumfa/lib/machine.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/machineresolver.py` & `edumfa-2.0.0/edumfa/lib/machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/machines/__init__.py` & `edumfa-2.0.0/edumfa/lib/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/machines/base.py` & `edumfa-2.0.0/edumfa/lib/machines/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/machines/hosts.py` & `edumfa-2.0.0/edumfa/lib/machines/hosts.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/machines/ldap.py` & `edumfa-2.0.0/edumfa/lib/machines/ldap.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/monitoringmodules/base.py` & `edumfa-2.0.0/edumfa/lib/monitoringmodules/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/monitoringmodules/sqlstats.py` & `edumfa-2.0.0/edumfa/lib/monitoringmodules/sqlstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/monitoringstats.py` & `edumfa-2.0.0/edumfa/lib/monitoringstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/passwordreset.py` & `edumfa-2.0.0/edumfa/lib/passwordreset.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/periodictask.py` & `edumfa-2.0.0/edumfa/lib/periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/pinhandling/base.py` & `edumfa-2.0.0/edumfa/lib/pinhandling/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/policy.py` & `edumfa-2.0.0/edumfa/lib/policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/policydecorators.py` & `edumfa-2.0.0/edumfa/lib/policydecorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/pooling.py` & `edumfa-2.0.0/edumfa/lib/pooling.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/queue.py` & `edumfa-2.0.0/edumfa/lib/queue.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/queues/__init__.py` & `edumfa-2.0.0/edumfa/lib/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/queues/base.py` & `edumfa-2.0.0/edumfa/lib/queues/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/queues/huey_queue.py` & `edumfa-2.0.0/edumfa/lib/queues/huey_queue.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/radiusserver.py` & `edumfa-2.0.0/edumfa/lib/radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/realm.py` & `edumfa-2.0.0/edumfa/lib/realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/resolver.py` & `edumfa-2.0.0/edumfa/lib/resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/resolvers/HTTPResolver.py` & `edumfa-2.0.0/edumfa/lib/resolvers/HTTPResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/resolvers/LDAPIdResolver.py` & `edumfa-2.0.0/edumfa/lib/resolvers/LDAPIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/resolvers/PasswdIdResolver.py` & `edumfa-2.0.0/edumfa/lib/resolvers/PasswdIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/resolvers/SCIMIdResolver.py` & `edumfa-2.0.0/edumfa/lib/resolvers/SCIMIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/resolvers/SQLIdResolver.py` & `edumfa-2.0.0/edumfa/lib/resolvers/SQLIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/resolvers/UserIdResolver.py` & `edumfa-2.0.0/edumfa/lib/resolvers/UserIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/security/aeshsm.py` & `edumfa-2.0.0/edumfa/lib/security/aeshsm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/security/default.py` & `edumfa-2.0.0/edumfa/lib/security/default.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/security/encryptkey.py` & `edumfa-2.0.0/edumfa/lib/security/encryptkey.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/serviceid.py` & `edumfa-2.0.0/edumfa/lib/serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/FirebaseProvider.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/FirebaseProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/HttpMessageToUidProvider.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/HttpMessageToUidProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/HttpSMSProvider.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/HttpSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/SMSProvider.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/SMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/ScriptSMSProvider.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/ScriptSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/SipgateSMSProvider.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/SipgateSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/SmppSMSProvider.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/SmppSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/SmtpSMSProvider.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/SmtpSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smsprovider/__init__.py` & `edumfa-2.0.0/edumfa/lib/smsprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/smtpserver.py` & `edumfa-2.0.0/edumfa/lib/smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/sqlutils.py` & `edumfa-2.0.0/edumfa/lib/sqlutils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/subscriptions.py` & `edumfa-2.0.0/edumfa/lib/subscriptions.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/task/base.py` & `edumfa-2.0.0/edumfa/lib/task/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/task/eventcounter.py` & `edumfa-2.0.0/edumfa/lib/task/eventcounter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/task/simplestats.py` & `edumfa-2.0.0/edumfa/lib/task/simplestats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/token.py` & `edumfa-2.0.0/edumfa/lib/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,16 +478,15 @@
             sortby = Token.serial
 
     if sortdir == "desc":
         sql_query = sql_query.order_by(sortby.desc())
     else:
         sql_query = sql_query.order_by(sortby.asc())
 
-    pagination = sql_query.paginate(page, per_page=psize,
-                                    error_out=False)
+    pagination = sql_query.paginate(page=page, per_page=psize, error_out=False)
     tokens = pagination.items
     prev = None
     if pagination.has_prev:
         prev = page-1
     next = None
     if pagination.has_next:
         next = page + 1
@@ -2074,15 +2073,15 @@
     r_chal, message, transaction_id, challenge_info = WebAuthnTokenClass.create_usernameless_challenge(options)
     message_list.append(message)
     if r_chal:
         challenge_info = challenge_info or {}
         challenge_info["transaction_id"] = transaction_id
         challenge_info["serial"] = ""
         challenge_info["type"] = ""
-        challenge_info["client_mode"] = False
+        challenge_info["client_mode"] = "webauthn"
         challenge_info["message"] = message
         reply_dict.update(challenge_info)
         reply_dict["multi_challenge"].append(challenge_info)
 
     if message_list:
         reply_dict["message"] = ", ".join(message_list)
         # The "messages" element is needed by some decorators
```

### Comparing `edumfa-1.5.1/edumfa/lib/tokenclass.py` & `edumfa-2.0.0/edumfa/lib/tokenclass.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokengroup.py` & `edumfa-2.0.0/edumfa/lib/tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/HMAC.py` & `edumfa-2.0.0/edumfa/lib/tokens/HMAC.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/applicationspecificpasswordtoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/applicationspecificpasswordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/certificatetoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/certificatetoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/daplugtoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/daplugtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/daypasswordtoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/daypasswordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/emailtoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/emailtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/foureyestoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/foureyestoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/hotptoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/hotptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/indexedsecrettoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/indexedsecrettoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/mOTP.py` & `edumfa-2.0.0/edumfa/lib/tokens/mOTP.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/motptoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/motptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/ocra.py` & `edumfa-2.0.0/edumfa/lib/tokens/ocra.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/ocratoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/ocratoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/papertoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/papertoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/passwordtoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/passwordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/pushtoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/pushtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/questionnairetoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/questionnairetoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/radiustoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/radiustoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/registrationtoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/registrationtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/remotetoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/remotetoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/smstoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/smstoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/spasstoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/spasstoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/sshkeytoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/sshkeytoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/tantoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/tantoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/tiqrtoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/tiqrtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/totptoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/totptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/u2f.py` & `edumfa-2.0.0/edumfa/lib/tokens/u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/u2ftoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/u2ftoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/vasco.py` & `edumfa-2.0.0/edumfa/lib/tokens/vasco.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/vascotoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/vascotoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/webauthn.py` & `edumfa-2.0.0/edumfa/lib/tokens/webauthn.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/webauthntoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/webauthntoken.py`

 * *Files 0% similar despite different names*

```diff
@@ -985,15 +985,15 @@
                 self.add_tokeninfo(WEBAUTHNINFO.ATTESTATION_SUBJECT,
                                    webauthn_credential.attestation_cert.subject.rfc4514_string())
                 self.add_tokeninfo(WEBAUTHNINFO.ATTESTATION_SERIAL,
                                    webauthn_credential.attestation_cert.serial_number)
 
                 cn = webauthn_credential.attestation_cert.subject.get_attributes_for_oid(x509.NameOID.COMMON_NAME)
                 automatic_description = cn[0].value if len(cn) else None
-
+            log.debug(f"Got client extensions from registration: {registration_client_extensions!s}")
             if registration_client_extensions:
                 try:
                     extensions = json.loads(webauthn_b64_decode(registration_client_extensions))
                     # Add info to token about whether a resident key/ discoverable credential was enrolled
                     resident_key = 'rk' in extensions and (extensions['rk'] or extensions['rk'] == 'true')
                     if resident_key:
                         self.add_tokeninfo(WEBAUTHNINFO.RESIDENT_KEY, "Yes")
```

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/yubicotoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/yubicotoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/tokens/yubikeytoken.py` & `edumfa-2.0.0/edumfa/lib/tokens/yubikeytoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/user.py` & `edumfa-2.0.0/edumfa/lib/user.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/usercache.py` & `edumfa-2.0.0/edumfa/lib/usercache.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/utils/__init__.py` & `edumfa-2.0.0/edumfa/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/utils/compare.py` & `edumfa-2.0.0/edumfa/lib/utils/compare.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/lib/utils/export.py` & `edumfa-2.0.0/edumfa/lib/utils/export.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/messages.pot` & `edumfa-2.0.0/edumfa/messages.pot`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/models.py` & `edumfa-2.0.0/edumfa/models.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/README.md` & `edumfa-2.0.0/edumfa/static/README.md`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/app.js` & `edumfa-2.0.0/edumfa/static/app.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/audit/controllers/auditControllers.js` & `edumfa-2.0.0/edumfa/static/components/audit/controllers/auditControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/audit/factories/audit.js` & `edumfa-2.0.0/edumfa/static/components/audit/factories/audit.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/audit/states/states.js` & `edumfa-2.0.0/edumfa/static/components/audit/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/audit/views/audit.html` & `edumfa-2.0.0/edumfa/static/components/audit/views/audit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/audit/views/audit.log.html` & `edumfa-2.0.0/edumfa/static/components/audit/views/audit.log.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/components/controllers/componentControllers.js` & `edumfa-2.0.0/edumfa/static/components/components/controllers/componentControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/components/factories/component.js` & `edumfa-2.0.0/edumfa/static/components/components/factories/component.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/components/states/states.js` & `edumfa-2.0.0/edumfa/static/components/components/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/components/views/component.clienttype.html` & `edumfa-2.0.0/edumfa/static/components/components/views/component.clienttype.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/components/views/component.html` & `edumfa-2.0.0/edumfa/static/components/components/views/component.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/configControllers.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/configControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/eduMfaServerController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/eduMfaServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/eventController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/eventController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/ldapMachineResolverController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/ldapMachineResolverController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/periodicTaskController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/periodicTaskController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/radiusServerController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/radiusServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/serviceidController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/serviceidController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/smsgatewayController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/smsgatewayController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/smtpServerController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/smtpServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/controllers/tokengroupController.js` & `edumfa-2.0.0/edumfa/static/components/config/controllers/tokengroupController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/factories/config.js` & `edumfa-2.0.0/edumfa/static/components/config/factories/config.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/states/states.js` & `edumfa-2.0.0/edumfa/static/components/config/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.caconnectors.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.caconnectors.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.caconnectors.local.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.caconnectors.local.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.caconnectors.microsoft.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.caconnectors.microsoft.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.edumfaserver.edit.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.edumfaserver.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.edumfaserver.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.edumfaserver.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.events.details.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.events.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.events.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.events.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.events.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.events.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.machineresolvers.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.machineresolvers.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.mresolvers.hosts.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.mresolvers.hosts.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.mresolvers.ldap.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.mresolvers.ldap.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.mresolvers.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.mresolvers.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.periodictasks.details.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.periodictasks.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.periodictasks.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.periodictasks.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.periodictasks.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.periodictasks.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.policies.details.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.policies.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.policies.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.policies.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.policies.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.policies.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.radius.edit.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.radius.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.radius.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.radius.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.realms.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.realms.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.realms.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.realms.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.http.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.http.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.ldap.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.ldap.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.passwd.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.passwd.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.scim.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.scim.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.resolvers.sql.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.resolvers.sql.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.serviceid.edit.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.serviceid.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.serviceid.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.serviceid.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.smsgateway.edit.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.smsgateway.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.smsgateway.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.smsgateway.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.smtp.edit.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.smtp.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.smtp.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.smtp.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.system.edit.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.system.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.system.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.system.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.daypassword.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.email.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.email.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.hotp.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.question.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.question.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.radius.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.radius.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.remote.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.remote.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.sms.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.sms.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.tiqr.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.tiqr.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.totp.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.u2f.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.u2f.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.webauthn.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.webauthn.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.yubico.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.yubico.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.token.yubikey.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.token.yubikey.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.tokengroup.edit.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.tokengroup.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.tokengroup.list.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.tokengroup.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/config.tokens.html` & `edumfa-2.0.0/edumfa/static/components/config/views/config.tokens.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/config/views/dialog.confirm_delete.html` & `edumfa-2.0.0/edumfa/static/components/config/views/dialog.confirm_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/dashboard/controllers/dashboardControllers.js` & `edumfa-2.0.0/edumfa/static/components/dashboard/controllers/dashboardControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/dashboard/states/states.js` & `edumfa-2.0.0/edumfa/static/components/dashboard/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/dashboard/views/dashboard.html` & `edumfa-2.0.0/edumfa/static/components/dashboard/views/dashboard.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.about.html` & `edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.about.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html` & `edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.lock.html` & `edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.lock.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.no.token.html` & `edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.no.token.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/dialogs/views/dialog.welcome.html` & `edumfa-2.0.0/edumfa/static/components/dialogs/views/dialog.welcome.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/directives/controllers/directives.js` & `edumfa-2.0.0/edumfa/static/components/directives/controllers/directives.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/directives/views/directive.assigntoken.html` & `edumfa-2.0.0/edumfa/static/components/directives/views/directive.assigntoken.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/directives/views/directive.assignuser.html` & `edumfa-2.0.0/edumfa/static/components/directives/views/directive.assignuser.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/directives/views/directive.attachmachine.html` & `edumfa-2.0.0/edumfa/static/components/directives/views/directive.attachmachine.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/directives/views/directive.attachtoken.html` & `edumfa-2.0.0/edumfa/static/components/directives/views/directive.attachtoken.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/directives/views/directive.policyconditions.html` & `edumfa-2.0.0/edumfa/static/components/directives/views/directive.policyconditions.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/directives/views/directive.tokendata.html` & `edumfa-2.0.0/edumfa/static/components/directives/views/directive.tokendata.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/filters/filters.js` & `edumfa-2.0.0/edumfa/static/components/filters/filters.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/login/controllers/loginControllers.js` & `edumfa-2.0.0/edumfa/static/components/login/controllers/loginControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/login/factories/auth.js` & `edumfa-2.0.0/edumfa/static/components/login/factories/auth.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/login/factories/u2f.js` & `edumfa-2.0.0/edumfa/static/components/login/factories/u2f.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/login/factories/webauthn.js` & `edumfa-2.0.0/edumfa/static/components/login/factories/webauthn.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/login/states/states.js` & `edumfa-2.0.0/edumfa/static/components/login/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/login/views/enter-response.html` & `edumfa-2.0.0/edumfa/static/components/login/views/enter-response.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/login/views/login.html` & `edumfa-2.0.0/edumfa/static/components/login/views/login.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/login/views/pinchange.html` & `edumfa-2.0.0/edumfa/static/components/login/views/pinchange.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/machine/controllers/machineController.js` & `edumfa-2.0.0/edumfa/static/components/machine/controllers/machineController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/machine/controllers/machineDetailsController.js` & `edumfa-2.0.0/edumfa/static/components/machine/controllers/machineDetailsController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/machine/factories/machine.js` & `edumfa-2.0.0/edumfa/static/components/machine/factories/machine.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/machine/states/states.js` & `edumfa-2.0.0/edumfa/static/components/machine/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/machine/views/machine.details.html` & `edumfa-2.0.0/edumfa/static/components/machine/views/machine.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/machine/views/machine.html` & `edumfa-2.0.0/edumfa/static/components/machine/views/machine.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/machine/views/machine.list.html` & `edumfa-2.0.0/edumfa/static/components/machine/views/machine.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/recovery/controllers/recoveryControllers.js` & `edumfa-2.0.0/edumfa/static/components/recovery/controllers/recoveryControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/recovery/factories/recoveryFactory.js` & `edumfa-2.0.0/edumfa/static/components/recovery/factories/recoveryFactory.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/recovery/states/states.js` & `edumfa-2.0.0/edumfa/static/components/recovery/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/recovery/views/recovery.html` & `edumfa-2.0.0/edumfa/static/components/recovery/views/recovery.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/recovery/views/recovery.reset.html` & `edumfa-2.0.0/edumfa/static/components/recovery/views/recovery.reset.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/register/controllers/registerControllers.js` & `edumfa-2.0.0/edumfa/static/components/register/controllers/registerControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/register/factories/registerFactory.js` & `edumfa-2.0.0/edumfa/static/components/register/factories/registerFactory.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/register/states/states.js` & `edumfa-2.0.0/edumfa/static/components/register/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/register/views/register.html` & `edumfa-2.0.0/edumfa/static/components/register/views/register.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/controllers/tokenApplicationsController.js` & `edumfa-2.0.0/edumfa/static/components/token/controllers/tokenApplicationsController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/controllers/tokenChallengesController.js` & `edumfa-2.0.0/edumfa/static/components/token/controllers/tokenChallengesController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/controllers/tokenControllers.js` & `edumfa-2.0.0/edumfa/static/components/token/controllers/tokenControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/controllers/tokenDetailController.js` & `edumfa-2.0.0/edumfa/static/components/token/controllers/tokenDetailController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/controllers/tokenGetSerialController.js` & `edumfa-2.0.0/edumfa/static/components/token/controllers/tokenGetSerialController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/controllers/tokenLostController.js` & `edumfa-2.0.0/edumfa/static/components/token/controllers/tokenLostController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/factories/token.js` & `edumfa-2.0.0/edumfa/static/components/token/factories/token.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/factories/validate.js` & `edumfa-2.0.0/edumfa/static/components/token/factories/validate.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/states/states.js` & `edumfa-2.0.0/edumfa/static/components/token/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/dialog.ask_token_delete.html` & `edumfa-2.0.0/edumfa/static/components/token/views/dialog.ask_token_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.applications.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.applications.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.applications.offline.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.applications.offline.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.applications.ssh.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.applications.ssh.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.assign.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.assign.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.challenges.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.challenges.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.details.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.4eyes.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.4eyes.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.applspec.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.applspec.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.certificate.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.certificate.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.daypassword.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.email.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.email.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.hotp.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.indexedsecret.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.indexedsecret.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.motp.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.motp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.push.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.push.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.question.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.question.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.radius.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.radius.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.remote.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.remote.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.sms.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.sms.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.sshkey.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.sshkey.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.totp.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.vasco.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.vasco.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.yubico.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.yubico.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enroll.yubikey.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enroll.yubikey.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.certificate.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.certificate.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.daypassword.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.hotp.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.motp.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.motp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.paper.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.paper.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.push.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.push.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.registration.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.registration.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.tan.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.tan.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.tiqr.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.tiqr.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.totp.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.u2f.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.u2f.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.enrolled.webauthn.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.enrolled.webauthn.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.getserial.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.getserial.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.import.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.import.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.list.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/token/views/token.lost.html` & `edumfa-2.0.0/edumfa/static/components/token/views/token.lost.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/translation/translations.js` & `edumfa-2.0.0/edumfa/static/components/translation/translations.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/controllers/userControllers.js` & `edumfa-2.0.0/edumfa/static/components/user/controllers/userControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/factories/user.js` & `edumfa-2.0.0/edumfa/static/components/user/factories/user.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/states/states.js` & `edumfa-2.0.0/edumfa/static/components/user/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/views/dialog.ask_user_delete.html` & `edumfa-2.0.0/edumfa/static/components/user/views/dialog.ask_user_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/views/user.add.dynamic.form.fields.html` & `edumfa-2.0.0/edumfa/static/components/user/views/user.add.dynamic.form.fields.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/views/user.add.html` & `edumfa-2.0.0/edumfa/static/components/user/views/user.add.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/views/user.details.html` & `edumfa-2.0.0/edumfa/static/components/user/views/user.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/views/user.html` & `edumfa-2.0.0/edumfa/static/components/user/views/user.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/views/user.list.html` & `edumfa-2.0.0/edumfa/static/components/user/views/user.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/components/user/views/user.password.html` & `edumfa-2.0.0/edumfa/static/components/user/views/user.password.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/css/angular-inform.css` & `edumfa-2.0.0/edumfa/static/contrib/css/angular-inform.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/css/angular-inform.css.map` & `edumfa-2.0.0/edumfa/static/contrib/css/angular-inform.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/css/bootstrap-theme.css` & `edumfa-2.0.0/edumfa/static/contrib/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/css/bootstrap-theme.css.map` & `edumfa-2.0.0/edumfa/static/contrib/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/css/bootstrap.css` & `edumfa-2.0.0/edumfa/static/contrib/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/css/bootstrap.css.map` & `edumfa-2.0.0/edumfa/static/contrib/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/css/hotkeys.css` & `edumfa-2.0.0/edumfa/static/contrib/css/hotkeys.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/css/isteven-multi-select.css` & `edumfa-2.0.0/edumfa/static/contrib/css/isteven-multi-select.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot` & `edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg` & `edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf` & `edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff` & `edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2` & `edumfa-2.0.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/angular-inform.js` & `edumfa-2.0.0/edumfa/static/contrib/js/angular-inform.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/angular-inform.js.map` & `edumfa-2.0.0/edumfa/static/contrib/js/angular-inform.js.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/angular.js` & `edumfa-2.0.0/edumfa/static/contrib/js/angular.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/bootstrap.js` & `edumfa-2.0.0/edumfa/static/contrib/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/hotkeys.js` & `edumfa-2.0.0/edumfa/static/contrib/js/hotkeys.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/jquery.js` & `edumfa-2.0.0/edumfa/static/contrib/js/jquery.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-gettext.js` & `edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-gettext.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-idle.js` & `edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-idle.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-sanitize.js` & `edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-sanitize.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-ui-router.js` & `edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map` & `edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js` & `edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/ngmodules/ng-file-upload.js` & `edumfa-2.0.0/edumfa/static/contrib/js/ngmodules/ng-file-upload.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/u2f-api.js` & `edumfa-2.0.0/edumfa/static/contrib/js/u2f-api.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/ui-bootstrap-tpls.js` & `edumfa-2.0.0/edumfa/static/contrib/js/ui-bootstrap-tpls.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js` & `edumfa-2.0.0/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/css/content.css` & `edumfa-2.0.0/edumfa/static/css/content.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/css/eduMFA-logo.png` & `edumfa-2.0.0/edumfa/static/css/eduMFA-logo.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/css/menu.css` & `edumfa-2.0.0/edumfa/static/css/menu.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/css/papertoken.css` & `edumfa-2.0.0/edumfa/static/css/papertoken.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/css/signin.css` & `edumfa-2.0.0/edumfa/static/css/signin.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/customize/README.rst` & `edumfa-2.0.0/edumfa/static/customize/README.rst`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/favicon.png` & `edumfa-2.0.0/edumfa/static/favicon.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png` & `edumfa-2.0.0/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/img/plugup.jpg` & `edumfa-2.0.0/edumfa/static/img/plugup.jpg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/img/solokeys.png` & `edumfa-2.0.0/edumfa/static/img/solokeys.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/img/u2fzero.png` & `edumfa-2.0.0/edumfa/static/img/u2fzero.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/package-lock.json` & `edumfa-2.0.0/edumfa/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/package.json` & `edumfa-2.0.0/edumfa/static/package.json`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/providers/errorMessageProvider.js` & `edumfa-2.0.0/edumfa/static/providers/errorMessageProvider.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/providers/versioningProvider.js` & `edumfa-2.0.0/edumfa/static/providers/versioningProvider.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/templates/cert_request_form.html` & `edumfa-2.0.0/edumfa/static/templates/cert_request_form.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/templates/documentation.rst` & `edumfa-2.0.0/edumfa/static/templates/documentation.rst`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/templates/footer.html` & `edumfa-2.0.0/edumfa/static/templates/footer.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/templates/header.html` & `edumfa-2.0.0/edumfa/static/templates/header.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/templates/index.html` & `edumfa-2.0.0/edumfa/static/templates/index.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/templates/menu.html` & `edumfa-2.0.0/edumfa/static/templates/menu.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/templates/token_enrolled.html` & `edumfa-2.0.0/edumfa/static/templates/token_enrolled.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/static/update_contrib.sh` & `edumfa-2.0.0/edumfa/static/update_contrib.sh`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/cs/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/cs/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/de/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/de/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/es/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/es/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/fr/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/fr/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/it/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/it/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/nl/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/nl/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/pl/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/pt_BR/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/ro/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/ro/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/ru/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/ru/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/si/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/si/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/si/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/si/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/tr/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/tr/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo` & `edumfa-2.0.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po` & `edumfa-2.0.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/webui/certificate.py` & `edumfa-2.0.0/edumfa/webui/certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa/webui/login.py` & `edumfa-2.0.0/edumfa/webui/login.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/edumfa.egg-info/PKG-INFO` & `edumfa-2.0.0/edumfa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edumfa
-Version: 1.5.1
+Version: 2.0.0
 Summary: eduMFA: identity, multifactor authentication (OTP), authorization, audit
 Home-page: https://www.edumfa.io
 Author: edumfa.io
 Author-email: edumfa@listserv.dfn.de
 License: AGPLv3
 Keywords: OTP,two factor authentication,management,security
 Classifier: Framework :: Flask
@@ -12,68 +12,69 @@
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: beautifulsoup4[lxml]>=4.3.2
+Requires-Dist: Flask-Babel>=4.0.0
+Requires-Dist: Flask-Migrate>=3.2.0
+Requires-Dist: Flask-SQLAlchemy>=3.0
+Requires-Dist: Flask-Versioned>=0.9.4
+Requires-Dist: Flask>=3.0
+Requires-Dist: PyJWT>=1.3.0
+Requires-Dist: PyMySQL>=0.6.6
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: SQLAlchemy>=1.4.0
+Requires-Dist: argon2_cffi>=20.1.0
+Requires-Dist: beautifulsoup4[lxml]>=4.12.3
 Requires-Dist: cbor2>=5.0.1
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: croniter>=0.3.8
-Requires-Dist: cryptography>=2.4.2
+Requires-Dist: cryptography>=42.0.5
 Requires-Dist: defusedxml>=0.4.1
-Requires-Dist: Flask<2.0,>=0.10.1
-Requires-Dist: Flask-Babel>=0.9
-Requires-Dist: Flask-Migrate<3.0,>=1.2.0
-Requires-Dist: Flask-Script>=2.0.5
-Requires-Dist: Flask-SQLAlchemy>=2.0
-Requires-Dist: Flask-Versioned>=0.9.4
 Requires-Dist: google-auth>=1.23.0
+Requires-Dist: grpcio>=1.62.1
 Requires-Dist: huey[redis]>=1.11.0
 Requires-Dist: importlib_metadata>=2.1.1
 Requires-Dist: ldap3>=2.6
+Requires-Dist: lxml>=5.0.0
 Requires-Dist: netaddr>=0.7.12
 Requires-Dist: passlib[bcrypt]>=1.7.0
-Requires-Dist: argon2_cffi>=20.1.0
+Requires-Dist: psycopg2-binary>=2.9.9
+Requires-Dist: pyOpenSSL>=24
 Requires-Dist: pydash>=4.7.4
-Requires-Dist: PyJWT>=1.3.0
-Requires-Dist: PyMySQL>=0.6.6
-Requires-Dist: pyOpenSSL>=17.5
 Requires-Dist: pyrad>=2.0
 Requires-Dist: python-dateutil>=2.7.3
 Requires-Dist: python-gnupg>=0.4.4
-Requires-Dist: PyYAML>=5.1
-Requires-Dist: requests>=2.7.0
+Requires-Dist: requests>=2.31.0
 Requires-Dist: segno>=1.5
 Requires-Dist: smpplib>=2.0
-Requires-Dist: SQLAlchemy<2.0,>=1.4.0
-Requires-Dist: MarkupSafe<2.1
+Requires-Dist: typing-extensions>=4.6.0
+Requires-Dist: urllib3>=2.2.1
 Provides-Extra: doc
 Requires-Dist: Pallets-Sphinx-Themes>=1.2.3; extra == "doc"
 Requires-Dist: Sphinx>=1.3.1; extra == "doc"
 Requires-Dist: sphinxcontrib-httpdomain>=1.3.0; extra == "doc"
 Requires-Dist: sphinxcontrib-plantuml>=0.18; extra == "doc"
 Requires-Dist: sphinxcontrib-spelling>=7.0.0; extra == "doc"
 Provides-Extra: test
 Requires-Dist: mock>=2.0.0; extra == "test"
 Requires-Dist: pytest>=3.6.0; extra == "test"
 Requires-Dist: pytest-cov>=2.5.1; extra == "test"
 Requires-Dist: responses>=0.9.0; extra == "test"
 Requires-Dist: testfixtures>=6.14.2; extra == "test"
-Provides-Extra: postgres
-Requires-Dist: psycopg2>=2.8.3; extra == "postgres"
 Provides-Extra: hsm
 Requires-Dist: PyKCS11>=1.5.10; extra == "hsm"
 Provides-Extra: kerberos
 Requires-Dist: gssapi>=1.7.0; extra == "kerberos"
 
 eduMFA
 ===========
```

### Comparing `edumfa-1.5.1/edumfa.egg-info/SOURCES.txt` & `edumfa-2.0.0/edumfa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 AUTHORS.md
 LICENSE
 MANIFEST.in
 README.rst
-edumfa-manage
 requirements.txt
 setup.py
 deploy/README.md
 deploy/docker-compose-example.yml
 deploy/docker-setup.sh
 deploy/edumfa_radius.pm
 deploy/logging.cfg
@@ -54,23 +53,25 @@
 deploy/ubuntu-server/edumfa-nginx.postrm
 deploy/ubuntu-server/rules
 deploy/ubuntu-server/source/format
 deploy/ubuntu-server/source/options
 deploy/ubuntu/source/format
 deploy/ubuntu/source/options
 deploy/uwsgi/apps-available/edumfa.xml
+doc/conf.py
 edumfa/__init__.py
 edumfa/app.py
 edumfa/babel.cfg
 edumfa/config.py
 edumfa/messages.pot
 edumfa/models.py
 edumfa.egg-info/PKG-INFO
 edumfa.egg-info/SOURCES.txt
 edumfa.egg-info/dependency_links.txt
+edumfa.egg-info/entry_points.txt
 edumfa.egg-info/not-zip-safe
 edumfa.egg-info/requires.txt
 edumfa.egg-info/top_level.txt
 edumfa/api/__init__.py
 edumfa/api/application.py
 edumfa/api/audit.py
 edumfa/api/auth.py
@@ -100,14 +101,32 @@
 edumfa/api/validate.py
 edumfa/api/lib/__init__.py
 edumfa/api/lib/decorators.py
 edumfa/api/lib/policyhelper.py
 edumfa/api/lib/postpolicy.py
 edumfa/api/lib/prepolicy.py
 edumfa/api/lib/utils.py
+edumfa/commands/__init__.py
+edumfa/commands/manage/__init__.py
+edumfa/commands/manage/admin.py
+edumfa/commands/manage/api.py
+edumfa/commands/manage/audit.py
+edumfa/commands/manage/authcache.py
+edumfa/commands/manage/backup.py
+edumfa/commands/manage/ca.py
+edumfa/commands/manage/config.py
+edumfa/commands/manage/core.py
+edumfa/commands/manage/event.py
+edumfa/commands/manage/helper.py
+edumfa/commands/manage/hsm.py
+edumfa/commands/manage/main.py
+edumfa/commands/manage/policy.py
+edumfa/commands/manage/realm.py
+edumfa/commands/manage/resolver.py
+edumfa/commands/manage/token.py
 edumfa/lib/__init__.py
 edumfa/lib/apps.py
 edumfa/lib/audit.py
 edumfa/lib/auth.py
 edumfa/lib/authcache.py
 edumfa/lib/caconnector.py
 edumfa/lib/challenge.py
@@ -733,14 +752,15 @@
 tests/testdata/audit.sqlite
 tests/testdata/dictionary
 tests/testdata/does_not_exist
 tests/testdata/emailtemplate.html
 tests/testdata/empty.oath
 tests/testdata/enckey
 tests/testdata/enckey.enc
+tests/testdata/event.conf
 tests/testdata/fancytoken.py
 tests/testdata/firebase-test.json
 tests/testdata/google-services.json
 tests/testdata/hosts
 tests/testdata/import.oath
 tests/testdata/import.oath.asc
 tests/testdata/jwt_sign.key
@@ -748,14 +768,15 @@
 tests/testdata/logging.yml
 tests/testdata/logging_broken.yaml
 tests/testdata/ocra.csv
 tests/testdata/passwd
 tests/testdata/passwd-duplicate-name
 tests/testdata/passwords
 tests/testdata/policy.cfg
+tests/testdata/policy.conf
 tests/testdata/policy_empty_file.cfg
 tests/testdata/private.pem
 tests/testdata/pskc-aes.xml
 tests/testdata/pskc-password.xml
 tests/testdata/public.pem
 tests/testdata/pw-2nd-resolver
 tests/testdata/test.sub
```

### Comparing `edumfa-1.5.1/migrations/alembic.ini` & `edumfa-2.0.0/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/env.py` & `edumfa-2.0.0/migrations/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         # In case of MySQL, add ``charset=utf8`` to the parameters (if no charset is set),
         # because this is what Flask-SQLAlchemy does
         if url.startswith("mysql"):
             parsed_url = make_url(url)
             parsed_url = parsed_url.update_query_dict({"charset": "utf8"})
             # We need to quote the password in case it contains special chars
             parsed_url = parsed_url.set(password=quote(parsed_url.password))
-            url = str(parsed_url)
+            url = parsed_url.render_as_string(hide_password=False)
     except Exception as exx:
         print(u"Attempted to set charset=utf8 on connection, but failed: {}".format(exx))
     # set_main_option() requires escaped "%" signs in the string
     config.set_main_option('sqlalchemy.url', url.replace('%', '%%'))
 
 
 set_database_url(config)
```

### Comparing `edumfa-1.5.1/migrations/versions/006d4747f858_.py` & `edumfa-2.0.0/migrations/versions/006d4747f858_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/00762b3f7a60_.py` & `edumfa-2.0.0/migrations/versions/00762b3f7a60_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/0c7123345224_.py` & `edumfa-2.0.0/migrations/versions/0c7123345224_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/0d011e94a8e8_.py` & `edumfa-2.0.0/migrations/versions/0d011e94a8e8_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/145ce80decd_.py` & `edumfa-2.0.0/migrations/versions/145ce80decd_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/14a1bcb10018_.py` & `edumfa-2.0.0/migrations/versions/14a1bcb10018_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/19f727d285e2_.py` & `edumfa-2.0.0/migrations/versions/19f727d285e2_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/1a0710df148b_.py` & `edumfa-2.0.0/migrations/versions/1a0710df148b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/1a69e5e5e2ac_.py` & `edumfa-2.0.0/migrations/versions/1a69e5e5e2ac_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/1edda52b619f_.py` & `edumfa-2.0.0/migrations/versions/1edda52b619f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/204d8d4f351e_.py` & `edumfa-2.0.0/migrations/versions/204d8d4f351e_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/205bda834127_.py` & `edumfa-2.0.0/migrations/versions/205bda834127_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/20969b4cbf06_.py` & `edumfa-2.0.0/migrations/versions/20969b4cbf06_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/2118e566df16_.py` & `edumfa-2.0.0/migrations/versions/2118e566df16_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/2181294eed0b_.py` & `edumfa-2.0.0/migrations/versions/2181294eed0b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/22558d9f3178_.py` & `edumfa-2.0.0/migrations/versions/22558d9f3178_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/239995464c48_.py` & `edumfa-2.0.0/migrations/versions/239995464c48_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/2551ee982544_.py` & `edumfa-2.0.0/migrations/versions/2551ee982544_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/2ac117d0a6f5_.py` & `edumfa-2.0.0/migrations/versions/2ac117d0a6f5_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/2c9430cfc66b_.py` & `edumfa-2.0.0/migrations/versions/2c9430cfc66b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/307a4fbe8a05_.py` & `edumfa-2.0.0/migrations/versions/307a4fbe8a05_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/3236a1abf1c6_.py` & `edumfa-2.0.0/migrations/versions/3236a1abf1c6_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/3429d523e51f_.py` & `edumfa-2.0.0/migrations/versions/3429d523e51f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/36428afb2457_.py` & `edumfa-2.0.0/migrations/versions/36428afb2457_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/37e6b49fc686_.py` & `edumfa-2.0.0/migrations/versions/37e6b49fc686_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/3ae3c668f444_.py` & `edumfa-2.0.0/migrations/versions/3ae3c668f444_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/3ba618f6b820_.py` & `edumfa-2.0.0/migrations/versions/3ba618f6b820_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/3c6e9dd7fbac_.py` & `edumfa-2.0.0/migrations/versions/3c6e9dd7fbac_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/3d7f8b29cbb1_.py` & `edumfa-2.0.0/migrations/versions/3d7f8b29cbb1_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/3f7e8583ea2_.py` & `edumfa-2.0.0/migrations/versions/3f7e8583ea2_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/4023571658f8_.py` & `edumfa-2.0.0/migrations/versions/4023571658f8_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/4238eac8ccab_.py` & `edumfa-2.0.0/migrations/versions/4238eac8ccab_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/449903fb6e35_.py` & `edumfa-2.0.0/migrations/versions/449903fb6e35_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/48ee74b8a7c8_.py` & `edumfa-2.0.0/migrations/versions/48ee74b8a7c8_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/49a04e560d96_.py` & `edumfa-2.0.0/migrations/versions/49a04e560d96_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/4a0aec37e7cf_.py` & `edumfa-2.0.0/migrations/versions/4a0aec37e7cf_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/4d9178fa8336_.py` & `edumfa-2.0.0/migrations/versions/4d9178fa8336_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/4f32a4e1bf33_.py` & `edumfa-2.0.0/migrations/versions/4f32a4e1bf33_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/50adc980d625_.py` & `edumfa-2.0.0/migrations/versions/50adc980d625_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/5402fd96fbca_.py` & `edumfa-2.0.0/migrations/versions/5402fd96fbca_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/58e4f7ebb705_.py` & `edumfa-2.0.0/migrations/versions/58e4f7ebb705_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/59ef3e03bc62_.py` & `edumfa-2.0.0/migrations/versions/59ef3e03bc62_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/5cb310101a1f_.py` & `edumfa-2.0.0/migrations/versions/5cb310101a1f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/631ec59e1ca6_.py` & `edumfa-2.0.0/migrations/versions/631ec59e1ca6_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/849170064430_.py` & `edumfa-2.0.0/migrations/versions/849170064430_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/86f40f535d7c_.py` & `edumfa-2.0.0/migrations/versions/86f40f535d7c_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/888b56ed5dcb_.py` & `edumfa-2.0.0/migrations/versions/888b56ed5dcb_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/89e57ed16379_.py` & `edumfa-2.0.0/migrations/versions/89e57ed16379_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/8d40dbcfda25_.py` & `edumfa-2.0.0/migrations/versions/8d40dbcfda25_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/9155f0d3d028_.py` & `edumfa-2.0.0/migrations/versions/9155f0d3d028_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/a28f2733897b_.py` & `edumfa-2.0.0/migrations/versions/a28f2733897b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/a63df077051a_.py` & `edumfa-2.0.0/migrations/versions/a63df077051a_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/a7e91b18a460_.py` & `edumfa-2.0.0/migrations/versions/a7e91b18a460_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/b9131d0686eb_.py` & `edumfa-2.0.0/migrations/versions/b9131d0686eb_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/cb6d7b7bae63_.py` & `edumfa-2.0.0/migrations/versions/cb6d7b7bae63_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/d2ae8e54b628_.py` & `edumfa-2.0.0/migrations/versions/d2ae8e54b628_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/d415d490eb05_.py` & `edumfa-2.0.0/migrations/versions/d415d490eb05_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/d6b40a745e5_.py` & `edumfa-2.0.0/migrations/versions/d6b40a745e5_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/d756b34061ff_.py` & `edumfa-2.0.0/migrations/versions/d756b34061ff_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/dceb6cd3c41e_.py` & `edumfa-2.0.0/migrations/versions/dceb6cd3c41e_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/e360c56bcf8c_.py` & `edumfa-2.0.0/migrations/versions/e360c56bcf8c_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/e5cbeb7c177_.py` & `edumfa-2.0.0/migrations/versions/e5cbeb7c177_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/ef29ba43e290_.py` & `edumfa-2.0.0/migrations/versions/ef29ba43e290_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/fa07bd604a75.py` & `edumfa-2.0.0/migrations/versions/fa07bd604a75.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/fabcf24d9304_.py` & `edumfa-2.0.0/migrations/versions/fabcf24d9304_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/migrations/versions/ff26585932ec_.py` & `edumfa-2.0.0/migrations/versions/ff26585932ec_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/setup.py` & `edumfa-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages, find_namespace_packages
 import os
 import stat
 import sys
 
-VERSION = "1.5.1"
+VERSION = "2.0.0"
 
 # Taken from kennethreitz/requests/setup.py
 package_directory = os.path.realpath(os.path.dirname(__file__))
 
 
 def get_file_contents(file_path):
     """Get the context of the file using full path name."""
@@ -20,50 +20,57 @@
         print("### could not open file {0!r}".format(file_path), file=sys.stderr)
     return content
 
 
 def get_file_list(file_path):
     full_path = os.path.join(package_directory, file_path)
     file_list = os.listdir(full_path)
+    # Filter out __pycache__
+    file_list = [x for x in file_list if "__pycache__" not in x]
     # now we need to add the path to the files
     return [file_path + f for f in file_list]
 
 
-install_requires = ["beautifulsoup4[lxml]>=4.3.2",
-                    "cbor2>=5.0.1",
-                    "configobj>=5.0.6",
-                    "croniter>=0.3.8",
-                    "cryptography>=2.4.2",
-                    "defusedxml>=0.4.1",
-                    "Flask>=0.10.1,<2.0",
-                    "Flask-Babel>=0.9",
-                    "Flask-Migrate>=1.2.0,<3.0",
-                    "Flask-Script>=2.0.5",
-                    "Flask-SQLAlchemy>=2.0",
-                    "Flask-Versioned>=0.9.4",
-                    "google-auth>=1.23.0",
-                    "huey[redis]>=1.11.0",
-                    "importlib_metadata>=2.1.1",
-                    "ldap3>=2.6",
-                    "netaddr>=0.7.12",
-                    "passlib[bcrypt]>=1.7.0",
-                    "argon2_cffi>=20.1.0",
-                    "pydash>=4.7.4",
-                    "PyJWT>=1.3.0",
-                    "PyMySQL>=0.6.6",
-                    "pyOpenSSL>=17.5",
-                    "pyrad>=2.0",
-                    "python-dateutil>=2.7.3",
-                    "python-gnupg>=0.4.4",
-                    "PyYAML>=5.1",
-                    "requests>=2.7.0",
-                    "segno>=1.5",
-                    "smpplib>=2.0",
-                    "SQLAlchemy>=1.4.0,<2.0",
-                    "MarkupSafe<2.1"]
+install_requires = [
+    "Flask-Babel>=4.0.0",
+    "Flask-Migrate>=3.2.0",
+    "Flask-SQLAlchemy>=3.0",
+    "Flask-Versioned>=0.9.4",
+    "Flask>=3.0",
+    "PyJWT>=1.3.0",
+    "PyMySQL>=0.6.6",
+    "PyYAML>=6.0.1",
+    "SQLAlchemy>=1.4.0",
+    "argon2_cffi>=20.1.0",
+    "beautifulsoup4[lxml]>=4.12.3",
+    "cbor2>=5.0.1",
+    "configobj>=5.0.6",
+    "croniter>=0.3.8",
+    "cryptography>=42.0.5",
+    "defusedxml>=0.4.1",
+    "google-auth>=1.23.0",
+    "grpcio>=1.62.1",
+    "huey[redis]>=1.11.0",
+    "importlib_metadata>=2.1.1",
+    "ldap3>=2.6",
+    "lxml>=5.0.0",
+    "netaddr>=0.7.12",
+    "passlib[bcrypt]>=1.7.0",
+    "psycopg2-binary>=2.9.9",
+    "pyOpenSSL>=24",
+    "pydash>=4.7.4",
+    "pyrad>=2.0",
+    "python-dateutil>=2.7.3",
+    "python-gnupg>=0.4.4",
+    "requests>=2.31.0",
+    "segno>=1.5",
+    "smpplib>=2.0",
+    "typing-extensions>=4.6.0",
+    "urllib3>=2.2.1",
+]
 
 
 def get_man_pages(dir):
     """
     Get man pages in a directory.
     :param dir:
     :return: list of file names
@@ -95,17 +102,26 @@
     version=VERSION,
     description='eduMFA: identity, multifactor authentication (OTP), authorization, audit',
     author='edumfa.io',
     license='AGPLv3',
     author_email='edumfa@listserv.dfn.de',
     url='https://www.edumfa.io',
     keywords='OTP, two factor authentication, management, security',
-    python_requires='>=3.6',
-    packages=find_packages(),
-    scripts=["edumfa-manage"] + get_scripts("tools"),
+    python_requires='>=3.8',
+    packages=find_namespace_packages(),
+    package_data={
+        'edumfa.translations': ["*", "**/*"],
+        'edumfa.static': ["*", "**/*"],
+    },
+    scripts=get_scripts("tools"),
+    entry_points={
+        'console_scripts': [
+            'edumfa-manage = edumfa.commands.manage.main:cli'
+        ]
+    },
     extras_require={
         'doc': [
             "Pallets-Sphinx-Themes>=1.2.3",
             "Sphinx>=1.3.1",
             "sphinxcontrib-httpdomain>=1.3.0",
             "sphinxcontrib-plantuml>=0.18",
             "sphinxcontrib-spelling>=7.0.0"
@@ -113,45 +129,37 @@
         'test': [
             "mock>=2.0.0",
             "pytest>=3.6.0",
             "pytest-cov>=2.5.1",
             "responses>=0.9.0",
             "testfixtures>=6.14.2"
         ],
-        'postgres': ['psycopg2>=2.8.3'],
         'hsm': ['PyKCS11>=1.5.10'],
         'kerberos': ['gssapi>=1.7.0']
     },
     install_requires=install_requires,
-    include_package_data=True,
-    data_files=[('etc/edumfa/',
-                 ['deploy/apache/edumfaapp.wsgi',
-                  'deploy/edumfa/dictionary']),
-                ('share/man/man1', get_man_pages("tools")),
-                ('lib/edumfa/migrations',
-                 ["migrations/alembic.ini",
-                  "migrations/env.py",
-                  "migrations/README",
-                  "migrations/script.py.mako"]),
-                ('lib/edumfa/migrations/versions',
-                 get_file_list("migrations/versions/")),
-                ('lib/edumfa/', ['requirements.txt'])
-                ],
-    classifiers=["Framework :: Flask",
-                 "License :: OSI Approved :: "
-                 "GNU Affero General Public License v3",
-                 "Programming Language :: Python",
-                 "Development Status :: 5 - Production/Stable",
-                 "Topic :: Internet",
-                 "Topic :: Security",
-                 "Topic :: System :: Systems Administration :: Authentication/Directory",
-                 'Programming Language :: Python',
-                 'Programming Language :: Python :: 3',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7',
-                 'Programming Language :: Python :: 3.8',
-                 'Programming Language :: Python :: 3.9',
-                 'Programming Language :: Python :: 3.10'
-                 ],
+    data_files=[
+        ('etc/edumfa/', ['deploy/apache/edumfaapp.wsgi', 'deploy/edumfa/dictionary']),
+        ('share/man/man1', get_man_pages("tools")),
+        ('lib/edumfa/migrations', ["migrations/alembic.ini", "migrations/env.py", "migrations/README", "migrations/script.py.mako"]),
+        ('lib/edumfa/migrations/versions', get_file_list("migrations/versions/")),
+        ('lib/edumfa/', ['requirements.txt'])
+    ],
+    classifiers=[
+        "Framework :: Flask",
+        "License :: OSI Approved :: GNU Affero General Public License v3",
+        "Programming Language :: Python",
+        "Development Status :: 5 - Production/Stable",
+        "Topic :: Internet",
+        "Topic :: Security",
+        "Topic :: System :: Systems Administration :: Authentication/Directory",
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12'
+    ],
     zip_safe=False,
     long_description=get_file_contents('README.rst')
 )
```

### Comparing `edumfa-1.5.1/tests/base.py` & `edumfa-2.0.0/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         cls.app_context.push()
         db.create_all()
         # save the current timestamp to the database to avoid hanging cached
         # data
         save_config_timestamp()
         db.session.commit()
         # Create an admin for tests.
-        create_db_admin(cls.app, cls.testadmin, cls.testadminmail, cls.testadminpw)
+        create_db_admin(cls.testadmin, cls.testadminmail, cls.testadminpw)
 
     def tearDown(self):
         # Commit all changes to the DB and close the session to avoid breaking
         # following tests due to unfinished transactions
         db.session.commit()
         db.session.close()
 
@@ -249,19 +249,22 @@
     def setUpClass(cls):
         """ override edumfa.config.config["testing"] with the inner config class """
         with mock.patch.dict("edumfa.config.config", {"testing": cls.Config}):
             MyTestCase.setUpClass()
 
 
 class MyApiTestCase(MyTestCase):
+
+    locale = "en"
+
     @classmethod
     def cls_auth(cls, app):
         with app.test_request_context('/auth', data={"username": cls.testadmin,
                                                      "password": cls.testadminpw},
-                                      method='POST'):
+                                      method='POST', headers={"Accept-Language": cls.locale}):
             res = app.full_dispatch_request()
             assert res.status_code == 200
             result = res.json.get("result")
             assert result.get("status")
             cls.at = result.get("value").get("token")
 
     @classmethod
```

### Comparing `edumfa-1.5.1/tests/ldap3mock.py` & `edumfa-2.0.0/tests/ldap3mock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/mscamock.py` & `edumfa-2.0.0/tests/mscamock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/pkcs11mock.py` & `edumfa-2.0.0/tests/pkcs11mock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/queuemock.py` & `edumfa-2.0.0/tests/queuemock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/radiusmock.py` & `edumfa-2.0.0/tests/radiusmock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/redismock.py` & `edumfa-2.0.0/tests/redismock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/smppmock.py` & `edumfa-2.0.0/tests/smppmock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/smtpmock.py` & `edumfa-2.0.0/tests/smtpmock.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import smtplib
 
-from inspect import formatargspec, getfullargspec as getargspec
+from inspect import getfullargspec as getargspec
 from collections.abc import Sequence, Sized
 
 from collections import namedtuple
 from functools import update_wrapper
 from smtplib import SMTPException
 
 
@@ -40,22 +40,26 @@
 
 def get_wrapped(func, wrapper_template, evaldict):
     # Preserve the argspec for the wrapped function so that testing
     # tools such as pytest can continue to use their fixture injection.
     args = getargspec(func)
     values = args.args[-len(args.defaults):] if args.defaults else None
 
-    signature = formatargspec(*args)
     is_bound_method = hasattr(func, '__self__')
     if is_bound_method:
         args.args = args.args[1:]     # Omit 'self'
-    callargs = formatargspec(*args, formatvalue=lambda v: '=' + v)
 
-    ctx = {'signature': signature, 'funcargs': callargs}
-    exec(wrapper_template % ctx, evaldict, evaldict)
+    s = args.args
+    if args.varargs:
+        s.append(f"*{args.varargs}")
+    if args.varkw:
+        s.append(f"**{args.varkw}")
+    ctx = {'signature': f'({",".join(s)})', 'funcargs': f'({",".join(s)})'}
+    exec (wrapper_template % ctx, evaldict, evaldict)
+
 
     wrapper = evaldict['wrapper']
 
     update_wrapper(wrapper, func)
     if is_bound_method:
         wrapper = wrapper.__get__(func.__self__, type(func.__self__))
     return wrapper
```

### Comparing `edumfa-1.5.1/tests/test_api_2stepinit.py` & `edumfa-2.0.0/tests/test_api_2stepinit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_applications.py` & `edumfa-2.0.0/tests/test_api_applications.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_audit.py` & `edumfa-2.0.0/tests/test_api_audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_auth.py` & `edumfa-2.0.0/tests/test_api_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
             result = res.json.get("result")
             self.assertTrue(result.get("status"), result)
             self.assertIn('token', result.get("value"), result)
             # role should be 'admin'
             self.assertEqual('admin', result['value']['role'], result)
 
         # add an admin with an '@' in the login name
-        create_db_admin(self.app, 'super@intern', password='testing')
+        create_db_admin('super@intern', password='testing')
         # as long as the part after the '@' does not resemble an existing realm,
         # this should work with 'spltAtSign' set to True
         with self.app.test_request_context('/auth',
                                            method='POST',
                                            data={"username": "super@intern",
                                                  "password": "testing"}):
             res = self.app.full_dispatch_request()
```

### Comparing `edumfa-1.5.1/tests/test_api_caconnector.py` & `edumfa-2.0.0/tests/test_api_caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_clienttype.py` & `edumfa-2.0.0/tests/test_api_clienttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_edumfaserver.py` & `edumfa-2.0.0/tests/test_api_edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_events.py` & `edumfa-2.0.0/tests/test_api_events.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_lib_policy.py` & `edumfa-2.0.0/tests/test_api_lib_policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_lib_utils.py` & `edumfa-2.0.0/tests/test_api_lib_utils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_machineresolver.py` & `edumfa-2.0.0/tests/test_api_machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_machines.py` & `edumfa-2.0.0/tests/test_api_machines.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_machines_serviceid.py` & `edumfa-2.0.0/tests/test_api_machines_serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_monitoring.py` & `edumfa-2.0.0/tests/test_api_monitoring.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_offline_no_token.py` & `edumfa-2.0.0/tests/test_api_offline_no_token.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_periodictask.py` & `edumfa-2.0.0/tests/test_api_periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_policy.py` & `edumfa-2.0.0/tests/test_api_policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_push_validate.py` & `edumfa-2.0.0/tests/test_api_push_validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_radiusserver.py` & `edumfa-2.0.0/tests/test_api_radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_register.py` & `edumfa-2.0.0/tests/test_api_register.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_roles.py` & `edumfa-2.0.0/tests/test_api_roles.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_serviceids.py` & `edumfa-2.0.0/tests/test_api_serviceids.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_smsgateway.py` & `edumfa-2.0.0/tests/test_api_smsgateway.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_smtpserver.py` & `edumfa-2.0.0/tests/test_api_smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_system.py` & `edumfa-2.0.0/tests/test_api_system.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_token.py` & `edumfa-2.0.0/tests/test_api_token.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_tokengroup.py` & `edumfa-2.0.0/tests/test_api_tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_ttype.py` & `edumfa-2.0.0/tests/test_api_ttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_u2f.py` & `edumfa-2.0.0/tests/test_api_u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_api_users.py` & `edumfa-2.0.0/tests/test_api_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
             # In self.at_user we store the user token
             wordy_auth_token = result.get("value").get("token")
             # check that this is a user
             role = result.get("value").get("role")
             self.assertTrue(role == "user", result)
 
         # Delete the users
-        with self.app.test_request_context('/user/{0!s}/{1!s}'.format(resolver, "wördy").encode('utf-8'),
+        with self.app.test_request_context('/user/{0!s}/{1!s}'.format(resolver, u"wördy"),
                                            method='DELETE',
                                            headers={'Authorization': self.at}):
             res = self.app.full_dispatch_request()
             self.assertTrue(res.status_code == 200, res)
             result = res.json.get("result")
             self.assertTrue(result.get("value"))
```

### Comparing `edumfa-1.5.1/tests/test_api_validate.py` & `edumfa-2.0.0/tests/test_api_validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_app.py` & `edumfa-2.0.0/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         self.logger.handlers = self.orig_handlers
         self.logger.level = self.level
 
     def test_01_create_default_app(self):
         # This will create the app with the 'development' configuration
         app = create_app()
         self.assertIsInstance(app, flask.app.Flask, app)
-        self.assertEqual(app.env, 'production', app)
         self.assertTrue(app.debug, app)
         self.assertFalse(app.testing, app)
         self.assertEqual(app.import_name, 'edumfa.app', app)
         self.assertEqual(app.name, 'edumfa.app', app)
         self.assertTrue(app.response_class == PiResponseClass, app)
         blueprints = ['validate_blueprint', 'token_blueprint', 'system_blueprint',
                       'resolver_blueprint', 'realm_blueprint', 'defaultrealm_blueprint',
```

### Comparing `edumfa-1.5.1/tests/test_db_model.py` & `edumfa-2.0.0/tests/test_db_model.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_applications.py` & `edumfa-2.0.0/tests/test_lib_applications.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_apps.py` & `edumfa-2.0.0/tests/test_lib_apps.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_audit.py` & `edumfa-2.0.0/tests/test_lib_audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_auth.py` & `edumfa-2.0.0/tests/test_lib_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 """
 This tests the files
   lib/auth.py and
 """
 
 from .base import MyTestCase
 from edumfa.lib.auth import (create_db_admin, verify_db_admin,
-                                  list_db_admin, delete_db_admin,
-                                  check_webui_user, db_admin_exist)
+                             delete_db_admin,
+                             check_webui_user, db_admin_exist)
 from edumfa.lib.user import User
 from flask import current_app
 
 
 class AuthTestCase(MyTestCase):
     """
     Test the Auth module
     """
 
     def test_01_db_admin(self):
-
-        create_db_admin(current_app, "mytestadmin", email="admin@localhost",
-                        password="PSTwort")
+        create_db_admin("mytestadmin", email="admin@localhost", password="PSTwort")
         r = verify_db_admin("mytestadmin", "PSTwort")
         self.assertTrue(r)
 
         self.assertTrue(db_admin_exist("mytestadmin"))
         self.assertFalse(db_admin_exist("noKnownUser"))
 
-        # This only prints to stdout!
-        list_db_admin()
-
         # Delete the admin
         delete_db_admin("mytestadmin")
 
     def test_02_users(self):
         r, role, detail = check_webui_user(User("cornelius"), "test")
         self.assertFalse(r)
         self.assertEqual(role, "user")
 
     def test_03_empty_passsword(self):
-        create_db_admin(current_app, "mytestadmin", email="admin@localhost",
-                        password="PSTwort")
+        create_db_admin("mytestadmin", email="admin@localhost", password="PSTwort")
         r = verify_db_admin("mytestadmin", None)
         self.assertFalse(r)
 
         # Delete the admin
-        delete_db_admin("mytestadmin")
+        delete_db_admin("mytestadmin")
```

### Comparing `edumfa-1.5.1/tests/test_lib_authcache.py` & `edumfa-2.0.0/tests/test_lib_authcache.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_caconnector.py` & `edumfa-2.0.0/tests/test_lib_caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_challenges.py` & `edumfa-2.0.0/tests/test_lib_challenges.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_clientapplication.py` & `edumfa-2.0.0/tests/test_lib_clientapplication.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_config.py` & `edumfa-2.0.0/tests/test_lib_config.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_counter.py` & `edumfa-2.0.0/tests/test_lib_counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_crypto.py` & `edumfa-2.0.0/tests/test_lib_crypto.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_edumfaserver.py` & `edumfa-2.0.0/tests/test_lib_edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_eventhandler_logging.py` & `edumfa-2.0.0/tests/test_lib_eventhandler_logging.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_eventhandler_usernotification.py` & `edumfa-2.0.0/tests/test_lib_eventhandler_usernotification.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_events.py` & `edumfa-2.0.0/tests/test_lib_events.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_framework.py` & `edumfa-2.0.0/tests/test_lib_framework.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_importotp.py` & `edumfa-2.0.0/tests/test_lib_importotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_lifecycle.py` & `edumfa-2.0.0/tests/test_lib_lifecycle.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_machine_resolver_ldap.py` & `edumfa-2.0.0/tests/test_lib_machine_resolver_ldap.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_machines.py` & `edumfa-2.0.0/tests/test_lib_machines.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_machinetokens.py` & `edumfa-2.0.0/tests/test_lib_machinetokens.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_monitoringstats.py` & `edumfa-2.0.0/tests/test_lib_monitoringstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_periodictask.py` & `edumfa-2.0.0/tests/test_lib_periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_policy.py` & `edumfa-2.0.0/tests/test_lib_policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_policydecorator.py` & `edumfa-2.0.0/tests/test_lib_policydecorator.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_pooling.py` & `edumfa-2.0.0/tests/test_lib_pooling.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         cls.app_context.push()
         db.create_all()
         # save the current timestamp to the database to avoid hanging cached
         # data
         save_config_timestamp()
         db.session.commit()
         # Create an admin for tests.
-        create_db_admin(cls.app, "testadmin", "admin@test.tld", "testpw")
+        create_db_admin("testadmin", "admin@test.tld", "testpw")
 
     def _create_engine(self):
         return create_engine('sqlite://')
 
     def test_01_registry(self):
         # test that we have one registry per app
         registry1 = get_registry()
```

### Comparing `edumfa-1.5.1/tests/test_lib_queue.py` & `edumfa-2.0.0/tests/test_lib_queue.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_radiusserver.py` & `edumfa-2.0.0/tests/test_lib_radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_realm.py` & `edumfa-2.0.0/tests/test_lib_realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_recovery.py` & `edumfa-2.0.0/tests/test_lib_recovery.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_resolver.py` & `edumfa-2.0.0/tests/test_lib_resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_serviceid.py` & `edumfa-2.0.0/tests/test_lib_serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_smsprovider.py` & `edumfa-2.0.0/tests/test_lib_smsprovider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_smtpserver.py` & `edumfa-2.0.0/tests/test_lib_smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_sqlutils.py` & `edumfa-2.0.0/tests/test_lib_sqlutils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_subscriptions.py` & `edumfa-2.0.0/tests/test_lib_subscriptions.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_task_eventcounter.py` & `edumfa-2.0.0/tests/test_lib_task_eventcounter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_task_simplestats.py` & `edumfa-2.0.0/tests/test_lib_task_simplestats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tasks.py` & `edumfa-2.0.0/tests/test_lib_tasks.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_token.py` & `edumfa-2.0.0/tests/test_lib_token.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokenclass.py` & `edumfa-2.0.0/tests/test_lib_tokenclass.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokengroup.py` & `edumfa-2.0.0/tests/test_lib_tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_certificate.py` & `edumfa-2.0.0/tests/test_lib_tokens_certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_daplug.py` & `edumfa-2.0.0/tests/test_lib_tokens_daplug.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_daypassword.py` & `edumfa-2.0.0/tests/test_lib_tokens_daypassword.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_email.py` & `edumfa-2.0.0/tests/test_lib_tokens_email.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_foureyes.py` & `edumfa-2.0.0/tests/test_lib_tokens_foureyes.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_hotp.py` & `edumfa-2.0.0/tests/test_lib_tokens_hotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_indexedsecret.py` & `edumfa-2.0.0/tests/test_lib_tokens_indexedsecret.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_motp.py` & `edumfa-2.0.0/tests/test_lib_tokens_motp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_paper.py` & `edumfa-2.0.0/tests/test_lib_tokens_paper.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_passwordtoken.py` & `edumfa-2.0.0/tests/test_lib_tokens_passwordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_push.py` & `edumfa-2.0.0/tests/test_lib_tokens_push.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_questionnaire.py` & `edumfa-2.0.0/tests/test_lib_tokens_questionnaire.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_radius.py` & `edumfa-2.0.0/tests/test_lib_tokens_radius.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_registration.py` & `edumfa-2.0.0/tests/test_lib_tokens_registration.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_remote.py` & `edumfa-2.0.0/tests/test_lib_tokens_remote.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_sms.py` & `edumfa-2.0.0/tests/test_lib_tokens_sms.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_spass.py` & `edumfa-2.0.0/tests/test_lib_tokens_spass.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_ssh.py` & `edumfa-2.0.0/tests/test_lib_tokens_ssh.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_tan.py` & `edumfa-2.0.0/tests/test_lib_tokens_tan.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_tiqr.py` & `edumfa-2.0.0/tests/test_lib_tokens_tiqr.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_totp.py` & `edumfa-2.0.0/tests/test_lib_tokens_totp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_u2f.py` & `edumfa-2.0.0/tests/test_lib_tokens_u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_vasco.py` & `edumfa-2.0.0/tests/test_lib_tokens_vasco.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_webauthn.py` & `edumfa-2.0.0/tests/test_lib_tokens_webauthn.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_yubico.py` & `edumfa-2.0.0/tests/test_lib_tokens_yubico.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_tokens_yubikey.py` & `edumfa-2.0.0/tests/test_lib_tokens_yubikey.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_user.py` & `edumfa-2.0.0/tests/test_lib_user.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_usercache.py` & `edumfa-2.0.0/tests/test_lib_usercache.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_utils.py` & `edumfa-2.0.0/tests/test_lib_utils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_lib_utils_compare.py` & `edumfa-2.0.0/tests/test_lib_utils_compare.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_mock_ldap3.py` & `edumfa-2.0.0/tests/test_mock_ldap3.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_resolver_realm.py` & `edumfa-2.0.0/tests/test_resolver_realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_ui_certificate.py` & `edumfa-2.0.0/tests/test_ui_certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/test_ui_login.py` & `edumfa-2.0.0/tests/test_ui_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 
 """
 This file tests the web UI Login
 
 implementation is contained webui/login.py
 """
+import flask_babel as babel
+
 from .base import MyTestCase, MyApiTestCase
 from edumfa.lib.policy import set_policy, SCOPE, ACTION, PolicyClass, delete_all_policies
 from edumfa.lib.utils import to_unicode
 import re
 from edumfa.app import create_app
 from edumfa.models import db, save_config_timestamp
 
@@ -127,15 +129,20 @@
                                            method='GET',
                                            headers={
                                                'Authorization': self.at,
                                                'Accept-Language': 'en'}):
             res = self.app.full_dispatch_request()
             self.assertEqual(res.json['result']['value']['totp'], 'TOTP: Time based One Time Passwords.')
 
-    def test_02_check_for_german_translation(self):
+
+class LanguageGermanTestCase(MyApiTestCase):
+
+    locale = "de"
+
+    def test_01_check_for_german_translation(self):
         with self.app.test_request_context('/auth/rights',
                                            method='GET',
                                            headers={
                                                'Authorization': self.at,
                                                'Accept-Language': 'de'}):
             res = self.app.full_dispatch_request()
             self.assertEqual(res.json['result']['value']['totp'], 'TOTP: Zeitbasiertes Einmalpasswort.')
```

### Comparing `edumfa-1.5.1/tests/testdata/FIDO-U2F-Security-Key-444x444.png` & `edumfa-2.0.0/tests/testdata/FIDO-U2F-Security-Key-444x444.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/attestation/yubico.pem` & `edumfa-2.0.0/tests/testdata/attestation/yubico.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/audit.sqlite` & `edumfa-2.0.0/tests/testdata/audit.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/ca/cacert.pem` & `edumfa-2.0.0/tests/testdata/ca/cacert.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/ca/cakey.pem` & `edumfa-2.0.0/tests/testdata/ca/cakey.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/ca/index.txt` & `edumfa-2.0.0/tests/testdata/ca/index.txt`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/ca/openssl.cnf` & `edumfa-2.0.0/tests/testdata/ca/openssl.cnf`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/dictionary` & `edumfa-2.0.0/tests/testdata/dictionary`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/firebase-test.json` & `edumfa-2.0.0/tests/testdata/firebase-test.json`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/google-services.json` & `edumfa-2.0.0/tests/testdata/google-services.json`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/gpg/pubring.gpg` & `edumfa-2.0.0/tests/testdata/gpg/pubring.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/gpg/random_seed` & `edumfa-2.0.0/tests/testdata/gpg/random_seed`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/gpg/secring.gpg` & `edumfa-2.0.0/tests/testdata/gpg/secring.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/gpg/trustdb.gpg` & `edumfa-2.0.0/tests/testdata/gpg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/import.oath.asc` & `edumfa-2.0.0/tests/testdata/import.oath.asc`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/jwt_sign.key` & `edumfa-2.0.0/tests/testdata/jwt_sign.key`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/logging.cfg` & `edumfa-2.0.0/tests/testdata/logging.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/logging.yml` & `edumfa-2.0.0/tests/testdata/logging.yml`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/msca-connector/ca.pem` & `edumfa-2.0.0/tests/testdata/msca-connector/ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/msca-connector/privacyidea-encrypted.key` & `edumfa-2.0.0/tests/testdata/msca-connector/privacyidea-encrypted.key`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/msca-connector/privacyidea.key` & `edumfa-2.0.0/tests/testdata/msca-connector/privacyidea.key`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/msca-connector/privacyidea.pem` & `edumfa-2.0.0/tests/testdata/msca-connector/privacyidea.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/passwd` & `edumfa-2.0.0/tests/testdata/passwd`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/passwords` & `edumfa-2.0.0/tests/testdata/passwords`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/private.pem` & `edumfa-2.0.0/tests/testdata/private.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/pskc-aes.xml` & `edumfa-2.0.0/tests/testdata/pskc-aes.xml`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/pskc-password.xml` & `edumfa-2.0.0/tests/testdata/pskc-password.xml`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/test.sub` & `edumfa-2.0.0/tests/testdata/test.sub`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/test2.sub` & `edumfa-2.0.0/tests/testdata/test2.sub`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/testuser-api.sqlite` & `edumfa-2.0.0/tests/testdata/testuser-api.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/testuser.sqlite` & `edumfa-2.0.0/tests/testdata/testuser.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/testusercache.sqlite` & `edumfa-2.0.0/tests/testdata/testusercache.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem` & `edumfa-2.0.0/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem` & `edumfa-2.0.0/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/yubico-oath-long.csv` & `edumfa-2.0.0/tests/testdata/yubico-oath-long.csv`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tests/testdata/yubico.csv` & `edumfa-2.0.0/tests/testdata/yubico.csv`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/creategoogleauthenticator-file` & `edumfa-2.0.0/tools/creategoogleauthenticator-file`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-authorizedkeys` & `edumfa-2.0.0/tools/edumfa-authorizedkeys`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-convert-base32.py` & `edumfa-2.0.0/tools/edumfa-convert-base32.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-convert-token` & `edumfa-2.0.0/tools/edumfa-convert-token`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-convert-token.1` & `edumfa-2.0.0/tools/edumfa-convert-token.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-convert-xml-to-csv` & `edumfa-2.0.0/tools/edumfa-convert-xml-to-csv`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-ad-users` & `edumfa-2.0.0/tools/edumfa-create-ad-users`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-ad-users.1` & `edumfa-2.0.0/tools/edumfa-create-ad-users.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-certificate` & `edumfa-2.0.0/tools/edumfa-create-certificate`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-certificate.1` & `edumfa-2.0.0/tools/edumfa-create-certificate.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-pwidresolver-user` & `edumfa-2.0.0/tools/edumfa-create-pwidresolver-user`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-pwidresolver-user.1` & `edumfa-2.0.0/tools/edumfa-create-pwidresolver-user.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-sqlidresolver-user` & `edumfa-2.0.0/tools/edumfa-create-sqlidresolver-user`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-sqlidresolver-user.1` & `edumfa-2.0.0/tools/edumfa-create-sqlidresolver-user.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-userdb` & `edumfa-2.0.0/tools/edumfa-create-userdb`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-create-userdb.1` & `edumfa-2.0.0/tools/edumfa-create-userdb.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-cron` & `edumfa-2.0.0/tools/edumfa-cron`

 * *Files 10% similar despite different names*

```diff
@@ -18,35 +18,41 @@
 # License along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 __doc__ = """
 This script is meant to be invoked periodically by the system cron daemon.
 It runs periodic tasks that are specified in the database.
 """
 __version__ = "0.1"
-
 import sys
 import warnings
 import json
 from datetime import datetime
 
 import dateutil
-from flask_script import Manager, Command
-
 from edumfa.app import create_app
 from edumfa.lib.config import get_edumfa_node
 from edumfa.lib.periodictask import (get_scheduled_periodic_tasks,
-                                          execute_task, get_periodic_tasks,
-                                          get_periodic_task_by_name,
-                                          set_periodic_task_last_run)
+                                     execute_task, get_periodic_tasks,
+                                     get_periodic_task_by_name,
+                                     set_periodic_task_last_run)
+import click
+from flask.cli import FlaskGroup
+from flask import current_app as app
+
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+
 
-warnings.simplefilter("ignore")
+def create_prod_app():
+    return create_app("production", silent=True, script=True)
 
-app = create_app(config_name='production', silent=True)
-manager = Manager(app)
 
+@click.group(cls=FlaskGroup, add_default_commands=False, create_app=create_prod_app, context_settings=CONTEXT_SETTINGS,
+             epilog='Check out our docs at https://edumfa.readthedocs.io/ for more details')
+def cli():
+    pass
 
 def print_stdout(*args, **kwargs):
     """
     Print to stdout, except if "cron mode" has been activated.
     """
     if not app.config.get("cron_mode", False):
         print(*args, **kwargs)
@@ -95,32 +101,33 @@
         print_stderr('This unsuccessful run is not recorded in the database.')
         if not ptask.get("retry_if_failed"):
             current_time = datetime.now(dateutil.tz.tzlocal())
             set_periodic_task_last_run(ptask["id"], node, current_time)
     return result
 
 
-@manager.option("-n", "--node",
-                help="Override the node name (read from eduMFA config by default)",
-                dest="node_string")
-@manager.option("-t", "--task",
-                help="Run the specified task",
-                required=True,
-                dest="task_name")
+
+@cli.command()
+@click.option("-n", "--node", "node_string",
+              help="Override the node name (read from eduMFA config by default)")
+@click.option("-t", "--task", "task_name",
+              help="Run the specified task",
+              required=True)
 def run_manually(node_string, task_name):
     """
     Manually run a periodic task.
     BEWARE: This does not check whether the task is active, or whether it should
     run on the given node at all.
     """
     node = get_node_name(node_string)
     ptask = get_periodic_task_by_name(task_name)
     run_task_on_node(ptask, node)
 
 
+@cli.command("list")
 def list_tasks():
     """
     Show a list of available tasks that could be run.
     """
     line_format = ('{active!s:7.7} {id:3} {name:16.16}\t{interval:16.16}\t{taskmodule:16}'
                    '\t{node_list:20}\t{options_json}')
     heading = line_format.format(
@@ -136,42 +143,36 @@
     print_stdout("=" * 120)
     for ptask in get_periodic_tasks():
         print_stdout(line_format.format(node_list=', '.join(ptask["nodes"]),
                                         options_json=json.dumps(ptask["options"]),
                                         **ptask))
 
 
-# add the list_tasks() function as flask command 'list'
-manager.add_command('list', Command(list_tasks))
-
-
-@manager.option("-d", "--dryrun",
-                action="store_true",
-                help="Do not run any tasks, only show what would be done")
-@manager.option("-n", "--node",
-                help="Override the node name (read from eduMFA config by default)",
-                dest="node_string")
-@manager.option("-c", "--cron",
-                dest="cron_mode",
-                action="store_true",
-                help="Run in 'cron mode', i.e. do not write to stdout, but write errors to stderr")
+@cli.command()
+@click.option("-d", "--dryrun",
+              is_flag=True,
+              help="Do not run any tasks, only show what would be done")
+@click.option("-n", "--node", "node_string",
+              help="Override the node name (read from eduMFA config by default)")
+@click.option("-c", "--cron",
+              is_flag=True,
+              help="Run in 'cron mode', i.e. do not write to stdout, but write errors to stderr")
 def run_scheduled(node_string=None, dryrun=False, cron_mode=False):
     """
     Execute all periodic tasks that are scheduled to run.
     """
     app.config['cron_mode'] = cron_mode
     node = get_node_name(node_string)
     current_time = datetime.now(dateutil.tz.tzlocal())
     scheduled_tasks = get_scheduled_periodic_tasks(node, current_time)
     if scheduled_tasks:
         print_stdout("The following tasks are scheduled to run on node {!s}:".format(node))
         print_stdout()
         for ptask in scheduled_tasks:
             print_stdout("  {name} ({interval!r}, {taskmodule})".format(**ptask))
-
         print_stdout()
         if not dryrun:
             results = []
             for ptask in scheduled_tasks:
                 result = run_task_on_node(ptask, node)
                 results.append(result)
             if all(results):
@@ -182,8 +183,8 @@
         else:
             print_stdout("Not running any tasks because --dryrun was passed.")
     else:
         print_stdout("There are no tasks scheduled on node {!s}.".format(node))
 
 
 if __name__ == '__main__':
-    manager.run()
+    cli()
```

### Comparing `edumfa-1.5.1/tools/edumfa-diag` & `edumfa-2.0.0/tools/edumfa-diag`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-expired-users` & `edumfa-2.0.0/tools/edumfa-expired-users`

 * *Files 17% similar despite different names*

```diff
@@ -71,39 +71,39 @@
 expect.
 """
 __version__ = "0.1"
 
 from edumfa.lib.user import get_user_list, User
 from edumfa.lib.token import get_tokens, remove_token, unassign_token
 from edumfa.app import create_app
-from flask_script import Manager
 import datetime
 import re
+import click
+from flask.cli import FlaskGroup
+from flask import current_app as app
 
-# If set to None, this condition does not match
-# Otherwise you may use a regular expression to match the serial numbers
-DELETE_SERIAL = None
-UNASSIGN_SERIAL = ".*"
-# You do not need to change this
-ATTRIBUTE_NAME = "accountExpires"
-
-#############################
-# Do not change this
-# one second contains 10^9 nano seconds. -> contains 10^7 100-nanoseconds
-MULTIPLYER = 10 ** 7
-MS_AD_START = datetime.datetime(1601, 1, 1)
-
-app = create_app(config_name='production', silent=True)
-manager = Manager(app)
-
-
-@manager.command
-def expire(realm=None, attribute_name=ATTRIBUTE_NAME,
-           delete_serial=DELETE_SERIAL, unassign_serial=UNASSIGN_SERIAL,
-           noaction=False):
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+
+
+def create_prod_app():
+    return create_app("production", silent=True, script=True)
+
+
+@click.group(cls=FlaskGroup, add_default_commands=False, create_app=create_prod_app, context_settings=CONTEXT_SETTINGS,
+             epilog='Check out our docs at https://edumfa.readthedocs.io/ for more details')
+def cli():
+    pass
+
+@cli.command()
+@click.option('--realm', help='The realm which should be checked')
+@click.option('--attribute_name', default='accountExpires', help='The attribute name that contains the expiration date')
+@click.option('--delete_serial', help='Regular expression to match the serial numbers of tokens to be deleted')
+@click.option('--unassign_serial', default='.*', help='Regular expression to match the serial numbers of tokens to be unassigned')
+@click.option('--noaction', is_flag=True, help='If set, the script will only show which accounts have expired, but do nothing')
+def expire(realm, attribute_name, delete_serial, unassign_serial, noaction):
     """
     This searches for expired Users in the specified realm.
     The attributeName should contain an integer like that in Microsoft(R)
     Active Directory. This is 100-nano-seconds steps since 1601/01/01.
 
     :param realm: The realm which should be checked
     :param attribute_name: The attribute name, that contains the expiration
@@ -115,15 +115,14 @@
     :return:
     """
     utc_now = datetime.datetime.utcnow()
     params = {"accountExpires": "1"}
     if realm:
         params["realm"] = realm
     users = get_user_list(params)
-
     for user in users:
         username = user.get("username")
         account_expires = user.get(attribute_name)
         if account_expires:
             if int(account_expires) == 0:
                 # 0 -> account never expires
                 print("%s does not expire." % username)
@@ -131,21 +130,19 @@
             td = datetime.timedelta(seconds=(int(account_expires) / MULTIPLYER))
             try:
                 exp_date = MS_AD_START + td
             except OverflowError:
                 # values like 9223372036854775807 do not expire
                 print("%s does not expire." % username)
                 continue
-
             print("= User %s has an expiration date." % username)
             print("== UTC now : %s" % utc_now)
             print("== expires : %s" % exp_date)
             if exp_date <= utc_now:
                 print("=== Account %s has expired." % username)
-
                 user = User(username, realm=realm)
                 tokens = get_tokens(user=user)
                 if not tokens:
                     print("=== The account has no tokens assigned.")
                 for token in tokens:
                     if unassign_serial:
                         m = re.search(unassign_serial, token.token.serial)
@@ -153,23 +150,20 @@
                             if noaction:
                                 print("=== I WOULD unassign token %s" %
                                       token.token.serial)
                             else:
                                 print("=== Unassigning token %s" %
                                       token.token.serial)
                                 unassign_token(token.token.serial)
-
                     if delete_serial:
                         m = re.search(delete_serial, token.token.serial)
                         if m:
                             if noaction:
                                 print("=== I WOULD delete token %s" %
                                       token.token.serial)
                             else:
                                 print("=== Deleting token %s" %
                                       token.token.serial)
                                 remove_token(token.token.serial)
 
-
 if __name__ == '__main__':
-    print()
-    manager.run()
+    cli()
```

### Comparing `edumfa-1.5.1/tools/edumfa-export-edumfa-counter.py` & `edumfa-2.0.0/tools/edumfa-export-edumfa-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-export-linotp-counter.py` & `edumfa-2.0.0/tools/edumfa-export-linotp-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-fetchssh` & `edumfa-2.0.0/tools/edumfa-fetchssh`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-fetchssh.1` & `edumfa-2.0.0/tools/edumfa-fetchssh.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-fix-access-rights` & `edumfa-2.0.0/tools/edumfa-fix-access-rights`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-fix-access-rights.1` & `edumfa-2.0.0/tools/edumfa-fix-access-rights.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-get-serial` & `edumfa-2.0.0/tools/edumfa-get-serial`

 * *Files 26% similar despite different names*

```diff
@@ -42,48 +42,59 @@
 
     edumfa-get-serial byotp --otp <otp> --type <type> --serial <serial>
         --unassigned --assigned --window <window>
 
 """
 __version__ = "0.1"
 
+import click
 from edumfa.lib.token import get_tokens, get_serial_by_otp
 from edumfa.app import create_app
-from flask_script import Manager
+from flask.cli import FlaskGroup
+from flask import current_app as app
 
-app = create_app(config_name='production', silent=True)
-manager = Manager(app)
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
+def create_prod_app():
+    return create_app("production", silent=True, script=True)
 
-@manager.command
-def byotp(otp=None, type=None, serial="", window=10, unassigned=False,
-          assigned=False):
+
+@click.group(cls=FlaskGroup, add_default_commands=False, create_app=create_prod_app, context_settings=CONTEXT_SETTINGS,
+             epilog='Check out our docs at https://edumfa.readthedocs.io/ for more details')
+def cli():
+    pass
+
+@cli.command()
+@click.option('--otp', help='The OTP value, which the token generates')
+@click.option('--type', help='The tokentype like hotp, totp, ...')
+@click.option('--serial', help='A part of the serial number')
+@click.option('--window', default=10, help='The OTP window for calculating OTP values')
+@click.option('--unassigned', is_flag=True, help='If set, searches only unassigned tokens')
+@click.option('--assigned', is_flag=True, help='If set, searches only assigned tokens')
+def byotp(otp, type, serial, window, unassigned, assigned):
     """
     This searches the list of the specified tokens for the given OTP value.
     :param otp: the OTP value, which the token generates
     :param type: The tokentype like hotp, totp, ...
     :param serial: A part of the serial number
     :param window: The OTP window for calculating OTP values. Default=10
     :param unassigned: If set, searches only unassigned tokens
     :param assigned: If set, searches only assigned tokens
     :return: The serial number of the token
     """
-    print()
     if not assigned and not unassigned:
         assigned = None
     count = get_tokens(tokentype=type, serial_wildcard="*{0!s}*".format(
             serial), assigned=assigned, count=True)
-    print("Searching in {0!s} tokens.".format(count))
-
+    click.echo("Searching in {0!s} tokens.".format(count))
     tokenobj_list = get_tokens(tokentype=type,
                                serial_wildcard="*{0!s}*".format(serial),
                                assigned=assigned)
     serial = get_serial_by_otp(tokenobj_list, otp=otp, window=window)
     if serial:
-        print("Found the token with serial {0!s}".format(serial))
+        click.echo("Found the token with serial {0!s}".format(serial))
     else:
-        print("No token found.")
-
+        click.echo("No token found.")
 
 if __name__ == '__main__':
-    print()
-    manager.run()
+    cli()
+
```

### Comparing `edumfa-1.5.1/tools/edumfa-get-unused-tokens` & `edumfa-2.0.0/tools/edumfa-get-unused-tokens`

 * *Files 20% similar despite different names*

```diff
@@ -47,89 +47,99 @@
 
 """
 __version__ = "0.1"
 
 from edumfa.lib.token import get_tokens, remove_token, enable_token
 from edumfa.lib.policy import ACTION
 from edumfa.app import create_app
-from flask_script import Manager
+import click
+from flask.cli import FlaskGroup
+from flask import current_app as app
 
-app = create_app(config_name='production', silent=True)
-manager = Manager(app)
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+
+
+def create_prod_app():
+    return create_app("production", silent=True, script=True)
+
+
+@click.group(cls=FlaskGroup, add_default_commands=False, create_app=create_prod_app, context_settings=CONTEXT_SETTINGS,
+             epilog='Check out our docs at https://edumfa.readthedocs.io/ for more details')
+def cli():
+    pass
 
 def _get_tokenlist(age):
     tlist = []
     tokenobj_list = get_tokens()
     for token_obj in tokenobj_list:
         if not token_obj.check_last_auth_newer(age):
             tlist.append(token_obj)
     return tlist
 
-
-@manager.option('age', help='Can be something like 10h, 7d, or 2y')
+@cli.command()
+@click.argument('age')
 def list(age):
     """
     finds all tokens, where the last_auth is too old.
     """
     # Oh bad performance, we have to look at *ALL* tokens!
     tlist = _get_tokenlist(age)
-    print("Token serial\tLast authentication")
-    print("="*42)
+    click.echo("Token serial\tLast authentication")
+    click.echo("="*42)
     for token_obj in tlist:
-        print("{0!s}\t{1!s}".format(token_obj.token.serial,
+        click.echo("{0!s}\t{1!s}".format(token_obj.token.serial,
                                     token_obj.get_tokeninfo(ACTION.LASTAUTH)))
 
-
-@manager.option('age', help='Can be something like 10h, 7d, or 2y')
-@manager.option('-d', '--description', help='The description that will be set.')
-@manager.option('-t', '--tokeninfo',
+@cli.command()
+@click.argument('age')
+@click.option('-d', '--description', help='The description that will be set.')
+@click.option('-t', '--tokeninfo',
                 help='The tokeninfo that will be set. It needs a key and a '
                      'value and should be specified like key=value.')
 def mark(age, description=None, tokeninfo=None):
     """
     Find unused tokens and mark them either by setting the description or by
     setting a tokeninfo.
 
     Tokeninfo parameter needs to be provided like key=value.
     """
     tlist = _get_tokenlist(age)
     for token_obj in tlist:
         if description:
-            print("Setting description for token {0!s}: {1!s}".format(
+            click.echo("Setting description for token {0!s}: {1!s}".format(
                 token_obj.token.serial, description))
             token_obj.set_description(description)
             token_obj.save()
         if tokeninfo:
             key, value = tokeninfo.split("=")
-            print("Setting tokeninfo for token {0!s}: {1!s}={2!s}".format(
+            click.echo("Setting tokeninfo for token {0!s}: {1!s}={2!s}".format(
                 token_obj.token.serial, key, value))
             token_obj.add_tokeninfo(key, value)
             token_obj.save()
 
-
-@manager.option('age', help='Can be something like 10h, 7d, or 2y')
+@cli.command()
+@click.argument('age')
 def delete(age):
     """
     Find unused tokens and delete them.
     """
     tlist = _get_tokenlist(age)
     for token_obj in tlist:
         serial = token_obj.token.serial
         remove_token(serial)
-        print("Token {0!s} deleted.".format(serial))
+        click.echo("Token {0!s} deleted.".format(serial))
 
-
-@manager.option('age', help='Can be something like 10h, 7d, or 2y')
+@cli.command()
+@click.argument('age')
 def disable(age):
     """
     Find unused tokens and delete them.
     """
     tlist = _get_tokenlist(age)
     for token_obj in tlist:
         serial = token_obj.token.serial
         enable_token(serial, enable=False)
-        print("Token {0!s} disabled.".format(serial))
-
+        click.echo("Token {0!s} disabled.".format(serial))
 
 if __name__ == '__main__':
-    manager.run()
+    cli()
```

### Comparing `edumfa-1.5.1/tools/edumfa-migrate-linotp.py` & `edumfa-2.0.0/tools/edumfa-migrate-linotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-pip-update` & `edumfa-2.0.0/tools/edumfa-pip-update`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-pip-update.1` & `edumfa-2.0.0/tools/edumfa-pip-update.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-queue-huey` & `edumfa-2.0.0/tools/edumfa-queue-huey`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-schema-upgrade` & `edumfa-2.0.0/tools/edumfa-schema-upgrade`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-standalone` & `edumfa-2.0.0/tools/edumfa-standalone`

 * *Files 7% similar despite different names*

```diff
@@ -49,19 +49,53 @@
 import subprocess
 from functools import wraps
 
 import sqlalchemy
 import sys
 import warnings
 
-from flask_script import Manager, Server
 from tempfile import NamedTemporaryFile
 
+from click import get_current_context
+
 from edumfa.app import create_app
 from edumfa.lib.security.default import DefaultSecurityModule
+import click
+from flask.cli import FlaskGroup, pass_script_info
+from flask import current_app
+
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+
+
+def create_prod_app(*args, **kwargs):
+    ctx = get_current_context(silent=True)
+    if ctx:
+        script_info = ctx.obj
+        instance = script_info.instance
+    elif kwargs.get("instance"):
+        # Production server, e.g., gunincorn 
+        # We don't have access to the current context, so must
+        # read kwargs instead.
+        instance = kwargs["instance"]
+    config_file = os.path.abspath(os.path.join(instance, 'edumfa.cfg'))
+    app = create_app("production", config_file=config_file, silent=True, script=True)
+    app.instance_directory = instance
+    return app
+
+
+@click.group(cls=FlaskGroup, add_default_commands=False, create_app=create_prod_app, context_settings=CONTEXT_SETTINGS,
+             epilog='Check out our docs at https://edumfa.readthedocs.io/ for more details')
+@click.option('-i', '--instance', 'instance', required=False,
+              default=os.path.expanduser('~/.edumfa'),
+              help='Location of the eduMFA instance (defaults to ~/.edumfa)')
+@pass_script_info
+def cli(script_info, instance):
+    script_info.instance = instance
+    pass
+
 
 warnings.simplefilter("ignore", category=sqlalchemy.exc.SAWarning)
 
 EDUMFA_CFG_TEMPLATE = """import os, logging
 
 INSTANCE_DIRECTORY = os.path.abspath(os.path.dirname(__file__))
 EDUMFA_ENCFILE = os.path.join(INSTANCE_DIRECTORY, 'encKey')
@@ -88,54 +122,30 @@
     :param edumfa_cfg: location of the eduMFA config file
     """
     environment = os.environ.copy()
     environment['EDUMFA_CONFIGFILE'] = edumfa_cfg
     subprocess.check_call(['edumfa-manage'] + commandline, env=environment)
 
 
-def _app_factory(instance):
-    """
-    Create a Flask app object with the given eduMFA standalone instance.
-    """
-    config_file = os.path.abspath(os.path.join(instance, 'edumfa.cfg'))
-    app = create_app(config_name='production', config_file=config_file, silent=True)
-    app.instance_directory = instance
-    return app
-
-
 def require_instance(f):
     """
     Decorator that marks commands that require an already set-up instance directory
     """
+
     @wraps(f)
     def deco(*args, **kwargs):
-        config_file = os.path.join(manager.app.instance_directory, 'edumfa.cfg')
+        config_file = os.path.join(current_app.instance_directory, 'edumfa.cfg')
         if not os.path.exists(config_file):
             raise RuntimeError("{!r} does not exist! Create a new instance using"
                                " ``edumfa-standalone create``.".format(config_file))
         return f(*args, **kwargs)
-    return deco
 
+    return deco
 
-class Configure(Server):
-    help = description = "Run a local webserver to configure eduMFA"
 
-    @require_instance
-    def __call__(self, *args, **kwargs):
-        Server.__call__(self, *args, **kwargs)
-
-    def run(self):
-        pass
-
-
-manager = Manager(_app_factory, with_default_commands=False, description=__doc__)
-manager.add_command("configure", Configure())
-manager.add_option('-i', '--instance', dest='instance', required=False,
-                   default=os.path.expanduser('~/.edumfa'),
-                   help='Location of the eduMFA instance (defaults to ~/.edumfa)')
 
 
 def read_credentials(fobj):
     """
     read username and password from a file. This could be sys.stdin.
 
     The first line specifies the username, the second line specifies the password.
@@ -194,20 +204,20 @@
     :return: boolean
     """
     return choice(question, {'y': True,
                              'n': False,
                              '': default})
 
 
-@manager.command
+@cli.command("create")
 def create():
     """ Create a new eduMFA instance """
-    instance_dir = os.path.abspath(manager.app.instance_directory)
-    if os.path.exists(manager.app.instance_directory):
-        print("Instance at {!s} exists already! Aborting.".format(manager.app.instance_directory))
+    instance_dir = os.path.abspath(current_app.instance_directory)
+    if os.path.exists(current_app.instance_directory):
+        print("Instance at {!s} exists already! Aborting.".format(current_app.instance_directory))
     else:
         try:
             os.makedirs(instance_dir)
 
             # create SECRET_KEY and EDUMFA_PEPPER
             secret_key = DefaultSecurityModule.random(24)
             edumfa_pepper = create_pepper()
@@ -246,30 +256,42 @@
                 })
                 if create_sql_resolver:
                     invoke_edumfa_config(['resolver', 'create_internal', 'defresolver'], edumfa_cfg)
                 else:
                     with NamedTemporaryFile(delete=False) as f:
                         f.write('{"fileName": "/etc/passwd"}')
                     invoke_edumfa_config(['resolver', 'create', 'defresolver', 'passwdresolver',
-                                      f.name], edumfa_cfg)
+                                          f.name], edumfa_cfg)
                     os.unlink(f.name)
                 invoke_edumfa_config(['realm', 'create', 'defrealm', 'defresolver'], edumfa_cfg)
 
             print()
             print('Configuration is complete. You can now configure eduMFA in '
                   'the web browser by running')
             print("  edumfa-standalone -i '{}' "
                   "configure".format(instance_dir))
         except Exception as e:
             print('Could not finish creation process! Removing instance.')
             shutil.rmtree(instance_dir)
             raise e
 
 
-@manager.option('-r', '--response', dest='show_response', action='store_true',
+@cli.command("configure")
+def configure():
+    """
+    Run a local webserver to configure eduMFA
+    """
+    # By default, it is prevented to run the Flask server using the CLI. We simply tell the Flask app that is not
+    # started by the CLI ;-)
+    os.environ.update({"FLASK_RUN_FROM_CLI": "false"})
+    current_app.run()
+
+
+@cli.command("check")
+@click.option('-r', '--response', 'show_response', is_flag=True,
                 help='Print the JSON response of eduMFA to standard output')
 @require_instance
 def check(show_response=False):
     """
     Check the given username and password against eduMFA.
     This command reads two lines from standard input: The first line is
     the username, the second line is the password (which consists of a
@@ -277,25 +299,25 @@
 
     This commands exits with return code 0 if the user could be authenticated
     successfully.
     """
     user, password = read_credentials(sys.stdin)
     exitcode = 255
     try:
-        with manager.app.test_request_context('/validate/check', method='POST',
+        with current_app.test_request_context('/validate/check', method='POST',
                                               data={'user': user, 'pass': password}):
-            response = manager.app.full_dispatch_request()
+            response = current_app.full_dispatch_request()
             data = json.loads(response.data)
             result = data['result']
             if result['value'] is True:
                 exitcode = 0
             else:
                 exitcode = 1
             if show_response:
                 print(response.data)
     except Exception as e:
         print(repr(e))
     sys.exit(exitcode)
 
 
 if __name__ == '__main__':
-    manager.run()
+    cli()
```

### Comparing `edumfa-1.5.1/tools/edumfa-sync-owncloud.py` & `edumfa-2.0.0/tools/edumfa-sync-owncloud.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-token-janitor` & `edumfa-2.0.0/tools/edumfa-token-janitor`

 * *Files 10% similar despite different names*

```diff
@@ -34,34 +34,30 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 from dateutil import parser
 from dateutil.tz import tzlocal, tzutc
-from flask_script.commands import InvalidCommand
 
 from edumfa.lib.policy import ACTION
 from edumfa.lib.utils import parse_legacy_time, to_unicode
 from edumfa.lib.importotp import export_pskc
 from edumfa.lib.token import (get_tokens, remove_token, enable_token,
-                                   unassign_token, import_token,
-                                   get_tokens_paginated_generator)
+                            unassign_token, import_token,
+                            get_tokens_paginated_generator)
 from edumfa.lib.user import User, split_user
 from edumfa.lib.realm import get_default_realm
 from edumfa.models import Token
 from edumfa.app import create_app
-from flask_script import Manager
 import re
 import sys
 from yaml import safe_dump as yaml_safe_dump
 from yaml import safe_load as yaml_safe_load
 
-
-
 __version__ = "0.1"
 
 ALLOWED_ACTIONS = ["disable", "delete", "unassign", "mark", "export", "listuser", "tokenrealms"]
 
 __doc__ = """
 This script can be used to clean up the token database.
 
@@ -113,23 +109,36 @@
    variable like this:
        export PYTHONIOENCODING=UTF-8
    Here is a good read about it:
    https://stackoverflow.com/questions/4545661/unicodedecodeerror-when-redirecting-to-file
 
 """.format("|".join(ALLOWED_ACTIONS))
 
-app = create_app(config_name='production', silent=True)
-manager = Manager(app)
+import click
+from flask.cli import FlaskGroup
+from flask import current_app as app
+
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+
+
+def create_prod_app():
+    return create_app("production", silent=True, script=True)
+
+
+@click.group(cls=FlaskGroup, add_default_commands=False, create_app=create_prod_app, context_settings=CONTEXT_SETTINGS,
+             epilog='Check out our docs at https://edumfa.readthedocs.io/ for more details')
+def cli():
+    pass
 
 
 def _try_convert_to_integer(given_value_string):
     try:
         return int(given_value_string)
     except ValueError:
-        raise InvalidCommand('Not an integer: {}'.format(given_value_string))
+        raise click.UsageError('Not an integer: {}'.format(given_value_string))
 
 
 def _compare_greater_than(_key, given_value_string):
     """
     :return: a function which returns True if its parameter (converted to an integer)
              is greater than *given_value_string* (converted to an integer).
     """
@@ -176,15 +185,15 @@
     try:
         parsed = parser.parse(given_value_string, dayfirst=False)
         if not parsed.tzinfo:
             # If not timezone is given we assume the timestamp is given in local time
             parsed = parsed.replace(tzinfo=tzlocal())
         return parsed
     except ValueError:
-        raise InvalidCommand('Not a valid datetime format: {}'.format(given_value_string))
+        raise click.UsageError('Not a valid datetime format: {}'.format(given_value_string))
 
 
 def _compare_after(key, given_value_string):
     """
     :return: a function which returns True if its parameter (converted to a datetime) occurs after
              *given_value_string* (converted to a datetime).
     """
@@ -356,35 +365,32 @@
 
     :param token_list:
     :param attributes: display additional user attributes
     :return:
     """
     tokens = []
     for token_obj in token_list:
-        token_data = ["{0!s}".format(token_obj.token.serial),
-                      "{0!s}".format(token_obj.token.tokentype)]
+        token_data = [f"{token_obj.token.serial!s}",
+                      f"{token_obj.token.tokentype!s}"]
         try:
             user = token_obj.user
             if user:
-                token_data.append("{0!s}".format(user.info.get("username", "")))
-                token_data.append("{0!s}".format(user.info.get("givenname", "")))
-                token_data.append("{0!s}".format(user.info.get("surname", "")))
-                token_data.append("{0!s}".format(user.uid))
-                token_data.append("{0!s}".format(user.resolver))
-                token_data.append("{0!s}".format(user.realm))
+                token_data.append(f"{user.info.get('username', '')!s}")
+                token_data.append(f"{user.info.get('givenname', '')!s}")
+                token_data.append(f"{user.info.get('surname', '')!s}")
+                token_data.append(f"{user.uid!s}")
+                token_data.append(f"{user.resolver!s}")
+                token_data.append(f"{user.realm!s}")
 
             if attributes:
                 for att in attributes.split(","):
-                    token_data.append("{0!s}".format(
-                        user.info.get(att, ""))
-                    )
+                    token_data.append(f"{user.info.get(att, '')!s}"
+                                      )
         except Exception:
-            sys.stderr.write("Failed to determine user for token {0!s}.\n".format(
-                token_obj.token.serial
-            ))
+            sys.stderr.write(f"Failed to determine user for token {token_obj.token.serial!s}.\n")
             token_data.append("**failed to resolve user**")
         tokens.append(token_data)
     return tokens
 
 
 def export_user_data(token_list, attributes=None):
     """
@@ -399,94 +405,85 @@
         try:
             user = token_obj.user
         except Exception:
             sys.stderr.write("Failed to determine user for token {0!s}.\n".format(
                 token_obj.token.serial
             ))
         if user:
-            uid = "'{0!s}','{1!s}','{2!s}','{3!s}','{4!s}','{5!s}'".format(
-                user.info.get("username", ""),
-                user.info.get("givenname", ""),
-                user.info.get("surname", ""),
-                user.uid,
-                user.resolver,
-                user.realm
-            )
+            uid = f"'{user.info.get('username', '')!s}','{user.info.get('givenname', '')!s}','{user.info.get('surname', '')!s}','{user.uid!s}','{user.resolver!s}','{user.realm!s}'"
             if attributes:
                 for att in attributes.split(","):
-                    uid += ",'{0!s}'".format(
-                        user.info.get(att, "")
-                    )
+                    uid += f",'{user.info.get(att, '')!s}'"
         else:
             uid = "N/A" + ", " * 5
 
         if uid in users.keys():
             users[uid].append(token_obj.token.serial)
         else:
             users[uid] = [token_obj.token.serial]
 
     return users
 
 
-@manager.option('--set-description', help='set a new description')
-@manager.option('--set-tokeninfo-key', help='set a new tokeninfo-key')
-@manager.option('--set-tokeninfo-value', help='set a new tokeninfo-value')
-@manager.option('--tokeninfo-value-before', metavar='DATETIME',
-                help='Interpret tokeninfo values as datetimes, match only if they occur before the given ISO 8601 datetime')
-@manager.option('--tokeninfo-value-after', metavar='DATETIME',
-                help='Interpret tokeninfo values as datetimes, match only if they occur after the given ISO 8601 datetime')
-@manager.option('--tokeninfo-value-greater-than', metavar='INTEGER',
-                help='Interpret tokeninfo values as integers and match only if they are '
-                     'greater than the given integer')
-@manager.option('--tokeninfo-value-less-than', metavar='INTEGER',
-                help='Interpret tokeninfo values as integers and match only if they are '
-                     'smaller than the given integer')
-@manager.option('--tokeninfo-value', metavar='REGEX|INTEGER', help='The tokeninfo value to match')
-@manager.option('--has-not-tokeninfo-key', help='filters for tokens that have not given the specified tokeninfo-key')
-@manager.option('--has-tokeninfo-key', help='filters for tokens that have given the specified tokeninfo-key.')
-@manager.option('--tokeninfo-key', help='The tokeninfo key to match. ')
-@manager.option('--tokenattribute-value-greater-than', metavar='INTEGER',
-                help="Match if the value of the token attribute is greater than the given value.")
-@manager.option('--tokenattribute-value-less-than', metavar='INTEGER',
-                help="Match if the value of the token attribute is less than the given value.")
-@manager.option('--tokenattribute-value', metavar='REGEX|INTEGER',
-                help='The value of the token attribute which should match.')
-@manager.option('--tokenattribute', help='Match for a certain token attribute from the database.')
-@manager.option('--tokentype', help='The tokentype to search.')
-@manager.option('--serial', help='A regular expression on the serial')
-@manager.option('--description', help='A regular expression on the description')
-@manager.option('--username', help='An exact username including the userrealm concatenated by "@". If no realm is given, '
+@cli.command()
+@click.option('--set-description', help='set a new description')
+@click.option('--set-tokeninfo-key', help='set a new tokeninfo-key')
+@click.option('--set-tokeninfo-value', help='set a new tokeninfo-value')
+@click.option('--tokeninfo-value-before', metavar='DATETIME',
+              help='Interpret tokeninfo values as datetimes, match only if they occur before the given ISO 8601 datetime')
+@click.option('--tokeninfo-value-after', metavar='DATETIME',
+              help='Interpret tokeninfo values as datetimes, match only if they occur after the given ISO 8601 datetime')
+@click.option('--tokeninfo-value-greater-than', metavar='INTEGER',
+              help='Interpret tokeninfo values as integers and match only if they are '
+                   'greater than the given integer')
+@click.option('--tokeninfo-value-less-than', metavar='INTEGER',
+              help='Interpret tokeninfo values as integers and match only if they are '
+                   'smaller than the given integer')
+@click.option('--tokeninfo-value', metavar='REGEX|INTEGER', help='The tokeninfo value to match')
+@click.option('--has-not-tokeninfo-key', help='filters for tokens that have not given the specified tokeninfo-key')
+@click.option('--has-tokeninfo-key', help='filters for tokens that have given the specified tokeninfo-key.')
+@click.option('--tokeninfo-key', help='The tokeninfo key to match. ')
+@click.option('--tokenattribute-value-greater-than', metavar='INTEGER',
+              help="Match if the value of the token attribute is greater than the given value.")
+@click.option('--tokenattribute-value-less-than', metavar='INTEGER',
+              help="Match if the value of the token attribute is less than the given value.")
+@click.option('--tokenattribute-value', metavar='REGEX|INTEGER',
+              help='The value of the token attribute which should match.')
+@click.option('--tokenattribute', help='Match for a certain token attribute from the database.')
+@click.option('--tokentype', help='The tokentype to search.')
+@click.option('--serial', help='A regular expression on the serial')
+@click.option('--description', help='A regular expression on the description')
+@click.option('--username', help='An exact username including the userrealm concatenated by "@". If no realm is given, '
                                    'the default realm will be used.')
-@manager.option('--attributes', help='Extends the "listuser" function to display additional user attributes')
-@manager.option('--tokenrealms', help='A comma separated list of realms, to which the tokens should be assigned.')
-@manager.option('--sum', help='In case of the action "listuser", this switch specifies if '
-                              'the output should only contain the number of tokens owned '
-                              'by the user.',
-                dest='sum_tokens', action='store_true')
-@manager.option('--action', help='Which action should be performed on the '
-                                 'found tokens. {0!s}. Exporting to PSKC only supports '
-                                 'HOTP, TOTP and PW tokens!'.format("|".join(ALLOWED_ACTIONS)))
-@manager.option('--csv', dest='csv', action='store_true',
-                help='In case of a simple find, the output is written as CSV instead of the '
-                     'formatted output.')
-@manager.option('--yaml', dest='yaml', action='store_true',
-                help='In case of a simple find, the output is written as YAML instead of the '
-                     'formatted output.')
-@manager.option('--last_auth', help='Can be something like 10h, 7d, or 2y')
-@manager.option('--assigned', help='True|False|None')
-@manager.option('--active', help='True|False|None')
-@manager.option('--orphaned',
-                help='Whether the token is an orphaned token. Set to 1')
-@manager.option('--b32', dest='b32', action='store_true',
-                help='In case of exporting found tokens to CSV the seed is written base32 encoded instead of hex.')
-@manager.option('--chunksize', default=None,
-                help='Read tokens from the database in smaller chunks to perform operations.')
-@manager.option('--limit', default=None,
-                help='If an action which writes changes to any token is given, then only apply these changes if ' 
-                     'less than or equal LIMIT tokens are affected.')
+@click.option('--attributes', help='Extends the "listuser" function to display additional user attributes')
+@click.option('--tokenrealms', help='A comma separated list of realms, to which the tokens should be assigned.')
+@click.option('--sum', 'sum_tokens', help='In case of the action "listuser", this switch specifies if '
+                                          'the output should only contain the number of tokens owned '
+                                          'by the user.', is_flag=True)
+@click.option('--action', help='Which action should be performed on the '
+                               'found tokens. {0!s}. Exporting to PSKC only supports '
+                               'HOTP, TOTP and PW tokens!'.format("|".join(ALLOWED_ACTIONS)))
+@click.option('--csv', is_flag=True,
+              help='In case of a simple find, the output is written as CSV instead of the '
+                   'formatted output.')
+@click.option('--yaml', is_flag=True,
+              help='In case of a simple find, the output is written as YAML instead of the '
+                   'formatted output.')
+@click.option('--last_auth', help='Can be something like 10h, 7d, or 2y')
+@click.option('--assigned', help='True|False|None')
+@click.option('--active', help='True|False|None')
+@click.option('--orphaned',
+              help='Whether the token is an orphaned token. Set to 1')
+@click.option('--b32', is_flag=True,
+              help='In case of exporting found tokens to CSV the seed is written base32 encoded instead of hex.')
+@click.option('--chunksize', default=None,
+              help='Read tokens from the database in smaller chunks to perform operations.')
+@click.option('--limit', default=None,
+              help='If an action which writes changes to any token is given, then only apply these changes if '
+                   'less than or equal LIMIT tokens are affected.')
 def find(last_auth, assigned, active, tokeninfo_key, tokeninfo_value,
          tokeninfo_value_greater_than, tokeninfo_value_less_than,
          tokeninfo_value_after, tokeninfo_value_before,
          orphaned, tokentype, serial, description, username, action, set_description,
          set_tokeninfo_key, set_tokeninfo_value, sum_tokens, tokenrealms, csv,
          chunksize, attributes, b32, has_not_tokeninfo_key, has_tokeninfo_key,
          tokenattribute, tokenattribute_value, tokenattribute_value_greater_than,
@@ -530,145 +527,135 @@
         sys.stderr.write("+ Reading tokens from database in chunks of {}...\n".format(chunksize))
     else:
         sys.stderr.write("+ Reading tokens from database...\n")
     for tlist in generator:
         sys.stderr.write("+ Tokens read. Starting action.\n")
         if not action:
             if not csv:
-                print("Token serial\tTokeninfo")
-                print("=" * 42)
+                click.echo("Token serial\tTokeninfo")
+                click.echo("=" * 42)
                 for token_obj in tlist:
-                    print("{0!s} ({1!s})\n\t\t{2!s}\n\t\t{3!s}".format(
-                        token_obj.token.serial,
-                        token_obj.token.tokentype,
-                        token_obj.token.description,
-                        token_obj.get_tokeninfo()))
+                    click.echo(
+                        f"{token_obj.token.serial!s} ({token_obj.token.tokentype!s})\n\t\t{token_obj.token.description!s}\n\t\t{token_obj.get_tokeninfo()!s}")
             else:
                 for token_obj in tlist:
-                    print("'{!s}','{!s}','{!s}','{!s}'".format(
-                        token_obj.token.serial,
-                        token_obj.token.tokentype,
-                        token_obj.token.description,
-                        token_obj.get_tokeninfo()
-                    ))
+                    click.echo(
+                        f"'{token_obj.token.serial!s}','{token_obj.token.tokentype!s}','{token_obj.token.description!s}','{token_obj.get_tokeninfo()!s}'")
 
         elif action == "listuser":
             if not sum_tokens:
                 tokens = export_token_data(tlist, attributes)
                 for token in tokens:
-                    print(",".join(["'{0!s}'".format(x) for x in token]))
+                    click.echo(",".join(["'{0!s}'".format(x) for x in token]))
             else:
                 users = export_user_data(tlist, attributes)
                 for user, tokens in users.items():
-                    print("{0!s},{1!s}".format(user, len(tokens)))
+                    click.echo(f"{user!s},{len(tokens)!s}")
 
         elif action == "export":
             if csv:
                 for tokenobj in tlist:
                     if tokenobj.type.lower() not in ["totp", "hotp"]:
                         continue
                     token_dict = tokenobj._to_dict(b32=b32)
-                    owner = "{!s}@{!s}".format(tokenobj.user.login, tokenobj.user.realm) if tokenobj.user else "n/a"
+                    owner = f"{tokenobj.user.login!s}@{tokenobj.user.realm!s}" if tokenobj.user else "n/a"
                     if type == "totp":
-                        print("{!s}, {!s}, {!s}, {!s}, {!s}, {!s}".format(owner, token_dict.get("serial"),
-                                                                          token_dict.get("otpkey"),
-                                                                          token_dict.get("type"),
-                                                                          token_dict.get("otplen"),
-                                                                          token_dict.get("timestep")))
+                        click.echo(
+                            f"{owner!s}, {token_dict.get('serial')!s}, {token_dict.get('otpkey')!s}, {token_dict.get('type')!s}, {token_dict.get('otplen')!s}, {token_dict.get('timestep')!s}")
                     else:
-                        print("{!s}, {!s}, {!s}, {!s}, {!s}".format(owner, token_dict.get("serial"),
-                                                                    token_dict.get("otpkey"),
-                                                                    token_dict.get("type"),
-                                                                    token_dict.get("otplen")))
+                        click.echo(
+                            f"{owner!s}, {token_dict.get('serial')!s}, {token_dict.get('otpkey')!s}, {token_dict.get('type')!s}, {token_dict.get('otplen')!s}")
             elif yaml:
                 token_list = []
                 for tokenobj in tlist:
                     try:
                         token_dict = tokenobj._to_dict(b32=b32)
-                        token_dict["owner"] = "{!s}@{!s}".format(tokenobj.user.login, tokenobj.user.realm) if tokenobj.user else "n/a"
+                        token_dict["owner"] = "{!s}@{!s}".format(tokenobj.user.login,
+                                                                 tokenobj.user.realm) if tokenobj.user else "n/a"
                         token_list.append(token_dict)
                     except Exception as e:
-                        sys.stderr.write("\nFailed to export token {0!s}.\n".format(token_dict.get("serial")))
+                        sys.stderr.write(f"\nFailed to export token {token_dict.get('serial')!s}.\n")
                 print(yaml_safe_dump(token_list))
             else:
                 key, token_num, soup = export_pskc(tlist)
                 sys.stderr.write("\n{0!s} tokens exported.\n".format(token_num))
                 sys.stderr.write("\nThis is the AES encryption key of the token seeds.\n"
                                  "You need this key to import the "
                                  "tokens again:\n\n\t{0!s}\n\n".format(key))
-                print("{0!s}".format(soup))
+                click.echo("{0!s}".format(soup))
         else:
             if limit is not None and int(limit) < len(tlist):
-                print("{0!s} tokens would be affected of given action \"{1!s}\", but limit was {2!s}. Aborting the action!".format(
-                    len(tlist), action, limit))
+                click.echo(
+                    f"{len(tlist)!s} tokens would be affected of given action \"{action!s}\", but limit was {limit!s}. Aborting the action!")
             else:
                 for token_obj in tlist:
                     try:
                         if action == "tokenrealms":
                             trealms = [r.strip() for r in tokenrealms.split(",") if r]
                             token_obj.set_realms(trealms)
-                            print("Setting realms of token {0!s} to {1!s}.".format(token_obj.token.serial, trealms))
+                            click.echo(f"Setting realms of token {token_obj.token.serial!s} to {trealms!s}.")
                         if action == "disable":
                             enable_token(serial=token_obj.token.serial, enable=False)
-                            print("Disabling token {0!s}".format(token_obj.token.serial))
+                            click.echo(f"Disabling token {token_obj.token.serial!s}")
                         elif action == "delete":
                             remove_token(serial=token_obj.token.serial)
-                            print("Deleting token {0!s}".format(token_obj.token.serial))
+                            click.echo(f"Deleting token {token_obj.token.serial!s}")
                         elif action == "unassign":
                             unassign_token(serial=token_obj.token.serial)
-                            print("Unassigning token {0!s}".format(token_obj.token.serial))
+                            click.echo(f"Unassigning token {token_obj.token.serial!s}")
                         elif action == "mark":
                             if set_description:
-                                print("Setting description for token {0!s}: {1!s}".format(
-                                    token_obj.token.serial, set_description))
+                                click.echo(
+                                    f"Setting description for token {token_obj.token.serial!s}: {set_description!s}")
                                 token_obj.set_description(set_description)
                                 token_obj.save()
                             if set_tokeninfo_value and set_tokeninfo_key:
-                                print("Setting tokeninfo for token {0!s}: {1!s}={2!s}".format(
-                                    token_obj.token.serial, set_tokeninfo_key, set_tokeninfo_value))
+                                click.echo(
+                                    f"Setting tokeninfo for token {token_obj.token.serial!s}: {set_tokeninfo_key!s}={set_tokeninfo_value!s}")
                                 token_obj.add_tokeninfo(set_tokeninfo_key, set_tokeninfo_value)
                                 token_obj.save()
                     except Exception as exx:
-                        print("Failed to process token {0}.".format(
-                            token_obj.token.serial))
-                        print("{0}".format(exx))
+                        click.echo(f"Failed to process token {token_obj.token.serial}.")
+                        click.echo("{0}".format(exx))
         del tlist
 
 
-@manager.option('--yaml', dest='yaml',
-                help='Specify the YAML file with the previously exported tokens.')
+@cli.command("updatetokens")
+@click.option('--yaml',
+              help='Specify the YAML file with the previously exported tokens.')
 def updatetokens(yaml):
     """
     This can update existing tokens in the eduMFA system. You can specify a yaml file with the tokendata.
     Can be used to reencrypt data, when changing the encryption key.
     """
     print("Loading YAML data. This may take a while.")
     token_list = yaml_safe_load(open(yaml, 'r').read())
     for tok in token_list:
-        del(tok["owner"])
+        del (tok["owner"])
         tok_objects = get_tokens(serial=tok.get("serial"))
         if len(tok_objects) == 0:
             sys.stderr.write("\nCan not find token {0!s}. Not updating.\n".format(tok.get("serial")))
         else:
             print("Updating token {0!s}.".format(tok.get("serial")))
             try:
                 tok_objects[0].update(tok)
             except Exception as e:
                 sys.stderr.write("\nFailed to update token {0!s}.".format(tok.get("serial")))
 
 
-@manager.option('--pskc', dest='pskc',
-                help='Import this PSKC file.')
-@manager.option('--preshared_key_hex', dest='preshared_key_hex',
-                help='The AES encryption key.')
-@manager.option('--validate_mac', dest='validate_mac', default='check_fail_hard',
-                help="How the file should be validated.\n"
-                     "'no_check' : Every token is parsed, ignoring HMAC\n"
-                     "'check_fail_soft' : Skip tokens with invalid HMAC\n"
-                     "'check_fail_hard' : Only import tokens if all HMAC are valid.")
+@cli.command("loadtokens")
+@click.option('--pskc',
+              help='Import this PSKC file.')
+@click.option('--preshared_key_hex',
+              help='The AES encryption key.')
+@click.option('--validate_mac', default='check_fail_hard',
+              help="How the file should be validated.\n"
+                   "'no_check' : Every token is parsed, ignoring HMAC\n"
+                   "'check_fail_soft' : Skip tokens with invalid HMAC\n"
+                   "'check_fail_hard' : Only import tokens if all HMAC are valid.")
 def loadtokens(pskc, preshared_key_hex, validate_mac):
     """
     Loads token data from a PSKC file.
     """
     from edumfa.lib.importotp import parsePSKCdata
 
     with open(pskc, 'r') as pskcfile:
@@ -694,8 +681,8 @@
         print("The following tokens were not read from the PSKC file"
               " because they could not be validated: {0!s}".format(not_parsed_tokens))
     print("Successfully imported {0!s} tokens.".format(success))
     print("Failed to import {0!s} tokens: {1!s}".format(failed, failed_tokens))
 
 
 if __name__ == '__main__':
-    manager.run()
+    cli()
```

### Comparing `edumfa-1.5.1/tools/edumfa-update-counter.py` & `edumfa-2.0.0/tools/edumfa-update-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-update-linotp-counter.py` & `edumfa-2.0.0/tools/edumfa-update-linotp-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-user-action` & `edumfa-2.0.0/tools/edumfa-user-action`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/edumfa-usercache-cleanup` & `edumfa-2.0.0/tools/edumfa-usercache-cleanup`

 * *Files 8% similar despite different names*

```diff
@@ -36,59 +36,66 @@
 
 __doc__ = """
 This script deletes expired entries from the user cache.
 """
 __version__ = "0.1"
 
 from edumfa.app import create_app
-from flask_script import Manager
+import click
+from edumfa.lib.usercache import create_filter, get_cache_time
+from edumfa.models import UserCache, db
+from edumfa.app import create_app
+from flask.cli import FlaskGroup
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+
 
-app = create_app(config_name='production', silent=True)
-manager = Manager(app)
+def create_prod_app():
+    return create_app("production", silent=True, script=True)
 
 
+@click.group(cls=FlaskGroup, add_default_commands=False, create_app=create_prod_app, context_settings=CONTEXT_SETTINGS,
+             epilog='Check out our docs at https://edumfa.readthedocs.io/ for more details')
+def cli():
+    pass
+
 def _get_expired_entries():
     """
     Returns a list of all cache entries that are considered expired.
     """
     filter_condition = create_filter(expired=True)
     return UserCache.query.filter(filter_condition).order_by(UserCache.timestamp.desc()).all()
 
-
-LIST_FORMAT = '{:<5} {:<10} {:<10} {:<30} {:<10}'
-
-
-@manager.command
-def delete(noaction=False):
+@cli.command()
+@click.option('--noaction', is_flag=True, help="List expired cache entries without deleting them.")
+def delete(noaction):
     """
     Delete all cache entries that are considered expired according to the
     UserCacheExpiration configuration setting.
     If the user cache is disabled, no entries are deleted.
     If '--noaction' is passed, expired cache entries are listed, but not
     actually deleted.
     """
     if not get_cache_time():
         print('User cache is disabled, not doing anything.')
     else:
         print('Expired entries:')
         entries = _get_expired_entries()
         if entries:
-            print(LIST_FORMAT.format('id', 'username', 'resolver', 'timestamp', 'user id'))
+            print('{:<5} {:<10} {:<10} {:<30} {:<10}'.format('id', 'username', 'resolver', 'timestamp', 'user id'))
         for entry in entries:
-            print(LIST_FORMAT.format(entry.id,
+            print('{:<5} {:<10} {:<10} {:<30} {:<10}'.format(entry.id,
                                      entry.username,
                                      entry.resolver,
                                      entry.timestamp.isoformat(),
                                      entry.user_id))
         print('{} entries'.format(len(entries)))
         if not noaction:
             for entry in entries:
                 print('Deleting entry with id={} ...'.format(entry.id))
                 entry.delete()
             print('Deleted {} expired entries.'.format(len(entries)))
             db.session.commit()
         else:
             print("'--noaction' was passed, not doing anything.")
 
-
 if __name__ == '__main__':
-    manager.run()
+    cli()
```

### Comparing `edumfa-1.5.1/tools/getgooglecodes` & `edumfa-2.0.0/tools/getgooglecodes`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/reset-edumfa` & `edumfa-2.0.0/tools/reset-edumfa`

 * *Files identical despite different names*

### Comparing `edumfa-1.5.1/tools/ssha.py` & `edumfa-2.0.0/tools/ssha.py`

 * *Files identical despite different names*


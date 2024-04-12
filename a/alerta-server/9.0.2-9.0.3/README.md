# Comparing `tmp/alerta-server-9.0.2.tar.gz` & `tmp/alerta-server-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alerta-server-9.0.2.tar", last modified: Tue Apr  9 09:50:11 2024, max compression
+gzip compressed data, was "alerta-server-9.0.3.tar", last modified: Fri Apr 12 08:45:58 2024, max compression
```

## Comparing `alerta-server-9.0.2.tar` & `alerta-server-9.0.3.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.876413 alerta-server-9.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 09:50:08.000000 alerta-server-9.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 09:50:08.000000 alerta-server-9.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 09:50:08.000000 alerta-server-9.0.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-09 09:50:11.876413 alerta-server-9.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-09 09:50:08.000000 alerta-server-9.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 09:50:08.000000 alerta-server-9.0.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/app.wsgi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/basic_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/database/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/database/backends/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71239 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/mongodb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/mongodb/queryparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/mongodb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.860413 alerta-server-9.0.2/alerta/database/backends/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70404 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/postgres/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/postgres/queryparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    17681 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/postgres/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.860413 alerta-server-9.0.2/alerta/management/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/management/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.860413 alerta-server-9.0.2/alerta/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.860413 alerta-server-9.0.2/alerta/models/alarms/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/alarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/alarms/alerta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/alarms/isa_18_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25626 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/blackout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/acked_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/blackout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/escalate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/forwarder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/reject.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/remote_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/sql/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/static/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/static/embed.js
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/templates/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/auth/saml2.html
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/templates/management/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/management/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/management/switchboard.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/templates/oembed/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/oembed/counts.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.868413 alerta-server-9.0.2/alerta/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7913 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/mailer.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/paging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.868413 alerta-server-9.0.2/alerta/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22749 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/blackouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/oembed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.872413 alerta-server-9.0.2/alerta/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/grafana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/graylog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/newrelic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/pagerduty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/pingdom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/riemann.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/serverdensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/stackdriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/telegram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.876413 alerta-server-9.0.2/alerta_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 09:50:11.880413 alerta-server-9.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-09 09:50:08.000000 alerta-server-9.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.876413 alerta-server-9.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.876413 alerta-server-9.0.2/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)    39105 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23677 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_authproxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    35064 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_blackouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_cors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17393 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_customers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (127)    17811 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    40388 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_isa_18_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    13243 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)   113133 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_queryparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_shelving.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    57492 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_zrouting.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 09:50:08.000000 alerta-server-9.0.2/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.529663 alerta-server-9.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 08:45:52.000000 alerta-server-9.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-12 08:45:52.000000 alerta-server-9.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-12 08:45:52.000000 alerta-server-9.0.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-12 08:45:58.529663 alerta-server-9.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-12 08:45:52.000000 alerta-server-9.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 08:45:52.000000 alerta-server-9.0.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.505663 alerta-server-9.0.3/alerta/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/app.wsgi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.509662 alerta-server-9.0.3/alerta/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/basic_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.509662 alerta-server-9.0.3/alerta/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.509662 alerta-server-9.0.3/alerta/database/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.509662 alerta-server-9.0.3/alerta/database/backends/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71239 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/mongodb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/mongodb/queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/mongodb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.513663 alerta-server-9.0.3/alerta/database/backends/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70404 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/postgres/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/postgres/queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17681 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/backends/postgres/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/database/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.513663 alerta-server-9.0.3/alerta/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/management/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.513663 alerta-server-9.0.3/alerta/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.513663 alerta-server-9.0.3/alerta/models/alarms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/alarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/alarms/alerta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/alarms/isa_18_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25626 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/blackout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.517663 alerta-server-9.0.3/alerta/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/acked_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/blackout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/escalate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/reject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/remote_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/plugins/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.517663 alerta-server-9.0.3/alerta/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/sql/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.517663 alerta-server-9.0.3/alerta/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/static/embed.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.517663 alerta-server-9.0.3/alerta/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.517663 alerta-server-9.0.3/alerta/templates/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/templates/auth/saml2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.517663 alerta-server-9.0.3/alerta/templates/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/templates/management/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/templates/management/switchboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.517663 alerta-server-9.0.3/alerta/templates/oembed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/templates/oembed/counts.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.521663 alerta-server-9.0.3/alerta/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7913 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/mailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/utils/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.521663 alerta-server-9.0.3/alerta/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22749 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/oembed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/views/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.525663 alerta-server-9.0.3/alerta/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/graylog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/newrelic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/pagerduty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/pingdom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/riemann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/serverdensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/stackdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-12 08:45:52.000000 alerta-server-9.0.3/alerta/webhooks/telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.529663 alerta-server-9.0.3/alerta_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-12 08:45:58.000000 alerta-server-9.0.3/alerta_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-12 08:45:58.000000 alerta-server-9.0.3/alerta_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:45:58.000000 alerta-server-9.0.3/alerta_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 08:45:58.000000 alerta-server-9.0.3/alerta_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:45:58.000000 alerta-server-9.0.3/alerta_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-12 08:45:58.000000 alerta-server-9.0.3/alerta_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 08:45:58.000000 alerta-server-9.0.3/alerta_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-12 08:45:58.529663 alerta-server-9.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-12 08:45:52.000000 alerta-server-9.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.529663 alerta-server-9.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:58.529663 alerta-server-9.0.3/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39105 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23677 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_authproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35064 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17393 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17811 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40388 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_isa_18_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13243 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113133 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_shelving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57492 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-12 08:45:52.000000 alerta-server-9.0.3/tests/test_zrouting.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 08:45:52.000000 alerta-server-9.0.3/wsgi.py
```

### Comparing `alerta-server-9.0.2/LICENSE` & `alerta-server-9.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/NOTICE` & `alerta-server-9.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/PKG-INFO` & `alerta-server-9.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerta-server
-Version: 9.0.2
+Version: 9.0.3
 Summary: Alerta server WSGI application
 Home-page: https://github.com/guardian/alerta
 Author: Nick Satterly
 Author-email: nfsatterly@gmail.com
 License: Apache License 2.0
 Keywords: alert monitoring system wsgi application api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alerta-server-9.0.2/README.md` & `alerta-server-9.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/app.py` & `alerta-server-9.0.3/alerta/app.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/__init__.py` & `alerta-server-9.0.3/alerta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/basic.py` & `alerta-server-9.0.3/alerta/auth/basic.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/basic_ldap.py` & `alerta-server-9.0.3/alerta/auth/basic_ldap.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/decorators.py` & `alerta-server-9.0.3/alerta/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/github.py` & `alerta-server-9.0.3/alerta/auth/github.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/hmac.py` & `alerta-server-9.0.3/alerta/auth/hmac.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/oidc.py` & `alerta-server-9.0.3/alerta/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/saml.py` & `alerta-server-9.0.3/alerta/auth/saml.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/userinfo.py` & `alerta-server-9.0.3/alerta/auth/userinfo.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/auth/utils.py` & `alerta-server-9.0.3/alerta/auth/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/commands.py` & `alerta-server-9.0.3/alerta/commands.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/database/backends/mongodb/base.py` & `alerta-server-9.0.3/alerta/database/backends/mongodb/base.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/database/backends/mongodb/queryparser.py` & `alerta-server-9.0.3/alerta/database/backends/mongodb/queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/database/backends/mongodb/utils.py` & `alerta-server-9.0.3/alerta/database/backends/mongodb/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/database/backends/postgres/base.py` & `alerta-server-9.0.3/alerta/database/backends/postgres/base.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/database/backends/postgres/queryparser.py` & `alerta-server-9.0.3/alerta/database/backends/postgres/queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/database/backends/postgres/utils.py` & `alerta-server-9.0.3/alerta/database/backends/postgres/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/database/base.py` & `alerta-server-9.0.3/alerta/database/base.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/exceptions.py` & `alerta-server-9.0.3/alerta/exceptions.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/management/views.py` & `alerta-server-9.0.3/alerta/management/views.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/alarms/__init__.py` & `alerta-server-9.0.3/alerta/models/alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/alarms/alerta.py` & `alerta-server-9.0.3/alerta/models/alarms/alerta.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/alarms/isa_18_2.py` & `alerta-server-9.0.3/alerta/models/alarms/isa_18_2.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/alert.py` & `alerta-server-9.0.3/alerta/models/alert.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/blackout.py` & `alerta-server-9.0.3/alerta/models/blackout.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/customer.py` & `alerta-server-9.0.3/alerta/models/customer.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/enums.py` & `alerta-server-9.0.3/alerta/models/enums.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/group.py` & `alerta-server-9.0.3/alerta/models/group.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/heartbeat.py` & `alerta-server-9.0.3/alerta/models/heartbeat.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/history.py` & `alerta-server-9.0.3/alerta/models/history.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/key.py` & `alerta-server-9.0.3/alerta/models/key.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/metrics.py` & `alerta-server-9.0.3/alerta/models/metrics.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/note.py` & `alerta-server-9.0.3/alerta/models/note.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/permission.py` & `alerta-server-9.0.3/alerta/models/permission.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/switch.py` & `alerta-server-9.0.3/alerta/models/switch.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/token.py` & `alerta-server-9.0.3/alerta/models/token.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/models/user.py` & `alerta-server-9.0.3/alerta/models/user.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/__init__.py` & `alerta-server-9.0.3/alerta/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/acked_by.py` & `alerta-server-9.0.3/alerta/plugins/acked_by.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/blackout.py` & `alerta-server-9.0.3/alerta/plugins/blackout.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/escalate.py` & `alerta-server-9.0.3/alerta/plugins/escalate.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/forwarder.py` & `alerta-server-9.0.3/alerta/plugins/forwarder.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/heartbeat.py` & `alerta-server-9.0.3/alerta/plugins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/reject.py` & `alerta-server-9.0.3/alerta/plugins/reject.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/remote_ip.py` & `alerta-server-9.0.3/alerta/plugins/remote_ip.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/plugins/timeout.py` & `alerta-server-9.0.3/alerta/plugins/timeout.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/settings.py` & `alerta-server-9.0.3/alerta/settings.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/sql/schema.sql` & `alerta-server-9.0.3/alerta/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/static/embed.js` & `alerta-server-9.0.3/alerta/static/embed.js`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/tasks.py` & `alerta-server-9.0.3/alerta/tasks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/templates/index.html` & `alerta-server-9.0.3/alerta/templates/index.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/templates/management/switchboard.html` & `alerta-server-9.0.3/alerta/templates/management/switchboard.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/templates/oembed/counts.html` & `alerta-server-9.0.3/alerta/templates/oembed/counts.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/api.py` & `alerta-server-9.0.3/alerta/utils/api.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/audit.py` & `alerta-server-9.0.3/alerta/utils/audit.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/client.py` & `alerta-server-9.0.3/alerta/utils/client.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/config.py` & `alerta-server-9.0.3/alerta/utils/config.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/format.py` & `alerta-server-9.0.3/alerta/utils/format.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/hooks.py` & `alerta-server-9.0.3/alerta/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/key.py` & `alerta-server-9.0.3/alerta/utils/key.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/logging.py` & `alerta-server-9.0.3/alerta/utils/logging.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/mailer.py` & `alerta-server-9.0.3/alerta/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/paging.py` & `alerta-server-9.0.3/alerta/utils/paging.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/plugin.py` & `alerta-server-9.0.3/alerta/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/response.py` & `alerta-server-9.0.3/alerta/utils/response.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/tracing.py` & `alerta-server-9.0.3/alerta/utils/tracing.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/utils/webhook.py` & `alerta-server-9.0.3/alerta/utils/webhook.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/__init__.py` & `alerta-server-9.0.3/alerta/views/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/alerts.py` & `alerta-server-9.0.3/alerta/views/alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/blackouts.py` & `alerta-server-9.0.3/alerta/views/blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/bulk.py` & `alerta-server-9.0.3/alerta/views/bulk.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/config.py` & `alerta-server-9.0.3/alerta/views/config.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/customers.py` & `alerta-server-9.0.3/alerta/views/customers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/groups.py` & `alerta-server-9.0.3/alerta/views/groups.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/heartbeats.py` & `alerta-server-9.0.3/alerta/views/heartbeats.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/keys.py` & `alerta-server-9.0.3/alerta/views/keys.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/oembed.py` & `alerta-server-9.0.3/alerta/views/oembed.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/permissions.py` & `alerta-server-9.0.3/alerta/views/permissions.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/views/users.py` & `alerta-server-9.0.3/alerta/views/users.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/__init__.py` & `alerta-server-9.0.3/alerta/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/cloudwatch.py` & `alerta-server-9.0.3/alerta/webhooks/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/custom.py` & `alerta-server-9.0.3/alerta/webhooks/custom.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/grafana.py` & `alerta-server-9.0.3/alerta/webhooks/grafana.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/graylog.py` & `alerta-server-9.0.3/alerta/webhooks/graylog.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/newrelic.py` & `alerta-server-9.0.3/alerta/webhooks/newrelic.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/pagerduty.py` & `alerta-server-9.0.3/alerta/webhooks/pagerduty.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/pingdom.py` & `alerta-server-9.0.3/alerta/webhooks/pingdom.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/prometheus.py` & `alerta-server-9.0.3/alerta/webhooks/prometheus.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/riemann.py` & `alerta-server-9.0.3/alerta/webhooks/riemann.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/serverdensity.py` & `alerta-server-9.0.3/alerta/webhooks/serverdensity.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/slack.py` & `alerta-server-9.0.3/alerta/webhooks/slack.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/stackdriver.py` & `alerta-server-9.0.3/alerta/webhooks/stackdriver.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta/webhooks/telegram.py` & `alerta-server-9.0.3/alerta/webhooks/telegram.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta_server.egg-info/PKG-INFO` & `alerta-server-9.0.3/alerta_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerta-server
-Version: 9.0.2
+Version: 9.0.3
 Summary: Alerta server WSGI application
 Home-page: https://github.com/guardian/alerta
 Author: Nick Satterly
 Author-email: nfsatterly@gmail.com
 License: Apache License 2.0
 Keywords: alert monitoring system wsgi application api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alerta-server-9.0.2/alerta_server.egg-info/SOURCES.txt` & `alerta-server-9.0.3/alerta_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/alerta_server.egg-info/entry_points.txt` & `alerta-server-9.0.3/alerta_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/setup.py` & `alerta-server-9.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/helpers/utils.py` & `alerta-server-9.0.3/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_actions.py` & `alerta-server-9.0.3/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_aggregations.py` & `alerta-server-9.0.3/tests/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_alerts.py` & `alerta-server-9.0.3/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_auth.py` & `alerta-server-9.0.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_authproxy.py` & `alerta-server-9.0.3/tests/test_authproxy.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_blackouts.py` & `alerta-server-9.0.3/tests/test_blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_builtins.py` & `alerta-server-9.0.3/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_commands.py` & `alerta-server-9.0.3/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_config.py` & `alerta-server-9.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_cors.py` & `alerta-server-9.0.3/tests/test_cors.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_customers.py` & `alerta-server-9.0.3/tests/test_customers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_forwarder.py` & `alerta-server-9.0.3/tests/test_forwarder.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_groups.py` & `alerta-server-9.0.3/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_heartbeats.py` & `alerta-server-9.0.3/tests/test_heartbeats.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_hooks.py` & `alerta-server-9.0.3/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_isa_18_2.py` & `alerta-server-9.0.3/tests/test_isa_18_2.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_logging.py` & `alerta-server-9.0.3/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_management.py` & `alerta-server-9.0.3/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_metrics.py` & `alerta-server-9.0.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_notes.py` & `alerta-server-9.0.3/tests/test_notes.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_plugins.py` & `alerta-server-9.0.3/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_providers.py` & `alerta-server-9.0.3/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_queryparser.py` & `alerta-server-9.0.3/tests/test_queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_response.py` & `alerta-server-9.0.3/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_scopes.py` & `alerta-server-9.0.3/tests/test_scopes.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_search.py` & `alerta-server-9.0.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_severity.py` & `alerta-server-9.0.3/tests/test_severity.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_shelving.py` & `alerta-server-9.0.3/tests/test_shelving.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_tags.py` & `alerta-server-9.0.3/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_users.py` & `alerta-server-9.0.3/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_webhooks.py` & `alerta-server-9.0.3/tests/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.2/tests/test_zrouting.py` & `alerta-server-9.0.3/tests/test_zrouting.py`

 * *Files identical despite different names*


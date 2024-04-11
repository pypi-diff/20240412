# Comparing `tmp/netdot-0.4.3rc1.tar.gz` & `tmp/netdot-0.4.4.tar.gz`

## Comparing `netdot-0.4.3rc1.tar` & `netdot-0.4.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/.groovylintrc.json
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/Jenkinsfile
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/Jenkinsfile.docs
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/README.md
--rw-r--r--   0        0        0   120008 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage-sources.zip
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/mkdocs.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/pytest.ini
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/.vscode/extensions.json
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/.vscode/launch.json
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/.vscode/settings.json
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot___init__.py.zip
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_actions.py.zip
--rw-r--r--   0        0        0     8369 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_client.py.zip
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_config.py.zip
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_csv_util.py.zip
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses___init__.py.zip
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_asset.py.zip
--rw-r--r--   0        0        0    19706 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_base.py.zip
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_bgp.py.zip
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_cables.py.zip
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_device.py.zip
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_dhcp.py.zip
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_dns.py.zip
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_entity.py.zip
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_fwtable.py.zip
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_interface.py.zip
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_ipblock.py.zip
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_misc.py.zip
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_physaddr.py.zip
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_products.py.zip
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_site.py.zip
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_users.py.zip
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_dataclasses_vlan.py.zip
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_exceptions.py.zip
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_gen_docs.py.zip
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_io.py.zip
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_mac_address.py.zip
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_parse.py.zip
--rw-r--r--   0        0        0    16218 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_repository.py.zip
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_trace.py.zip
--rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_unitofwork.py.zip
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_utils.py.zip
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_validate.py.zip
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/coverage/src_netdot_version.py.zip
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/README.md
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/api.md
--rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/changelog.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/dependencies.md
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/design.md
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/development.md
--rw-r--r--   0        0        0   516405 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/generated-api-docs.md
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/generated-env-var-docs.md
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/package-deployment.md
--rw-r--r--   0        0        0    25240 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/user-guide.md
--rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/assets/converted_netdot_schema.py
--rw-r--r--   0        0        0    43933 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/docs/assets/netdot_schema.sql
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/__init__.py
--rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/actions.py
--rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/client.py
--rw-r--r--   0        0        0     8279 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/config.py
--rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/csv_util.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/exceptions.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/gen_docs.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/io.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/mac_address.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/parse.py
--rw-r--r--   0        0        0    30831 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/repository.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/trace.py
--rw-r--r--   0        0        0    18562 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/unitofwork.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/utils.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/validate.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/version.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/__init__.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/asset.py
--rw-r--r--   0        0        0    40723 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/base.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/bgp.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/cables.py
--rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/device.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/dhcp.py
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/dns.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/entity.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/fwtable.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/interface.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/ipblock.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/misc.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/physaddr.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/products.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/site.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/users.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/src/netdot/dataclasses/vlan.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/conftest.py
--rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_NetdotAPIDataclass.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_client.py
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_csv_util.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_generated_docs.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_mac_address.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_netdotAction.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_parse_dto.py
--rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_repository.py
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_repository_CRUD.py
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_repository_DRY_RUN.py
--rw-r--r--   0        0        0    27831 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_repository_get_where.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_repository_indexes.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_site.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_trace.py
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_unitofwork.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/tests/test_utils.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/LICENSE
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/hatch.toml
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/pyproject.toml
--rw-r--r--   0        0        0   561830 2020-02-02 00:00:00.000000 netdot-0.4.3rc1/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 netdot-0.4.4/.groovylintrc.json
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 netdot-0.4.4/Jenkinsfile
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 netdot-0.4.4/Jenkinsfile.docs
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 netdot-0.4.4/README.md
+-rw-r--r--   0        0        0   120009 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage-sources.zip
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 netdot-0.4.4/mkdocs.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 netdot-0.4.4/pytest.ini
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 netdot-0.4.4/.vscode/extensions.json
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 netdot-0.4.4/.vscode/launch.json
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 netdot-0.4.4/.vscode/settings.json
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot___init__.py.zip
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_actions.py.zip
+-rw-r--r--   0        0        0     8369 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_client.py.zip
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_config.py.zip
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_csv_util.py.zip
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses___init__.py.zip
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_asset.py.zip
+-rw-r--r--   0        0        0    19706 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_base.py.zip
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_bgp.py.zip
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_cables.py.zip
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_device.py.zip
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_dhcp.py.zip
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_dns.py.zip
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_entity.py.zip
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_fwtable.py.zip
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_interface.py.zip
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_ipblock.py.zip
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_misc.py.zip
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_physaddr.py.zip
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_products.py.zip
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_site.py.zip
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_users.py.zip
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_dataclasses_vlan.py.zip
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_exceptions.py.zip
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_gen_docs.py.zip
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_io.py.zip
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_mac_address.py.zip
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_parse.py.zip
+-rw-r--r--   0        0        0    16218 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_repository.py.zip
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_trace.py.zip
+-rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_unitofwork.py.zip
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_utils.py.zip
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_validate.py.zip
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 netdot-0.4.4/coverage/src_netdot_version.py.zip
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/README.md
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/api.md
+-rw-r--r--   0        0        0    12764 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/changelog.md
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/dependencies.md
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/design.md
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/development.md
+-rw-r--r--   0        0        0   516405 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/generated-api-docs.md
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/generated-env-var-docs.md
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/package-deployment.md
+-rw-r--r--   0        0        0    25240 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/user-guide.md
+-rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/assets/converted_netdot_schema.py
+-rw-r--r--   0        0        0    43933 2020-02-02 00:00:00.000000 netdot-0.4.4/docs/assets/netdot_schema.sql
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/__init__.py
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/actions.py
+-rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/client.py
+-rw-r--r--   0        0        0     8279 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/config.py
+-rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/csv_util.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/exceptions.py
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/gen_docs.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/io.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/mac_address.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/parse.py
+-rw-r--r--   0        0        0    30831 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/repository.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/trace.py
+-rw-r--r--   0        0        0    18562 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/unitofwork.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/utils.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/validate.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/version.py
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/__init__.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/asset.py
+-rw-r--r--   0        0        0    40723 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/base.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/bgp.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/cables.py
+-rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/device.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/dhcp.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/dns.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/entity.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/fwtable.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/interface.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/ipblock.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/misc.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/physaddr.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/products.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/site.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/users.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 netdot-0.4.4/src/netdot/dataclasses/vlan.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_NetdotAPIDataclass.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_client.py
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_csv_util.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_generated_docs.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_mac_address.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_netdotAction.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_parse_dto.py
+-rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_repository.py
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_repository_CRUD.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_repository_DRY_RUN.py
+-rw-r--r--   0        0        0    27831 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_repository_get_where.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_repository_indexes.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_site.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_trace.py
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_unitofwork.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 netdot-0.4.4/tests/test_utils.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 netdot-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 netdot-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 netdot-0.4.4/hatch.toml
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 netdot-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0   561977 2020-02-02 00:00:00.000000 netdot-0.4.4/PKG-INFO
```

### Comparing `netdot-0.4.3rc1/coverage-sources.zip` & `netdot-0.4.4/coverage-sources.zip`

 * *Files 23% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,37 @@
-Zip file size: 120008 bytes, number of entries: 35
-?rwxrwxr-x  2.0 unx        0 bl defN 24-Feb-24 08:31 coverage/
-?rw-rw-r--  2.0 unx     3543 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_device.py.zip
-?rw-rw-r--  2.0 unx      890 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_physaddr.py.zip
-?rw-rw-r--  2.0 unx    16218 bl defN 24-Feb-24 08:31 coverage/src_netdot_repository.py.zip
-?rw-rw-r--  2.0 unx     1253 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_dhcp.py.zip
-?rw-rw-r--  2.0 unx     1485 bl defN 24-Feb-24 08:31 coverage/src_netdot_trace.py.zip
-?rw-rw-r--  2.0 unx     2090 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_ipblock.py.zip
-?rw-rw-r--  2.0 unx     1857 bl defN 24-Feb-24 08:31 coverage/src_netdot_mac_address.py.zip
-?rw-rw-r--  2.0 unx     1238 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_misc.py.zip
-?rw-rw-r--  2.0 unx     2710 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_dns.py.zip
-?rw-rw-r--  2.0 unx     1368 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_fwtable.py.zip
-?rw-rw-r--  2.0 unx     1016 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_entity.py.zip
-?rw-rw-r--  2.0 unx      966 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_bgp.py.zip
-?rw-rw-r--  2.0 unx     2517 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_interface.py.zip
-?rw-rw-r--  2.0 unx     1806 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_cables.py.zip
-?rw-rw-r--  2.0 unx     2036 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_users.py.zip
-?rw-rw-r--  2.0 unx      938 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_asset.py.zip
-?rw-rw-r--  2.0 unx     2586 bl defN 24-Feb-24 08:31 coverage/src_netdot_parse.py.zip
-?rw-rw-r--  2.0 unx      902 bl defN 24-Feb-24 08:31 coverage/src_netdot_validate.py.zip
-?rw-rw-r--  2.0 unx      293 bl defN 24-Feb-24 08:31 coverage/src_netdot_version.py.zip
-?rw-rw-r--  2.0 unx     3986 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses___init__.py.zip
-?rw-rw-r--  2.0 unx    19706 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_base.py.zip
-?rw-rw-r--  2.0 unx     9493 bl defN 24-Feb-24 08:31 coverage/src_netdot_unitofwork.py.zip
-?rw-rw-r--  2.0 unx      977 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_vlan.py.zip
-?rw-rw-r--  2.0 unx      874 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_products.py.zip
-?rw-rw-r--  2.0 unx     2872 bl defN 24-Feb-24 08:31 coverage/src_netdot_dataclasses_site.py.zip
-?rw-rw-r--  2.0 unx     3714 bl defN 24-Feb-24 08:31 coverage/src_netdot_csv_util.py.zip
-?rw-rw-r--  2.0 unx     8369 bl defN 24-Feb-24 08:31 coverage/src_netdot_client.py.zip
-?rw-rw-r--  2.0 unx     1189 bl defN 24-Feb-24 08:31 coverage/src_netdot_exceptions.py.zip
-?rw-rw-r--  2.0 unx     3241 bl defN 24-Feb-24 08:31 coverage/src_netdot_gen_docs.py.zip
-?rw-rw-r--  2.0 unx      458 bl defN 24-Feb-24 08:31 coverage/src_netdot_io.py.zip
-?rw-rw-r--  2.0 unx     2975 bl defN 24-Feb-24 08:31 coverage/src_netdot___init__.py.zip
-?rw-rw-r--  2.0 unx     2116 bl defN 24-Feb-24 08:31 coverage/src_netdot_utils.py.zip
-?rw-rw-r--  2.0 unx     5006 bl defN 24-Feb-24 08:31 coverage/src_netdot_config.py.zip
-?rw-rw-r--  2.0 unx     3922 bl defN 24-Feb-24 08:31 coverage/src_netdot_actions.py.zip
-35 files, 114610 bytes uncompressed, 114046 bytes compressed:  0.5%
+Zip file size: 120009 bytes, number of entries: 35
+?rwxrwxr-x  2.0 unx        0 bl defN 24-Apr-11 14:46 coverage/
+?rw-rw-r--  2.0 unx     3543 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_device.py.zip
+?rw-rw-r--  2.0 unx     1253 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_dhcp.py.zip
+?rw-rw-r--  2.0 unx     2710 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_dns.py.zip
+?rw-rw-r--  2.0 unx     1016 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_entity.py.zip
+?rw-rw-r--  2.0 unx      890 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_physaddr.py.zip
+?rw-rw-r--  2.0 unx      874 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_products.py.zip
+?rw-rw-r--  2.0 unx     2036 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_users.py.zip
+?rw-rw-r--  2.0 unx      977 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_vlan.py.zip
+?rw-rw-r--  2.0 unx     2872 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_site.py.zip
+?rw-rw-r--  2.0 unx     2090 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_ipblock.py.zip
+?rw-rw-r--  2.0 unx     1238 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_misc.py.zip
+?rw-rw-r--  2.0 unx     1368 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_fwtable.py.zip
+?rw-rw-r--  2.0 unx     2517 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_interface.py.zip
+?rw-rw-r--  2.0 unx      966 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_bgp.py.zip
+?rw-rw-r--  2.0 unx     1806 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_cables.py.zip
+?rw-rw-r--  2.0 unx      938 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_asset.py.zip
+?rw-rw-r--  2.0 unx     3714 bl defN 24-Apr-11 15:56 coverage/src_netdot_csv_util.py.zip
+?rw-rw-r--  2.0 unx     1189 bl defN 24-Apr-11 15:56 coverage/src_netdot_exceptions.py.zip
+?rw-rw-r--  2.0 unx     3241 bl defN 24-Apr-11 15:56 coverage/src_netdot_gen_docs.py.zip
+?rw-rw-r--  2.0 unx      458 bl defN 24-Apr-11 15:56 coverage/src_netdot_io.py.zip
+?rw-rw-r--  2.0 unx     8369 bl defN 24-Apr-11 15:56 coverage/src_netdot_client.py.zip
+?rw-rw-r--  2.0 unx    16218 bl defN 24-Apr-11 15:56 coverage/src_netdot_repository.py.zip
+?rw-rw-r--  2.0 unx    19706 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses_base.py.zip
+?rw-rw-r--  2.0 unx     1485 bl defN 24-Apr-11 15:56 coverage/src_netdot_trace.py.zip
+?rw-rw-r--  2.0 unx     1857 bl defN 24-Apr-11 15:56 coverage/src_netdot_mac_address.py.zip
+?rw-rw-r--  2.0 unx     2586 bl defN 24-Apr-11 15:56 coverage/src_netdot_parse.py.zip
+?rw-rw-r--  2.0 unx      902 bl defN 24-Apr-11 15:56 coverage/src_netdot_validate.py.zip
+?rw-rw-r--  2.0 unx      293 bl defN 24-Apr-11 15:56 coverage/src_netdot_version.py.zip
+?rw-rw-r--  2.0 unx     3986 bl defN 24-Apr-11 15:56 coverage/src_netdot_dataclasses___init__.py.zip
+?rw-rw-r--  2.0 unx     5006 bl defN 24-Apr-11 15:56 coverage/src_netdot_config.py.zip
+?rw-rw-r--  2.0 unx     2975 bl defN 24-Apr-11 15:56 coverage/src_netdot___init__.py.zip
+?rw-rw-r--  2.0 unx     9493 bl defN 24-Apr-11 15:56 coverage/src_netdot_unitofwork.py.zip
+?rw-rw-r--  2.0 unx     2116 bl defN 24-Apr-11 15:56 coverage/src_netdot_utils.py.zip
+?rw-rw-r--  2.0 unx     3922 bl defN 24-Apr-11 15:56 coverage/src_netdot_actions.py.zip
+35 files, 114610 bytes uncompressed, 114047 bytes compressed:  0.5%
```

#### zipnote {}

```diff
@@ -1,106 +1,106 @@
 Filename: coverage/
 Comment: 
 
 Filename: coverage/src_netdot_dataclasses_device.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_physaddr.py.zip
+Filename: coverage/src_netdot_dataclasses_dhcp.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_repository.py.zip
+Filename: coverage/src_netdot_dataclasses_dns.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_dhcp.py.zip
+Filename: coverage/src_netdot_dataclasses_entity.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_trace.py.zip
+Filename: coverage/src_netdot_dataclasses_physaddr.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_ipblock.py.zip
+Filename: coverage/src_netdot_dataclasses_products.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_mac_address.py.zip
+Filename: coverage/src_netdot_dataclasses_users.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_misc.py.zip
+Filename: coverage/src_netdot_dataclasses_vlan.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_dns.py.zip
+Filename: coverage/src_netdot_dataclasses_site.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_fwtable.py.zip
+Filename: coverage/src_netdot_dataclasses_ipblock.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_entity.py.zip
+Filename: coverage/src_netdot_dataclasses_misc.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_bgp.py.zip
+Filename: coverage/src_netdot_dataclasses_fwtable.py.zip
 Comment: 
 
 Filename: coverage/src_netdot_dataclasses_interface.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_cables.py.zip
+Filename: coverage/src_netdot_dataclasses_bgp.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_users.py.zip
+Filename: coverage/src_netdot_dataclasses_cables.py.zip
 Comment: 
 
 Filename: coverage/src_netdot_dataclasses_asset.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_parse.py.zip
+Filename: coverage/src_netdot_csv_util.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_validate.py.zip
+Filename: coverage/src_netdot_exceptions.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_version.py.zip
+Filename: coverage/src_netdot_gen_docs.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses___init__.py.zip
+Filename: coverage/src_netdot_io.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_base.py.zip
+Filename: coverage/src_netdot_client.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_unitofwork.py.zip
+Filename: coverage/src_netdot_repository.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_vlan.py.zip
+Filename: coverage/src_netdot_dataclasses_base.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_products.py.zip
+Filename: coverage/src_netdot_trace.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_dataclasses_site.py.zip
+Filename: coverage/src_netdot_mac_address.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_csv_util.py.zip
+Filename: coverage/src_netdot_parse.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_client.py.zip
+Filename: coverage/src_netdot_validate.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_exceptions.py.zip
+Filename: coverage/src_netdot_version.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_gen_docs.py.zip
+Filename: coverage/src_netdot_dataclasses___init__.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_io.py.zip
+Filename: coverage/src_netdot_config.py.zip
 Comment: 
 
 Filename: coverage/src_netdot___init__.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_utils.py.zip
+Filename: coverage/src_netdot_unitofwork.py.zip
 Comment: 
 
-Filename: coverage/src_netdot_config.py.zip
+Filename: coverage/src_netdot_utils.py.zip
 Comment: 
 
 Filename: coverage/src_netdot_actions.py.zip
 Comment: 
 
 Zip file comment:
```

#### coverage/src_netdot_dataclasses_device.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3543 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    35748 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_device.py
+?rw-rw-r--  2.0 unx    35748 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_device.py
 1 file, 35748 bytes uncompressed, 3365 bytes compressed:  90.6%
```

#### coverage/src_netdot_dataclasses_physaddr.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 890 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     6141 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_physaddr.py
+?rw-rw-r--  2.0 unx     6141 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_physaddr.py
 1 file, 6141 bytes uncompressed, 708 bytes compressed:  88.5%
```

#### coverage/src_netdot_repository.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 16218 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx   135887 bl defN 24-Feb-24 08:31 src_netdot_repository.py
+?rw-rw-r--  2.0 unx   135887 bl defN 24-Apr-11 15:56 src_netdot_repository.py
 1 file, 135887 bytes uncompressed, 16056 bytes compressed:  88.2%
```

#### coverage/src_netdot_dataclasses_dhcp.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1253 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    11839 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_dhcp.py
+?rw-rw-r--  2.0 unx    11839 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_dhcp.py
 1 file, 11839 bytes uncompressed, 1079 bytes compressed:  90.9%
```

#### coverage/src_netdot_trace.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1485 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     9583 bl defN 24-Feb-24 08:31 src_netdot_trace.py
+?rw-rw-r--  2.0 unx     9583 bl defN 24-Apr-11 15:56 src_netdot_trace.py
 1 file, 9583 bytes uncompressed, 1333 bytes compressed:  86.1%
```

#### coverage/src_netdot_dataclasses_ipblock.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2090 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    19101 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_ipblock.py
+?rw-rw-r--  2.0 unx    19101 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_ipblock.py
 1 file, 19101 bytes uncompressed, 1910 bytes compressed:  90.0%
```

#### coverage/src_netdot_mac_address.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1857 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    12700 bl defN 24-Feb-24 08:31 src_netdot_mac_address.py
+?rw-rw-r--  2.0 unx    12700 bl defN 24-Apr-11 15:56 src_netdot_mac_address.py
 1 file, 12700 bytes uncompressed, 1693 bytes compressed:  86.7%
```

#### coverage/src_netdot_dataclasses_misc.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1238 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     9670 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_misc.py
+?rw-rw-r--  2.0 unx     9670 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_misc.py
 1 file, 9670 bytes uncompressed, 1064 bytes compressed:  89.0%
```

#### coverage/src_netdot_dataclasses_dns.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2710 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    31822 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_dns.py
+?rw-rw-r--  2.0 unx    31822 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_dns.py
 1 file, 31822 bytes uncompressed, 2538 bytes compressed:  92.0%
```

#### coverage/src_netdot_dataclasses_fwtable.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1368 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     9081 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_fwtable.py
+?rw-rw-r--  2.0 unx     9081 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_fwtable.py
 1 file, 9081 bytes uncompressed, 1188 bytes compressed:  86.9%
```

#### coverage/src_netdot_dataclasses_entity.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1016 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     8604 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_entity.py
+?rw-rw-r--  2.0 unx     8604 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_entity.py
 1 file, 8604 bytes uncompressed, 838 bytes compressed:  90.3%
```

#### coverage/src_netdot_dataclasses_bgp.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 966 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     7046 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_bgp.py
+?rw-rw-r--  2.0 unx     7046 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_bgp.py
 1 file, 7046 bytes uncompressed, 794 bytes compressed:  88.7%
```

#### coverage/src_netdot_dataclasses_interface.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2517 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    21862 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_interface.py
+?rw-rw-r--  2.0 unx    21862 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_interface.py
 1 file, 21862 bytes uncompressed, 2333 bytes compressed:  89.3%
```

#### coverage/src_netdot_dataclasses_cables.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1806 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    21569 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_cables.py
+?rw-rw-r--  2.0 unx    21569 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_cables.py
 1 file, 21569 bytes uncompressed, 1628 bytes compressed:  92.5%
```

#### coverage/src_netdot_dataclasses_users.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2036 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    22267 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_users.py
+?rw-rw-r--  2.0 unx    22267 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_users.py
 1 file, 22267 bytes uncompressed, 1860 bytes compressed:  91.6%
```

#### coverage/src_netdot_dataclasses_asset.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 938 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     6494 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_asset.py
+?rw-rw-r--  2.0 unx     6494 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_asset.py
 1 file, 6494 bytes uncompressed, 762 bytes compressed:  88.3%
```

#### coverage/src_netdot_parse.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2586 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    18406 bl defN 24-Feb-24 08:31 src_netdot_parse.py
+?rw-rw-r--  2.0 unx    18406 bl defN 24-Apr-11 15:56 src_netdot_parse.py
 1 file, 18406 bytes uncompressed, 2434 bytes compressed:  86.8%
```

#### coverage/src_netdot_validate.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 902 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     4157 bl defN 24-Feb-24 08:31 src_netdot_validate.py
+?rw-rw-r--  2.0 unx     4157 bl defN 24-Apr-11 15:56 src_netdot_validate.py
 1 file, 4157 bytes uncompressed, 744 bytes compressed:  82.1%
```

#### coverage/src_netdot_version.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 293 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx      188 bl defN 24-Feb-24 08:31 src_netdot_version.py
+?rw-rw-r--  2.0 unx      188 bl defN 24-Apr-11 15:56 src_netdot_version.py
 1 file, 188 bytes uncompressed, 137 bytes compressed:  27.1%
```

##### src_netdot_version.py

```diff
@@ -1 +1 @@
-<tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="1">1</a></td><td class="hits">1</td><td class="code">__version__ &#61; &#39;0.4.3&#39;</td></tr>
+<tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="1">1</a></td><td class="hits">1</td><td class="code">__version__ &#61; &#39;0.4.4&#39;</td></tr>
```

#### coverage/src_netdot_dataclasses___init__.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3986 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    43692 bl defN 24-Feb-24 08:31 src_netdot_dataclasses___init__.py
+?rw-rw-r--  2.0 unx    43692 bl defN 24-Apr-11 15:56 src_netdot_dataclasses___init__.py
 1 file, 43692 bytes uncompressed, 3804 bytes compressed:  91.3%
```

#### coverage/src_netdot_dataclasses_base.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 19706 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx   183362 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_base.py
+?rw-rw-r--  2.0 unx   183362 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_base.py
 1 file, 183362 bytes uncompressed, 19532 bytes compressed:  89.3%
```

#### coverage/src_netdot_unitofwork.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 9493 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    87260 bl defN 24-Feb-24 08:31 src_netdot_unitofwork.py
+?rw-rw-r--  2.0 unx    87260 bl defN 24-Apr-11 15:56 src_netdot_unitofwork.py
 1 file, 87260 bytes uncompressed, 9331 bytes compressed:  89.3%
```

#### coverage/src_netdot_dataclasses_vlan.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 977 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     6839 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_vlan.py
+?rw-rw-r--  2.0 unx     6839 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_vlan.py
 1 file, 6839 bytes uncompressed, 803 bytes compressed:  88.3%
```

#### coverage/src_netdot_dataclasses_products.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 874 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     5645 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_products.py
+?rw-rw-r--  2.0 unx     5645 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_products.py
 1 file, 5645 bytes uncompressed, 692 bytes compressed:  87.7%
```

#### coverage/src_netdot_dataclasses_site.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2872 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    27319 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_site.py
+?rw-rw-r--  2.0 unx    27319 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_site.py
 1 file, 27319 bytes uncompressed, 2698 bytes compressed:  90.1%
```

#### coverage/src_netdot_csv_util.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3714 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    27455 bl defN 24-Feb-24 08:31 src_netdot_csv_util.py
+?rw-rw-r--  2.0 unx    27455 bl defN 24-Apr-11 15:56 src_netdot_csv_util.py
 1 file, 27455 bytes uncompressed, 3556 bytes compressed:  87.0%
```

#### coverage/src_netdot_client.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 8369 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    68935 bl defN 24-Feb-24 08:31 src_netdot_client.py
+?rw-rw-r--  2.0 unx    68935 bl defN 24-Apr-11 15:56 src_netdot_client.py
 1 file, 68935 bytes uncompressed, 8215 bytes compressed:  88.1%
```

#### coverage/src_netdot_exceptions.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1189 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     7915 bl defN 24-Feb-24 08:31 src_netdot_exceptions.py
+?rw-rw-r--  2.0 unx     7915 bl defN 24-Apr-11 15:56 src_netdot_exceptions.py
 1 file, 7915 bytes uncompressed, 1027 bytes compressed:  87.0%
```

#### coverage/src_netdot_gen_docs.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3241 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    23275 bl defN 24-Feb-24 08:31 src_netdot_gen_docs.py
+?rw-rw-r--  2.0 unx    23275 bl defN 24-Apr-11 15:56 src_netdot_gen_docs.py
 1 file, 23275 bytes uncompressed, 3083 bytes compressed:  86.8%
```

#### coverage/src_netdot_io.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 458 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     1297 bl defN 24-Feb-24 08:31 src_netdot_io.py
+?rw-rw-r--  2.0 unx     1297 bl defN 24-Apr-11 15:56 src_netdot_io.py
 1 file, 1297 bytes uncompressed, 312 bytes compressed:  75.9%
```

#### coverage/src_netdot___init__.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2975 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    28301 bl defN 24-Feb-24 08:31 src_netdot___init__.py
+?rw-rw-r--  2.0 unx    28301 bl defN 24-Apr-11 15:56 src_netdot___init__.py
 1 file, 28301 bytes uncompressed, 2817 bytes compressed:  90.0%
```

#### coverage/src_netdot_utils.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2116 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    15105 bl defN 24-Feb-24 08:31 src_netdot_utils.py
+?rw-rw-r--  2.0 unx    15105 bl defN 24-Apr-11 15:56 src_netdot_utils.py
 1 file, 15105 bytes uncompressed, 1964 bytes compressed:  87.0%
```

#### coverage/src_netdot_config.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 5006 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    37605 bl defN 24-Feb-24 08:31 src_netdot_config.py
+?rw-rw-r--  2.0 unx    37605 bl defN 24-Apr-11 15:56 src_netdot_config.py
 1 file, 37605 bytes uncompressed, 4852 bytes compressed:  87.1%
```

#### coverage/src_netdot_actions.py.zip

##### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3922 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    29481 bl defN 24-Feb-24 08:31 src_netdot_actions.py
+?rw-rw-r--  2.0 unx    29481 bl defN 24-Apr-11 15:56 src_netdot_actions.py
 1 file, 29481 bytes uncompressed, 3766 bytes compressed:  87.2%
```

### Comparing `netdot-0.4.3rc1/.vscode/launch.json` & `netdot-0.4.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/.vscode/settings.json` & `netdot-0.4.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/coverage/src_netdot___init__.py.zip` & `netdot-0.4.4/coverage/src_netdot___init__.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2975 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    28301 bl defN 24-Feb-24 08:31 src_netdot___init__.py
+?rw-rw-r--  2.0 unx    28301 bl defN 24-Apr-11 15:56 src_netdot___init__.py
 1 file, 28301 bytes uncompressed, 2817 bytes compressed:  90.0%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_actions.py.zip` & `netdot-0.4.4/coverage/src_netdot_actions.py.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3922 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    29481 bl defN 24-Feb-24 08:31 src_netdot_actions.py
+?rw-rw-r--  2.0 unx    29481 bl defN 24-Apr-11 15:56 src_netdot_actions.py
 1 file, 29481 bytes uncompressed, 3766 bytes compressed:  87.2%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_client.py.zip` & `netdot-0.4.4/coverage/src_netdot_client.py.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 8369 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    68935 bl defN 24-Feb-24 08:31 src_netdot_client.py
+?rw-rw-r--  2.0 unx    68935 bl defN 24-Apr-11 15:56 src_netdot_client.py
 1 file, 68935 bytes uncompressed, 8215 bytes compressed:  88.1%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_config.py.zip` & `netdot-0.4.4/coverage/src_netdot_config.py.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 5006 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    37605 bl defN 24-Feb-24 08:31 src_netdot_config.py
+?rw-rw-r--  2.0 unx    37605 bl defN 24-Apr-11 15:56 src_netdot_config.py
 1 file, 37605 bytes uncompressed, 4852 bytes compressed:  87.1%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_csv_util.py.zip` & `netdot-0.4.4/coverage/src_netdot_csv_util.py.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3714 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    27455 bl defN 24-Feb-24 08:31 src_netdot_csv_util.py
+?rw-rw-r--  2.0 unx    27455 bl defN 24-Apr-11 15:56 src_netdot_csv_util.py
 1 file, 27455 bytes uncompressed, 3556 bytes compressed:  87.0%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses___init__.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses___init__.py.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3986 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    43692 bl defN 24-Feb-24 08:31 src_netdot_dataclasses___init__.py
+?rw-rw-r--  2.0 unx    43692 bl defN 24-Apr-11 15:56 src_netdot_dataclasses___init__.py
 1 file, 43692 bytes uncompressed, 3804 bytes compressed:  91.3%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_asset.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_asset.py.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 938 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     6494 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_asset.py
+?rw-rw-r--  2.0 unx     6494 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_asset.py
 1 file, 6494 bytes uncompressed, 762 bytes compressed:  88.3%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_base.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_base.py.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 19706 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx   183362 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_base.py
+?rw-rw-r--  2.0 unx   183362 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_base.py
 1 file, 183362 bytes uncompressed, 19532 bytes compressed:  89.3%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_bgp.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_bgp.py.zip`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 966 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     7046 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_bgp.py
+?rw-rw-r--  2.0 unx     7046 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_bgp.py
 1 file, 7046 bytes uncompressed, 794 bytes compressed:  88.7%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_cables.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_cables.py.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1806 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    21569 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_cables.py
+?rw-rw-r--  2.0 unx    21569 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_cables.py
 1 file, 21569 bytes uncompressed, 1628 bytes compressed:  92.5%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_device.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_device.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3543 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    35748 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_device.py
+?rw-rw-r--  2.0 unx    35748 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_device.py
 1 file, 35748 bytes uncompressed, 3365 bytes compressed:  90.6%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_dhcp.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_dhcp.py.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1253 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    11839 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_dhcp.py
+?rw-rw-r--  2.0 unx    11839 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_dhcp.py
 1 file, 11839 bytes uncompressed, 1079 bytes compressed:  90.9%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_dns.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_dns.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2710 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    31822 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_dns.py
+?rw-rw-r--  2.0 unx    31822 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_dns.py
 1 file, 31822 bytes uncompressed, 2538 bytes compressed:  92.0%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_entity.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_entity.py.zip`

 * *Files 27% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1016 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     8604 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_entity.py
+?rw-rw-r--  2.0 unx     8604 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_entity.py
 1 file, 8604 bytes uncompressed, 838 bytes compressed:  90.3%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_fwtable.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_fwtable.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1368 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     9081 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_fwtable.py
+?rw-rw-r--  2.0 unx     9081 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_fwtable.py
 1 file, 9081 bytes uncompressed, 1188 bytes compressed:  86.9%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_interface.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_interface.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2517 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    21862 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_interface.py
+?rw-rw-r--  2.0 unx    21862 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_interface.py
 1 file, 21862 bytes uncompressed, 2333 bytes compressed:  89.3%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_ipblock.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_ipblock.py.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2090 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    19101 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_ipblock.py
+?rw-rw-r--  2.0 unx    19101 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_ipblock.py
 1 file, 19101 bytes uncompressed, 1910 bytes compressed:  90.0%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_physaddr.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_physaddr.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 890 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     6141 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_physaddr.py
+?rw-rw-r--  2.0 unx     6141 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_physaddr.py
 1 file, 6141 bytes uncompressed, 708 bytes compressed:  88.5%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_products.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_products.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 874 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     5645 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_products.py
+?rw-rw-r--  2.0 unx     5645 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_products.py
 1 file, 5645 bytes uncompressed, 692 bytes compressed:  87.7%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_site.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_site.py.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2872 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    27319 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_site.py
+?rw-rw-r--  2.0 unx    27319 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_site.py
 1 file, 27319 bytes uncompressed, 2698 bytes compressed:  90.1%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_users.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_users.py.zip`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2036 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    22267 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_users.py
+?rw-rw-r--  2.0 unx    22267 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_users.py
 1 file, 22267 bytes uncompressed, 1860 bytes compressed:  91.6%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_dataclasses_vlan.py.zip` & `netdot-0.4.4/coverage/src_netdot_dataclasses_vlan.py.zip`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 977 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     6839 bl defN 24-Feb-24 08:31 src_netdot_dataclasses_vlan.py
+?rw-rw-r--  2.0 unx     6839 bl defN 24-Apr-11 15:56 src_netdot_dataclasses_vlan.py
 1 file, 6839 bytes uncompressed, 803 bytes compressed:  88.3%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_exceptions.py.zip` & `netdot-0.4.4/coverage/src_netdot_exceptions.py.zip`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1189 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     7915 bl defN 24-Feb-24 08:31 src_netdot_exceptions.py
+?rw-rw-r--  2.0 unx     7915 bl defN 24-Apr-11 15:56 src_netdot_exceptions.py
 1 file, 7915 bytes uncompressed, 1027 bytes compressed:  87.0%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_gen_docs.py.zip` & `netdot-0.4.4/coverage/src_netdot_gen_docs.py.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 3241 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    23275 bl defN 24-Feb-24 08:31 src_netdot_gen_docs.py
+?rw-rw-r--  2.0 unx    23275 bl defN 24-Apr-11 15:56 src_netdot_gen_docs.py
 1 file, 23275 bytes uncompressed, 3083 bytes compressed:  86.8%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_mac_address.py.zip` & `netdot-0.4.4/coverage/src_netdot_mac_address.py.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1857 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    12700 bl defN 24-Feb-24 08:31 src_netdot_mac_address.py
+?rw-rw-r--  2.0 unx    12700 bl defN 24-Apr-11 15:56 src_netdot_mac_address.py
 1 file, 12700 bytes uncompressed, 1693 bytes compressed:  86.7%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_parse.py.zip` & `netdot-0.4.4/coverage/src_netdot_parse.py.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2586 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    18406 bl defN 24-Feb-24 08:31 src_netdot_parse.py
+?rw-rw-r--  2.0 unx    18406 bl defN 24-Apr-11 15:56 src_netdot_parse.py
 1 file, 18406 bytes uncompressed, 2434 bytes compressed:  86.8%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_repository.py.zip` & `netdot-0.4.4/coverage/src_netdot_repository.py.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 16218 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx   135887 bl defN 24-Feb-24 08:31 src_netdot_repository.py
+?rw-rw-r--  2.0 unx   135887 bl defN 24-Apr-11 15:56 src_netdot_repository.py
 1 file, 135887 bytes uncompressed, 16056 bytes compressed:  88.2%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_trace.py.zip` & `netdot-0.4.4/coverage/src_netdot_trace.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1485 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     9583 bl defN 24-Feb-24 08:31 src_netdot_trace.py
+?rw-rw-r--  2.0 unx     9583 bl defN 24-Apr-11 15:56 src_netdot_trace.py
 1 file, 9583 bytes uncompressed, 1333 bytes compressed:  86.1%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_unitofwork.py.zip` & `netdot-0.4.4/coverage/src_netdot_unitofwork.py.zip`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 9493 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    87260 bl defN 24-Feb-24 08:31 src_netdot_unitofwork.py
+?rw-rw-r--  2.0 unx    87260 bl defN 24-Apr-11 15:56 src_netdot_unitofwork.py
 1 file, 87260 bytes uncompressed, 9331 bytes compressed:  89.3%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_utils.py.zip` & `netdot-0.4.4/coverage/src_netdot_utils.py.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2116 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    15105 bl defN 24-Feb-24 08:31 src_netdot_utils.py
+?rw-rw-r--  2.0 unx    15105 bl defN 24-Apr-11 15:56 src_netdot_utils.py
 1 file, 15105 bytes uncompressed, 1964 bytes compressed:  87.0%
```

### Comparing `netdot-0.4.3rc1/coverage/src_netdot_validate.py.zip` & `netdot-0.4.4/coverage/src_netdot_validate.py.zip`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 902 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     4157 bl defN 24-Feb-24 08:31 src_netdot_validate.py
+?rw-rw-r--  2.0 unx     4157 bl defN 24-Apr-11 15:56 src_netdot_validate.py
 1 file, 4157 bytes uncompressed, 744 bytes compressed:  82.1%
```

### Comparing `netdot-0.4.3rc1/docs/README.md` & `netdot-0.4.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/docs/api.md` & `netdot-0.4.4/docs/api.md`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/docs/changelog.md` & `netdot-0.4.4/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,21 @@
 * Generate a prettier document for ["Feature Flags" Environment Variables](./generated-env-var-docs.md).
     * Today, we [ab]use [configargparse](https://pypi.org/project/ConfigArgParse/) to generate that documentation.
 * GitHub Repository for this project.
     * Ideally, this repository will live in the official "uoregon" GitHub Organization.
     * Instead, it will likely be a 'personal repository' belonging to @ryeleo.
 
 
+## [0.4.4]
+
+### Changed
+
+* Internal-only change: Update CICD workflow to use [`ntsjenkins` shared library](https://confluence.uoregon.edu/x/TQRaGw)
+
+
 ## [0.4.3]
 
 ### Changed
 
 * A call to `save_changes` will now print, "No changes need to be saved," if that is the case. 
     * BEFORE: `save_changes` would print "Saved changes!", even if there was no changes.
 * FIX: auto-update when updating relationships between Netdot objects:
```

### Comparing `netdot-0.4.3rc1/docs/dependencies.md` & `netdot-0.4.4/docs/dependencies.md`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/docs/design.md` & `netdot-0.4.4/docs/design.md`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/docs/development.md` & `netdot-0.4.4/docs/development.md`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/docs/generated-api-docs.md` & `netdot-0.4.4/docs/generated-api-docs.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 # Netdot Python API Generated Documentation
 
 <a id="netdot-python-api-generated-documentation"></a>
-> Version 0.4.3 documentation generated on Feb 24, 2024 at 08:31AM 
+> Version 0.4.4 documentation generated on Apr 11, 2024 at 03:55PM 
 >
 > Netdot Python API contains many generated methods.
 > This documentation is intended to help you understand what is available.
 
 
 
 ## class `netdot.Repository`
@@ -5547,15 +5547,15 @@
 
 Returns:
     UnitOfWork: The Unit of Work that was loaded.
 ```
 
 #### UnitOfWork.save_as_pickle
 
-> ```save_as_pickle(self, filename: str = 'netdot-cli-0.4.3-proposed_changes-2024-02-24_08-31.pickle') -> str```
+> ```save_as_pickle(self, filename: str = 'netdot-cli-0.4.4-proposed_changes-2024-04-11_15-55.pickle') -> str```
 
 ```
 Save this Unit of Work to a file.
 
 To be loaded in the future using :func:`load()`.
 
 Args:
```

### Comparing `netdot-0.4.3rc1/docs/generated-env-var-docs.md` & `netdot-0.4.4/docs/generated-env-var-docs.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 # Netdot Python API Environment Variables
 <a id="netdot-python-api-environment-variables"></a>
 
 > Generated using `netdot.config.help()`
 >
-> Version 0.4.3 documentation generated on Feb 24, 2024 at 08:31AM 
+> Version 0.4.4 documentation generated on Apr 11, 2024 at 03:55PM 
 
 ```
 
   --terse TERSE         Print terse output (that generally tries to fit the
                         screen width). [env var: NETDOT_CLI_TERSE] (default:
                         False)
   --server-url SERVER_URL
@@ -92,15 +92,15 @@
                         error occurs. [env var:
                         NETDOT_CLI_SAVE_AS_FILE_ON_ERROR] (default: True)
   --error-pickle-filename ERROR_PICKLE_FILENAME
                         The filename to use when saving proposed changes to a
                         file when an error occurs. (timestamp based on when
                         the script is run) [env var:
                         NETDOT_CLI_ERROR_PICKLE_FILENAME] (default: netdot-
-                        cli-0.4.3-proposed_changes-2024-02-24_08-31.pickle)
+                        cli-0.4.4-proposed_changes-2024-04-11_15-55.pickle)
 
  In general, command-line values override environment variables which override
 defaults.
 
 
 ⚠ NOTICE: These defaults are read from Environment Variables when 
 `netdot.config` module is imported (via `netdot.config.parse_env_vars`).
```

### Comparing `netdot-0.4.3rc1/docs/package-deployment.md` & `netdot-0.4.4/docs/package-deployment.md`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/docs/user-guide.md` & `netdot-0.4.4/docs/user-guide.md`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/docs/assets/converted_netdot_schema.py` & `netdot-0.4.4/docs/assets/converted_netdot_schema.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/docs/assets/netdot_schema.sql` & `netdot-0.4.4/docs/assets/netdot_schema.sql`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/__init__.py` & `netdot-0.4.4/src/netdot/__init__.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/actions.py` & `netdot-0.4.4/src/netdot/actions.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/client.py` & `netdot-0.4.4/src/netdot/client.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/config.py` & `netdot-0.4.4/src/netdot/config.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/csv_util.py` & `netdot-0.4.4/src/netdot/csv_util.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/exceptions.py` & `netdot-0.4.4/src/netdot/exceptions.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/gen_docs.py` & `netdot-0.4.4/src/netdot/gen_docs.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/mac_address.py` & `netdot-0.4.4/src/netdot/mac_address.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/parse.py` & `netdot-0.4.4/src/netdot/parse.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/repository.py` & `netdot-0.4.4/src/netdot/repository.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/trace.py` & `netdot-0.4.4/src/netdot/trace.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/unitofwork.py` & `netdot-0.4.4/src/netdot/unitofwork.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/utils.py` & `netdot-0.4.4/src/netdot/utils.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/validate.py` & `netdot-0.4.4/src/netdot/validate.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/__init__.py` & `netdot-0.4.4/src/netdot/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/asset.py` & `netdot-0.4.4/src/netdot/dataclasses/asset.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/base.py` & `netdot-0.4.4/src/netdot/dataclasses/base.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/bgp.py` & `netdot-0.4.4/src/netdot/dataclasses/bgp.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/cables.py` & `netdot-0.4.4/src/netdot/dataclasses/cables.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/device.py` & `netdot-0.4.4/src/netdot/dataclasses/device.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/dhcp.py` & `netdot-0.4.4/src/netdot/dataclasses/dhcp.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/dns.py` & `netdot-0.4.4/src/netdot/dataclasses/dns.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/entity.py` & `netdot-0.4.4/src/netdot/dataclasses/entity.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/fwtable.py` & `netdot-0.4.4/src/netdot/dataclasses/fwtable.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/interface.py` & `netdot-0.4.4/src/netdot/dataclasses/interface.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/ipblock.py` & `netdot-0.4.4/src/netdot/dataclasses/ipblock.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/misc.py` & `netdot-0.4.4/src/netdot/dataclasses/misc.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/physaddr.py` & `netdot-0.4.4/src/netdot/dataclasses/physaddr.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/products.py` & `netdot-0.4.4/src/netdot/dataclasses/products.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/site.py` & `netdot-0.4.4/src/netdot/dataclasses/site.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/users.py` & `netdot-0.4.4/src/netdot/dataclasses/users.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/src/netdot/dataclasses/vlan.py` & `netdot-0.4.4/src/netdot/dataclasses/vlan.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/conftest.py` & `netdot-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_NetdotAPIDataclass.py` & `netdot-0.4.4/tests/test_NetdotAPIDataclass.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_client.py` & `netdot-0.4.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_csv_util.py` & `netdot-0.4.4/tests/test_csv_util.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_generated_docs.py` & `netdot-0.4.4/tests/test_generated_docs.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_mac_address.py` & `netdot-0.4.4/tests/test_mac_address.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_netdotAction.py` & `netdot-0.4.4/tests/test_netdotAction.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_parse_dto.py` & `netdot-0.4.4/tests/test_parse_dto.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_repository.py` & `netdot-0.4.4/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_repository_CRUD.py` & `netdot-0.4.4/tests/test_repository_CRUD.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_repository_DRY_RUN.py` & `netdot-0.4.4/tests/test_repository_DRY_RUN.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_repository_get_where.py` & `netdot-0.4.4/tests/test_repository_get_where.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_trace.py` & `netdot-0.4.4/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_unitofwork.py` & `netdot-0.4.4/tests/test_unitofwork.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/tests/test_utils.py` & `netdot-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/.gitignore` & `netdot-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/LICENSE` & `netdot-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/hatch.toml` & `netdot-0.4.4/hatch.toml`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/pyproject.toml` & `netdot-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `netdot-0.4.3rc1/PKG-INFO` & `netdot-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: netdot
-Version: 0.4.3rc1
+Version: 0.4.4
 Summary: Python wrapper for Netdot Web API.
 Author-email: University of Oregon <ntsjenkins@uoregon.edu>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: API,IPAM,NTS,REST,UO,VRA,netdot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -792,14 +792,21 @@
 * Generate a prettier document for ["Feature Flags" Environment Variables](#netdot-python-api-environment-variables).
     * Today, we [ab]use [configargparse](https://pypi.org/project/ConfigArgParse/) to generate that documentation.
 * GitHub Repository for this project.
     * Ideally, this repository will live in the official "uoregon" GitHub Organization.
     * Instead, it will likely be a 'personal repository' belonging to @ryeleo.
 
 
+## [0.4.4]
+
+### Changed
+
+* Internal-only change: Update CICD workflow to use [`ntsjenkins` shared library](https://confluence.uoregon.edu/x/TQRaGw)
+
+
 ## [0.4.3]
 
 ### Changed
 
 * A call to `save_changes` will now print, "No changes need to be saved," if that is the case. 
     * BEFORE: `save_changes` would print "Saved changes!", even if there was no changes.
 * FIX: auto-update when updating relationships between Netdot objects:
@@ -1009,15 +1016,15 @@
 
 * Provide Python Netdot Client, as originally authored by Francisco Gray.
 
 
 # Netdot Python API Generated Documentation
 
 <a id="netdot-python-api-generated-documentation"></a>
-> Version 0.4.3 documentation generated on Feb 24, 2024 at 08:31AM 
+> Version 0.4.4 documentation generated on Apr 11, 2024 at 03:55PM 
 >
 > Netdot Python API contains many generated methods.
 > This documentation is intended to help you understand what is available.
 
 
 
 ## class `netdot.Repository`
@@ -6557,15 +6564,15 @@
 
 Returns:
     UnitOfWork: The Unit of Work that was loaded.
 ```
 
 #### UnitOfWork.save_as_pickle
 
-> ```save_as_pickle(self, filename: str = 'netdot-cli-0.4.3-proposed_changes-2024-02-24_08-31.pickle') -> str```
+> ```save_as_pickle(self, filename: str = 'netdot-cli-0.4.4-proposed_changes-2024-04-11_15-55.pickle') -> str```
 
 ```
 Save this Unit of Work to a file.
 
 To be loaded in the future using :func:`load()`.
 
 Args:
@@ -19727,15 +19734,15 @@
 
 
 # Netdot Python API Environment Variables
 <a id="netdot-python-api-environment-variables"></a>
 
 > Generated using `netdot.config.help()`
 >
-> Version 0.4.3 documentation generated on Feb 24, 2024 at 08:31AM 
+> Version 0.4.4 documentation generated on Apr 11, 2024 at 03:55PM 
 
 ```
 
   --terse TERSE         Print terse output (that generally tries to fit the
                         screen width). [env var: NETDOT_CLI_TERSE] (default:
                         False)
   --server-url SERVER_URL
@@ -19818,15 +19825,15 @@
                         error occurs. [env var:
                         NETDOT_CLI_SAVE_AS_FILE_ON_ERROR] (default: True)
   --error-pickle-filename ERROR_PICKLE_FILENAME
                         The filename to use when saving proposed changes to a
                         file when an error occurs. (timestamp based on when
                         the script is run) [env var:
                         NETDOT_CLI_ERROR_PICKLE_FILENAME] (default: netdot-
-                        cli-0.4.3-proposed_changes-2024-02-24_08-31.pickle)
+                        cli-0.4.4-proposed_changes-2024-04-11_15-55.pickle)
 
  In general, command-line values override environment variables which override
 defaults.
 
 
 ⚠ NOTICE: These defaults are read from Environment Variables when 
 `netdot.config` module is imported (via `netdot.config.parse_env_vars`).
```


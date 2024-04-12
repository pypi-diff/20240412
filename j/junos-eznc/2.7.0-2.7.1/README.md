# Comparing `tmp/junos-eznc-2.7.0.tar.gz` & `tmp/junos-eznc-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junos-eznc-2.7.0.tar", last modified: Fri Jan 12 07:01:42 2024, max compression
+gzip compressed data, was "junos-eznc-2.7.1.tar", last modified: Fri Apr 12 05:44:24 2024, max compression
```

## Comparing `junos-eznc-2.7.0.tar` & `junos-eznc-2.7.1.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.959576 junos-eznc-2.7.0/
--rw-r--r--   0 babud      (501) staff       (20)    11351 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/LICENSE
--rw-r--r--   0 babud      (501) staff       (20)      110 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/MANIFEST.in
--rw-r--r--   0 babud      (501) staff       (20)     1706 2024-01-12 07:01:42.959099 junos-eznc-2.7.0/PKG-INFO
--rw-r--r--   0 babud      (501) staff       (20)       33 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/README.txt
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.699044 junos-eznc-2.7.0/lib/
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.704117 junos-eznc-2.7.0/lib/jnpr/
--rw-r--r--   0 babud      (501) staff       (20)       56 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/__init__.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.710196 junos-eznc-2.7.0/lib/jnpr/junos/
--rw-r--r--   0 babud      (501) staff       (20)     1295 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)      497 2024-01-12 07:01:42.961060 junos-eznc-2.7.0/lib/jnpr/junos/_version.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.713042 junos-eznc-2.7.0/lib/jnpr/junos/cfg/
--rw-r--r--   0 babud      (501) staff       (20)       45 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfg/__init__.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.717131 junos-eznc-2.7.0/lib/jnpr/junos/cfg/phyport/
--rw-r--r--   0 babud      (501) staff       (20)      457 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfg/phyport/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)     2386 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfg/phyport/base.py
--rw-r--r--   0 babud      (501) staff       (20)     1564 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfg/phyport/classic.py
--rw-r--r--   0 babud      (501) staff       (20)     2228 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfg/phyport/switch.py
--rw-r--r--   0 babud      (501) staff       (20)    26638 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfg/resource.py
--rw-r--r--   0 babud      (501) staff       (20)     2883 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfg/user.py
--rw-r--r--   0 babud      (501) staff       (20)     3372 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfg/user_ssh_key.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.718714 junos-eznc-2.7.0/lib/jnpr/junos/cfgro/
--rw-r--r--   0 babud      (501) staff       (20)        0 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfgro/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)     1951 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/cfgro/srx.yml
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.779556 junos-eznc-2.7.0/lib/jnpr/junos/command/
--rw-r--r--   0 babud      (501) staff       (20)     1369 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)      227 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/chassis_fan.yml
--rw-r--r--   0 babud      (501) staff       (20)      353 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/cm_error.yml
--rw-r--r--   0 babud      (501) staff       (20)      802 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_drd_error.yml
--rw-r--r--   0 babud      (501) staff       (20)     1246 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_fi_error.yml
--rw-r--r--   0 babud      (501) staff       (20)      503 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_fi_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      316 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_fo_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      234 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_host_drop.yml
--rw-r--r--   0 babud      (501) staff       (20)      533 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_li_error.yml
--rw-r--r--   0 babud      (501) staff       (20)      446 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_lo_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      345 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_pt_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      892 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_wi_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      688 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ea_wo_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)       83 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/fpc_link_stats.yml
--rw-r--r--   0 babud      (501) staff       (20)      300 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/fpc_memory.yml
--rw-r--r--   0 babud      (501) staff       (20)      268 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/fpc_threads.yml
--rw-r--r--   0 babud      (501) staff       (20)      242 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/host_loopback_status.yml
--rw-r--r--   0 babud      (501) staff       (20)      650 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ithrottle.yml
--rw-r--r--   0 babud      (501) staff       (20)      318 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/jnh_exceptions.yml
--rw-r--r--   0 babud      (501) staff       (20)      286 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/jnh_ifd_stream.yml
--rw-r--r--   0 babud      (501) staff       (20)      487 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/jnhexceptionpkt.yml
--rw-r--r--   0 babud      (501) staff       (20)     3409 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/linecard_ethernet_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      307 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/ospf_neighbor.yml
--rw-r--r--   0 babud      (501) staff       (20)      359 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/pci_error.yml
--rw-r--r--   0 babud      (501) staff       (20)      356 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/pfe_ddos_policer.yml
--rw-r--r--   0 babud      (501) staff       (20)      607 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/pre_classifier.yml
--rw-r--r--   0 babud      (501) staff       (20)      628 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/scheduler_info.yml
--rw-r--r--   0 babud      (501) staff       (20)      273 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/system_proc_ext.yml
--rw-r--r--   0 babud      (501) staff       (20)      526 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/system_queues.yml
--rw-r--r--   0 babud      (501) staff       (20)      217 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/task_io.yml
--rw-r--r--   0 babud      (501) staff       (20)      699 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/toe_pfe.yml
--rw-r--r--   0 babud      (501) staff       (20)      238 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/veriexec.yml
--rw-r--r--   0 babud      (501) staff       (20)      186 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/vmcores.yml
--rw-r--r--   0 babud      (501) staff       (20)      728 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_drd_error.yml
--rw-r--r--   0 babud      (501) staff       (20)      437 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_fi_error.yml
--rw-r--r--   0 babud      (501) staff       (20)      448 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_fi_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      236 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_fo_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      464 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_host_drop.yml
--rw-r--r--   0 babud      (501) staff       (20)      527 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_li_error.yml
--rw-r--r--   0 babud      (501) staff       (20)      438 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_lo_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      520 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_pt_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      959 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_wi_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)      696 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/command/xm_wo_statistics.yml
--rw-r--r--   0 babud      (501) staff       (20)    12654 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/console.py
--rw-r--r--   0 babud      (501) staff       (20)     7311 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/decorators.py
--rw-r--r--   0 babud      (501) staff       (20)    56961 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/device.py
--rw-r--r--   0 babud      (501) staff       (20)     9037 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/exception.py
--rw-r--r--   0 babud      (501) staff       (20)    12824 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factcache.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.812516 junos-eznc-2.7.0/lib/jnpr/junos/factory/
--rw-r--r--   0 babud      (501) staff       (20)     1002 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)    26947 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/cfgtable.py
--rw-r--r--   0 babud      (501) staff       (20)    15712 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/cmdtable.py
--rw-r--r--   0 babud      (501) staff       (20)     2017 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/cmdview.py
--rw-r--r--   0 babud      (501) staff       (20)     6056 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/factory_cls.py
--rw-r--r--   0 babud      (501) staff       (20)    14596 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/factory_loader.py
--rw-r--r--   0 babud      (501) staff       (20)     7429 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/optable.py
--rw-r--r--   0 babud      (501) staff       (20)    39236 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/state_machine.py
--rw-r--r--   0 babud      (501) staff       (20)    11672 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/table.py
--rw-r--r--   0 babud      (501) staff       (20)     2491 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/to_json.py
--rw-r--r--   0 babud      (501) staff       (20)    11843 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/view.py
--rw-r--r--   0 babud      (501) staff       (20)     2175 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/factory/viewfields.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.851752 junos-eznc-2.7.0/lib/jnpr/junos/facts/
--rw-r--r--   0 babud      (501) staff       (20)     4106 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/__example.py
--rw-r--r--   0 babud      (501) staff       (20)     3516 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)     5318 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/current_re.py
--rw-r--r--   0 babud      (501) staff       (20)     1889 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/domain.py
--rw-r--r--   0 babud      (501) staff       (20)     2419 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/ethernet_mac_table.py
--rw-r--r--   0 babud      (501) staff       (20)      758 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/file_list.py
--rw-r--r--   0 babud      (501) staff       (20)     3434 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/get_chassis_cluster_status.py
--rw-r--r--   0 babud      (501) staff       (20)     1542 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/get_chassis_inventory.py
--rw-r--r--   0 babud      (501) staff       (20)     5813 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/get_route_engine_information.py
--rw-r--r--   0 babud      (501) staff       (20)    11235 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/get_software_information.py
--rw-r--r--   0 babud      (501) staff       (20)     2611 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/get_virtual_chassis_information.py
--rw-r--r--   0 babud      (501) staff       (20)      648 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/ifd_style.py
--rw-r--r--   0 babud      (501) staff       (20)     2970 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/iri_mapping.py
--rw-r--r--   0 babud      (501) staff       (20)      882 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/is_linux.py
--rw-r--r--   0 babud      (501) staff       (20)     2908 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/personality.py
--rw-r--r--   0 babud      (501) staff       (20)     3616 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/facts/swver.py
--rw-r--r--   0 babud      (501) staff       (20)     7339 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/jxml.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.868316 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/
--rw-r--r--   0 babud      (501) staff       (20)      808 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)     1794 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/chassis.py
--rw-r--r--   0 babud      (501) staff       (20)     1196 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/domain.py
--rw-r--r--   0 babud      (501) staff       (20)      185 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/ifd_style.py
--rw-r--r--   0 babud      (501) staff       (20)     1319 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/personality.py
--rw-r--r--   0 babud      (501) staff       (20)     2919 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/routing_engines.py
--rw-r--r--   0 babud      (501) staff       (20)      214 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/session.py
--rw-r--r--   0 babud      (501) staff       (20)      991 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/srx_cluster.py
--rw-r--r--   0 babud      (501) staff       (20)      505 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/switch_style.py
--rw-r--r--   0 babud      (501) staff       (20)     4581 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/ofacts/swver.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.912030 junos-eznc-2.7.0/lib/jnpr/junos/op/
--rw-r--r--   0 babud      (501) staff       (20)     1412 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)      247 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/arp.yml
--rw-r--r--   0 babud      (501) staff       (20)     1768 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/bfd.yml
--rw-r--r--   0 babud      (501) staff       (20)      272 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/bgp.yml
--rw-r--r--   0 babud      (501) staff       (20)      415 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/ccc.yml
--rw-r--r--   0 babud      (501) staff       (20)      308 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/ddos.yml
--rw-r--r--   0 babud      (501) staff       (20)      807 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/elsethernetswitchingtable.yml
--rw-r--r--   0 babud      (501) staff       (20)      989 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/ethernetswitchingtable.yml
--rw-r--r--   0 babud      (501) staff       (20)      668 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/ethport.yml
--rw-r--r--   0 babud      (501) staff       (20)     1818 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/fpc.yml
--rw-r--r--   0 babud      (501) staff       (20)      189 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/idpattacks.yml
--rw-r--r--   0 babud      (501) staff       (20)      518 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/intopticdiag.yml
--rw-r--r--   0 babud      (501) staff       (20)      289 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/inventory.yml
--rw-r--r--   0 babud      (501) staff       (20)      933 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/isis.yml
--rw-r--r--   0 babud      (501) staff       (20)      914 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/l2circuit.yml
--rw-r--r--   0 babud      (501) staff       (20)     1793 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/lacp.yml
--rw-r--r--   0 babud      (501) staff       (20)     1151 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/ldp.yml
--rw-r--r--   0 babud      (501) staff       (20)      535 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/lldp.yml
--rw-r--r--   0 babud      (501) staff       (20)      293 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/nd.yml
--rw-r--r--   0 babud      (501) staff       (20)     1930 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/ospf.yml
--rw-r--r--   0 babud      (501) staff       (20)      804 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/pfestats.yml
--rw-r--r--   0 babud      (501) staff       (20)     2678 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/phyport.yml
--rw-r--r--   0 babud      (501) staff       (20)      366 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/ppm.yml
--rw-r--r--   0 babud      (501) staff       (20)     1200 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/routes.yml
--rw-r--r--   0 babud      (501) staff       (20)      535 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/securityzone.yml
--rw-r--r--   0 babud      (501) staff       (20)      308 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/systemstorage.yml
--rw-r--r--   0 babud      (501) staff       (20)      429 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/taskmemory.yml
--rw-r--r--   0 babud      (501) staff       (20)     1683 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/teddb.yml
--rw-r--r--   0 babud      (501) staff       (20)      298 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/vlan.yml
--rw-r--r--   0 babud      (501) staff       (20)      325 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/op/xcvr.yml
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.926770 junos-eznc-2.7.0/lib/jnpr/junos/resources/
--rw-r--r--   0 babud      (501) staff       (20)        0 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)      188 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/autosys.py
--rw-r--r--   0 babud      (501) staff       (20)      314 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/autosys.yml
--rw-r--r--   0 babud      (501) staff       (20)      184 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/bgp.py
--rw-r--r--   0 babud      (501) staff       (20)      565 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/bgp.yml
--rw-r--r--   0 babud      (501) staff       (20)      190 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/interface.py
--rw-r--r--   0 babud      (501) staff       (20)      442 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/interface.yml
--rw-r--r--   0 babud      (501) staff       (20)      193 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/staticroutes.py
--rw-r--r--   0 babud      (501) staff       (20)      339 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/staticroutes.yml
--rw-r--r--   0 babud      (501) staff       (20)      187 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/syslog.py
--rw-r--r--   0 babud      (501) staff       (20)      463 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/syslog.yml
--rw-r--r--   0 babud      (501) staff       (20)      185 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/user.py
--rw-r--r--   0 babud      (501) staff       (20)      521 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/resources/user.yml
--rw-r--r--   0 babud      (501) staff       (20)    16129 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/rpcmeta.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.934395 junos-eznc-2.7.0/lib/jnpr/junos/transport/
--rw-r--r--   0 babud      (501) staff       (20)        0 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/transport/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)     9069 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/transport/tty.py
--rw-r--r--   0 babud      (501) staff       (20)     7810 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/transport/tty_netconf.py
--rw-r--r--   0 babud      (501) staff       (20)     3060 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/transport/tty_serial.py
--rw-r--r--   0 babud      (501) staff       (20)     7113 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/transport/tty_ssh.py
--rw-r--r--   0 babud      (501) staff       (20)     3858 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/transport/tty_telnet.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.948990 junos-eznc-2.7.0/lib/jnpr/junos/utils/
--rw-r--r--   0 babud      (501) staff       (20)       39 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/__init__.py
--rw-r--r--   0 babud      (501) staff       (20)    36394 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/config.py
--rw-r--r--   0 babud      (501) staff       (20)    18526 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/fs.py
--rw-r--r--   0 babud      (501) staff       (20)     4122 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/ftp.py
--rw-r--r--   0 babud      (501) staff       (20)     3804 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/scp.py
--rw-r--r--   0 babud      (501) staff       (20)     1780 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/ssh_client.py
--rw-r--r--   0 babud      (501) staff       (20)     7660 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/start_shell.py
--rw-r--r--   0 babud      (501) staff       (20)    58422 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/sw.py
--rw-r--r--   0 babud      (501) staff       (20)     1134 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/utils/util.py
--rw-r--r--   0 babud      (501) staff       (20)      248 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/lib/jnpr/junos/version.py
-drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-01-12 07:01:42.957735 junos-eznc-2.7.0/lib/junos_eznc.egg-info/
--rw-r--r--   0 babud      (501) staff       (20)     1706 2024-01-12 07:01:42.000000 junos-eznc-2.7.0/lib/junos_eznc.egg-info/PKG-INFO
--rw-r--r--   0 babud      (501) staff       (20)     5993 2024-01-12 07:01:42.000000 junos-eznc-2.7.0/lib/junos_eznc.egg-info/SOURCES.txt
--rw-r--r--   0 babud      (501) staff       (20)        1 2024-01-12 07:01:42.000000 junos-eznc-2.7.0/lib/junos_eznc.egg-info/dependency_links.txt
--rw-r--r--   0 babud      (501) staff       (20)        5 2024-01-12 07:01:42.000000 junos-eznc-2.7.0/lib/junos_eznc.egg-info/namespace_packages.txt
--rw-r--r--   0 babud      (501) staff       (20)      140 2024-01-12 07:01:42.000000 junos-eznc-2.7.0/lib/junos_eznc.egg-info/requires.txt
--rw-r--r--   0 babud      (501) staff       (20)        5 2024-01-12 07:01:42.000000 junos-eznc-2.7.0/lib/junos_eznc.egg-info/top_level.txt
--rwxr-xr-x   0 babud      (501) staff       (20)      223 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/requirements.txt
--rw-r--r--   0 babud      (501) staff       (20)      182 2024-01-12 07:01:42.960543 junos-eznc-2.7.0/setup.cfg
--rwxr-xr-x   0 babud      (501) staff       (20)     2006 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/setup.py
--rw-r--r--   0 babud      (501) staff       (20)    86854 2024-01-12 07:00:08.000000 junos-eznc-2.7.0/versioneer.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.602869 junos-eznc-2.7.1/
+-rw-r--r--   0 babud      (501) staff       (20)    11351 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/LICENSE
+-rw-r--r--   0 babud      (501) staff       (20)      110 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/MANIFEST.in
+-rw-r--r--   0 babud      (501) staff       (20)     1674 2024-04-12 05:44:24.602315 junos-eznc-2.7.1/PKG-INFO
+-rw-r--r--   0 babud      (501) staff       (20)       33 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/README.txt
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.523207 junos-eznc-2.7.1/lib/
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.526708 junos-eznc-2.7.1/lib/jnpr/
+-rw-r--r--   0 babud      (501) staff       (20)       56 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/__init__.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.531948 junos-eznc-2.7.1/lib/jnpr/junos/
+-rw-r--r--   0 babud      (501) staff       (20)     1295 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)      497 2024-04-12 05:44:24.604480 junos-eznc-2.7.1/lib/jnpr/junos/_version.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.535035 junos-eznc-2.7.1/lib/jnpr/junos/cfg/
+-rw-r--r--   0 babud      (501) staff       (20)       45 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfg/__init__.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.537076 junos-eznc-2.7.1/lib/jnpr/junos/cfg/phyport/
+-rw-r--r--   0 babud      (501) staff       (20)      457 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfg/phyport/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)     2385 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfg/phyport/base.py
+-rw-r--r--   0 babud      (501) staff       (20)     1564 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfg/phyport/classic.py
+-rw-r--r--   0 babud      (501) staff       (20)     2228 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfg/phyport/switch.py
+-rw-r--r--   0 babud      (501) staff       (20)    26638 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfg/resource.py
+-rw-r--r--   0 babud      (501) staff       (20)     2882 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfg/user.py
+-rw-r--r--   0 babud      (501) staff       (20)     3371 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfg/user_ssh_key.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.537831 junos-eznc-2.7.1/lib/jnpr/junos/cfgro/
+-rw-r--r--   0 babud      (501) staff       (20)        0 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfgro/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)     1951 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/cfgro/srx.yml
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.556356 junos-eznc-2.7.1/lib/jnpr/junos/command/
+-rw-r--r--   0 babud      (501) staff       (20)     1369 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)      227 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/chassis_fan.yml
+-rw-r--r--   0 babud      (501) staff       (20)      353 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/cm_error.yml
+-rw-r--r--   0 babud      (501) staff       (20)      802 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_drd_error.yml
+-rw-r--r--   0 babud      (501) staff       (20)     1246 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_fi_error.yml
+-rw-r--r--   0 babud      (501) staff       (20)      503 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_fi_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      316 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_fo_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      234 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_host_drop.yml
+-rw-r--r--   0 babud      (501) staff       (20)      533 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_li_error.yml
+-rw-r--r--   0 babud      (501) staff       (20)      446 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_lo_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      345 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_pt_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      892 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_wi_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      688 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ea_wo_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)       83 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/fpc_link_stats.yml
+-rw-r--r--   0 babud      (501) staff       (20)      300 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/fpc_memory.yml
+-rw-r--r--   0 babud      (501) staff       (20)      268 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/fpc_threads.yml
+-rw-r--r--   0 babud      (501) staff       (20)      242 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/host_loopback_status.yml
+-rw-r--r--   0 babud      (501) staff       (20)      650 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ithrottle.yml
+-rw-r--r--   0 babud      (501) staff       (20)      318 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/jnh_exceptions.yml
+-rw-r--r--   0 babud      (501) staff       (20)      286 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/jnh_ifd_stream.yml
+-rw-r--r--   0 babud      (501) staff       (20)      487 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/jnhexceptionpkt.yml
+-rw-r--r--   0 babud      (501) staff       (20)     3409 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/linecard_ethernet_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      307 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/ospf_neighbor.yml
+-rw-r--r--   0 babud      (501) staff       (20)      359 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/pci_error.yml
+-rw-r--r--   0 babud      (501) staff       (20)      356 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/pfe_ddos_policer.yml
+-rw-r--r--   0 babud      (501) staff       (20)      607 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/pre_classifier.yml
+-rw-r--r--   0 babud      (501) staff       (20)      628 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/scheduler_info.yml
+-rw-r--r--   0 babud      (501) staff       (20)      273 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/system_proc_ext.yml
+-rw-r--r--   0 babud      (501) staff       (20)      526 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/system_queues.yml
+-rw-r--r--   0 babud      (501) staff       (20)      217 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/task_io.yml
+-rw-r--r--   0 babud      (501) staff       (20)      699 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/toe_pfe.yml
+-rw-r--r--   0 babud      (501) staff       (20)      238 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/veriexec.yml
+-rw-r--r--   0 babud      (501) staff       (20)      186 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/vmcores.yml
+-rw-r--r--   0 babud      (501) staff       (20)      728 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_drd_error.yml
+-rw-r--r--   0 babud      (501) staff       (20)      437 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_fi_error.yml
+-rw-r--r--   0 babud      (501) staff       (20)      448 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_fi_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      236 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_fo_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      464 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_host_drop.yml
+-rw-r--r--   0 babud      (501) staff       (20)      527 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_li_error.yml
+-rw-r--r--   0 babud      (501) staff       (20)      438 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_lo_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      520 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_pt_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      959 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_wi_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)      696 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/command/xm_wo_statistics.yml
+-rw-r--r--   0 babud      (501) staff       (20)    12654 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/console.py
+-rw-r--r--   0 babud      (501) staff       (20)     7311 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/decorators.py
+-rw-r--r--   0 babud      (501) staff       (20)    56958 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/device.py
+-rw-r--r--   0 babud      (501) staff       (20)     9020 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/exception.py
+-rw-r--r--   0 babud      (501) staff       (20)    12824 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factcache.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.561790 junos-eznc-2.7.1/lib/jnpr/junos/factory/
+-rw-r--r--   0 babud      (501) staff       (20)     1002 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)    26947 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/cfgtable.py
+-rw-r--r--   0 babud      (501) staff       (20)    15712 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/cmdtable.py
+-rw-r--r--   0 babud      (501) staff       (20)     2016 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/cmdview.py
+-rw-r--r--   0 babud      (501) staff       (20)     6056 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/factory_cls.py
+-rw-r--r--   0 babud      (501) staff       (20)    14596 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/factory_loader.py
+-rw-r--r--   0 babud      (501) staff       (20)     7429 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/optable.py
+-rw-r--r--   0 babud      (501) staff       (20)    39238 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/state_machine.py
+-rw-r--r--   0 babud      (501) staff       (20)    11672 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/table.py
+-rw-r--r--   0 babud      (501) staff       (20)     2491 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/to_json.py
+-rw-r--r--   0 babud      (501) staff       (20)    11842 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/view.py
+-rw-r--r--   0 babud      (501) staff       (20)     2174 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/factory/viewfields.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.568220 junos-eznc-2.7.1/lib/jnpr/junos/facts/
+-rw-r--r--   0 babud      (501) staff       (20)     4106 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/__example.py
+-rw-r--r--   0 babud      (501) staff       (20)     3517 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)     5318 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/current_re.py
+-rw-r--r--   0 babud      (501) staff       (20)     1889 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/domain.py
+-rw-r--r--   0 babud      (501) staff       (20)     2419 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/ethernet_mac_table.py
+-rw-r--r--   0 babud      (501) staff       (20)      758 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/file_list.py
+-rw-r--r--   0 babud      (501) staff       (20)     3434 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/get_chassis_cluster_status.py
+-rw-r--r--   0 babud      (501) staff       (20)     1542 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/get_chassis_inventory.py
+-rw-r--r--   0 babud      (501) staff       (20)     5813 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/get_route_engine_information.py
+-rw-r--r--   0 babud      (501) staff       (20)    11235 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/get_software_information.py
+-rw-r--r--   0 babud      (501) staff       (20)     2611 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/get_virtual_chassis_information.py
+-rw-r--r--   0 babud      (501) staff       (20)      648 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/ifd_style.py
+-rw-r--r--   0 babud      (501) staff       (20)     2970 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/iri_mapping.py
+-rw-r--r--   0 babud      (501) staff       (20)      882 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/is_linux.py
+-rw-r--r--   0 babud      (501) staff       (20)     2908 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/personality.py
+-rw-r--r--   0 babud      (501) staff       (20)     3616 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/facts/swver.py
+-rw-r--r--   0 babud      (501) staff       (20)     7339 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/jxml.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.572458 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/
+-rw-r--r--   0 babud      (501) staff       (20)      808 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)     1794 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/chassis.py
+-rw-r--r--   0 babud      (501) staff       (20)     1196 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/domain.py
+-rw-r--r--   0 babud      (501) staff       (20)      185 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/ifd_style.py
+-rw-r--r--   0 babud      (501) staff       (20)     1319 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/personality.py
+-rw-r--r--   0 babud      (501) staff       (20)     2919 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/routing_engines.py
+-rw-r--r--   0 babud      (501) staff       (20)      215 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/session.py
+-rw-r--r--   0 babud      (501) staff       (20)      991 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/srx_cluster.py
+-rw-r--r--   0 babud      (501) staff       (20)      505 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/switch_style.py
+-rw-r--r--   0 babud      (501) staff       (20)     4581 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/ofacts/swver.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.584600 junos-eznc-2.7.1/lib/jnpr/junos/op/
+-rw-r--r--   0 babud      (501) staff       (20)     1412 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)      247 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/arp.yml
+-rw-r--r--   0 babud      (501) staff       (20)     1768 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/bfd.yml
+-rw-r--r--   0 babud      (501) staff       (20)      272 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/bgp.yml
+-rw-r--r--   0 babud      (501) staff       (20)      415 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/ccc.yml
+-rw-r--r--   0 babud      (501) staff       (20)      308 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/ddos.yml
+-rw-r--r--   0 babud      (501) staff       (20)      807 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/elsethernetswitchingtable.yml
+-rw-r--r--   0 babud      (501) staff       (20)      989 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/ethernetswitchingtable.yml
+-rw-r--r--   0 babud      (501) staff       (20)      668 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/ethport.yml
+-rw-r--r--   0 babud      (501) staff       (20)     1818 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/fpc.yml
+-rw-r--r--   0 babud      (501) staff       (20)      189 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/idpattacks.yml
+-rw-r--r--   0 babud      (501) staff       (20)      518 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/intopticdiag.yml
+-rw-r--r--   0 babud      (501) staff       (20)      289 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/inventory.yml
+-rw-r--r--   0 babud      (501) staff       (20)      933 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/isis.yml
+-rw-r--r--   0 babud      (501) staff       (20)      914 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/l2circuit.yml
+-rw-r--r--   0 babud      (501) staff       (20)     1793 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/lacp.yml
+-rw-r--r--   0 babud      (501) staff       (20)     1151 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/ldp.yml
+-rw-r--r--   0 babud      (501) staff       (20)      535 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/lldp.yml
+-rw-r--r--   0 babud      (501) staff       (20)      293 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/nd.yml
+-rw-r--r--   0 babud      (501) staff       (20)     1930 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/ospf.yml
+-rw-r--r--   0 babud      (501) staff       (20)      804 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/pfestats.yml
+-rw-r--r--   0 babud      (501) staff       (20)     2804 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/phyport.yml
+-rw-r--r--   0 babud      (501) staff       (20)      366 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/ppm.yml
+-rw-r--r--   0 babud      (501) staff       (20)     1200 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/routes.yml
+-rw-r--r--   0 babud      (501) staff       (20)      535 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/securityzone.yml
+-rw-r--r--   0 babud      (501) staff       (20)      308 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/systemstorage.yml
+-rw-r--r--   0 babud      (501) staff       (20)      429 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/taskmemory.yml
+-rw-r--r--   0 babud      (501) staff       (20)     1683 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/teddb.yml
+-rw-r--r--   0 babud      (501) staff       (20)      298 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/vlan.yml
+-rw-r--r--   0 babud      (501) staff       (20)      325 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/op/xcvr.yml
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.590152 junos-eznc-2.7.1/lib/jnpr/junos/resources/
+-rw-r--r--   0 babud      (501) staff       (20)        0 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)      189 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/autosys.py
+-rw-r--r--   0 babud      (501) staff       (20)      314 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/autosys.yml
+-rw-r--r--   0 babud      (501) staff       (20)      185 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/bgp.py
+-rw-r--r--   0 babud      (501) staff       (20)      565 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/bgp.yml
+-rw-r--r--   0 babud      (501) staff       (20)      191 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/interface.py
+-rw-r--r--   0 babud      (501) staff       (20)      442 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/interface.yml
+-rw-r--r--   0 babud      (501) staff       (20)      194 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/staticroutes.py
+-rw-r--r--   0 babud      (501) staff       (20)      339 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/staticroutes.yml
+-rw-r--r--   0 babud      (501) staff       (20)      188 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/syslog.py
+-rw-r--r--   0 babud      (501) staff       (20)      463 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/syslog.yml
+-rw-r--r--   0 babud      (501) staff       (20)      186 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/user.py
+-rw-r--r--   0 babud      (501) staff       (20)      521 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/resources/user.yml
+-rw-r--r--   0 babud      (501) staff       (20)    16129 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/rpcmeta.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.592455 junos-eznc-2.7.1/lib/jnpr/junos/transport/
+-rw-r--r--   0 babud      (501) staff       (20)        0 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/transport/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)     9068 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/transport/tty.py
+-rw-r--r--   0 babud      (501) staff       (20)     7809 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/transport/tty_netconf.py
+-rw-r--r--   0 babud      (501) staff       (20)     3060 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/transport/tty_serial.py
+-rw-r--r--   0 babud      (501) staff       (20)     7113 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/transport/tty_ssh.py
+-rw-r--r--   0 babud      (501) staff       (20)     3858 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/transport/tty_telnet.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.596589 junos-eznc-2.7.1/lib/jnpr/junos/utils/
+-rw-r--r--   0 babud      (501) staff       (20)       39 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/__init__.py
+-rw-r--r--   0 babud      (501) staff       (20)    36394 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/config.py
+-rw-r--r--   0 babud      (501) staff       (20)    18525 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/fs.py
+-rw-r--r--   0 babud      (501) staff       (20)     4122 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/ftp.py
+-rw-r--r--   0 babud      (501) staff       (20)     3804 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/scp.py
+-rw-r--r--   0 babud      (501) staff       (20)     1780 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/ssh_client.py
+-rw-r--r--   0 babud      (501) staff       (20)     7659 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/start_shell.py
+-rw-r--r--   0 babud      (501) staff       (20)    58641 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/sw.py
+-rw-r--r--   0 babud      (501) staff       (20)     1134 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/utils/util.py
+-rw-r--r--   0 babud      (501) staff       (20)      248 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/lib/jnpr/junos/version.py
+drwxr-xr-x   0 babud      (501) staff       (20)        0 2024-04-12 05:44:24.600134 junos-eznc-2.7.1/lib/junos_eznc.egg-info/
+-rw-r--r--   0 babud      (501) staff       (20)     1674 2024-04-12 05:44:24.000000 junos-eznc-2.7.1/lib/junos_eznc.egg-info/PKG-INFO
+-rw-r--r--   0 babud      (501) staff       (20)     5993 2024-04-12 05:44:24.000000 junos-eznc-2.7.1/lib/junos_eznc.egg-info/SOURCES.txt
+-rw-r--r--   0 babud      (501) staff       (20)        1 2024-04-12 05:44:24.000000 junos-eznc-2.7.1/lib/junos_eznc.egg-info/dependency_links.txt
+-rw-r--r--   0 babud      (501) staff       (20)        5 2024-04-12 05:44:24.000000 junos-eznc-2.7.1/lib/junos_eznc.egg-info/namespace_packages.txt
+-rw-r--r--   0 babud      (501) staff       (20)      123 2024-04-12 05:44:24.000000 junos-eznc-2.7.1/lib/junos_eznc.egg-info/requires.txt
+-rw-r--r--   0 babud      (501) staff       (20)        5 2024-04-12 05:44:24.000000 junos-eznc-2.7.1/lib/junos_eznc.egg-info/top_level.txt
+-rwxr-xr-x   0 babud      (501) staff       (20)      206 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/requirements.txt
+-rw-r--r--   0 babud      (501) staff       (20)      182 2024-04-12 05:44:24.603947 junos-eznc-2.7.1/setup.cfg
+-rwxr-xr-x   0 babud      (501) staff       (20)     2125 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/setup.py
+-rw-r--r--   0 babud      (501) staff       (20)    86854 2024-04-12 05:42:59.000000 junos-eznc-2.7.1/versioneer.py
```

### Comparing `junos-eznc-2.7.0/LICENSE` & `junos-eznc-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/PKG-INFO` & `junos-eznc-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junos-eznc
-Version: 2.7.0
+Version: 2.7.1
 Summary: Junos 'EZ' automation for non-programmers
 Home-page: http://www.github.com/Juniper/py-junos-eznc
 Author: Jeremy Schulman, Nitin Kumar, Rick Sherman, Stacy Smith
 Author-email: jnpr-community-netdev@juniper.net
 License: Apache 2.0
 Keywords: Junos NETCONF networking automation
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,15 +26,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: lxml>=3.2.4
 Requires-Dist: ncclient>=0.6.15
-Requires-Dist: paramiko>=1.15.2
 Requires-Dist: scp>=0.7.0
 Requires-Dist: jinja2>=2.7.1
 Requires-Dist: PyYAML>=5.1
 Requires-Dist: six
 Requires-Dist: pyserial
 Requires-Dist: yamlordereddictloader
 Requires-Dist: pyparsing
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/__init__.py` & `junos-eznc-2.7.1/lib/jnpr/junos/__init__.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/cfg/phyport/base.py` & `junos-eznc-2.7.1/lib/jnpr/junos/cfg/phyport/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from lxml.builder import E
 
 # local module
 from jnpr.junos.cfg.resource import Resource
 
 
 class PhyPortBase(Resource):
-
     """
     [edit interfaces <name>]
 
     Resource name: str
       <name> is the interface-name (IFD), e.g. 'ge-0/0/0'
     """
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/cfg/phyport/classic.py` & `junos-eznc-2.7.1/lib/jnpr/junos/cfg/phyport/classic.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/cfg/phyport/switch.py` & `junos-eznc-2.7.1/lib/jnpr/junos/cfg/phyport/switch.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/cfg/resource.py` & `junos-eznc-2.7.1/lib/jnpr/junos/cfg/resource.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/cfg/user.py` & `junos-eznc-2.7.1/lib/jnpr/junos/cfg/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # module packages
 from jnpr.junos.cfg import Resource
 from jnpr.junos import jxml as JXML
 from jnpr.junos.cfg.user_ssh_key import UserSSHKey
 
 
 class User(Resource):
-
     """
     [edit system login user <name>]
 
     Resource name: str
       <name> is the user login name
 
     Manages resources:
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/cfg/user_ssh_key.py` & `junos-eznc-2.7.1/lib/jnpr/junos/cfg/user_ssh_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 # local module
 from jnpr.junos.cfg import Resource
 from jnpr.junos import jxml as JXML
 
 
 class UserSSHKey(Resource):
-
     """
     [edit system login user <name> authentication <key-type> <key-value> ]
 
     Resource name: tuple(<key-type>, <key-value>)
       <key-type> : ['ssh-dsa', 'ssh-rsa']
       <key-value> : SSH public key string (usually something very long)
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/cfgro/srx.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/cfgro/srx.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/__init__.py` & `junos-eznc-2.7.1/lib/jnpr/junos/command/__init__.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/ea_drd_error.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/ea_drd_error.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/ea_fi_error.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/ea_fi_error.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/ea_li_error.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/ea_li_error.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/ea_wi_statistics.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/ea_wi_statistics.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/ea_wo_statistics.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/ea_wo_statistics.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/ithrottle.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/ithrottle.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/linecard_ethernet_statistics.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/linecard_ethernet_statistics.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/pre_classifier.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/pre_classifier.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/scheduler_info.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/scheduler_info.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/system_queues.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/system_queues.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/toe_pfe.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/toe_pfe.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/xm_drd_error.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/xm_drd_error.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/xm_li_error.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/xm_li_error.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/xm_pt_statistics.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/xm_pt_statistics.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/xm_wi_statistics.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/xm_wi_statistics.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/command/xm_wo_statistics.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/command/xm_wo_statistics.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/console.py` & `junos-eznc-2.7.1/lib/jnpr/junos/console.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/decorators.py` & `junos-eznc-2.7.1/lib/jnpr/junos/decorators.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/device.py` & `junos-eznc-2.7.1/lib/jnpr/junos/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
 _MODULEPATH = os.path.dirname(__file__)
 
 logger = logging.getLogger("jnpr.junos.device")
 
 
 class _MyTemplateLoader(jinja2.BaseLoader):
-
     """
     Create a jinja2 template loader class that can be used to
     load templates from all over the filesystem, but defaults
     to the CWD and the 'templates' directory of the module
     """
 
     def __init__(self):
@@ -1019,15 +1018,14 @@
     # -----------------------------------------------------------------------
 
     def __repr__(self):
         return "Device(%s)" % self.hostname
 
 
 class DeviceSessionListener(SessionListener):
-
     """
     Listens to Session class of Netconf Transport
     and detects errors in the transport.
     """
 
     def __init__(self, device):
         self._device = device
@@ -1041,15 +1039,14 @@
         Set the device's connected status to False.
         :type ex: :exc:`Exception`
         """
         self._device.connected = False
 
 
 class Device(_Connection):
-
     """
     Junos Device class.
 
     :attr:`ON_JUNOS`:
         **READ-ONLY** -
         Auto-set to ``True`` when this code is running on a Junos device,
         vs. running on a local-server remotely connecting to a device.
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/exception.py` & `junos-eznc-2.7.1/lib/jnpr/junos/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     Generated when there is a loop in fact gathering.
     """
 
     pass
 
 
 class RpcError(Exception):
-
     """
     Parent class for all junos-pyez RPC Exceptions
     """
 
     def __init__(self, cmd=None, rsp=None, errs=None, dev=None, timeout=None, re=None):
         """
         :cmd: is the rpc command
@@ -83,15 +82,14 @@
         else:
             return self.__class__.__name__
 
     __str__ = __repr__
 
 
 class CommitError(RpcError):
-
     """
     Generated in response to a commit-check or a commit action.
     """
 
     def __init__(self, rsp, cmd=None, errs=None):
         RpcError.__init__(self, cmd, rsp, errs)
 
@@ -103,15 +101,14 @@
             self.message,
         )
 
     __str__ = __repr__
 
 
 class ConfigLoadError(RpcError):
-
     """
     Generated in response to a failure when loading a configuration.
     """
 
     def __init__(self, rsp, cmd=None, errs=None):
         RpcError.__init__(self, cmd, rsp, errs)
 
@@ -123,52 +120,48 @@
             self.message,
         )
 
     __str__ = __repr__
 
 
 class LockError(RpcError):
-
     """
     Generated in response to attempting to take an exclusive
     lock on the configuration database.
     """
 
     def __init__(self, rsp):
         RpcError.__init__(self, rsp=rsp)
 
 
 class UnlockError(RpcError):
-
     """
     Generated in response to attempting to unlock the
     configuration database.
     """
 
     def __init__(self, rsp):
         RpcError.__init__(self, rsp=rsp)
 
 
 class PermissionError(RpcError):
-
     """
     Generated in response to invoking an RPC for which the
     auth user does not have user-class permissions.
 
     PermissionError.message gives you the specific RPC that cause
     the exceptions
     """
 
     def __init__(self, rsp, cmd=None, errs=None):
         RpcError.__init__(self, cmd=cmd, rsp=rsp, errs=errs)
         self.message = rsp.findtext(".//bad-element")
 
 
 class RpcTimeoutError(RpcError):
-
     """
     Generated in response to a RPC execution timeout.
     """
 
     def __init__(self, dev, cmd, timeout):
         RpcError.__init__(self, dev=dev, cmd=cmd, timeout=timeout)
 
@@ -177,15 +170,14 @@
             self.__class__.__name__, self.dev.hostname, self.cmd, self.timeout
         )
 
     __str__ = __repr__
 
 
 class SwRollbackError(RpcError):
-
     """
     Generated in response to a SW rollback error.
     """
 
     def __init__(self, rsp, re=None):
         RpcError.__init__(self, re=re, rsp=rsp)
 
@@ -204,15 +196,14 @@
 # ================================================================
 #                    Connection Exceptions
 # ================================================================
 # ================================================================
 
 
 class ConnectError(Exception):
-
     """
     Parent class for all connection related exceptions
     """
 
     def __init__(self, dev, msg=None):
         self.dev = dev
         self._orig = msg
@@ -245,86 +236,78 @@
         else:
             return "{}({})".format(self.__class__.__name__, self.dev.hostname)
 
     __str__ = __repr__
 
 
 class ProbeError(ConnectError):
-
     """
     Generated if auto_probe is enabled and the probe action fails
     """
 
     pass
 
 
 class ConnectAuthError(ConnectError):
-
     """
     Generated if the user-name, password is invalid
     """
 
     pass
 
 
 class ConnectTimeoutError(ConnectError):
-
     """
     Generated if the NETCONF session fails to connect, could
     be due to the fact the device is not ip reachable; bad
     ipaddr or just due to routing
     """
 
     pass
 
 
 class ConnectUnknownHostError(ConnectError):
-
     """
     Generated if the specific hostname does not DNS resolve
     """
 
     pass
 
 
 class ConnectRefusedError(ConnectError):
-
     """
     Generated if the specified host denies the NETCONF; could
     be that the services is not enabled, or the host has
     too many connections already.
     """
 
     pass
 
 
 class ConnectNotMasterError(ConnectError):
-
     """
     Generated if the connection is made to a non-master
     routing-engine.  This could be a backup RE on an MX
     device, or a virtual-chassis member (linecard), for example
     """
 
     pass
 
 
 class ConnectClosedError(ConnectError):
-
     """
     Generated if connection unexpectedly closed
     """
 
     def __init__(self, dev):
         ConnectError.__init__(self, dev=dev)
         dev.connected = False
 
 
 class JSONLoadError(Exception):
-
     """
     Generated if json content of rpc reply fails to load
     """
 
     def __init__(self, exception, rpc_content):
         self.ex_msg = str(exception)
         self.rpc_content = rpc_content
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factcache.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factcache.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/__init__.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/cfgtable.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/cfgtable.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/cmdtable.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/cmdtable.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/cmdview.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/cmdview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 class CMDView(object):
-
     """
     View is the base-class that makes extracting values from XML
     data appear as objects with attributes.
     """
 
     KEY = "name"
     KEY_ITEMS = []
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/factory_cls.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/factory_cls.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/factory_loader.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/factory_loader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This file contains the FactoryLoader class that is used to dynamically
 create Runstat Table and View objects from a <dict> of data.  The <dict> can
 originate from any kind of source: YAML, JSON, program.  For examples of YAML
 refer to the .yml files in this jnpr.junos.op directory.
 """
+
 # stdlib
 from copy import deepcopy
 import re
 
 from jinja2 import Environment
 
 # locally
@@ -25,15 +26,14 @@
 _TABLE = FactoryTable
 _CFGTBL = FactoryCfgTable
 _CMDTBL = FactoryCMDTable
 _CMDCHILDTBL = FactoryCMDChildTable
 
 
 class FactoryLoader(object):
-
     """
     Used to load a <dict> of data that contains Table and View definitions.
 
     The primary method is :load(): which will return a <dict> of item-name and
     item-class definitions.
 
     If you want to import these definitions directly into your namespace,
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/optable.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/optable.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/state_machine.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/state_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -806,17 +806,17 @@
                 # write a different function for this
                 for key, val in self._view.REGEX.items():
                     if val not in Identifiers.__dict__:
                         obj = re.search(
                             val, result[list(self._view.REGEX.keys()).index(key)], re.I
                         )
                         if obj and len(obj.groups()) >= 1:
-                            result[
-                                list(self._view.REGEX.keys()).index(key)
-                            ] = obj.groups()[0]
+                            result[list(self._view.REGEX.keys()).index(key)] = (
+                                obj.groups()[0]
+                            )
                 items = convert_to_data_type(result)
                 tmp_dict = dict(zip(self._view.REGEX.keys(), items))
                 if len(tmp_dict) > 0:
                     self._insert_data(
                         self._table.KEY, tmp_dict, list(self._view.REGEX.keys())
                     )
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/table.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/table.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/to_json.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/to_json.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/view.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from jinja2 import Template, meta
 
 from jnpr.junos.factory.viewfields import ViewFields
 from jnpr.junos.factory.to_json import TableViewJSONEncoder
 
 
 class View(object):
-
     """
     View is the base-class that makes extracting values from XML
     data appear as objects with attributes.
     """
 
     ITEM_NAME_XPATH = "name"
     FIELDS = {}
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/factory/viewfields.py` & `junos-eznc-2.7.1/lib/jnpr/junos/factory/viewfields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 class ViewFields(object):
-
     """
     Used to dynamically create a field dictionary used with the
     RunstatView class
     """
 
     def __init__(self):
         self._fields = dict()
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/__example.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/__example.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/__init__.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
       Accessing a dictionary key which does not correspond to an available fact
       will raise a KeyError (the same behavior as accessing a non-existent key
       of a normal dict.)
 
 The following dictionary keys represent the available facts and their meaning:
 
 """
+
 import sys
 
 import jnpr.junos.facts.current_re
 import jnpr.junos.facts.domain
 import jnpr.junos.facts.ethernet_mac_table
 import jnpr.junos.facts.file_list
 import jnpr.junos.facts.get_chassis_cluster_status
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/current_re.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/current_re.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/domain.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/domain.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/ethernet_mac_table.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/ethernet_mac_table.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/file_list.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/file_list.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/get_chassis_cluster_status.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/get_chassis_cluster_status.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/get_chassis_inventory.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/get_chassis_inventory.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/get_route_engine_information.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/get_route_engine_information.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/get_software_information.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/get_software_information.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/get_virtual_chassis_information.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/get_virtual_chassis_information.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/ifd_style.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/ifd_style.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/iri_mapping.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/iri_mapping.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/is_linux.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/is_linux.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/personality.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/personality.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/facts/swver.py` & `junos-eznc-2.7.1/lib/jnpr/junos/facts/swver.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/jxml.py` & `junos-eznc-2.7.1/lib/jnpr/junos/jxml.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/ofacts/__init__.py` & `junos-eznc-2.7.1/lib/jnpr/junos/ofacts/__init__.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/ofacts/chassis.py` & `junos-eznc-2.7.1/lib/jnpr/junos/ofacts/chassis.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/ofacts/domain.py` & `junos-eznc-2.7.1/lib/jnpr/junos/ofacts/domain.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/ofacts/personality.py` & `junos-eznc-2.7.1/lib/jnpr/junos/ofacts/personality.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/ofacts/routing_engines.py` & `junos-eznc-2.7.1/lib/jnpr/junos/ofacts/routing_engines.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/ofacts/srx_cluster.py` & `junos-eznc-2.7.1/lib/jnpr/junos/ofacts/srx_cluster.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/ofacts/swver.py` & `junos-eznc-2.7.1/lib/jnpr/junos/ofacts/swver.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/__init__.py` & `junos-eznc-2.7.1/lib/jnpr/junos/op/__init__.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/bfd.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/bfd.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/elsethernetswitchingtable.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/elsethernetswitchingtable.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/ethernetswitchingtable.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/ethernetswitchingtable.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/ethport.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/ethport.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/fpc.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/fpc.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/intopticdiag.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/intopticdiag.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/isis.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/isis.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/l2circuit.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/l2circuit.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/lacp.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/lacp.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/ldp.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/ldp.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/lldp.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/lldp.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/ospf.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/ospf.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/pfestats.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/pfestats.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/phyport.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/phyport.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,20 @@
 
   # fields that are part of groups are called
   # "fields_<group-name>"
 
   fields_ts:
     rx_bytes: { input-bytes: int }
     rx_packets: { input-packets: int }
+    rx_bps: { input-bps: int }
+    rx_pps: { input-pps: int }
     tx_bytes: { output-bytes: int }
     tx_packets: { output-packets: int }
+    tx_bps: { output-bps: int }
+    tx_pps: { output-pps: int }
 
   fields_rxerrs:
     rx_err_input: { input-errors: int }
     rx_err_drops: { input-drops: int }
 
 PhyPortErrorTable:
   rpc: get-interface-information
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/routes.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/routes.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/securityzone.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/securityzone.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/op/teddb.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/op/teddb.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/resources/bgp.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/resources/bgp.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/resources/user.yml` & `junos-eznc-2.7.1/lib/jnpr/junos/resources/user.yml`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/rpcmeta.py` & `junos-eznc-2.7.1/lib/jnpr/junos/rpcmeta.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/transport/tty.py` & `junos-eznc-2.7.1/lib/jnpr/junos/transport/tty.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 # =========================================================================
 # Terminal class
 # =========================================================================
 
 
 class Terminal(object):
-
     """
     Terminal is used to bootstrap Junos New Out of the Box (NOOB) device
     over the CONSOLE port. The general use-case is to setup the minimal
     configuration so that the device is IP reachable using SSH
     and NETCONF for remote management.
 
     Serial is needed for Junos devices that do not support
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/transport/tty_netconf.py` & `junos-eznc-2.7.1/lib/jnpr/junos/transport/tty_netconf.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 # =========================================================================
 # xmlmode_netconf
 # =========================================================================
 
 
 class tty_netconf(object):
-
     """
     Basic Junos XML API for bootstraping through the TTY
     """
 
     def __init__(self, tty):
         self._tty = tty
         self.hello = None
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/transport/tty_serial.py` & `junos-eznc-2.7.1/lib/jnpr/junos/transport/tty_serial.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/transport/tty_ssh.py` & `junos-eznc-2.7.1/lib/jnpr/junos/transport/tty_ssh.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/transport/tty_telnet.py` & `junos-eznc-2.7.1/lib/jnpr/junos/transport/tty_telnet.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/utils/config.py` & `junos-eznc-2.7.1/lib/jnpr/junos/utils/config.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/utils/fs.py` & `junos-eznc-2.7.1/lib/jnpr/junos/utils/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from jnpr.junos.utils.util import Util
 from jnpr.junos.utils.start_shell import StartShell
 
 from jnpr.junos.exception import RpcError
 
 
 class FS(Util):
-
     """
     Filesystem (FS) utilities:
 
     * :meth:`cat`: show the contents of a file
     * :meth:`checksum`: calculate file checksum (md5,sha256,sha1)
     * :meth:`cp`: local file copy (not scp)
     * :meth:`cwd`: change working directory
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/utils/ftp.py` & `junos-eznc-2.7.1/lib/jnpr/junos/utils/ftp.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/utils/scp.py` & `junos-eznc-2.7.1/lib/jnpr/junos/utils/scp.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/utils/ssh_client.py` & `junos-eznc-2.7.1/lib/jnpr/junos/utils/ssh_client.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/utils/start_shell.py` & `junos-eznc-2.7.1/lib/jnpr/junos/utils/start_shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 _JUNOS_PROMPT = "> "
 _SHELL_PROMPT = r"(%|#|\$)\s"
 _SELECT_WAIT = 0.1
 _RECVSZ = 1024
 
 
 class StartShell(object):
-
     """
     Junos shell execution utility.  This utility is written to
     support the "context manager" design pattern.  For example::
 
         def _ssh_exec(self, command):
             with StartShell(self._dev) as sh:
                 got = sh.run(command)
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/utils/sw.py` & `junos-eznc-2.7.1/lib/jnpr/junos/utils/sw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1127,21 +1127,20 @@
             if self._multi_RE is True and vmhost is True:
                 cmd.append(E("routing-engine", "both"))
             elif self._multi_RE is True and self._multi_VC is False:
                 cmd.append(E("both-routing-engines"))
             elif self._mixed_VC is True:
                 cmd.append(E("all-members"))
         elif (
-            self._multi_VC_nsync is True
-            or self._multi_VC is True
-            and member_id is not None
-        ):
+            self._multi_VC_nsync is True or self._multi_VC is True
+        ) and member_id is not None:
             cmd.append(E("member", str(member_id)))
         if in_min >= 0 and at is None:
-            cmd.append(E("in", str(in_min)))
+            if vmhost is not True:
+                cmd.append(E("in", str(in_min)))
         elif at is not None:
             cmd.append(E("at", str(at)))
         try:
             rsp = self.rpc(cmd, ignore_warning=True, normalize=True)
             if self._dev.facts["_is_linux"]:
                 got = rsp.text
             else:
@@ -1228,15 +1227,17 @@
             raise err
         except Exception as err:
             raise err
 
     # -------------------------------------------------------------------------
     # poweroff - system shutdown
     # -------------------------------------------------------------------------
-    def poweroff(self, in_min=0, at=None, on_node=None, all_re=True, other_re=False):
+    def poweroff(
+        self, in_min=0, at=None, on_node=None, all_re=True, other_re=False, vmhost=False
+    ):
         """
         Perform a system shutdown, with optional delay (in minutes) .
 
         If the device is equipped with dual-RE, then both RE will be
         shut down.  This code also handles EX/QFX VC.
 
         :param int in_min: time (minutes) before shutting down the device.
@@ -1250,33 +1251,36 @@
 
         :param bool all_re: In case of dual re or VC setup, function by default
             will shutdown all. If all is False will only shutdown connected device
 
         :param str other_re: If the system has dual Routing Engines and this option is C(true),
             then the action is performed on the other REs in the system.
 
+        :param str vmhost: If the device is vmhost device then the shutdown will be performed on the device
+
         :returns:
             * power-off message (string) if command successful
 
         :raises RpcError: when command is not successful.
 
         .. todo:: need to better handle the exception event.
         """
         if self._dev.facts["_is_linux"]:
             if on_node is None:
                 cmd = E("request-shutdown-power-off")
             else:
                 cmd = E("request-node-power-off")
                 cmd.append(E("node", on_node))
+        elif vmhost is True:
+            cmd = E("request-vmhost-poweroff")
+            all_re = False
         else:
             cmd = E("request-power-off")
         try:
-            return self._system_operation(
-                cmd, in_min, at, all_re, other_re, vmhost=False
-            )
+            return self._system_operation(cmd, in_min, at, all_re, other_re, vmhost)
         except Exception as err:
             if err.rsp.findtext(".//error-severity") != "warning":
                 raise err
 
     # -------------------------------------------------------------------------
     # halt - system halt
     # -------------------------------------------------------------------------
```

### Comparing `junos-eznc-2.7.0/lib/jnpr/junos/utils/util.py` & `junos-eznc-2.7.1/lib/jnpr/junos/utils/util.py`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/lib/junos_eznc.egg-info/PKG-INFO` & `junos-eznc-2.7.1/lib/junos_eznc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junos-eznc
-Version: 2.7.0
+Version: 2.7.1
 Summary: Junos 'EZ' automation for non-programmers
 Home-page: http://www.github.com/Juniper/py-junos-eznc
 Author: Jeremy Schulman, Nitin Kumar, Rick Sherman, Stacy Smith
 Author-email: jnpr-community-netdev@juniper.net
 License: Apache 2.0
 Keywords: Junos NETCONF networking automation
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,15 +26,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: lxml>=3.2.4
 Requires-Dist: ncclient>=0.6.15
-Requires-Dist: paramiko>=1.15.2
 Requires-Dist: scp>=0.7.0
 Requires-Dist: jinja2>=2.7.1
 Requires-Dist: PyYAML>=5.1
 Requires-Dist: six
 Requires-Dist: pyserial
 Requires-Dist: yamlordereddictloader
 Requires-Dist: pyparsing
```

### Comparing `junos-eznc-2.7.0/lib/junos_eznc.egg-info/SOURCES.txt` & `junos-eznc-2.7.1/lib/junos_eznc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `junos-eznc-2.7.0/setup.py` & `junos-eznc-2.7.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from setuptools import setup, find_packages
 import versioneer
+import os
 
+# Install customer paramiko
+os.system("pip install git+https://github.com/Juniper/paramiko.git@v3.4.0-JNPR")
 # parse requirements
 req_lines = [line.strip() for line in open("requirements.txt").readlines()]
 install_reqs = list(filter(None, req_lines))
 
 setup(
     name="junos-eznc",
     namespace_packages=["jnpr"],
```

### Comparing `junos-eznc-2.7.0/versioneer.py` & `junos-eznc-2.7.1/versioneer.py`

 * *Files identical despite different names*


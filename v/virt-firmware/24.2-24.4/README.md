# Comparing `tmp/virt-firmware-24.2.tar.gz` & `tmp/virt-firmware-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virt-firmware-24.2.tar", last modified: Thu Feb 15 22:11:22 2024, max compression
+gzip compressed data, was "virt-firmware-24.4.tar", last modified: Fri Apr 12 15:00:03 2024, max compression
```

## Comparing `virt-firmware-24.2.tar` & `virt-firmware-24.4.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.179868 virt-firmware-24.2/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    18012 2022-04-20 16:46:39.000000 virt-firmware-24.2/LICENSE
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      130 2023-09-11 14:11:19.000000 virt-firmware-24.2/MANIFEST.in
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2764 2024-02-15 22:11:22.179868 virt-firmware-24.2/PKG-INFO
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2355 2023-06-20 07:38:51.000000 virt-firmware-24.2/README.md
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.170868 virt-firmware-24.2/experimental/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)    15720 2024-02-15 21:52:27.000000 virt-firmware-24.2/experimental/addons.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3211 2024-01-10 11:20:38.000000 virt-firmware-24.2/experimental/authenticode.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1889 2023-11-24 14:17:04.000000 virt-firmware-24.2/experimental/dbxupdate.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1289 2023-11-27 16:22:48.000000 virt-firmware-24.2/experimental/fixup-partitions-for-uki.sh
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1615 2023-12-20 15:02:26.000000 virt-firmware-24.2/experimental/generate-bootcsv-for-uki.sh
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2506 2024-01-09 12:50:04.000000 virt-firmware-24.2/experimental/lscert.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     9940 2024-02-15 12:42:54.000000 virt-firmware-24.2/experimental/measure.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2781 2023-11-24 14:20:39.000000 virt-firmware-24.2/experimental/textual-boot-menu.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.172868 virt-firmware-24.2/man/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1841 2024-02-15 21:55:17.000000 virt-firmware-24.2/man/kernel-bootcfg.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2023-09-12 11:41:50.000000 virt-firmware-24.2/man/kernel-bootcfg.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      716 2024-02-15 21:55:17.000000 virt-firmware-24.2/man/pe-inspect.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2024-01-08 12:49:35.000000 virt-firmware-24.2/man/pe-inspect.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      463 2024-02-15 21:55:17.000000 virt-firmware-24.2/man/uefi-boot-menu.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2023-09-12 11:46:02.000000 virt-firmware-24.2/man/uefi-boot-menu.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      995 2024-02-15 21:55:16.000000 virt-firmware-24.2/man/virt-fw-dump.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      223 2022-10-05 11:46:37.000000 virt-firmware-24.2/man/virt-fw-dump.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      735 2024-02-15 21:55:16.000000 virt-firmware-24.2/man/virt-fw-sigdb.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2022-10-05 11:46:32.000000 virt-firmware-24.2/man/virt-fw-sigdb.inc
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4604 2024-02-15 21:55:16.000000 virt-firmware-24.2/man/virt-fw-vars.1
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      514 2024-01-08 12:49:35.000000 virt-firmware-24.2/man/virt-fw-vars.inc
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       81 2022-03-30 09:41:51.000000 virt-firmware-24.2/pyproject.toml
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1197 2024-02-15 22:11:22.179868 virt-firmware-24.2/setup.cfg
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       69 2022-03-30 09:41:51.000000 virt-firmware-24.2/setup.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.172868 virt-firmware-24.2/systemd/
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)     2474 2023-11-24 14:17:01.000000 virt-firmware-24.2/systemd/99-uki-uefi-setup.install
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      436 2023-11-24 14:17:00.000000 virt-firmware-24.2/systemd/kernel-bootcfg-boot-successful.service
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.173868 virt-firmware-24.2/tests/
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.173868 virt-firmware-24.2/tests/data/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3737 2022-11-24 12:28:42.000000 virt-firmware-24.2/tests/data/DBXUpdate-20100307.x64.bin
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1772 2022-05-11 20:36:49.000000 virt-firmware-24.2/tests/data/secboot.aws
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      106 2023-06-19 09:43:59.000000 virt-firmware-24.2/tests/test-bootcfg.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      345 2022-12-02 08:59:55.000000 virt-firmware-24.2/tests/test-dump.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      271 2023-04-14 07:25:30.000000 virt-firmware-24.2/tests/test-pe.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      185 2022-09-02 08:19:03.000000 virt-firmware-24.2/tests/test-sigdb.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      689 2022-09-02 08:10:06.000000 virt-firmware-24.2/tests/test-vars.sh
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     3711 2023-05-10 05:55:51.000000 virt-firmware-24.2/tests/tests.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.168868 virt-firmware-24.2/virt/
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.174868 virt-firmware-24.2/virt/firmware/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      141 2023-05-11 13:53:51.000000 virt-firmware-24.2/virt/firmware/__init__.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.174868 virt-firmware-24.2/virt/firmware/aws/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    11381 2022-05-11 20:36:49.000000 virt-firmware-24.2/virt/firmware/aws/dict.v0
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.174868 virt-firmware-24.2/virt/firmware/bootcfg/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       83 2023-06-19 09:21:32.000000 virt-firmware-24.2/virt/firmware/bootcfg/__init__.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6427 2024-01-10 11:43:48.000000 virt-firmware-24.2/virt/firmware/bootcfg/bootcfg.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6253 2024-01-10 11:40:59.000000 virt-firmware-24.2/virt/firmware/bootcfg/linuxcfg.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)    10084 2024-01-08 12:49:35.000000 virt-firmware-24.2/virt/firmware/bootcfg/main.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1545 2023-11-24 14:09:56.000000 virt-firmware-24.2/virt/firmware/bootcfg/menu.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.176868 virt-firmware-24.2/virt/firmware/certs/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4323 2022-07-07 16:26:41.000000 virt-firmware-24.2/virt/firmware/certs/CentOSSecureBootCA2.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4339 2022-07-07 16:26:41.000000 virt-firmware-24.2/virt/firmware/certs/CentOSSecureBootCAkey1.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6633 2024-02-15 14:27:12.000000 virt-firmware-24.2/virt/firmware/certs/MicrosoftCorporationKEK2KCA2023.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6739 2022-03-30 10:39:05.000000 virt-firmware-24.2/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6869 2022-03-30 10:39:05.000000 virt-firmware-24.2/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6599 2024-02-15 21:15:45.000000 virt-firmware-24.2/virt/firmware/certs/MicrosoftUEFICA2023.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6698 2022-03-30 10:39:05.000000 virt-firmware-24.2/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4615 2022-07-07 08:32:28.000000 virt-firmware-24.2/virt/firmware/certs/RedHatSecureBootCA3.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4431 2022-07-07 08:32:38.000000 virt-firmware-24.2/virt/firmware/certs/RedHatSecureBootCA5.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     7159 2024-01-08 13:07:34.000000 virt-firmware-24.2/virt/firmware/certs/RedHatSecureBootCA8.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4500 2022-03-30 10:39:05.000000 virt-firmware-24.2/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     7138 2024-01-08 13:07:34.000000 virt-firmware-24.2/virt/firmware/certs/RedHatUEFICA2023.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6603 2024-02-15 14:27:34.000000 virt-firmware-24.2/virt/firmware/certs/WindowsUEFICA2023.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5007 2022-07-16 16:13:52.000000 virt-firmware-24.2/virt/firmware/certs/fedoraca-20200709.pem
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    22297 2024-01-08 12:49:35.000000 virt-firmware-24.2/virt/firmware/dump.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.177868 virt-firmware-24.2/virt/firmware/efi/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      123 2023-04-28 10:54:50.000000 virt-firmware-24.2/virt/firmware/efi/__init__.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1961 2023-11-24 14:04:54.000000 virt-firmware-24.2/virt/firmware/efi/bootentry.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4419 2024-02-15 21:25:34.000000 virt-firmware-24.2/virt/firmware/efi/certs.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6196 2023-11-24 14:04:53.000000 virt-firmware-24.2/virt/firmware/efi/devpath.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1732 2023-11-24 14:04:53.000000 virt-firmware-24.2/virt/firmware/efi/efijson.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)    18645 2024-02-15 21:25:33.000000 virt-firmware-24.2/virt/firmware/efi/efivar.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5312 2023-11-24 14:04:52.000000 virt-firmware-24.2/virt/firmware/efi/guids.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6447 2024-01-02 15:59:36.000000 virt-firmware-24.2/virt/firmware/efi/siglist.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1452 2023-11-24 14:04:50.000000 virt-firmware-24.2/virt/firmware/efi/ucs16.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1529 2023-11-24 14:12:42.000000 virt-firmware-24.2/virt/firmware/host.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1758 2023-11-24 14:12:40.000000 virt-firmware-24.2/virt/firmware/migrate.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      563 2023-11-24 14:12:39.000000 virt-firmware-24.2/virt/firmware/misc.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1657 2023-11-24 14:12:39.000000 virt-firmware-24.2/virt/firmware/sigdb.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)    13830 2024-01-09 11:20:03.000000 virt-firmware-24.2/virt/firmware/vars.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.177868 virt-firmware-24.2/virt/firmware/varstore/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       90 2023-11-24 14:33:47.000000 virt-firmware-24.2/virt/firmware/varstore/__init__.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      668 2023-11-24 14:36:20.000000 virt-firmware-24.2/virt/firmware/varstore/autodetect.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5523 2023-11-24 14:09:54.000000 virt-firmware-24.2/virt/firmware/varstore/aws.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6971 2023-11-24 14:09:56.000000 virt-firmware-24.2/virt/firmware/varstore/edk2.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1350 2023-11-24 14:09:55.000000 virt-firmware-24.2/virt/firmware/varstore/jstore.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2890 2023-11-24 14:09:51.000000 virt-firmware-24.2/virt/firmware/varstore/linux.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.178868 virt-firmware-24.2/virt/peutils/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       70 2024-01-08 12:49:35.000000 virt-firmware-24.2/virt/peutils/__init__.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4977 2024-01-24 12:59:38.000000 virt-firmware-24.2/virt/peutils/pesign.py
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    12930 2024-01-10 11:20:40.000000 virt-firmware-24.2/virt/peutils/peutils.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-02-15 22:11:22.179868 virt-firmware-24.2/virt_firmware.egg-info/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2764 2024-02-15 22:11:22.000000 virt-firmware-24.2/virt_firmware.egg-info/PKG-INFO
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2569 2024-02-15 22:11:22.000000 virt-firmware-24.2/virt_firmware.egg-info/SOURCES.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)        1 2024-02-15 22:11:22.000000 virt-firmware-24.2/virt_firmware.egg-info/dependency_links.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      502 2024-02-15 22:11:22.000000 virt-firmware-24.2/virt_firmware.egg-info/entry_points.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       31 2024-02-15 22:11:22.000000 virt-firmware-24.2/virt_firmware.egg-info/requires.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       90 2024-02-15 22:11:22.000000 virt-firmware-24.2/virt_firmware.egg-info/top_level.txt
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.513210 virt-firmware-24.4/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    18012 2023-10-05 12:16:47.000000 virt-firmware-24.4/LICENSE
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      130 2023-10-05 12:16:47.000000 virt-firmware-24.4/MANIFEST.in
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2764 2024-04-12 15:00:03.513210 virt-firmware-24.4/PKG-INFO
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2355 2023-10-05 12:16:47.000000 virt-firmware-24.4/README.md
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.506210 virt-firmware-24.4/experimental/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    15720 2024-03-05 15:07:12.000000 virt-firmware-24.4/experimental/addons.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3211 2024-01-10 16:38:19.000000 virt-firmware-24.4/experimental/authenticode.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3731 2024-04-11 19:59:59.000000 virt-firmware-24.4/experimental/authfiles.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1889 2023-12-05 21:55:51.000000 virt-firmware-24.4/experimental/dbxupdate.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1289 2023-12-05 21:55:51.000000 virt-firmware-24.4/experimental/fixup-partitions-for-uki.sh
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1615 2023-12-12 20:13:59.000000 virt-firmware-24.4/experimental/generate-bootcsv-for-uki.sh
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2483 2024-04-11 19:59:59.000000 virt-firmware-24.4/experimental/lscert.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     9940 2024-03-05 15:07:12.000000 virt-firmware-24.4/experimental/measure.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2781 2023-12-05 21:55:51.000000 virt-firmware-24.4/experimental/textual-boot-menu.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.507210 virt-firmware-24.4/man/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1838 2024-04-12 14:36:19.000000 virt-firmware-24.4/man/kernel-bootcfg.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2023-10-05 12:16:47.000000 virt-firmware-24.4/man/kernel-bootcfg.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      713 2024-04-12 14:36:19.000000 virt-firmware-24.4/man/pe-inspect.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2024-01-10 16:38:19.000000 virt-firmware-24.4/man/pe-inspect.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      460 2024-04-12 14:36:19.000000 virt-firmware-24.4/man/uefi-boot-menu.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2023-10-05 12:16:47.000000 virt-firmware-24.4/man/uefi-boot-menu.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      992 2024-04-12 14:36:18.000000 virt-firmware-24.4/man/virt-fw-dump.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      223 2023-10-05 12:16:47.000000 virt-firmware-24.4/man/virt-fw-dump.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      732 2024-04-12 14:36:19.000000 virt-firmware-24.4/man/virt-fw-sigdb.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2023-10-05 12:16:47.000000 virt-firmware-24.4/man/virt-fw-sigdb.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4601 2024-04-12 14:36:18.000000 virt-firmware-24.4/man/virt-fw-vars.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      514 2024-01-10 16:38:19.000000 virt-firmware-24.4/man/virt-fw-vars.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       81 2023-10-05 12:16:47.000000 virt-firmware-24.4/pyproject.toml
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1197 2024-04-12 15:00:03.513210 virt-firmware-24.4/setup.cfg
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       69 2023-10-05 12:16:47.000000 virt-firmware-24.4/setup.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.507210 virt-firmware-24.4/systemd/
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)     3343 2024-04-11 19:59:59.000000 virt-firmware-24.4/systemd/99-uki-uefi-setup.install
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      436 2023-12-05 21:55:51.000000 virt-firmware-24.4/systemd/kernel-bootcfg-boot-successful.service
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.508210 virt-firmware-24.4/tests/
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.508210 virt-firmware-24.4/tests/data/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3737 2023-10-05 12:16:47.000000 virt-firmware-24.4/tests/data/DBXUpdate-20100307.x64.bin
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1772 2023-10-05 12:16:47.000000 virt-firmware-24.4/tests/data/secboot.aws
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      106 2023-10-05 12:16:47.000000 virt-firmware-24.4/tests/test-bootcfg.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      345 2023-10-05 12:16:47.000000 virt-firmware-24.4/tests/test-dump.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      271 2023-10-05 12:16:47.000000 virt-firmware-24.4/tests/test-pe.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      185 2023-10-05 12:16:47.000000 virt-firmware-24.4/tests/test-sigdb.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      689 2023-10-05 12:16:47.000000 virt-firmware-24.4/tests/test-vars.sh
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     5033 2024-04-12 13:34:15.000000 virt-firmware-24.4/tests/tests.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.505210 virt-firmware-24.4/virt/
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.508210 virt-firmware-24.4/virt/firmware/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      141 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/__init__.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.508210 virt-firmware-24.4/virt/firmware/aws/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    11381 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/aws/dict.v0
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.509210 virt-firmware-24.4/virt/firmware/bootcfg/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       83 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/bootcfg/__init__.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6755 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/firmware/bootcfg/bootcfg.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6767 2024-04-12 13:34:15.000000 virt-firmware-24.4/virt/firmware/bootcfg/linuxcfg.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    12188 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/firmware/bootcfg/main.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1545 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/bootcfg/menu.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.512210 virt-firmware-24.4/virt/firmware/certs/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4323 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/CentOSSecureBootCA2.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4339 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/CentOSSecureBootCAkey1.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6633 2024-03-05 15:07:12.000000 virt-firmware-24.4/virt/firmware/certs/MicrosoftCorporationKEK2KCA2023.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6739 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6869 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6599 2024-03-05 15:07:12.000000 virt-firmware-24.4/virt/firmware/certs/MicrosoftUEFICA2023.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6698 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4615 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/RedHatSecureBootCA3.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4431 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/RedHatSecureBootCA5.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     7159 2024-01-10 16:38:19.000000 virt-firmware-24.4/virt/firmware/certs/RedHatSecureBootCA8.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4500 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     5773 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/firmware/certs/RedHatUEFICA2024.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6603 2024-03-05 15:07:12.000000 virt-firmware-24.4/virt/firmware/certs/WindowsUEFICA2023.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     5007 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/certs/fedoraca-20200709.pem
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    22297 2024-01-10 16:38:19.000000 virt-firmware-24.4/virt/firmware/dump.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.512210 virt-firmware-24.4/virt/firmware/efi/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      123 2023-10-05 12:16:47.000000 virt-firmware-24.4/virt/firmware/efi/__init__.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1961 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/efi/bootentry.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4419 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/firmware/efi/certs.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6196 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/efi/devpath.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1732 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/efi/efijson.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    18845 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/firmware/efi/efivar.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     5312 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/efi/guids.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6447 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/efi/siglist.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1452 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/efi/ucs16.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1529 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/host.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1758 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/migrate.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      563 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/misc.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2095 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/firmware/sigdb.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    14208 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/firmware/vars.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.512210 virt-firmware-24.4/virt/firmware/varstore/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       90 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/varstore/__init__.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      668 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/firmware/varstore/autodetect.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     5523 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/varstore/aws.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6971 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/varstore/edk2.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1350 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/varstore/jstore.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2890 2023-12-05 21:55:51.000000 virt-firmware-24.4/virt/firmware/varstore/linux.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.512210 virt-firmware-24.4/virt/peutils/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       82 2024-04-12 13:34:15.000000 virt-firmware-24.4/virt/peutils/__init__.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1877 2024-04-12 13:34:15.000000 virt-firmware-24.4/virt/peutils/pedecode.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     5148 2024-04-11 19:59:59.000000 virt-firmware-24.4/virt/peutils/pesign.py
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    11971 2024-04-12 13:34:15.000000 virt-firmware-24.4/virt/peutils/peutils.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2024-04-12 15:00:03.513210 virt-firmware-24.4/virt_firmware.egg-info/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2764 2024-04-12 15:00:03.000000 virt-firmware-24.4/virt_firmware.egg-info/PKG-INFO
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2620 2024-04-12 15:00:03.000000 virt-firmware-24.4/virt_firmware.egg-info/SOURCES.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)        1 2024-04-12 15:00:03.000000 virt-firmware-24.4/virt_firmware.egg-info/dependency_links.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      502 2024-04-12 15:00:03.000000 virt-firmware-24.4/virt_firmware.egg-info/entry_points.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       31 2024-04-12 15:00:03.000000 virt-firmware-24.4/virt_firmware.egg-info/requires.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       90 2024-04-12 15:00:03.000000 virt-firmware-24.4/virt_firmware.egg-info/top_level.txt
```

### Comparing `virt-firmware-24.2/LICENSE` & `virt-firmware-24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/PKG-INFO` & `virt-firmware-24.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virt-firmware
-Version: 24.2
+Version: 24.4
 Summary: tools for virtual machine firmware volumes
 Author: Gerd Hoffmann
 Author-email: kraxel@redhat.com
 License: GPLv2
 Project-URL: GitLab, https://gitlab.com/kraxel/virt-firmware
 Keywords: ovmf,armvirt,edk2,aws
 Description-Content-Type: text/markdown
```

### Comparing `virt-firmware-24.2/README.md` & `virt-firmware-24.4/README.md`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/experimental/addons.py` & `virt-firmware-24.4/experimental/addons.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/experimental/authenticode.py` & `virt-firmware-24.4/experimental/authenticode.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/experimental/dbxupdate.py` & `virt-firmware-24.4/experimental/dbxupdate.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/experimental/fixup-partitions-for-uki.sh` & `virt-firmware-24.4/experimental/fixup-partitions-for-uki.sh`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/experimental/generate-bootcsv-for-uki.sh` & `virt-firmware-24.4/experimental/generate-bootcsv-for-uki.sh`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/experimental/lscert.py` & `virt-firmware-24.4/experimental/lscert.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 def ls_files(flist, verbose, basename = False):
     plen = 0
     for filename in flist:
         pname = filename
         if basename:
             pname = '  ' + os.path.basename(pname)
-        if plen < len(pname):
-            plen = len(pname)
+        plen = max(plen, len(pname))
 
     for filename in flist:
         # read filename
         with open(filename, 'rb') as f:
             blob = f.read()
         if b'-----BEGIN' in blob:
             cert = x509.load_pem_x509_certificate(blob, default_backend())
```

### Comparing `virt-firmware-24.2/experimental/measure.py` & `virt-firmware-24.4/experimental/measure.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/experimental/textual-boot-menu.py` & `virt-firmware-24.4/experimental/textual-boot-menu.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/man/kernel-bootcfg.1` & `virt-firmware-24.4/man/kernel-bootcfg.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.49.3.
-.TH KERNEL-BOOTCFG "1" "February 2024" "kernel-bootcfg 24.2" "User Commands"
+.TH KERNEL-BOOTCFG "1" "April 2024" "kernel-bootcfg 24.4" "User Commands"
 .SH NAME
-kernel-bootcfg \- manual page for kernel-bootcfg 24.2
+kernel-bootcfg \- manual page for kernel-bootcfg 24.4
 .SH DESCRIPTION
 usage: kernel\-bootcfg [\-h] [\-l LEVEL] [\-\-vars FILE] [\-\-show] [\-v]
 .TP
 [\-\-add\-uki FILE] [\-\-update\-uki FILE] [\-\-remove\-uki FILE]
 [\-\-boot\-ok] [\-\-update\-csv] [\-\-add\-uri URI]
 [\-\-remove\-entry NNNN] [\-\-once] [\-\-boot\-order POS]
 [\-\-dry\-run] [\-\-title TITLE] [\-\-shim FILE]
```

### Comparing `virt-firmware-24.2/man/pe-inspect.1` & `virt-firmware-24.4/man/pe-inspect.1`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.49.3.
-.TH PE-INSPECT "1" "February 2024" "pe-inspect 24.2" "User Commands"
+.TH PE-INSPECT "1" "April 2024" "pe-inspect 24.4" "User Commands"
 .SH NAME
-pe-inspect \- manual page for pe-inspect 24.2
+pe-inspect \- manual page for pe-inspect 24.4
 .SH DESCRIPTION
 usage: pe\-inspect [\-h] [\-x] [\-v] [\-\-findcert] [FILES ...]
 .PP
 Print informations about PE/EFI binaries.
 .SS "positional arguments:"
 .TP
 FILES
```

### Comparing `virt-firmware-24.2/man/virt-fw-dump.1` & `virt-firmware-24.4/man/virt-fw-dump.1`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.49.3.
-.TH VIRT-FW-DUMP "1" "February 2024" "virt-fw-dump 24.2" "User Commands"
+.TH VIRT-FW-DUMP "1" "April 2024" "virt-fw-dump 24.4" "User Commands"
 .SH NAME
-virt-fw-dump \- manual page for virt-fw-dump 24.2
+virt-fw-dump \- manual page for virt-fw-dump 24.4
 .SH DESCRIPTION
 
 The virt-fw-dump utility prints the structure and content of edk2
 firmware volumes to stdout.
 .PP
 usage: virt\-fw\-dump [\-h] [\-i FILE] [\-\-all] [\-\-volumes] [\-\-modules]
 .IP
```

### Comparing `virt-firmware-24.2/man/virt-fw-sigdb.1` & `virt-firmware-24.4/man/virt-fw-sigdb.1`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.49.3.
-.TH VIRT-FW-SIGDB "1" "February 2024" "virt-fw-sigdb 24.2" "User Commands"
+.TH VIRT-FW-SIGDB "1" "April 2024" "virt-fw-sigdb 24.4" "User Commands"
 .SH NAME
-virt-fw-sigdb \- manual page for virt-fw-sigdb 24.2
+virt-fw-sigdb \- manual page for virt-fw-sigdb 24.4
 .SH DESCRIPTION
 usage: virt\-fw\-sigdb [\-h] [\-i FILE] [\-o FILE] [\-\-add\-cert GUID FILE] [\-p]
 .SS "options:"
 .TP
 \fB\-h\fR, \fB\-\-help\fR
 show this help message and exit
 .TP
```

### Comparing `virt-firmware-24.2/man/virt-fw-vars.1` & `virt-firmware-24.4/man/virt-fw-vars.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.49.3.
-.TH VIRT-FW-VARS "1" "February 2024" "virt-fw-vars 24.2" "User Commands"
+.TH VIRT-FW-VARS "1" "April 2024" "virt-fw-vars 24.4" "User Commands"
 .SH NAME
-virt-fw-vars \- manual page for virt-fw-vars 24.2
+virt-fw-vars \- manual page for virt-fw-vars 24.4
 .SH DESCRIPTION
 
 The virt-fw-vars utility can print and modify UEFI variable stores.
 Supported formats are standard edk2 (as used by ovmf and armvirt) and
 aws.
 .PP
 usage: virt\-fw\-vars [\-h] [\-l LEVEL] [\-i FILE] [\-\-inplace FILE]
```

### Comparing `virt-firmware-24.2/man/virt-fw-vars.inc` & `virt-firmware-24.4/man/virt-fw-vars.inc`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/setup.cfg` & `virt-firmware-24.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = virt-firmware
-version = 24.2
+version = 24.4
 description = tools for virtual machine firmware volumes
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ovmf, armvirt, edk2, aws
 license = GPLv2
 license_files = LICENSE
 author = Gerd Hoffmann
```

### Comparing `virt-firmware-24.2/systemd/99-uki-uefi-setup.install` & `virt-firmware-24.4/systemd/99-uki-uefi-setup.install`

 * *Files 27% similar despite different names*

```diff
@@ -64,17 +64,36 @@
             mv "$UKI_FILE_BOOT" "$UKI_FILE_ESP" || {
                 echo "Error: could not move '$UKI_FILE_BOOT' to '$UKI_FILE_ESP'." >&2
 	        exit 1
             }
             sync
         fi
 
-        [ "$KERNEL_INSTALL_VERBOSE" -gt 0 ] && \
-            echo "Adding $UKI_FILE_ESP to UEFI boot entries"
-        kernel-bootcfg $LOGLEVEL --add-uki "$UKI_FILE_ESP" --title "$KERNEL_VERSION" --once
+        # Adapted from systemd's 90-loadentry.install
+        if [ -n "$KERNEL_INSTALL_CONF_ROOT" ]; then
+            if [ -f "$KERNEL_INSTALL_CONF_ROOT/cmdline" ]; then
+                CMDLINE="$(tr -s "$IFS" ' ' <"$KERNEL_INSTALL_CONF_ROOT/cmdline")"
+            fi
+        elif [ -f /etc/kernel/cmdline ]; then
+            CMDLINE="$(tr -s "$IFS" ' ' </etc/kernel/cmdline)"
+        elif [ -f /usr/lib/kernel/cmdline ]; then
+            CMDLINE="$(tr -s "$IFS" ' ' </usr/lib/kernel/cmdline)"
+        else
+            CMDLINE=
+        fi
+
+        if [ -n "$CMDLINE" ]; then
+            [ "$KERNEL_INSTALL_VERBOSE" -gt 0 ] && \
+                echo "Adding $UKI_FILE_ESP to UEFI boot entries with cmdline: $CMDLINE"
+            kernel-bootcfg $LOGLEVEL --add-uki "$UKI_FILE_ESP" --title "$KERNEL_VERSION" --cmdline "$CMDLINE" --once
+        else
+            [ "$KERNEL_INSTALL_VERBOSE" -gt 0 ] && \
+                echo "Adding $UKI_FILE_ESP to UEFI boot entries"
+            kernel-bootcfg $LOGLEVEL --add-uki "$UKI_FILE_ESP" --title "$KERNEL_VERSION" --once
+        fi
         ;;
     *)
         exit 0
         ;;
 esac
 
 exit 0
```

### Comparing `virt-firmware-24.2/tests/data/DBXUpdate-20100307.x64.bin` & `virt-firmware-24.4/tests/data/DBXUpdate-20100307.x64.bin`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/tests/data/secboot.aws` & `virt-firmware-24.4/tests/data/secboot.aws`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/tests/test-vars.sh` & `virt-firmware-24.4/tests/test-vars.sh`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/tests/tests.py` & `virt-firmware-24.4/tests/tests.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 import os
 import json
+import argparse
 import unittest
+import subprocess
 
 from virt.firmware.efi import certs
 from virt.firmware.efi import efivar
 from virt.firmware.efi import efijson
 from virt.firmware.efi import devpath
 
 from virt.firmware.varstore import edk2
 from virt.firmware.varstore import linux
 from virt.firmware.varstore import aws
 
+from virt.firmware.bootcfg import linuxcfg
+from virt.firmware.bootcfg import main as bcfgmain
+
 VARS_EMPTY   = "/usr/share/OVMF/OVMF_VARS.fd"
 VARS_SECBOOT = "/usr/share/OVMF/OVMF_VARS.secboot.fd"
 
 TEST_DATA    = os.path.join(os.path.dirname(__file__), "data")
 TEST_AWS     = os.path.join(TEST_DATA, 'secboot.aws')
 TEST_DBX     = os.path.join(TEST_DATA, 'DBXUpdate-20100307.x64.bin')
 
+cache_detect_container = None
+
+def detect_container():
+    global cache_detect_container
+    if cache_detect_container is None:
+        result = subprocess.run([ 'systemd-detect-virt', '--container', '--quiet' ])
+        if result.returncode == 0:
+            cache_detect_container = True
+        else:
+            cache_detect_container = False
+    return cache_detect_container
+
 class TestsEdk2(unittest.TestCase):
 
     @unittest.skipUnless(os.path.exists(VARS_EMPTY), 'no empty vars file')
     def test_probe_edk2_good(self):
         self.assertTrue(edk2.Edk2VarStore.probe(VARS_EMPTY))
 
     def test_probe_edk2_bad(self):
@@ -96,9 +113,27 @@
         with open(TEST_DBX, 'rb') as f:
             blob = f.read()
         dbx = efivar.EfiVar('dbx', authdata = blob)
 
     def test_generate_pk(self):
         certs.pk_generate()
 
+    @unittest.skipIf(detect_container(), 'in container')
+    @unittest.skipUnless(os.path.exists('/sys/firmware/efi/efivars'), 'no efivars fs')
+    def test_add_uki(self):
+        info = linuxcfg.LinuxOsInfo()
+        esp  = info.esp_path()
+        if esp is None:
+            return
+        shim = info.shim_path()
+        cfg  = linuxcfg.LinuxEfiBootConfig()
+        options = argparse.Namespace(shim      = shim,
+                                     title     = 'test',
+                                     adduki    = f'{esp}/EFI/Linux/test.eki',
+                                     cmdline   = None,
+                                     bootnext  = True,
+                                     bootorder = None,
+                                     dryrun    = True)
+        bcfgmain.add_uki(cfg, options)
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `virt-firmware-24.2/virt/firmware/aws/dict.v0` & `virt-firmware-24.4/virt/firmware/aws/dict.v0`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/bootcfg/bootcfg.py` & `virt-firmware-24.4/virt/firmware/bootcfg/bootcfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from virt.firmware.varstore import autodetect
 
 class EfiBootConfig:
     """ efi boot configuration """
 
     def __init__(self):
+        self.secureboot  = False
         self.bootorder   = None
         self.bootcurrent = None
         self.bootnext    = None
         self.bcurr = None  # parsed BootCurrent
         self.bnext = None  # parsed BootNext
         self.blist = []    # parsed BootOrder
         self.unused = []   # unused BootNNNN entry list
@@ -96,30 +97,36 @@
         for nr in self.unused:
             self.print_entry(nr, verbose)
 
     def find_uki_entry(self, uki):
         for (nr, entry) in self.bentr.items():
             if not entry or not entry.optdata:
                 continue
-            optpath = str(ucs16.from_ucs16(entry.optdata, 0)).strip()
-            if optpath == str(uki):
-                return nr
+            try:
+                optpath = str(ucs16.from_ucs16(entry.optdata, 0)).split()[0]
+            except (UnicodeDecodeError, IndexError):
+                continue
+            else:
+                if optpath == str(uki):
+                    return nr
         return None
 
     def find_title_entry(self, title):
         for (nr, entry) in self.bentr.items():
             if not entry:
                 continue
             if str(entry.title) == str(title):
                 return nr
         return None
 
     def find_devpath_entry(self, devicepath):
         blob = bytes(devicepath)
         for (nr, entry) in self.bentr.items():
+            if not entry:
+                continue
             if blob == bytes(entry.devicepath):
                 return nr
         return None
 
     def find_unused_entry(self):
         nr = 0
         while nr in self.bentr:
@@ -182,7 +189,11 @@
         self.bootnext = self.varlist.get('BootNext')
         self.parse_boot_variables()
         self.add_unused_entries(self.varlist.keys())
         for nr in self.bentr.keys():
             var = self.varlist.get(f'Boot{nr:04X}')
             if var:
                 self.bentr[nr] = bootentry.BootEntry(data = var.data)
+
+        sb = self.varlist.get('SecureBootEnable')
+        if sb and sb.data[0]:
+            self.secureboot = True
```

### Comparing `virt-firmware-24.2/virt/firmware/bootcfg/linuxcfg.py` & `virt-firmware-24.4/virt/firmware/bootcfg/linuxcfg.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         self.parse_boot_variables()
         self.add_unused_entries(self.varstore.scan.get(guids.EfiGlobalVariable))
         for nr in self.bentr.keys():
             var = self.linux_read_variable(f'Boot{nr:04X}')
             if var:
                 self.bentr[nr] = bootentry.BootEntry(data = var.data)
 
+        sb = self.linux_read_variable('SecureBoot')
+        if sb and sb.data[0]:
+            self.secureboot = True
 
 class LinuxEfiFile:
     """ class representing a file on a linux file system which we want reference in efi """
 
     def __init__(self, filename):
         self.udevenv = {}
         self.filename = os.path.abspath(filename)
@@ -174,17 +177,24 @@
 
     def efi_arch(self):
         arch = os.uname().machine
         return self.efi_arch_map.get(arch)
 
     def esp_path(self):
         if not self.esp:
-            result = subprocess.run([ 'bootctl', '--print-esp-path' ],
-                                    stdout = subprocess.PIPE, check = True)
-            self.esp = result.stdout.decode().strip('\n')
+            try:
+                result = subprocess.run([ 'bootctl', '--print-esp-path' ],
+                                        stdout = subprocess.PIPE, check = True)
+            except (FileNotFoundError, subprocess.CalledProcessError):
+                # If bootctl is not installed find the EFI directory at the usual mount points
+                for candidate in '/efi', '/boot/efi', '/boot/EFI', '/boot':
+                    if os.path.isdir(candidate + '/EFI/BOOT'):
+                        self.esp = candidate
+            else:
+                self.esp = result.stdout.decode().strip('\n')
         return self.esp
 
     def shim_path(self):
         esp    = self.esp_path()
         subdir = self.esp_distro_dir()
         arch   = self.efi_arch()
         shim   = f'{esp}/EFI/{subdir}/shim{arch}.efi'
```

### Comparing `virt-firmware-24.2/virt/firmware/bootcfg/main.py` & `virt-firmware-24.4/virt/firmware/bootcfg/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 #
 """ experimental efi boot config tool """
 import os
 import sys
 import logging
 import argparse
 
+import pefile
+
 from virt.firmware.efi import ucs16
+from virt.firmware.efi import guids
 from virt.firmware.efi import devpath
 from virt.firmware.efi import bootentry
 
 from virt.firmware.bootcfg import bootcfg
 from virt.firmware.bootcfg import linuxcfg
 
+from virt.peutils import pesign
+
 
 ########################################################################
 # main
 
 def update_next_or_order(cfg, options, nr):
     if options.bootnext:
         cfg.set_boot_next(nr)
@@ -28,73 +33,116 @@
 
     if options.bootorder is not None:
         cfg.set_boot_order(nr, options.bootorder)
         if not options.dryrun:
             cfg.linux_update_order()
 
 
+def firmware_loads_efi_binary(cfg, efibinary):
+    if not cfg.secureboot:
+        return True
+    if pesign.cryptography_major < 40:
+        # can't use pesign.pe_check_cert() -> play safe
+        return False
+    db = cfg.varstore.get_variable('db', guids.EfiImageSecurityDatabase)
+    pe = pefile.PE(efibinary)
+    siglist = pesign.pe_type2_signatures(pe)
+    if pesign.pe_check_cert(siglist, db):
+        return True
+    return False
+
+
+def create_boot_entry(efiuki, options):
+    if options.shim:
+        efishim = linuxcfg.LinuxEfiFile(options.shim)
+        if efishim.device != efiuki.device:
+            logging.error('shim and uki are on different filesystems')
+            sys.exit(1)
+        if options.cmdline:
+            optdata = ucs16.from_string(efiuki.efi_filename() + ' ' + options.cmdline)
+        else:
+            optdata = ucs16.from_string(efiuki.efi_filename())
+        entry = bootentry.BootEntry(title = ucs16.from_string(options.title),
+                                    attr = bootentry.LOAD_OPTION_ACTIVE,
+                                    devicepath = efishim.dev_path_file(),
+                                    optdata = bytes(optdata))
+    else:
+        if options.cmdline:
+            optdata = ucs16.from_string(options.cmdline)
+            entry = bootentry.BootEntry(title = ucs16.from_string(options.title),
+                                        attr = bootentry.LOAD_OPTION_ACTIVE,
+                                        devicepath = efiuki.dev_path_file(),
+                                        optdata = bytes(optdata))
+        else:
+            entry = bootentry.BootEntry(title = ucs16.from_string(options.title),
+                                        attr = bootentry.LOAD_OPTION_ACTIVE,
+                                        devicepath = efiuki.dev_path_file())
+    return entry
+
+
 def add_uki(cfg, options):
-    if not options.shim:
-        logging.error('shim binary not specified')
+    if not options.shim and not firmware_loads_efi_binary(cfg, options.adduki):
+        logging.error('shim binary needed but not found or specified')
         sys.exit(1)
     if not options.title:
         logging.error('entry title not specified')
         sys.exit(1)
+    if options.cmdline and cfg.secureboot:
+        logging.warning('Overriding built-in UKI cmdline is not possible'
+                        ' when Secure Boot is enabled')
 
     efiuki = linuxcfg.LinuxEfiFile(options.adduki)
     nr = cfg.find_uki_entry(efiuki.efi_filename())
+    if nr is None:
+        nr = cfg.find_devpath_entry(efiuki.dev_path_file())
     if nr is not None:
         logging.info('Entry exists (Boot%04X)', nr)
     else:
-        efishim = linuxcfg.LinuxEfiFile(options.shim)
-        if efishim.device != efiuki.device:
-            logging.error('shim and uki are on different filesystems')
-            sys.exit(1)
-        optdata = ucs16.from_string(efiuki.efi_filename())
-        entry = bootentry.BootEntry(title = ucs16.from_string(options.title),
-                                    attr = bootentry.LOAD_OPTION_ACTIVE,
-                                    devicepath = efishim.dev_path_file(),
-                                    optdata = bytes(optdata))
+        entry = create_boot_entry(efiuki, options)
         logging.info('Create new entry: %s', str(entry))
         nr = cfg.add_entry(entry)
         logging.info('Added entry (Boot%04X)', nr)
         if not options.dryrun:
             cfg.linux_write_entry(nr)
 
     update_next_or_order(cfg, options, nr)
 
 
 def update_uki(cfg, options):
     efiuki = linuxcfg.LinuxEfiFile(options.updateuki)
     nr = cfg.find_uki_entry(efiuki.efi_filename())
     if nr is None:
+        nr = cfg.find_devpath_entry(efiuki.dev_path_file())
+    if nr is None:
         logging.error('No entry found for %s', options.updateuki)
         sys.exit(1)
 
     update_next_or_order(cfg, options, nr)
 
 
 def remove_uki(cfg, options):
     efiuki = linuxcfg.LinuxEfiFile(options.removeuki)
     nr = cfg.find_uki_entry(efiuki.efi_filename())
     if nr is None:
+        nr = cfg.find_devpath_entry(efiuki.dev_path_file())
+    if nr is None:
         logging.warning('No entry found for %s', options.removeuki)
         return
 
     logging.info('Removing entry (Boot%04X)', nr)
     cfg.remove_entry(nr)
     if not options.dryrun:
         cfg.linux_remove_entry(nr)
         cfg.linux_update_next()
         cfg.linux_update_order()
 
 
 def boot_success(cfg, options):
-    if cfg.bcurr == cfg.blist[0]:
-        logging.info('No update needed, BootCurrent already comes first in BootOrder.')
+    if cfg.bcurr in cfg.blist:
+        logging.info('No update needed, BootCurrent is already in BootOrder.')
         return
     logging.info('Add BootCurrent (Boot%04X) to BootOrder', cfg.bcurr)
     cfg.set_boot_order(cfg.bcurr, 0)
     if not options.dryrun:
         cfg.linux_update_order()
 
 
@@ -181,18 +229,20 @@
     group = parser.add_argument_group('update unified kernel image (UKI) boot entries')
     group.add_argument('--add-uki', dest = 'adduki', type = str,
                        help = 'add boot entry for UKI image FILE', metavar = 'FILE')
     group.add_argument('--update-uki', dest = 'updateuki', type = str,
                        help = 'update boot entry for UKI image FILE', metavar = 'FILE')
     group.add_argument('--remove-uki', dest = 'removeuki', type = str,
                        help = 'remove boot entry for UKI image FILE', metavar = 'FILE')
+    group.add_argument('--cmdline', dest = 'cmdline', type = str,
+                       help = 'override UKIs cmdline when adding boot entry '
+                       '(ignored when Secure Boot is enabled)', metavar = 'CMDLINE')
     group.add_argument('--boot-ok', '--boot-successful', dest = 'bootok',
                        action = 'store_true', default = False,
-                       help = 'boot is successful, update BootOrder to have '
-                       'current entry listed first.')
+                       help = 'boot is successful, add BootCurrent to BootOrder.')
     group.add_argument('--update-csv', dest = 'updatecsv',
                        action = 'store_true', default = False,
                        help = 'update BOOT.CSV')
 
     group = parser.add_argument_group('update other boot entries')
     group.add_argument('--add-uri', dest = 'adduri', type = str,
                        help = 'add boot entry to netboot URI', metavar = 'URI')
@@ -247,15 +297,15 @@
         add_uki(cfg, options)
     elif options.updateuki:
         update_uki(cfg, options)
     elif options.removeuki:
         remove_uki(cfg, options)
     elif options.bootok:
         boot_success(cfg, options)
-        if options.updatecsv:
+        if options.updatecsv and options.shim:
             update_boot_csv(cfg, options)
     elif options.updatecsv:
         update_boot_csv(cfg, options)
     elif options.adduri:
         add_uri(cfg, options)
     elif options.removeentry:
         remove_entry(cfg, options)
```

### Comparing `virt-firmware-24.2/virt/firmware/bootcfg/menu.py` & `virt-firmware-24.4/virt/firmware/bootcfg/menu.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/CentOSSecureBootCA2.pem` & `virt-firmware-24.4/virt/firmware/certs/CentOSSecureBootCA2.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/CentOSSecureBootCAkey1.pem` & `virt-firmware-24.4/virt/firmware/certs/CentOSSecureBootCAkey1.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/MicrosoftCorporationKEK2KCA2023.pem` & `virt-firmware-24.4/virt/firmware/certs/MicrosoftCorporationKEK2KCA2023.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem` & `virt-firmware-24.4/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem` & `virt-firmware-24.4/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/MicrosoftUEFICA2023.pem` & `virt-firmware-24.4/virt/firmware/certs/MicrosoftUEFICA2023.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem` & `virt-firmware-24.4/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/RedHatSecureBootCA3.pem` & `virt-firmware-24.4/virt/firmware/certs/RedHatSecureBootCA3.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/RedHatSecureBootCA5.pem` & `virt-firmware-24.4/virt/firmware/certs/RedHatSecureBootCA5.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/RedHatSecureBootCA8.pem` & `virt-firmware-24.4/virt/firmware/certs/RedHatSecureBootCA8.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem` & `virt-firmware-24.4/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/RedHatUEFICA2023.pem` & `virt-firmware-24.4/virt/firmware/certs/RedHatUEFICA2024.pem`

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,101 @@
 Certificate:
     Data:
         Version: 3 (0x2)
         Serial Number:
-            d3:30:64:a8:bd:a7:c8:02
+            ab:52:70:0c:fe:6a:54:27
         Signature Algorithm: sha256WithRSAEncryption
-        Issuer: CN = Red Hat UEFI CA 2023, emailAddress = secalert@redhat.com
+        Issuer: CN = Red Hat UEFI CA 2024, emailAddress = secalert@redhat.com
         Validity
-            Not Before: Nov 30 20:11:15 2023 GMT
-            Not After : Jan 18 20:11:15 2038 GMT
-        Subject: CN = Red Hat UEFI CA 2023, emailAddress = secalert@redhat.com
+            Not Before: Mar 27 19:08:30 2024 GMT
+            Not After : Jan 18 19:08:30 2038 GMT
+        Subject: CN = Red Hat UEFI CA 2024, emailAddress = secalert@redhat.com
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
-                Public-Key: (4096 bit)
+                Public-Key: (3072 bit)
                 Modulus:
-                    00:aa:d1:f4:47:16:a6:95:35:ba:87:ae:4c:95:13:
-                    4e:d0:8a:92:2a:57:c9:a1:89:f9:20:ae:99:a8:5c:
-                    f1:75:89:5f:de:f6:c7:98:13:90:28:8f:24:e0:a6:
-                    40:9b:4d:68:1d:73:49:26:8e:97:81:1f:1c:30:ea:
-                    3a:e1:af:e5:4e:76:ac:0b:26:3c:8e:94:8c:51:8f:
-                    c2:a1:c4:28:45:b6:3c:0e:6d:d9:a5:22:00:07:49:
-                    43:a2:6e:ca:0a:ee:90:a1:89:9a:81:f7:55:7a:d1:
-                    fa:6a:34:c2:59:64:3f:8d:32:1d:5b:59:51:d7:16:
-                    cb:87:1b:7f:07:c1:d8:8d:c5:e1:15:f3:d7:9f:06:
-                    3b:2e:42:9c:81:77:07:8f:5d:a1:70:b6:70:9c:04:
-                    89:f6:cc:3e:0d:77:31:8a:57:29:b8:b7:ef:26:59:
-                    bf:a4:0b:2e:2a:f1:7c:a1:20:ec:06:62:41:20:2c:
-                    69:32:d9:10:6a:ca:93:67:d5:b1:6b:52:21:58:61:
-                    d1:09:87:ad:37:50:f3:12:9d:4c:bf:1b:17:16:85:
-                    48:49:12:bf:b9:f3:ed:b9:60:15:2a:ca:b7:21:24:
-                    85:6d:58:02:41:6f:53:6a:04:fe:25:10:44:81:fa:
-                    44:d2:9d:8b:53:32:1e:45:37:5f:1a:31:e7:f7:a2:
-                    4d:cb:40:b9:42:12:f4:fd:67:30:08:ff:83:2c:f8:
-                    a2:0d:f8:ef:93:80:81:8a:f0:b1:20:35:16:4e:03:
-                    5a:b4:f1:a8:9f:08:f0:73:c0:dc:be:4f:a8:29:32:
-                    8a:cc:2a:c3:38:a1:00:cd:1a:95:78:31:14:01:25:
-                    4d:cb:f8:35:ca:4b:21:27:15:57:d2:24:fc:f1:24:
-                    9a:23:5b:41:72:7b:8d:d0:8c:89:18:9f:e8:1b:3e:
-                    ed:ef:6f:63:d3:0b:a2:bd:f4:f9:5e:22:19:be:5b:
-                    9d:1e:87:e4:4e:c2:43:58:b9:87:06:7f:e2:26:aa:
-                    1b:6a:12:b3:a7:c5:28:22:0d:c5:40:18:a8:80:4c:
-                    8b:ad:2a:56:86:0a:bb:f3:6b:e9:70:a0:f5:0b:e8:
-                    e9:d7:de:30:02:4f:3c:64:b8:7c:04:1c:91:b3:04:
-                    0d:58:3d:5a:ea:31:d0:5d:e0:92:a2:0c:20:81:77:
-                    8d:6a:70:ef:ca:5b:81:61:4f:7b:ee:01:b5:88:0d:
-                    6d:5e:da:b8:bb:64:fb:6b:ab:49:fe:52:51:03:b4:
-                    72:ef:c5:e0:bc:a1:12:5d:5b:0f:ab:c2:b8:56:c5:
-                    85:33:d2:9d:3b:74:a8:8e:af:b6:9a:57:7e:11:e9:
-                    1d:86:ff:15:d6:13:8f:7f:05:7f:94:e2:60:50:c2:
-                    fe:6f:11
+                    00:bd:5a:13:26:02:60:6d:6e:6d:ca:15:be:56:f5:
+                    b7:a8:e9:3e:d2:b9:49:ae:86:76:e6:84:fb:59:95:
+                    80:20:70:6f:34:54:4d:d1:cc:2d:66:ec:04:f3:bd:
+                    9d:ca:cc:2f:cb:be:c6:c5:3b:9f:8f:cf:e2:27:59:
+                    7e:64:c7:ab:0f:aa:93:e4:21:e7:5c:67:c2:18:c1:
+                    75:b0:c8:fe:5a:83:af:bd:c2:87:cc:48:27:df:55:
+                    4b:91:fc:15:48:76:2c:6d:f7:a1:e6:99:40:35:71:
+                    81:59:9d:75:35:72:04:f6:2c:e1:1c:77:e5:17:a1:
+                    99:48:f7:16:50:6a:4f:48:21:18:c6:93:1a:0f:75:
+                    28:3e:cd:64:eb:66:36:1a:7b:99:0a:21:f0:1d:64:
+                    2e:ce:76:60:af:78:7e:7e:80:f7:fe:43:1f:fc:c3:
+                    6d:ec:2d:2f:19:72:e9:ad:5e:09:c6:04:99:63:5b:
+                    8b:c2:5b:a9:0c:69:f2:8f:a1:71:dd:f9:d2:fc:b2:
+                    29:52:80:fb:d7:df:10:37:fa:84:61:45:dd:f4:f3:
+                    34:ec:5d:63:ad:7b:a7:d1:44:cc:d8:db:6a:19:77:
+                    97:4e:9a:dc:70:0c:dd:a1:66:b5:84:5c:cb:02:23:
+                    51:92:9f:b5:73:fb:a4:94:39:cd:c9:d4:93:f8:c3:
+                    d2:84:14:f9:dd:d3:89:f1:27:af:0b:3d:7a:9c:b7:
+                    61:19:7f:b7:57:8c:08:33:ea:da:31:7f:ff:d2:09:
+                    e6:46:d3:93:fe:2b:56:62:b4:d5:18:9d:6f:dc:ca:
+                    93:bc:4d:8b:05:d8:5c:9b:ea:91:e3:d8:60:f6:bb:
+                    ef:28:f3:5f:8a:55:e8:55:70:88:93:1b:7b:d3:40:
+                    ef:42:c3:0f:8b:a0:d5:76:eb:12:ae:1b:68:cc:e1:
+                    e9:f6:1b:b5:a1:f6:5c:5b:66:19:f8:10:29:35:3b:
+                    b2:62:17:b0:80:04:2a:d0:95:7e:fd:d3:ac:0d:28:
+                    b2:58:20:f0:74:08:d4:d2:e1:95
                 Exponent: 65537 (0x10001)
         X509v3 extensions:
             X509v3 Basic Constraints: critical
                 CA:TRUE
             X509v3 Subject Key Identifier: 
-                87:D5:37:58:18:CE:19:48:BB:A4:4F:CB:18:2A:F8:8F:80:D1:6E:69
+                0E:C0:7D:62:68:FE:35:9C:E2:27:E2:41:68:AF:0E:DE:0C:7A:7A:C3
             X509v3 Authority Key Identifier: 
-                87:D5:37:58:18:CE:19:48:BB:A4:4F:CB:18:2A:F8:8F:80:D1:6E:69
+                0E:C0:7D:62:68:FE:35:9C:E2:27:E2:41:68:AF:0E:DE:0C:7A:7A:C3
             X509v3 Key Usage: critical
                 Digital Signature, Certificate Sign, CRL Sign
     Signature Algorithm: sha256WithRSAEncryption
     Signature Value:
-        75:12:72:8a:5a:a4:6d:c2:55:4c:02:79:4f:1c:73:c5:b1:80:
-        48:db:21:84:70:d1:03:cb:a5:93:7e:da:76:c5:c0:52:a2:8b:
-        91:7b:88:3a:02:33:d8:77:d8:a7:7b:31:12:a3:0c:96:c9:a7:
-        ab:41:3c:03:74:49:c6:82:a5:7a:22:39:5e:9c:37:19:a1:31:
-        c6:14:a4:15:98:55:19:b9:b1:e1:e8:0a:57:49:39:f5:dd:9b:
-        ec:41:c1:82:fe:5b:83:e6:ab:21:55:53:db:f0:1d:09:06:a3:
-        4f:f2:1d:cf:53:9d:d8:c4:00:cc:ea:33:d0:15:91:ef:80:c4:
-        f1:5f:94:c3:01:05:a3:ec:bf:c9:24:0b:00:85:2b:d9:1f:bb:
-        3b:5e:59:83:94:26:b0:80:83:c3:6e:0f:dc:af:c6:38:5e:7b:
-        80:36:21:ed:b4:b9:ed:04:54:79:a3:8a:ff:83:76:a1:fc:36:
-        ef:f1:97:3a:71:b0:18:fd:bc:37:9f:2f:7e:c1:40:1e:f8:b9:
-        f6:d9:e0:a1:6e:04:92:43:7d:e8:c6:33:2e:a2:ef:54:55:05:
-        e1:f7:f3:b5:32:92:23:d4:2b:8d:82:ad:86:13:dd:c3:4b:83:
-        7c:98:69:72:a8:4c:07:b1:49:c5:47:70:27:91:b6:dd:cf:e9:
-        4d:72:7d:b4:13:7e:28:9b:be:61:c3:1c:88:42:57:31:12:e5:
-        2a:fd:18:76:1f:c2:c5:1c:99:d8:b8:30:80:91:b3:4f:a5:21:
-        8d:46:54:1b:d4:f2:ed:b6:fd:64:ae:51:f0:2d:ba:71:32:d1:
-        d9:2b:7c:e8:bf:2e:5d:41:d4:04:bb:11:3f:6e:e0:b9:e3:95:
-        f4:c8:14:f1:0f:f4:81:bd:a3:6a:3d:00:93:e9:d7:b0:f6:22:
-        1c:b5:ca:72:1a:97:34:da:b6:21:02:a6:34:2a:a3:9f:ca:3d:
-        01:71:80:dc:f7:34:0a:41:b5:d4:6f:ed:02:fc:28:20:30:bf:
-        26:28:04:2e:72:3d:e3:9c:99:62:29:31:4a:9b:f3:d1:63:12:
-        75:88:87:9b:35:be:d2:15:66:cb:fb:5e:4f:d2:73:5d:a0:e7:
-        74:35:5b:10:cb:fb:50:23:eb:ac:7e:7d:4f:8e:f1:48:d8:77:
-        a9:dd:fd:e6:2b:38:2a:c8:db:6c:46:ab:f9:d7:62:d7:eb:ad:
-        05:ce:7e:40:68:37:72:32:db:f8:e7:1e:48:29:83:51:40:50:
-        2c:a5:92:a1:b9:93:52:45:b1:22:a6:c1:71:c3:16:d4:ff:51:
-        83:ae:28:0c:6b:e9:78:96:c5:e0:c5:f5:0e:fc:13:41:8d:52:
-        2b:84:7e:04:65:49:db:ae
+        a3:43:2c:b8:1e:92:53:4f:3a:5c:05:17:f0:37:a0:b7:5b:73:
+        c6:36:99:f4:ef:d6:8b:8a:eb:41:12:c8:0b:2a:c9:83:fd:bc:
+        4d:f2:37:53:ef:c4:43:d2:19:ef:2f:10:42:47:00:fa:2d:b5:
+        6b:1e:a5:42:a1:c4:ca:7a:ea:52:fb:d9:6c:d2:f6:37:83:c4:
+        e7:8a:36:07:88:00:09:d9:c4:eb:29:97:8e:ad:96:5c:3d:19:
+        e6:d6:52:f8:fa:78:7c:57:49:d1:62:4c:e1:13:f5:d2:cc:a3:
+        a1:9f:c2:c0:0d:2d:bd:5c:e2:2b:94:4a:fb:2d:0a:41:04:dd:
+        27:48:77:34:33:ee:ca:b9:20:b7:5c:cd:2a:4d:6c:b2:08:72:
+        09:1e:11:61:69:34:54:42:7b:d5:ce:fc:55:7b:ca:4a:52:20:
+        43:72:4b:c4:0e:02:c5:72:df:d2:28:5f:99:72:88:fb:94:53:
+        51:f9:c4:c3:81:a2:1e:dc:22:9f:18:05:02:50:5f:e7:a1:5d:
+        70:b7:de:a8:96:7b:21:bf:85:28:21:4b:6f:e4:93:3e:56:c8:
+        be:06:85:71:6f:85:f1:32:95:ea:29:a2:5a:92:22:d9:6b:13:
+        69:d4:01:85:2d:9b:76:7c:63:9a:95:d6:99:32:fe:4a:c8:90:
+        53:5a:ce:c3:35:23:d0:82:3c:ed:de:66:ee:15:bc:4d:03:09:
+        77:bd:37:1c:2e:7d:85:1d:64:e9:06:02:14:35:ed:32:66:31:
+        e1:d6:dd:ab:2c:e9:73:88:a1:9f:1a:71:12:11:b3:5f:b8:fa:
+        db:5f:fc:d0:3b:38:5a:47:9c:80:25:bf:5f:5f:9c:b6:cf:ad:
+        ed:04:a0:8f:7c:df:91:28:7d:9c:89:d4:0c:d1:b9:85:74:a9:
+        77:38:33:de:c4:70:c9:5a:8a:d8:6b:08:e4:03:36:f1:04:eb:
+        e3:3c:e6:cc:07:ee:6c:3e:da:88:d3:c7:05:12:2d:f8:17:f8:
+        a2:75:e2:60:5c:ea
 -----BEGIN CERTIFICATE-----
-MIIFbDCCA1SgAwIBAgIJANMwZKi9p8gCMA0GCSqGSIb3DQEBCwUAMEMxHTAbBgNV
-BAMMFFJlZCBIYXQgVUVGSSBDQSAyMDIzMSIwIAYJKoZIhvcNAQkBFhNzZWNhbGVy
-dEByZWRoYXQuY29tMB4XDTIzMTEzMDIwMTExNVoXDTM4MDExODIwMTExNVowQzEd
-MBsGA1UEAwwUUmVkIEhhdCBVRUZJIENBIDIwMjMxIjAgBgkqhkiG9w0BCQEWE3Nl
-Y2FsZXJ0QHJlZGhhdC5jb20wggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoIC
-AQCq0fRHFqaVNbqHrkyVE07QipIqV8mhifkgrpmoXPF1iV/e9seYE5AojyTgpkCb
-TWgdc0kmjpeBHxww6jrhr+VOdqwLJjyOlIxRj8KhxChFtjwObdmlIgAHSUOibsoK
-7pChiZqB91V60fpqNMJZZD+NMh1bWVHXFsuHG38HwdiNxeEV89efBjsuQpyBdweP
-XaFwtnCcBIn2zD4NdzGKVym4t+8mWb+kCy4q8XyhIOwGYkEgLGky2RBqypNn1bFr
-UiFYYdEJh603UPMSnUy/GxcWhUhJEr+58+25YBUqyrchJIVtWAJBb1NqBP4lEESB
-+kTSnYtTMh5FN18aMef3ok3LQLlCEvT9ZzAI/4Ms+KIN+O+TgIGK8LEgNRZOA1q0
-8aifCPBzwNy+T6gpMorMKsM4oQDNGpV4MRQBJU3L+DXKSyEnFVfSJPzxJJojW0Fy
-e43QjIkYn+gbPu3vb2PTC6K99PleIhm+W50eh+ROwkNYuYcGf+ImqhtqErOnxSgi
-DcVAGKiATIutKlaGCrvza+lwoPUL6OnX3jACTzxkuHwEHJGzBA1YPVrqMdBd4JKi
-DCCBd41qcO/KW4FhT3vuAbWIDW1e2ri7ZPtrq0n+UlEDtHLvxeC8oRJdWw+rwrhW
-xYUz0p07dKiOr7aaV34R6R2G/xXWE49/BX+U4mBQwv5vEQIDAQABo2MwYTAPBgNV
-HRMBAf8EBTADAQH/MB0GA1UdDgQWBBSH1TdYGM4ZSLukT8sYKviPgNFuaTAfBgNV
-HSMEGDAWgBSH1TdYGM4ZSLukT8sYKviPgNFuaTAOBgNVHQ8BAf8EBAMCAYYwDQYJ
-KoZIhvcNAQELBQADggIBAHUScopapG3CVUwCeU8cc8WxgEjbIYRw0QPLpZN+2nbF
-wFKii5F7iDoCM9h32Kd7MRKjDJbJp6tBPAN0ScaCpXoiOV6cNxmhMcYUpBWYVRm5
-seHoCldJOfXdm+xBwYL+W4PmqyFVU9vwHQkGo0/yHc9TndjEAMzqM9AVke+AxPFf
-lMMBBaPsv8kkCwCFK9kfuzteWYOUJrCAg8NuD9yvxjhee4A2Ie20ue0EVHmjiv+D
-dqH8Nu/xlzpxsBj9vDefL37BQB74ufbZ4KFuBJJDfejGMy6i71RVBeH387UykiPU
-K42CrYYT3cNLg3yYaXKoTAexScVHcCeRtt3P6U1yfbQTfiibvmHDHIhCVzES5Sr9
-GHYfwsUcmdi4MICRs0+lIY1GVBvU8u22/WSuUfAtunEy0dkrfOi/Ll1B1AS7ET9u
-4LnjlfTIFPEP9IG9o2o9AJPp17D2Ihy1ynIalzTatiECpjQqo5/KPQFxgNz3NApB
-tdRv7QL8KCAwvyYoBC5yPeOcmWIpMUqb89FjEnWIh5s1vtIVZsv7Xk/Sc12g53Q1
-WxDL+1Aj66x+fU+O8UjYd6nd/eYrOCrI22xGq/nXYtfrrQXOfkBoN3Iy2/jnHkgp
-g1FAUCylkqG5k1JFsSKmwXHDFtT/UYOuKAxr6XiWxeDF9Q78E0GNUiuEfgRlSduu
+MIIEbDCCAtSgAwIBAgIJAKtScAz+alQnMA0GCSqGSIb3DQEBCwUAMEMxHTAbBgNV
+BAMMFFJlZCBIYXQgVUVGSSBDQSAyMDI0MSIwIAYJKoZIhvcNAQkBFhNzZWNhbGVy
+dEByZWRoYXQuY29tMB4XDTI0MDMyNzE5MDgzMFoXDTM4MDExODE5MDgzMFowQzEd
+MBsGA1UEAwwUUmVkIEhhdCBVRUZJIENBIDIwMjQxIjAgBgkqhkiG9w0BCQEWE3Nl
+Y2FsZXJ0QHJlZGhhdC5jb20wggGiMA0GCSqGSIb3DQEBAQUAA4IBjwAwggGKAoIB
+gQC9WhMmAmBtbm3KFb5W9beo6T7SuUmuhnbmhPtZlYAgcG80VE3RzC1m7ATzvZ3K
+zC/LvsbFO5+Pz+InWX5kx6sPqpPkIedcZ8IYwXWwyP5ag6+9wofMSCffVUuR/BVI
+dixt96HmmUA1cYFZnXU1cgT2LOEcd+UXoZlI9xZQak9IIRjGkxoPdSg+zWTrZjYa
+e5kKIfAdZC7OdmCveH5+gPf+Qx/8w23sLS8ZcumtXgnGBJljW4vCW6kMafKPoXHd
++dL8silSgPvX3xA3+oRhRd308zTsXWOte6fRRMzY22oZd5dOmtxwDN2hZrWEXMsC
+I1GSn7Vz+6SUOc3J1JP4w9KEFPnd04nxJ68LPXqct2EZf7dXjAgz6toxf//SCeZG
+05P+K1ZitNUYnW/cypO8TYsF2Fyb6pHj2GD2u+8o81+KVehVcIiTG3vTQO9Cww+L
+oNV26xKuG2jM4en2G7Wh9lxbZhn4ECk1O7JiF7CABCrQlX7906wNKLJYIPB0CNTS
+4ZUCAwEAAaNjMGEwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUDsB9Ymj+NZzi
+J+JBaK8O3gx6esMwHwYDVR0jBBgwFoAUDsB9Ymj+NZziJ+JBaK8O3gx6esMwDgYD
+VR0PAQH/BAQDAgGGMA0GCSqGSIb3DQEBCwUAA4IBgQCjQyy4HpJTTzpcBRfwN6C3
+W3PGNpn079aLiutBEsgLKsmD/bxN8jdT78RD0hnvLxBCRwD6LbVrHqVCocTKeupS
++9ls0vY3g8TnijYHiAAJ2cTrKZeOrZZcPRnm1lL4+nh8V0nRYkzhE/XSzKOhn8LA
+DS29XOIrlEr7LQpBBN0nSHc0M+7KuSC3XM0qTWyyCHIJHhFhaTRUQnvVzvxVe8pK
+UiBDckvEDgLFct/SKF+Zcoj7lFNR+cTDgaIe3CKfGAUCUF/noV1wt96olnshv4Uo
+IUtv5JM+Vsi+BoVxb4XxMpXqKaJakiLZaxNp1AGFLZt2fGOaldaZMv5KyJBTWs7D
+NSPQgjzt3mbuFbxNAwl3vTccLn2FHWTpBgIUNe0yZjHh1t2rLOlziKGfGnESEbNf
+uPrbX/zQOzhaR5yAJb9fX5y2z63tBKCPfN+RKH2cidQM0bmFdKl3ODPexHDJWorY
+awjkAzbxBOvjPObMB+5sPtqI08cFEi34F/iideJgXOo=
 -----END CERTIFICATE-----
```

### Comparing `virt-firmware-24.2/virt/firmware/certs/WindowsUEFICA2023.pem` & `virt-firmware-24.4/virt/firmware/certs/WindowsUEFICA2023.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/certs/fedoraca-20200709.pem` & `virt-firmware-24.4/virt/firmware/certs/fedoraca-20200709.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/dump.py` & `virt-firmware-24.4/virt/firmware/dump.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/efi/bootentry.py` & `virt-firmware-24.4/virt/firmware/efi/bootentry.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/efi/certs.py` & `virt-firmware-24.4/virt/firmware/efi/certs.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             resource_filename('virt.firmware', 'certs/RedHatSecureBootCA5.pem'),
             resource_filename('virt.firmware', 'certs/RedHatSecureBootCA8.pem'),
     ],
     },
     'rh-uefi' : {
         'desc'  : 'Red Hat UEFI CA',
         'certs' : [
-            resource_filename('virt.firmware', 'certs/RedHatUEFICA2023.pem'),
+            resource_filename('virt.firmware', 'certs/RedHatUEFICA2024.pem'),
         ],
     },
 
     #
     # fedora keys
     #
     'fedora' : {
```

### Comparing `virt-firmware-24.2/virt/firmware/efi/devpath.py` & `virt-firmware-24.4/virt/firmware/efi/devpath.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/efi/efijson.py` & `virt-firmware-24.4/virt/firmware/efi/efijson.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/efi/efivar.py` & `virt-firmware-24.4/virt/firmware/efi/efivar.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,27 +447,30 @@
 
     def enable_secureboot(self):
         self.add_dummy_dbx(guids.OvmfEnrollDefaultKeys)
         self.set_bool('SecureBootEnable', True)
         self.set_bool('CustomMode', False)
 
     def enroll_platform_with_cert(self, cert,
-                                  guid = guids.OvmfEnrollDefaultKeys):
+                                  guid = guids.OvmfEnrollDefaultKeys,
+                                  ms_kek = 'all'):
         self.add_cert('PK', guid, cert, True)
         self.add_cert('KEK', guid, cert, True)
-        self.add_cert('KEK', guids.MicrosoftVendor, certs.MS_KEK_2011, False)
-        self.add_cert('KEK', guids.MicrosoftVendor, certs.MS_KEK_2023, False)
+        if ms_kek in ('2011', 'all'):
+            self.add_cert('KEK', guids.MicrosoftVendor, certs.MS_KEK_2011, False)
+        if ms_kek in ('2023', 'all'):
+            self.add_cert('KEK', guids.MicrosoftVendor, certs.MS_KEK_2023, False)
         self.add_dummy_dbx(guids.OvmfEnrollDefaultKeys)
 
-    def enroll_platform_redhat(self):
-        self.enroll_platform_with_cert(certs.REDHAT_PK)
+    def enroll_platform_redhat(self, ms_kek = 'all'):
+        self.enroll_platform_with_cert(certs.REDHAT_PK, ms_kek = ms_kek)
 
-    def enroll_platform_generate(self, name):
+    def enroll_platform_generate(self, name, ms_kek = 'all'):
         pk = certs.pk_generate(cn = name)
-        self.enroll_platform_with_cert(pk.name)
+        self.enroll_platform_with_cert(pk.name, ms_kek = ms_kek)
 
     def add_microsoft_keys(self):
         self.add_cert('db', guids.MicrosoftVendor, certs.MS_WIN_2011, False)
         self.add_cert('db', guids.MicrosoftVendor, certs.MS_WIN_2023, False)
         self.add_cert('db', guids.MicrosoftVendor, certs.MS_3RD_2011, False)
         self.add_cert('db', guids.MicrosoftVendor, certs.MS_3RD_2023, False)
```

### Comparing `virt-firmware-24.2/virt/firmware/efi/guids.py` & `virt-firmware-24.4/virt/firmware/efi/guids.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/efi/siglist.py` & `virt-firmware-24.4/virt/firmware/efi/siglist.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/efi/ucs16.py` & `virt-firmware-24.4/virt/firmware/efi/ucs16.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/host.py` & `virt-firmware-24.4/virt/firmware/host.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/migrate.py` & `virt-firmware-24.4/virt/firmware/migrate.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/misc.py` & `virt-firmware-24.4/virt/firmware/misc.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/sigdb.py` & `virt-firmware-24.4/virt/firmware/sigdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
                         help = 'read efi sigdb FILE', metavar = 'FILE')
     parser.add_argument('-o', '--output', dest = 'output', type = str,
                         help = 'write efi sigdb FILE.', metavar = 'FILE')
     parser.add_argument('--add-cert', dest = 'certs',  action = 'append', nargs = 2,
                         help = 'add x509 cert to sigdb, loaded in pem format ' +
                         'from FILE and with owner GUID, can be specified multiple times',
                         metavar = ('GUID', 'FILE'))
+    parser.add_argument('--add-hash', dest = 'hashes',  action = 'append', nargs = 2,
+                        help = 'add sha256 hash to sigdb, with owner GUID, '
+                        'can be specified multiple times',
+                        metavar = ('GUID', 'HASH'))
     parser.add_argument('-p', '--print', dest = 'print',
                         action = 'store_true', default = False,
                         help = 'print sigdb')
     options = parser.parse_args()
 
     if options.input:
         with open(options.input, "rb") as f:
@@ -32,14 +36,19 @@
     else:
         sigdb = siglist.EfiSigDB()
 
     if options.certs:
         for item in options.certs:
             sigdb.add_cert(guids.parse_str(item[0]), item[1])
 
+    if options.hashes:
+        for item in options.hashes:
+            sigdb.add_hash(guids.parse_str(item[0]),
+                           bytes.fromhex(item[1]))
+
     if options.print and sigdb:
         for slist in sigdb:
             efivar.EfiVarList.print_siglist(slist)
 
     if options.output:
         with open(options.output, "wb") as f:
             f.write(bytes(sigdb))
```

### Comparing `virt-firmware-24.2/virt/firmware/vars.py` & `virt-firmware-24.4/virt/firmware/vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,18 @@
                         help = 'enroll default certificates for redhat platform')
     pgroup.add_argument('--enroll-cert', dest = 'enroll_cert',
                         help = 'enroll using specified certificate', metavar = "CERT")
     pgroup.add_argument('--enroll-generate', dest = 'enroll_generate',
                         help = 'enroll using generated cert with given common name', metavar = "CN")
     pgroup.add_argument('--no-microsoft', dest = 'microsoft',
                         action = 'store_false', default = True,
-                        help = 'do not add microsoft keys')
+                        help = 'do not add microsoft keys to db')
+    pgroup.add_argument('--microsoft-kek', dest = 'ms_kek',
+                        choices = [ 'none', '2011', '2023', 'all' ], default = 'all',
+                        help = 'choose microsoft KEK keys to enroll')
     pgroup.add_argument('--distro-keys', dest = 'distro', type = str, action = 'append',
                         help = 'add ca keys for DISTRO', metavar = 'DISTRO')
     pgroup.add_argument('--distro-list', dest = 'distrolist',
                         action = 'store_true', default = False,
                         help = 'list known distros')
     pgroup.add_argument('--sb', '--secure-boot', dest = 'secureboot',
                         action = 'store_true', default = False,
@@ -234,25 +237,27 @@
         with open(options.set_json, "r", encoding = 'utf-8') as f:
             l = json.loads(f.read(), object_hook = efijson.efi_decode)
         for (key, item) in l.items():
             logging.info('set variable %s from %s', key, options.set_json)
             varlist[key] = item
 
     if options.redhat:
-        varlist.enroll_platform_redhat()
+        varlist.enroll_platform_redhat(ms_kek = options.ms_kek)
         if options.microsoft:
             varlist.add_microsoft_keys()
 
     if options.enroll_cert:
-        varlist.enroll_platform_with_cert(options.enroll_cert)
+        varlist.enroll_platform_with_cert(options.enroll_cert,
+                                          ms_kek = options.ms_kek)
         if options.microsoft:
             varlist.add_microsoft_keys()
 
     if options.enroll_generate:
-        varlist.enroll_platform_generate(options.enroll_generate)
+        varlist.enroll_platform_generate(options.enroll_generate,
+                                         ms_kek = options.ms_kek)
         if options.microsoft:
             varlist.add_microsoft_keys()
 
     if options.distro:
         for item in options.distro:
             varlist.add_distro_keys(item)
```

### Comparing `virt-firmware-24.2/virt/firmware/varstore/autodetect.py` & `virt-firmware-24.4/virt/firmware/varstore/autodetect.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 """ autodetect varstore format, using the probe method """
 
 from virt.firmware.varstore import aws
 from virt.firmware.varstore import edk2
 from virt.firmware.varstore import jstore
 
 def open_varstore(filename):
-    if edk2.Edk2VarStore.probe(filename):
-        return edk2.Edk2VarStore(filename)
-
     if edk2.Edk2VarStoreQcow2.probe(filename):
         return edk2.Edk2VarStoreQcow2(filename)
 
+    if edk2.Edk2VarStore.probe(filename):
+        return edk2.Edk2VarStore(filename)
+
     if aws.AwsVarStore.probe(filename):
         return aws.AwsVarStore(filename)
 
     if jstore.JsonVarStore.probe(filename):
         return jstore.JsonVarStore(filename)
 
     return None
```

### Comparing `virt-firmware-24.2/virt/firmware/varstore/aws.py` & `virt-firmware-24.4/virt/firmware/varstore/aws.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/varstore/edk2.py` & `virt-firmware-24.4/virt/firmware/varstore/edk2.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/varstore/jstore.py` & `virt-firmware-24.4/virt/firmware/varstore/jstore.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/firmware/varstore/linux.py` & `virt-firmware-24.4/virt/firmware/varstore/linux.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-24.2/virt/peutils/pesign.py` & `virt-firmware-24.4/virt/peutils/pesign.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import struct
 import hashlib
 import logging
 
 import pkg_resources
 
 from cryptography import x509
+from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives.serialization import pkcs7
 
 from virt.firmware.efi import guids
 
 cryptography_version = pkg_resources.get_distribution('cryptography').version
 cryptography_major = int(cryptography_version.split('.')[0])
 
@@ -124,27 +125,31 @@
 #
 # This does only check whenever one of the certificates in the pkcs7
 # signature is found in the given efi variable, either the certificate
 # itself or the issuer of the certificate.
 #
 # The pkcs7 signature itself is NOT verified.
 #
+# This requires cryptography_major >= 40.
+#
 def pe_check_cert(siglist, variable):
     if not variable:
         return None
     for sig in siglist:
         sigcerts = pkcs7.load_der_pkcs7_certificates(sig)
         for sigcert in sigcerts:
             for dbcert in variable.sigdb:
                 if dbcert.x509:
                     try:
                         sigcert.verify_directly_issued_by(dbcert.x509)
                         return sigcert
                     except (ValueError, TypeError):
                         pass
+                    except InvalidSignature:
+                        pass
                     if sigcert == dbcert.x509:
                         return sigcert
     return None
 
 def pe_check_hash(digest, variable):
     if not variable:
         return False
```

### Comparing `virt-firmware-24.2/virt/peutils/peutils.py` & `virt-firmware-24.4/virt/peutils/peutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 import gzip
 import struct
 import argparse
 
 import pefile
 
 from cryptography import x509
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.serialization import pkcs7
 
 from virt.firmware.efi import guids
-from virt.firmware.efi import siglist
 from virt.firmware.varstore import linux
 
 from virt.peutils import pesign
+from virt.peutils import pedecode
 
 def is_ca_cert(cert):
     try:
         bc = cert.extensions.get_extension_for_oid(x509.oid.ExtensionOID.BASIC_CONSTRAINTS)
     except x509.extensions.ExtensionNotFound:
         bc = False
     if bc:
@@ -41,24 +40,15 @@
     else:
         scn = pesign.cert_common_name(cert.subject)
         icn = pesign.cert_common_name(cert.issuer)
         print(f'# {ii}      subject CN: {scn}')
         print(f'# {ii}      issuer  CN: {icn}')
 
 def print_vendor_cert(db, ii, verbose = False):
-    # VENDOR_CERT_FILE
-    try:
-        crt = x509.load_der_x509_certificate(db, default_backend())
-        print_cert(crt, ii, verbose)
-        return
-    except ValueError:
-        pass
-
-    # VENDOR_DB_FILE
-    sigdb = siglist.EfiSigDB(db)
+    sigdb = pedecode.vendor_cert_sigdb(db)
     for sl in sigdb:
         if str(sl.guid) == guids.EfiCertX509:
             print_cert(sl.x509, ii, verbose)
         elif str(sl.guid) == guids.EfiCertSha256:
             print(f'# {ii}   sha256')
             print(f'# {ii}      {len(sl)} entries')
         else:
@@ -84,30 +74,14 @@
         if extract:
             scn = pesign.cert_common_name(cert.subject)
             fn = "".join(x for x in scn if x.isalnum()) + '.pem'
             print(f'# {ii}      >>> {fn}')
             with open(fn, 'wb') as f:
                 f.write(cert.public_bytes(serialization.Encoding.PEM))
 
-def getcstr(data):
-    """ get C string (terminated by null byte) """
-    idx = 0
-    for b in data:
-        if b == 0:
-            break
-        idx += 1
-    return data[:idx]
-
-def pe_string(pe, index):
-    """ lookup string in string table (right after symbol table) """
-    strtab  = pe.FILE_HEADER.PointerToSymbolTable
-    strtab += pe.FILE_HEADER.NumberOfSymbols * 18
-    strtab += index
-    return getcstr(pe.__data__[strtab:])
-
 def pe_section_flags(sec):
     r = '-'
     w = '-'
     x = '-'
     if sec.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_READ']:
         r = 'r'
     if sec.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_WRITE']:
@@ -153,15 +127,15 @@
 
 def zboot_binary(pe, indent, verbose, varlist = None):
     i = f'{"":{indent}s}'
     (mz, zimg, zoff, zsize, r1, r2, alg) = struct.unpack_from('<I4sIIII8s', pe.get_data())
     if zimg != b'zimg':
         return
 
-    zalg = getcstr(alg).decode()
+    zalg = pedecode.getcstr(alg).decode()
     print(f'# {i}zboot: 0x{zoff:x} +0x{zsize:x} ({zalg})')
 
     zdata = pe.__data__[ zoff : zoff + zsize ]
     if zalg == 'gzip':
         data = gzip.decompress(zdata)
     else:
         return
@@ -176,51 +150,44 @@
     except pefile.PEFormatError:
         print(f'# {i}      not a PE binary')
 
 # pylint: disable=too-many-branches
 def pe_print_section(pe, sec, indent, verbose, varlist = None):
     i  = f'{"":{indent}s}'
     ii = f'{"":{indent+3}s}'
-    if sec.Name.startswith(b'/'):
-        idx = getcstr(sec.Name[1:])
-        sec.Name = pe_string(pe, int(idx))
-    else:
-        sec.Name = getcstr(sec.Name)
+    secname = pedecode.pe_section_name(pe, sec)
     print(f'# {i}section:'
           f' file 0x{sec.PointerToRawData:08x} +0x{sec.SizeOfRawData:08x}'
           f'  virt 0x{sec.VirtualAddress:08x} +0x{sec.Misc_VirtualSize:08x}'
-          f'  {pe_section_flags(sec)} ({sec.Name.decode()})')
-    if sec.Name == b'.vendor_cert':
-        vcert = sec.get_data()
-        (dbs, dbxs, dbo, dbxo) = struct.unpack_from('<IIII', vcert)
-        if dbs:
-            print(f'# {ii}db: {dbo} +{dbs}')
-            db = vcert [ dbo : dbo + dbs ]
+          f'  {pe_section_flags(sec)} ({secname.decode()})')
+    if secname == b'.vendor_cert':
+        (db, dbx) = pedecode.pe_vendor_cert(sec)
+        if db:
+            print(f'# {ii}db')
             print_vendor_cert(db, ii, verbose)
-        if dbxs:
-            print(f'# {ii}dbx: {dbxo} +{dbxs}')
-            dbx = vcert [ dbxo : dbxo + dbxs ]
+        if dbx:
+            print(f'# {ii}dbx')
             print_vendor_cert(dbx, ii, verbose)
-    if sec.Name == b'.sbatlevel':
+    if secname == b'.sbatlevel':
         levels = sec.get_data()
         (version, poff, loff) = struct.unpack_from('<III', levels)
-        print_sbat_entries(ii, 'previous', getcstr(levels[poff + 4:]))
-        print_sbat_entries(ii, 'latest', getcstr(levels[loff + 4:]))
-    if sec.Name in (b'.sdmagic', b'.data.ident', b'.cmdline',
+        print_sbat_entries(ii, 'previous', pedecode.getcstr(levels[poff + 4:]))
+        print_sbat_entries(ii, 'latest', pedecode.getcstr(levels[loff + 4:]))
+    if secname in (b'.sdmagic', b'.data.ident', b'.cmdline',
                     b'.uname', b'.sbat'):
         lines = sec.get_data().decode().rstrip('\n\0')
         for line in lines.split('\n'):
             print(f'# {ii}{line}')
-    if sec.Name == b'.osrel':
+    if secname == b'.osrel':
         osrel = sec.get_data().decode().rstrip('\n\0')
         entries = osrel.split('\n')
         for entry in entries:
             if entry.startswith('PRETTY_NAME'):
                 print(f'# {ii}{entry}')
-    if sec.Name == b'.linux':
+    if secname == b'.linux':
         print(f'# {ii}embedded binary')
         try:
             npe = pefile.PE(data = sec.get_data())
             pe_print_header(npe, indent + 6)
             for nsec in npe.sections:
                 pe_print_section(npe, nsec, indent + 6, verbose, varlist)
             zboot_binary(npe, indent + 6, verbose, varlist)
```

### Comparing `virt-firmware-24.2/virt_firmware.egg-info/PKG-INFO` & `virt-firmware-24.4/virt_firmware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virt-firmware
-Version: 24.2
+Version: 24.4
 Summary: tools for virtual machine firmware volumes
 Author: Gerd Hoffmann
 Author-email: kraxel@redhat.com
 License: GPLv2
 Project-URL: GitLab, https://gitlab.com/kraxel/virt-firmware
 Keywords: ovmf,armvirt,edk2,aws
 Description-Content-Type: text/markdown
```

### Comparing `virt-firmware-24.2/virt_firmware.egg-info/SOURCES.txt` & `virt-firmware-24.4/virt_firmware.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 experimental/addons.py
 experimental/authenticode.py
+experimental/authfiles.py
 experimental/dbxupdate.py
 experimental/fixup-partitions-for-uki.sh
 experimental/generate-bootcsv-for-uki.sh
 experimental/lscert.py
 experimental/measure.py
 experimental/textual-boot-menu.py
 man/kernel-bootcfg.1
@@ -54,15 +55,15 @@
 virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
 virt/firmware/certs/MicrosoftUEFICA2023.pem
 virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
 virt/firmware/certs/RedHatSecureBootCA3.pem
 virt/firmware/certs/RedHatSecureBootCA5.pem
 virt/firmware/certs/RedHatSecureBootCA8.pem
 virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
-virt/firmware/certs/RedHatUEFICA2023.pem
+virt/firmware/certs/RedHatUEFICA2024.pem
 virt/firmware/certs/WindowsUEFICA2023.pem
 virt/firmware/certs/fedoraca-20200709.pem
 virt/firmware/efi/__init__.py
 virt/firmware/efi/bootentry.py
 virt/firmware/efi/certs.py
 virt/firmware/efi/devpath.py
 virt/firmware/efi/efijson.py
@@ -73,14 +74,15 @@
 virt/firmware/varstore/__init__.py
 virt/firmware/varstore/autodetect.py
 virt/firmware/varstore/aws.py
 virt/firmware/varstore/edk2.py
 virt/firmware/varstore/jstore.py
 virt/firmware/varstore/linux.py
 virt/peutils/__init__.py
+virt/peutils/pedecode.py
 virt/peutils/pesign.py
 virt/peutils/peutils.py
 virt_firmware.egg-info/PKG-INFO
 virt_firmware.egg-info/SOURCES.txt
 virt_firmware.egg-info/dependency_links.txt
 virt_firmware.egg-info/entry_points.txt
 virt_firmware.egg-info/requires.txt
```


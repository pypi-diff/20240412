# Comparing `tmp/shippo-3.2.2.tar.gz` & `tmp/shippo-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.2.2.tar", last modified: Mon Apr  8 19:04:24 2024, max compression
+gzip compressed data, was "shippo-3.2.3.tar", last modified: Fri Apr 12 18:13:47 2024, max compression
```

## Comparing `shippo-3.2.2.tar` & `shippo-3.2.3.tar`

### file list

```diff
@@ -1,249 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.101134 shippo-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-08 19:04:24.101134 shippo-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-08 19:03:54.000000 shippo-3.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:04:24.101134 shippo-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-08 19:03:54.000000 shippo-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.065134 shippo-3.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.069134 shippo-3.2.2/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.069134 shippo-3.2.2/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    28886 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.069134 shippo-3.2.2/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.089134 shippo-3.2.2/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carriers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/connectexistingownupsaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/distanceunit.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/instanttransactionrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/labelfiletype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/objectstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegrouptype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    41853 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/weightunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.089134 shippo-3.2.2/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/badrequestwithdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/badrequestwitherror.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.089134 shippo-3.2.2/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.101134 shippo-3.2.2/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15887 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.101134 shippo-3.2.2/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.069134 shippo-3.2.2/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-08 19:04:21.000000 shippo-3.2.2/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-08 19:04:23.000000 shippo-3.2.2/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:04:21.000000 shippo-3.2.2/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 19:04:21.000000 shippo-3.2.2/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 19:04:21.000000 shippo-3.2.2/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.554701 shippo-3.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-12 18:13:47.554701 shippo-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-12 18:13:35.000000 shippo-3.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:13:47.554701 shippo-3.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-12 18:13:35.000000 shippo-3.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.514701 shippo-3.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.522701 shippo-3.2.3/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.522701 shippo-3.2.3/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28983 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.522701 shippo-3.2.3/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.542701 shippo-3.2.3/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carriers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/connectexistingownupsaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/distanceunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/instanttransactionrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/labelfiletype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/objectstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegrouptype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41991 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/weightunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.542701 shippo-3.2.3/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/badrequestwithdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/badrequestwitherror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.542701 shippo-3.2.3/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.554701 shippo-3.2.3/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15887 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.554701 shippo-3.2.3/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.522701 shippo-3.2.3/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11400 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.2.2/PKG-INFO` & `shippo-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.2
+Version: 3.2.3
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.2/README.md` & `shippo-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/setup.py` & `shippo-3.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.2.2',
+    version='3.2.3',
     author='Shippo',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `shippo-3.2.2/src/shippo/_hooks/registration.py` & `shippo-3.2.3/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/_hooks/sdkhooks.py` & `shippo-3.2.3/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/_hooks/types.py` & `shippo-3.2.3/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/addresses.py` & `shippo-3.2.3/src/shippo/addresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/batches.py` & `shippo-3.2.3/src/shippo/batches.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/carrier_accounts.py` & `shippo-3.2.3/src/shippo/carrier_accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def register(self, shippo_api_version: Optional[str] = None, request_body: Optional[Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest]] = None) -> components.CarrierAccount:
+    def register(self, shippo_api_version: Optional[str] = None, request_body: Optional[Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountFedExCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountMondialRelayCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest]] = None) -> components.CarrierAccount:
         r"""Add a Shippo carrier account
         Adds a Shippo carrier account
         """
         hook_ctx = HookContext(operation_id='RegisterCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.RegisterCarrierAccountRequest(
             shippo_api_version=shippo_api_version,
             request_body=request_body,
```

### Comparing `shippo-3.2.2/src/shippo/carrier_parcel_templates.py` & `shippo-3.2.3/src/shippo/carrier_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/customs_declarations.py` & `shippo-3.2.3/src/shippo/customs_declarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/customs_items.py` & `shippo-3.2.3/src/shippo/customs_items.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/debug.py` & `shippo-3.2.3/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/manifests.py` & `shippo-3.2.3/src/shippo/manifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/__init__.py` & `shippo-3.2.3/src/shippo/models/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 from .carrieraccountcolissimocreaterequest import *
 from .carrieraccountcorreoscreaterequest import *
 from .carrieraccountdeutschepostcreaterequest import *
 from .carrieraccountdhlexpresscreaterequest import *
 from .carrieraccountdhlexpresscreaterequestparameters import *
 from .carrieraccountdpddecreaterequest import *
 from .carrieraccountdpdukcreaterequest import *
+from .carrieraccountfedexcreaterequest import *
 from .carrieraccounthermesukcreaterequest import *
+from .carrieraccountmondialrelaycreaterequest import *
 from .carrieraccountpaginatedlist import *
 from .carrieraccountposteitalianecreaterequest import *
 from .carrieraccountregistrationstatus import *
 from .carrieraccountservicelevel import *
 from .carrieraccountupscreaterequest import *
 from .carrieraccountupscreaterequestparameters import *
 from .carrieraccountuspscreaterequest import *
@@ -121,8 +123,8 @@
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunit import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnUPSAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DryIce","EelPfc","ErrorMessage","HTTPMetadata","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectInfo","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parameters","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnUPSAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DryIce","EelPfc","ErrorMessage","HTTPMetadata","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectInfo","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parameters","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
```

### Comparing `shippo-3.2.2/src/shippo/models/components/address.py` & `shippo-3.2.3/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/addressimporter.py` & `shippo-3.2.3/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.2.3/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.2.3/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/alcohol.py` & `shippo-3.2.3/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/batch.py` & `shippo-3.2.3/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/batchshipment.py` & `shippo-3.2.3/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.2.3/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/billing.py` & `shippo-3.2.3/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccount.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.2.3/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.2.3/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/carriers.py` & `shippo-3.2.3/src/shippo/models/components/carriers.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/cod.py` & `shippo-3.2.3/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/connectexistingownupsaccountrequest.py` & `shippo-3.2.3/src/shippo/models/components/connectexistingownupsaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customerreference.py` & `shippo-3.2.3/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customsdeclaration.py` & `shippo-3.2.3/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.2.3/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.2.3/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customsitem.py` & `shippo-3.2.3/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customsitembase.py` & `shippo-3.2.3/src/shippo/models/components/customsitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/customstaxidentification.py` & `shippo-3.2.3/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.2.3/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.2.3/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.2.3/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.2.3/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.2.3/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/departmentnumber.py` & `shippo-3.2.3/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/dryice.py` & `shippo-3.2.3/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/errormessage.py` & `shippo-3.2.3/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/httpmetadata.py` & `shippo-3.2.3/src/shippo/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/instanttransactionrequestbody.py` & `shippo-3.2.3/src/shippo/models/components/instanttransactionrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/insurance.py` & `shippo-3.2.3/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/invoicenumber.py` & `shippo-3.2.3/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/labelfiletype.py` & `shippo-3.2.3/src/shippo/models/components/labelfiletype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/lineitem.py` & `shippo-3.2.3/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/lineitembase.py` & `shippo-3.2.3/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/liverate.py` & `shippo-3.2.3/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/location.py` & `shippo-3.2.3/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/manifest.py` & `shippo-3.2.3/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/order.py` & `shippo-3.2.3/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/parcel.py` & `shippo-3.2.3/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/parcelextra.py` & `shippo-3.2.3/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/parcelinsurance.py` & `shippo-3.2.3/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/parcelrequest.py` & `shippo-3.2.3/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.2.3/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/pickup.py` & `shippo-3.2.3/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/pickupbase.py` & `shippo-3.2.3/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/ponumber.py` & `shippo-3.2.3/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/rate.py` & `shippo-3.2.3/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/ratemessage.py` & `shippo-3.2.3/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/refund.py` & `shippo-3.2.3/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/refundrequestbody.py` & `shippo-3.2.3/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/rmanumber.py` & `shippo-3.2.3/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/servicegroup.py` & `shippo-3.2.3/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.2.3/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/servicegrouptype.py` & `shippo-3.2.3/src/shippo/models/components/servicegrouptype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.2.3/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/servicelevel.py` & `shippo-3.2.3/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.2.3/src/shippo/models/components/servicelevelenumset.py`

 * *Files 0% similar despite different names*

```diff
@@ -628,24 +628,26 @@
     | australia_post_pack_and_track_international | Pack and Track International|
     | australia_post_international_airmail | International Airmail|
     | australia_post_express_post_international | Express Post International|
     | australia_post_express_courier_international | Express Courier International|
     | australia_post_international_express | International Express|
     | australia_post_international_standard | International Standard|
     | australia_post_international_economy | International Economy|
+    | australia_post_parcel_post_return | Parcel Post Return|
     """
     AUSTRALIA_POST_EXPRESS_POST = 'australia_post_express_post'
     AUSTRALIA_POST_PARCEL_POST = 'australia_post_parcel_post'
     AUSTRALIA_POST_PACK_AND_TRACK_INTERNATIONAL = 'australia_post_pack_and_track_international'
     AUSTRALIA_POST_INTERNATIONAL_AIRMAIL = 'australia_post_international_airmail'
     AUSTRALIA_POST_EXPRESS_POST_INTERNATIONAL = 'australia_post_express_post_international'
     AUSTRALIA_POST_EXPRESS_COURIER_INTERNATIONAL = 'australia_post_express_courier_international'
     AUSTRALIA_POST_INTERNATIONAL_EXPRESS = 'australia_post_international_express'
     AUSTRALIA_POST_INTERNATIONAL_STANDARD = 'australia_post_international_standard'
     AUSTRALIA_POST_INTERNATIONAL_ECONOMY = 'australia_post_international_economy'
+    AUSTRALIA_POST_PARCEL_POST_RETURN = 'australia_post_parcel_post_return'
 
 class ServiceLevelAsendia(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | asendia_us_priority_tracked | Asendia USA Priority Tracked|
     | asendia_us_international_express | Asendia USA International Express|
     | asendia_us_international_priority_airmail | Asendia USA International Priority Airmail|
```

### Comparing `shippo-3.2.2/src/shippo/models/components/shipment.py` & `shippo-3.2.3/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/shipmentextra.py` & `shippo-3.2.3/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/shippoaccount.py` & `shippo-3.2.3/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.2.3/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/track.py` & `shippo-3.2.3/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/trackingstatus.py` & `shippo-3.2.3/src/shippo/models/components/trackingstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.2.3/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.2.3/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/tracksrequest.py` & `shippo-3.2.3/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/transaction.py` & `shippo-3.2.3/src/shippo/models/components/transaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.2.3/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.2.3/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/userparceltemplate.py` & `shippo-3.2.3/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.2.3/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.2.3/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/errors/badrequestwithdetail.py` & `shippo-3.2.3/src/shippo/models/errors/badrequestwithdetail.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/errors/badrequestwitherror.py` & `shippo-3.2.3/src/shippo/models/errors/badrequestwitherror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.2.3/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/errors/sdkerror.py` & `shippo-3.2.3/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/__init__.py` & `shippo-3.2.3/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.2.3/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createaddress.py` & `shippo-3.2.3/src/shippo/models/operations/createaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createbatch.py` & `shippo-3.2.3/src/shippo/models/operations/createbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createcarrieraccount.py` & `shippo-3.2.3/src/shippo/models/operations/createcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createcustomsdeclaration.py` & `shippo-3.2.3/src/shippo/models/operations/createcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createcustomsitem.py` & `shippo-3.2.3/src/shippo/models/operations/createcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createliverate.py` & `shippo-3.2.3/src/shippo/models/operations/createliverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createmanifest.py` & `shippo-3.2.3/src/shippo/models/operations/createmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createorder.py` & `shippo-3.2.3/src/shippo/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createparcel.py` & `shippo-3.2.3/src/shippo/models/operations/createparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createpickup.py` & `shippo-3.2.3/src/shippo/models/operations/createpickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createrefund.py` & `shippo-3.2.3/src/shippo/models/operations/createrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createservicegroup.py` & `shippo-3.2.3/src/shippo/models/operations/createservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createshipment.py` & `shippo-3.2.3/src/shippo/models/operations/createshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createshippoaccount.py` & `shippo-3.2.3/src/shippo/models/operations/createshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createtrack.py` & `shippo-3.2.3/src/shippo/models/operations/createtrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createtransaction.py` & `shippo-3.2.3/src/shippo/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/createuserparceltemplate.py` & `shippo-3.2.3/src/shippo/models/operations/createuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.2.3/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.2.3/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.2.3/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getaddress.py` & `shippo-3.2.3/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getbatch.py` & `shippo-3.2.3/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.2.3/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.2.3/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.2.3/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.2.3/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.2.3/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.2.3/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getmanifest.py` & `shippo-3.2.3/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getorder.py` & `shippo-3.2.3/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getparcel.py` & `shippo-3.2.3/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getrate.py` & `shippo-3.2.3/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getrefund.py` & `shippo-3.2.3/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getshipment.py` & `shippo-3.2.3/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.2.3/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/gettrack.py` & `shippo-3.2.3/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/gettransaction.py` & `shippo-3.2.3/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.2.3/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.2.3/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listaddresses.py` & `shippo-3.2.3/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.2.3/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.2.3/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.2.3/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.2.3/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listmanifests.py` & `shippo-3.2.3/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listorders.py` & `shippo-3.2.3/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listparcels.py` & `shippo-3.2.3/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listrefunds.py` & `shippo-3.2.3/src/shippo/models/operations/listrefunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listservicegroups.py` & `shippo-3.2.3/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.2.3/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.2.3/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listshipments.py` & `shippo-3.2.3/src/shippo/models/operations/listshipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.2.3/src/shippo/models/operations/listshippoaccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listtransactions.py` & `shippo-3.2.3/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.2.3/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/purchasebatch.py` & `shippo-3.2.3/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/registercarrieraccount.py` & `shippo-3.2.3/src/shippo/models/operations/registercarrieraccount.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from ...models.components import carrieraccountchronopostcreaterequest as components_carrieraccountchronopostcreaterequest
 from ...models.components import carrieraccountcolissimocreaterequest as components_carrieraccountcolissimocreaterequest
 from ...models.components import carrieraccountcorreoscreaterequest as components_carrieraccountcorreoscreaterequest
 from ...models.components import carrieraccountdeutschepostcreaterequest as components_carrieraccountdeutschepostcreaterequest
 from ...models.components import carrieraccountdhlexpresscreaterequest as components_carrieraccountdhlexpresscreaterequest
 from ...models.components import carrieraccountdpddecreaterequest as components_carrieraccountdpddecreaterequest
 from ...models.components import carrieraccountdpdukcreaterequest as components_carrieraccountdpdukcreaterequest
+from ...models.components import carrieraccountfedexcreaterequest as components_carrieraccountfedexcreaterequest
 from ...models.components import carrieraccounthermesukcreaterequest as components_carrieraccounthermesukcreaterequest
+from ...models.components import carrieraccountmondialrelaycreaterequest as components_carrieraccountmondialrelaycreaterequest
 from ...models.components import carrieraccountposteitalianecreaterequest as components_carrieraccountposteitalianecreaterequest
 from ...models.components import carrieraccountupscreaterequest as components_carrieraccountupscreaterequest
 from ...models.components import carrieraccountuspscreaterequest as components_carrieraccountuspscreaterequest
 from typing import Optional, Union
 
 
 @dataclasses.dataclass
@@ -25,11 +27,11 @@
 
 
 
 @dataclasses.dataclass
 class RegisterCarrierAccountRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    request_body: Optional[Union[components_carrieraccountcanadapostcreaterequest.CarrierAccountCanadaPostCreateRequest, components_carrieraccountchronopostcreaterequest.CarrierAccountChronopostCreateRequest, components_carrieraccountcolissimocreaterequest.CarrierAccountColissimoCreateRequest, components_carrieraccountcorreoscreaterequest.CarrierAccountCorreosCreateRequest, components_carrieraccountdeutschepostcreaterequest.CarrierAccountDeutschePostCreateRequest, components_carrieraccountdhlexpresscreaterequest.CarrierAccountDHLExpressCreateRequest, components_carrieraccountdpddecreaterequest.CarrierAccountDpdDeCreateRequest, components_carrieraccountdpdukcreaterequest.CarrierAccountDPDUKCreateRequest, components_carrieraccounthermesukcreaterequest.CarrierAccountHermesUKCreateRequest, components_carrieraccountposteitalianecreaterequest.CarrierAccountPosteItalianeCreateRequest, components_carrieraccountupscreaterequest.CarrierAccountUPSCreateRequest, components_carrieraccountuspscreaterequest.CarrierAccountUSPSCreateRequest]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    request_body: Optional[Union[components_carrieraccountcanadapostcreaterequest.CarrierAccountCanadaPostCreateRequest, components_carrieraccountchronopostcreaterequest.CarrierAccountChronopostCreateRequest, components_carrieraccountcolissimocreaterequest.CarrierAccountColissimoCreateRequest, components_carrieraccountcorreoscreaterequest.CarrierAccountCorreosCreateRequest, components_carrieraccountdeutschepostcreaterequest.CarrierAccountDeutschePostCreateRequest, components_carrieraccountdhlexpresscreaterequest.CarrierAccountDHLExpressCreateRequest, components_carrieraccountdpddecreaterequest.CarrierAccountDpdDeCreateRequest, components_carrieraccountdpdukcreaterequest.CarrierAccountDPDUKCreateRequest, components_carrieraccountfedexcreaterequest.CarrierAccountFedExCreateRequest, components_carrieraccounthermesukcreaterequest.CarrierAccountHermesUKCreateRequest, components_carrieraccountmondialrelaycreaterequest.CarrierAccountMondialRelayCreateRequest, components_carrieraccountposteitalianecreaterequest.CarrierAccountPosteItalianeCreateRequest, components_carrieraccountupscreaterequest.CarrierAccountUPSCreateRequest, components_carrieraccountuspscreaterequest.CarrierAccountUSPSCreateRequest]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Examples."""
```

### Comparing `shippo-3.2.2/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.2.3/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.2.3/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/updatedefaultparceltemplate.py` & `shippo-3.2.3/src/shippo/models/operations/updatedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/updateservicegroup.py` & `shippo-3.2.3/src/shippo/models/operations/updateservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.2.3/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.2.3/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/models/operations/validateaddress.py` & `shippo-3.2.3/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/orders.py` & `shippo-3.2.3/src/shippo/orders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/parcels.py` & `shippo-3.2.3/src/shippo/parcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/pickups.py` & `shippo-3.2.3/src/shippo/pickups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/rates.py` & `shippo-3.2.3/src/shippo/rates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/rates_at_checkout.py` & `shippo-3.2.3/src/shippo/rates_at_checkout.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/refunds.py` & `shippo-3.2.3/src/shippo/refunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/sdk.py` & `shippo-3.2.3/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/sdkconfiguration.py` & `shippo-3.2.3/src/shippo/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.2.2'
-    gen_version: str = '2.301.0'
-    user_agent: str = 'speakeasy-sdk/python 3.2.2 2.301.0 2018-02-08 shippo'
+    sdk_version: str = '3.2.3'
+    gen_version: str = '2.304.1'
+    user_agent: str = 'speakeasy-sdk/python 3.2.3 2.304.1 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.2.2/src/shippo/service_groups.py` & `shippo-3.2.3/src/shippo/service_groups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/shipments.py` & `shippo-3.2.3/src/shippo/shipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/shippo_accounts.py` & `shippo-3.2.3/src/shippo/shippo_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/tracking_status.py` & `shippo-3.2.3/src/shippo/tracking_status.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/transactions.py` & `shippo-3.2.3/src/shippo/transactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/user_parcel_templates.py` & `shippo-3.2.3/src/shippo/user_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/utils/retries.py` & `shippo-3.2.3/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo/utils/utils.py` & `shippo-3.2.3/src/shippo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.2/src/shippo.egg-info/PKG-INFO` & `shippo-3.2.3/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.2
+Version: 3.2.3
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.2/src/shippo.egg-info/SOURCES.txt` & `shippo-3.2.3/src/shippo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 src/shippo/models/components/carrieraccountcolissimocreaterequest.py
 src/shippo/models/components/carrieraccountcorreoscreaterequest.py
 src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
 src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
 src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
 src/shippo/models/components/carrieraccountdpddecreaterequest.py
 src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+src/shippo/models/components/carrieraccountfedexcreaterequest.py
 src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
 src/shippo/models/components/carrieraccountpaginatedlist.py
 src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
 src/shippo/models/components/carrieraccountregistrationstatus.py
 src/shippo/models/components/carrieraccountservicelevel.py
 src/shippo/models/components/carrieraccountupscreaterequest.py
 src/shippo/models/components/carrieraccountupscreaterequestparameters.py
 src/shippo/models/components/carrieraccountuspscreaterequest.py
```


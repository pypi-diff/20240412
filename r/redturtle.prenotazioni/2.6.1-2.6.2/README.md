# Comparing `tmp/redturtle.prenotazioni-2.6.1.tar.gz` & `tmp/redturtle.prenotazioni-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-2.6.1.tar", last modified: Tue Apr  2 08:17:55 2024, max compression
+gzip compressed data, was "redturtle.prenotazioni-2.6.2.tar", last modified: Fri Apr 12 11:59:54 2024, max compression
```

## Comparing `redturtle.prenotazioni-2.6.1.tar` & `redturtle.prenotazioni-2.6.2.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.900811 redturtle.prenotazioni-2.6.1/
--rw-r--r--   0 roman      (502) staff       (20)      748 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/APP_IO.txt
--rw-r--r--   0 roman      (502) staff       (20)    17095 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/CHANGES.rst
--rw-r--r--   0 roman      (502) staff       (20)      152 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/CONTRIBUTORS.rst
--rw-r--r--   0 roman      (502) staff       (20)      586 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/DEVELOP.rst
--rw-r--r--   0 roman      (502) staff       (20)    18092 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/LICENSE.GPL
--rw-r--r--   0 roman      (502) staff       (20)      667 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/LICENSE.rst
--rw-r--r--   0 roman      (502) staff       (20)      110 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/MANIFEST.in
--rw-r--r--   0 roman      (502) staff       (20)    59967 2024-04-02 08:17:55.901265 redturtle.prenotazioni-2.6.1/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)    27252 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/README.rst
--rw-r--r--   0 roman      (502) staff       (20)      164 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/TODO.txt
--rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/constraints-5.2.x.txt
--rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/constraints.txt
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.829983 redturtle.prenotazioni-2.6.1/docs/
--rw-r--r--   0 roman      (502) staff       (20)     7984 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/docs/conf.py
--rw-r--r--   0 roman      (502) staff       (20)       89 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/docs/index.rst
--rw-r--r--   0 roman      (502) staff       (20)      476 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/requirements-6.0.x.txt
--rw-r--r--   0 roman      (502) staff       (20)       48 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/requirements.txt
--rw-r--r--   0 roman      (502) staff       (20)      344 2024-04-02 08:17:55.901774 redturtle.prenotazioni-2.6.1/setup.cfg
--rw-r--r--   0 roman      (502) staff       (20)     3420 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/setup.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.817195 redturtle.prenotazioni-2.6.1/src/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.830227 redturtle.prenotazioni-2.6.1/src/redturtle/
--rw-r--r--   0 roman      (502) staff       (20)       80 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.834887 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/
--rw-r--r--   0 roman      (502) staff       (20)     4638 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.835615 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/actions/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/actions/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      226 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/actions/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3333 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/actions/mail.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.838287 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)    15273 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/booker.py
--rw-r--r--   0 roman      (502) staff       (20)      729 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/booking_code.py
--rw-r--r--   0 roman      (502) staff       (20)     5974 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     4786 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/conflict.py
--rw-r--r--   0 roman      (502) staff       (20)     5037 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/ical.py
--rw-r--r--   0 roman      (502) staff       (20)      273 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
--rw-r--r--   0 roman      (502) staff       (20)     9662 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/slot.py
--rw-r--r--   0 roman      (502) staff       (20)     8771 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/stringinterp.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.838554 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.839508 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      563 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1766 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.839999 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/
--rw-r--r--   0 roman      (502) staff       (20)     1454 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.841627 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/
--rw-r--r--   0 roman      (502) staff       (20)    10220 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     4071 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py
--rw-r--r--   0 roman      (502) staff       (20)     2364 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2592 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py
--rw-r--r--   0 roman      (502) staff       (20)     3178 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py
--rw-r--r--   0 roman      (502) staff       (20)     1151 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py
--rw-r--r--   0 roman      (502) staff       (20)      423 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.842877 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/
--rw-r--r--   0 roman      (502) staff       (20)     9647 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1607 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py
--rw-r--r--   0 roman      (502) staff       (20)     2284 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3600 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py
--rw-r--r--   0 roman      (502) staff       (20)    11940 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.844037 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/
--rw-r--r--   0 roman      (502) staff       (20)     5724 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1115 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py
--rw-r--r--   0 roman      (502) staff       (20)     1689 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2931 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py
--rw-r--r--   0 roman      (502) staff       (20)     2216 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py
--rw-r--r--   0 roman      (502) staff       (20)      284 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.848711 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1817 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/base.py
--rw-r--r--   0 roman      (502) staff       (20)     7331 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      655 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/custom_radio_input.pt
--rw-r--r--   0 roman      (502) staff       (20)     5709 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/delete_reservation.py
--rw-r--r--   0 roman      (502) staff       (20)      673 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/folderfactories.py
--rw-r--r--   0 roman      (502) staff       (20)      155 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.848945 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/overrides/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/overrides/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)     3169 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)    10057 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazione_add.py
--rw-r--r--   0 roman      (502) staff       (20)     5252 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazione_move.py
--rw-r--r--   0 roman      (502) staff       (20)     2721 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazione_print.py
--rw-r--r--   0 roman      (502) staff       (20)    37552 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
--rw-r--r--   0 roman      (502) staff       (20)     1735 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
--rw-r--r--   0 roman      (502) staff       (20)    13800 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazioni_search.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.850412 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)      364 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/calendar-add.png
--rw-r--r--   0 roman      (502) staff       (20)      503 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/calendar-icon.png
--rw-r--r--   0 roman      (502) staff       (20)      266 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/cross-icon.png
--rw-r--r--   0 roman      (502) staff       (20)     9794 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
--rw-r--r--   0 roman      (502) staff       (20)     1600 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
--rw-r--r--   0 roman      (502) staff       (20)      922 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/times-solid.png
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.819113 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.818992 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.851692 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
--rw-r--r--   0 roman      (502) staff       (20)     3239 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
--rw-r--r--   0 roman      (502) staff       (20)     3808 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
--rw-r--r--   0 roman      (502) staff       (20)   349785 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
--rw-r--r--   0 roman      (502) staff       (20)      148 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.851915 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.852182 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
--rw-r--r--   0 roman      (502) staff       (20)     5095 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.852835 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
--rw-r--r--   0 roman      (502) staff       (20)     4705 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
--rw-r--r--   0 roman      (502) staff       (20)     1059 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.855219 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/
--rw-r--r--   0 roman      (502) staff       (20)     3010 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
--rw-r--r--   0 roman      (502) staff       (20)      204 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
--rw-r--r--   0 roman      (502) staff       (20)     2874 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js
--rw-r--r--   0 roman      (502) staff       (20)      401 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.less
--rw-r--r--   0 roman      (502) staff       (20)     1888 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
--rw-r--r--   0 roman      (502) staff       (20)      314 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
--rw-r--r--   0 roman      (502) staff       (20)     4187 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js
--rw-r--r--   0 roman      (502) staff       (20)      337 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.less
--rw-r--r--   0 roman      (502) staff       (20)     1745 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
--rw-r--r--   0 roman      (502) staff       (20)      961 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
--rw-r--r--   0 roman      (502) staff       (20)     1261 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/index.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.855673 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/utils/
--rw-r--r--   0 roman      (502) staff       (20)      941 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
--rw-r--r--   0 roman      (502) staff       (20)      298 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.856636 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/stats/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/stats/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      698 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
--rw-r--r--   0 roman      (502) staff       (20)     3863 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/stats/booking_stats.py
--rw-r--r--   0 roman      (502) staff       (20)      575 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/stats/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.859876 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/
--rw-r--r--   0 roman      (502) staff       (20)     2836 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
--rw-r--r--   0 roman      (502) staff       (20)     1518 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
--rw-r--r--   0 roman      (502) staff       (20)     4828 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
--rw-r--r--   0 roman      (502) staff       (20)     2417 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
--rw-r--r--   0 roman      (502) staff       (20)       48 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/nofollow.pt
--rw-r--r--   0 roman      (502) staff       (20)     7714 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
--rw-r--r--   0 roman      (502) staff       (20)     9592 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
--rw-r--r--   0 roman      (502) staff       (20)    16384 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
--rw-r--r--   0 roman      (502) staff       (20)     2227 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
--rw-r--r--   0 roman      (502) staff       (20)     5299 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
--rw-r--r--   0 roman      (502) staff       (20)     5241 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
--rw-r--r--   0 roman      (502) staff       (20)     1858 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/week.pt
--rw-r--r--   0 roman      (502) staff       (20)      362 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.860609 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/utilities/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/utilities/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      494 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/utilities/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1676 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py
--rw-r--r--   0 roman      (502) staff       (20)     8087 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/vacations.py
--rw-r--r--   0 roman      (502) staff       (20)     1524 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/viewlets.py
--rw-r--r--   0 roman      (502) staff       (20)    10867 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/week.py
--rw-r--r--   0 roman      (502) staff       (20)     1193 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/widget.py
--rw-r--r--   0 roman      (502) staff       (20)     6310 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
--rw-r--r--   0 roman      (502) staff       (20)      485 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/config.py
--rw-r--r--   0 roman      (502) staff       (20)     2049 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.863252 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      111 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/booking_type.py
--rw-r--r--   0 roman      (502) staff       (20)     1537 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/pause.py
--rw-r--r--   0 roman      (502) staff       (20)     7504 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)     1251 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazione_type.py
--rw-r--r--   0 roman      (502) staff       (20)      367 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazioni_day.py
--rw-r--r--   0 roman      (502) staff       (20)    19501 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazioni_folder.py
--rw-r--r--   0 roman      (502) staff       (20)      371 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazioni_week.py
--rw-r--r--   0 roman      (502) staff       (20)      371 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazioni_year.py
--rw-r--r--   0 roman      (502) staff       (20)     8518 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/validators.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.864480 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/
--rw-r--r--   0 roman      (502) staff       (20)       77 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1088 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      227 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.820698 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.865002 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)      208 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/profiles/default/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.865234 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      133 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      630 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/setuphandlers.py
--rw-r--r--   0 roman      (502) staff       (20)     1347 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/smsdemo.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.866483 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/
--rw-r--r--   0 roman      (502) staff       (20)      270 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1615 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2128 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/events_logger.py
--rw-r--r--   0 roman      (502) staff       (20)     1907 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)     1189 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/prenotazioni_folder.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.866934 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/exceptions/
--rw-r--r--   0 roman      (502) staff       (20)      129 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/exceptions/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      712 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/exceptions/booker.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.867657 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/indexers/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/indexers/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      476 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/indexers/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1410 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/indexers/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)     1445 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.870100 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/
--rw-r--r--   0 roman      (502) staff       (20)     5302 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/README.md
--rw-r--r--   0 roman      (502) staff       (20)      207 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     9443 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/api.py
--rw-r--r--   0 roman      (502) staff       (20)     1035 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/cli.py
--rw-r--r--   0 roman      (502) staff       (20)    16384 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/io.db
--rw-r--r--   0 roman      (502) staff       (20)       45 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/io_tools.py
--rw-r--r--   0 roman      (502) staff       (20)     1945 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/monkey.py
--rw-r--r--   0 roman      (502) staff       (20)     2833 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/rdbms.py
--rw-r--r--   0 roman      (502) staff       (20)    27521 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/spec.yaml
--rw-r--r--   0 roman      (502) staff       (20)      961 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/storage.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.871127 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.821504 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/en/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.871367 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)    56804 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.821704 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/it/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.871903 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)      623 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 roman      (502) staff       (20)    73449 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
--rw-r--r--   0 roman      (502) staff       (20)      830 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/manual.pot
--rw-r--r--   0 roman      (502) staff       (20)    56913 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
--rw-r--r--   0 roman      (502) staff       (20)     1618 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/update.py
--rwxr-xr-x   0 roman      (502) staff       (20)      521 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/update.sh
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.872444 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/monkeypatcher/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/monkeypatcher/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      499 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1565 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/permissions.zcml
--rw-r--r--   0 roman      (502) staff       (20)      507 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/prenotazione_event.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.823416 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.874599 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)     2656 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/actions.xml
--rw-r--r--   0 roman      (502) staff       (20)      185 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      349 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/catalog.xml
--rw-r--r--   0 roman      (502) staff       (20)       71 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/contentrules.xml
--rw-r--r--   0 roman      (502) staff       (20)      325 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.875283 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/registry/
--rw-r--r--   0 roman      (502) staff       (20)     5140 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
--rw-r--r--   0 roman      (502) staff       (20)     2015 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
--rw-r--r--   0 roman      (502) staff       (20)     1001 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
--rw-r--r--   0 roman      (502) staff       (20)     3277 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/rolemap.xml
--rw-r--r--   0 roman      (502) staff       (20)      277 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/sharing.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.876705 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/
--rw-r--r--   0 roman      (502) staff       (20)     3607 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
--rw-r--r--   0 roman      (502) staff       (20)     2983 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
--rw-r--r--   0 roman      (502) staff       (20)     3861 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
--rw-r--r--   0 roman      (502) staff       (20)     3257 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
--rw-r--r--   0 roman      (502) staff       (20)     3845 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
--rw-r--r--   0 roman      (502) staff       (20)     3846 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
--rw-r--r--   0 roman      (502) staff       (20)      713 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.822590 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.876948 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
--rw-r--r--   0 roman      (502) staff       (20)    12711 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.877183 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
--rw-r--r--   0 roman      (502) staff       (20)     8877 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
--rw-r--r--   0 roman      (502) staff       (20)      613 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.877416 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_1402/
--rw-r--r--   0 roman      (502) staff       (20)     1508 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.877645 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_1500/
--rw-r--r--   0 roman      (502) staff       (20)      226 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_1500/types.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.878145 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2005/
--rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2005/metadata.xml
--rw-r--r--   0 roman      (502) staff       (20)      638 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.878591 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2006/
--rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2006/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.823291 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2006/workflows/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.878891 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/
--rw-r--r--   0 roman      (502) staff       (20)    12711 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml
--rw-r--r--   0 roman      (502) staff       (20)      279 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2006/workflows.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.879201 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      125 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.879705 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/uninstall/registry/
--rw-r--r--   0 roman      (502) staff       (20)      431 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
--rw-r--r--   0 roman      (502) staff       (20)      152 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.880105 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      199 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.880510 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.881916 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      468 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     7441 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)      973 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py
--rw-r--r--   0 roman      (502) staff       (20)      925 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py
--rw-r--r--   0 roman      (502) staff       (20)     1721 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
--rw-r--r--   0 roman      (502) staff       (20)      162 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.882151 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.882803 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/available_slots/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/available_slots/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      352 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/available_slots/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3537 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/available_slots/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.884603 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     6595 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/add.py
--rw-r--r--   0 roman      (502) staff       (20)     1641 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1209 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/delete.py
--rw-r--r--   0 roman      (502) staff       (20)     1166 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/get.py
--rw-r--r--   0 roman      (502) staff       (20)     1328 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/move.py
--rw-r--r--   0 roman      (502) staff       (20)     1152 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py
--rw-r--r--   0 roman      (502) staff       (20)      966 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/vacation.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.885274 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking_schema/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      404 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     4916 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.885939 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/bookings/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      548 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3898 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/bookings/search.py
--rw-r--r--   0 roman      (502) staff       (20)      336 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.886592 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/day/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/day/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      365 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/day/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     6731 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/day/day.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.887244 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/types/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/types/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      216 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/types/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      915 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/types/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.887664 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/scripts/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/scripts/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      892 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py
--rw-r--r--   0 roman      (502) staff       (20)     1062 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/setuphandlers.py
--rw-r--r--   0 roman      (502) staff       (20)     3443 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/testing.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.896271 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/
--rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1223 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/helpers.py
--rw-r--r--   0 roman      (502) staff       (20)     3222 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_add_block.py
--rw-r--r--   0 roman      (502) staff       (20)    24795 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_add_booking.py
--rw-r--r--   0 roman      (502) staff       (20)     1980 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_add_booking_type.py
--rw-r--r--   0 roman      (502) staff       (20)    17344 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_available_slots.py
--rw-r--r--   0 roman      (502) staff       (20)     2011 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_base_slot.py
--rw-r--r--   0 roman      (502) staff       (20)     4387 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py
--rw-r--r--   0 roman      (502) staff       (20)     6402 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_booking_info.py
--rw-r--r--   0 roman      (502) staff       (20)     6901 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_booking_notify.py
--rw-r--r--   0 roman      (502) staff       (20)     8748 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_booking_schema.py
--rw-r--r--   0 roman      (502) staff       (20)     8696 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py
--rw-r--r--   0 roman      (502) staff       (20)     5952 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py
--rw-r--r--   0 roman      (502) staff       (20)     3088 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
--rw-r--r--   0 roman      (502) staff       (20)     6317 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_day.py
--rw-r--r--   0 roman      (502) staff       (20)    10871 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_delete_booking.py
--rw-r--r--   0 roman      (502) staff       (20)    10361 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
--rw-r--r--   0 roman      (502) staff       (20)     4000 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_gates_overrides.py
--rw-r--r--   0 roman      (502) staff       (20)     8150 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_move_booking_api.py
--rw-r--r--   0 roman      (502) staff       (20)     5216 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
--rw-r--r--   0 roman      (502) staff       (20)    14545 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_pauses_overrides.py
--rw-r--r--   0 roman      (502) staff       (20)     5029 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
--rw-r--r--   0 roman      (502) staff       (20)    15081 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazione_events.py
--rw-r--r--   0 roman      (502) staff       (20)     4861 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
--rw-r--r--   0 roman      (502) staff       (20)     7049 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
--rw-r--r--   0 roman      (502) staff       (20)      740 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
--rw-r--r--   0 roman      (502) staff       (20)    19833 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
--rw-r--r--   0 roman      (502) staff       (20)     2485 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_restapi_types_override.py
--rw-r--r--   0 roman      (502) staff       (20)     9722 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_send_ical.py
--rw-r--r--   0 roman      (502) staff       (20)     4180 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_setup.py
--rw-r--r--   0 roman      (502) staff       (20)     3046 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_stringinterp.py
--rw-r--r--   0 roman      (502) staff       (20)      905 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_utils.py
--rw-r--r--   0 roman      (502) staff       (20)     6486 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_vacation_api.py
--rw-r--r--   0 roman      (502) staff       (20)     1198 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py
--rw-r--r--   0 roman      (502) staff       (20)     2349 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_vocabularies.py
--rw-r--r--   0 roman      (502) staff       (20)    23517 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
--rw-r--r--   0 roman      (502) staff       (20)    16547 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/upgrades.py
--rw-r--r--   0 roman      (502) staff       (20)    10360 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/upgrades.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.897506 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utilities/
--rw-r--r--   0 roman      (502) staff       (20)       94 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utilities/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     2900 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utilities/dateutils.py
--rw-r--r--   0 roman      (502) staff       (20)      489 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utilities/email.py
--rw-r--r--   0 roman      (502) staff       (20)      504 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utilities/log_errors.py
--rw-r--r--   0 roman      (502) staff       (20)     1118 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utilities/urls.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.897985 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utils/
--rw-r--r--   0 roman      (502) staff       (20)       67 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utils/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      597 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.900603 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1444 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      607 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/gates.py
--rw-r--r--   0 roman      (502) staff       (20)     1011 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
--rw-r--r--   0 roman      (502) staff       (20)      598 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/review_states.py
--rw-r--r--   0 roman      (502) staff       (20)     1814 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/tipologies.py
--rw-r--r--   0 roman      (502) staff       (20)      776 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py
--rw-r--r--   0 roman      (502) staff       (20)     1128 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
--rw-r--r--   0 roman      (502) staff       (20)     2549 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_months.py
--rw-r--r--   0 roman      (502) staff       (20)     1367 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
--rw-r--r--   0 roman      (502) staff       (20)      440 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_pause_scheduler.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-02 08:17:55.832297 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/
--rw-r--r--   0 roman      (502) staff       (20)    59967 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)    17548 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (502) staff       (20)      295 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/entry_points.txt
--rw-r--r--   0 roman      (502) staff       (20)       10 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/not-zip-safe
--rw-r--r--   0 roman      (502) staff       (20)      425 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/requires.txt
--rw-r--r--   0 roman      (502) staff       (20)       10 2024-04-02 08:17:55.000000 redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/top_level.txt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.140083 redturtle.prenotazioni-2.6.2/
+-rw-r--r--   0 roman      (502) staff       (20)      748 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/APP_IO.txt
+-rw-r--r--   0 roman      (502) staff       (20)    17425 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/CHANGES.rst
+-rw-r--r--   0 roman      (502) staff       (20)      152 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/CONTRIBUTORS.rst
+-rw-r--r--   0 roman      (502) staff       (20)      586 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/DEVELOP.rst
+-rw-r--r--   0 roman      (502) staff       (20)    18092 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/LICENSE.GPL
+-rw-r--r--   0 roman      (502) staff       (20)      667 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/LICENSE.rst
+-rw-r--r--   0 roman      (502) staff       (20)      110 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/MANIFEST.in
+-rw-r--r--   0 roman      (502) staff       (20)    60401 2024-04-12 11:59:54.140545 redturtle.prenotazioni-2.6.2/PKG-INFO
+-rw-r--r--   0 roman      (502) staff       (20)    27252 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/README.rst
+-rw-r--r--   0 roman      (502) staff       (20)      164 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/TODO.txt
+-rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/constraints-5.2.x.txt
+-rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/constraints.txt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.068440 redturtle.prenotazioni-2.6.2/docs/
+-rw-r--r--   0 roman      (502) staff       (20)     7984 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/docs/conf.py
+-rw-r--r--   0 roman      (502) staff       (20)       89 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/docs/index.rst
+-rw-r--r--   0 roman      (502) staff       (20)      476 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/requirements-6.0.x.txt
+-rw-r--r--   0 roman      (502) staff       (20)       48 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/requirements.txt
+-rw-r--r--   0 roman      (502) staff       (20)      344 2024-04-12 11:59:54.141036 redturtle.prenotazioni-2.6.2/setup.cfg
+-rw-r--r--   0 roman      (502) staff       (20)     3420 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/setup.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.054993 redturtle.prenotazioni-2.6.2/src/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.068654 redturtle.prenotazioni-2.6.2/src/redturtle/
+-rw-r--r--   0 roman      (502) staff       (20)       80 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.073079 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/
+-rw-r--r--   0 roman      (502) staff       (20)     4638 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.073821 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/actions/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/actions/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      226 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/actions/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     3333 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/actions/mail.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.075983 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)    15273 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/booker.py
+-rw-r--r--   0 roman      (502) staff       (20)      729 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/booking_code.py
+-rw-r--r--   0 roman      (502) staff       (20)     5974 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     4786 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/conflict.py
+-rw-r--r--   0 roman      (502) staff       (20)     5037 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/ical.py
+-rw-r--r--   0 roman      (502) staff       (20)      273 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
+-rw-r--r--   0 roman      (502) staff       (20)     9662 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/slot.py
+-rw-r--r--   0 roman      (502) staff       (20)     8771 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/stringinterp.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.076206 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.076867 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      563 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1766 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.077446 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/
+-rw-r--r--   0 roman      (502) staff       (20)     1454 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.078827 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/
+-rw-r--r--   0 roman      (502) staff       (20)    10220 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     4071 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py
+-rw-r--r--   0 roman      (502) staff       (20)     2364 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     2592 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py
+-rw-r--r--   0 roman      (502) staff       (20)     3178 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py
+-rw-r--r--   0 roman      (502) staff       (20)     1151 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py
+-rw-r--r--   0 roman      (502) staff       (20)      423 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.080079 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/
+-rw-r--r--   0 roman      (502) staff       (20)     9647 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1607 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py
+-rw-r--r--   0 roman      (502) staff       (20)     2284 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     3600 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py
+-rw-r--r--   0 roman      (502) staff       (20)    11940 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.081181 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/
+-rw-r--r--   0 roman      (502) staff       (20)     5724 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1115 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py
+-rw-r--r--   0 roman      (502) staff       (20)     1689 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     2931 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py
+-rw-r--r--   0 roman      (502) staff       (20)     2216 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py
+-rw-r--r--   0 roman      (502) staff       (20)      284 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.085508 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1817 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/base.py
+-rw-r--r--   0 roman      (502) staff       (20)     7331 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      655 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/custom_radio_input.pt
+-rw-r--r--   0 roman      (502) staff       (20)     5709 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/delete_reservation.py
+-rw-r--r--   0 roman      (502) staff       (20)      673 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/folderfactories.py
+-rw-r--r--   0 roman      (502) staff       (20)      155 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/interfaces.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.085726 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/overrides/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/overrides/.gitkeep
+-rw-r--r--   0 roman      (502) staff       (20)     3169 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)    10057 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazione_add.py
+-rw-r--r--   0 roman      (502) staff       (20)     5252 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazione_move.py
+-rw-r--r--   0 roman      (502) staff       (20)     2721 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazione_print.py
+-rw-r--r--   0 roman      (502) staff       (20)    38319 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
+-rw-r--r--   0 roman      (502) staff       (20)     1735 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
+-rw-r--r--   0 roman      (502) staff       (20)    13800 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazioni_search.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.087397 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/.gitkeep
+-rw-r--r--   0 roman      (502) staff       (20)      364 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/calendar-add.png
+-rw-r--r--   0 roman      (502) staff       (20)      503 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/calendar-icon.png
+-rw-r--r--   0 roman      (502) staff       (20)      266 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/cross-icon.png
+-rw-r--r--   0 roman      (502) staff       (20)     9794 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
+-rw-r--r--   0 roman      (502) staff       (20)     1600 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
+-rw-r--r--   0 roman      (502) staff       (20)      922 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/times-solid.png
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.057204 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.057053 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.089041 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
+-rw-r--r--   0 roman      (502) staff       (20)     3239 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+-rw-r--r--   0 roman      (502) staff       (20)     3808 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+-rw-r--r--   0 roman      (502) staff       (20)   349785 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+-rw-r--r--   0 roman      (502) staff       (20)      148 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.089356 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.089602 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
+-rw-r--r--   0 roman      (502) staff       (20)     5095 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.090060 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
+-rw-r--r--   0 roman      (502) staff       (20)     4705 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+-rw-r--r--   0 roman      (502) staff       (20)     1059 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.092569 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/
+-rw-r--r--   0 roman      (502) staff       (20)     3010 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+-rw-r--r--   0 roman      (502) staff       (20)      204 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+-rw-r--r--   0 roman      (502) staff       (20)     2874 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js
+-rw-r--r--   0 roman      (502) staff       (20)      401 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.less
+-rw-r--r--   0 roman      (502) staff       (20)     1888 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+-rw-r--r--   0 roman      (502) staff       (20)      314 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+-rw-r--r--   0 roman      (502) staff       (20)     4187 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js
+-rw-r--r--   0 roman      (502) staff       (20)      337 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.less
+-rw-r--r--   0 roman      (502) staff       (20)     1745 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+-rw-r--r--   0 roman      (502) staff       (20)      961 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+-rw-r--r--   0 roman      (502) staff       (20)     1261 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/index.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.093018 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/utils/
+-rw-r--r--   0 roman      (502) staff       (20)      941 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+-rw-r--r--   0 roman      (502) staff       (20)      298 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.093946 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/stats/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/stats/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      698 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
+-rw-r--r--   0 roman      (502) staff       (20)     3863 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/stats/booking_stats.py
+-rw-r--r--   0 roman      (502) staff       (20)      575 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/stats/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.097298 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/
+-rw-r--r--   0 roman      (502) staff       (20)     2836 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
+-rw-r--r--   0 roman      (502) staff       (20)     1518 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
+-rw-r--r--   0 roman      (502) staff       (20)     4828 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
+-rw-r--r--   0 roman      (502) staff       (20)     2417 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
+-rw-r--r--   0 roman      (502) staff       (20)       48 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/nofollow.pt
+-rw-r--r--   0 roman      (502) staff       (20)     7714 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
+-rw-r--r--   0 roman      (502) staff       (20)     9592 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
+-rw-r--r--   0 roman      (502) staff       (20)    16384 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
+-rw-r--r--   0 roman      (502) staff       (20)     2227 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
+-rw-r--r--   0 roman      (502) staff       (20)     5299 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
+-rw-r--r--   0 roman      (502) staff       (20)     5241 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
+-rw-r--r--   0 roman      (502) staff       (20)     1858 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/week.pt
+-rw-r--r--   0 roman      (502) staff       (20)      362 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.097971 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/utilities/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/utilities/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      494 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/utilities/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1676 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py
+-rw-r--r--   0 roman      (502) staff       (20)     8087 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/vacations.py
+-rw-r--r--   0 roman      (502) staff       (20)     1524 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/viewlets.py
+-rw-r--r--   0 roman      (502) staff       (20)    10867 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/week.py
+-rw-r--r--   0 roman      (502) staff       (20)     1193 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/widget.py
+-rw-r--r--   0 roman      (502) staff       (20)     6310 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
+-rw-r--r--   0 roman      (502) staff       (20)      485 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/config.py
+-rw-r--r--   0 roman      (502) staff       (20)     2049 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.100300 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      111 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/booking_type.py
+-rw-r--r--   0 roman      (502) staff       (20)     1537 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/pause.py
+-rw-r--r--   0 roman      (502) staff       (20)     7504 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)     1251 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazione_type.py
+-rw-r--r--   0 roman      (502) staff       (20)      367 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazioni_day.py
+-rw-r--r--   0 roman      (502) staff       (20)    19501 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazioni_folder.py
+-rw-r--r--   0 roman      (502) staff       (20)      371 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazioni_week.py
+-rw-r--r--   0 roman      (502) staff       (20)      371 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazioni_year.py
+-rw-r--r--   0 roman      (502) staff       (20)     8518 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/validators.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.101421 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/
+-rw-r--r--   0 roman      (502) staff       (20)       77 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1088 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      227 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/interfaces.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.058887 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/profiles/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.101879 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/profiles/default/
+-rw-r--r--   0 roman      (502) staff       (20)      208 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/profiles/default/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/profiles/default/metadata.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.102157 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/profiles/uninstall/
+-rw-r--r--   0 roman      (502) staff       (20)      133 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)      630 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/setuphandlers.py
+-rw-r--r--   0 roman      (502) staff       (20)     1347 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/smsdemo.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.103404 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/
+-rw-r--r--   0 roman      (502) staff       (20)      270 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1615 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     2128 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/events_logger.py
+-rw-r--r--   0 roman      (502) staff       (20)     1907 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)     1189 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/prenotazioni_folder.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.103940 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/exceptions/
+-rw-r--r--   0 roman      (502) staff       (20)      129 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/exceptions/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      712 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/exceptions/booker.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.104640 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/indexers/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/indexers/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      476 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/indexers/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1410 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/indexers/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)     1445 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/interfaces.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.107175 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/
+-rw-r--r--   0 roman      (502) staff       (20)     5302 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/README.md
+-rw-r--r--   0 roman      (502) staff       (20)      207 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     9443 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/api.py
+-rw-r--r--   0 roman      (502) staff       (20)     1035 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/cli.py
+-rw-r--r--   0 roman      (502) staff       (20)    16384 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/io.db
+-rw-r--r--   0 roman      (502) staff       (20)       45 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/io_tools.py
+-rw-r--r--   0 roman      (502) staff       (20)     1945 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/monkey.py
+-rw-r--r--   0 roman      (502) staff       (20)     2833 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/rdbms.py
+-rw-r--r--   0 roman      (502) staff       (20)    27521 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/spec.yaml
+-rw-r--r--   0 roman      (502) staff       (20)      961 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/storage.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.108274 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.059837 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/en/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.108497 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
+-rw-r--r--   0 roman      (502) staff       (20)    56804 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.060075 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/it/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.109102 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
+-rw-r--r--   0 roman      (502) staff       (20)      623 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 roman      (502) staff       (20)    73449 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
+-rw-r--r--   0 roman      (502) staff       (20)      830 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/manual.pot
+-rw-r--r--   0 roman      (502) staff       (20)    56913 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
+-rw-r--r--   0 roman      (502) staff       (20)     1618 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/update.py
+-rwxr-xr-x   0 roman      (502) staff       (20)      521 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/update.sh
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.109592 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/monkeypatcher/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/monkeypatcher/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      499 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1565 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/permissions.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      507 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/prenotazione_event.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.062044 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.111756 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/
+-rw-r--r--   0 roman      (502) staff       (20)     2656 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/actions.xml
+-rw-r--r--   0 roman      (502) staff       (20)      185 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)      349 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/catalog.xml
+-rw-r--r--   0 roman      (502) staff       (20)       71 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/contentrules.xml
+-rw-r--r--   0 roman      (502) staff       (20)      325 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/metadata.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.112536 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/registry/
+-rw-r--r--   0 roman      (502) staff       (20)     5140 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
+-rw-r--r--   0 roman      (502) staff       (20)     2015 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
+-rw-r--r--   0 roman      (502) staff       (20)     1001 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3277 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/rolemap.xml
+-rw-r--r--   0 roman      (502) staff       (20)      277 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/sharing.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.113991 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/
+-rw-r--r--   0 roman      (502) staff       (20)     3607 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
+-rw-r--r--   0 roman      (502) staff       (20)     2983 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3861 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3257 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3845 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3846 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
+-rw-r--r--   0 roman      (502) staff       (20)      713 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.061136 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.114220 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
+-rw-r--r--   0 roman      (502) staff       (20)    12711 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.114504 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
+-rw-r--r--   0 roman      (502) staff       (20)     8877 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+-rw-r--r--   0 roman      (502) staff       (20)      613 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.114736 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_1402/
+-rw-r--r--   0 roman      (502) staff       (20)     1508 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.114964 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_1500/
+-rw-r--r--   0 roman      (502) staff       (20)      226 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_1500/types.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.115407 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2005/
+-rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2005/metadata.xml
+-rw-r--r--   0 roman      (502) staff       (20)      638 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.115886 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2006/
+-rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2006/metadata.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.061913 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2006/workflows/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.116106 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/
+-rw-r--r--   0 roman      (502) staff       (20)    12711 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml
+-rw-r--r--   0 roman      (502) staff       (20)      279 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2006/workflows.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.116333 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/uninstall/
+-rw-r--r--   0 roman      (502) staff       (20)      125 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.116951 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/uninstall/registry/
+-rw-r--r--   0 roman      (502) staff       (20)      431 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
+-rw-r--r--   0 roman      (502) staff       (20)      152 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.117353 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      199 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.117820 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.119228 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      468 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     7441 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)      973 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py
+-rw-r--r--   0 roman      (502) staff       (20)      925 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py
+-rw-r--r--   0 roman      (502) staff       (20)     1721 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
+-rw-r--r--   0 roman      (502) staff       (20)      162 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.119470 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.120233 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/available_slots/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/available_slots/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      352 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/available_slots/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     3736 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/available_slots/get.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.122012 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     6595 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/add.py
+-rw-r--r--   0 roman      (502) staff       (20)     1641 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1209 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/delete.py
+-rw-r--r--   0 roman      (502) staff       (20)     1166 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/get.py
+-rw-r--r--   0 roman      (502) staff       (20)     1328 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/move.py
+-rw-r--r--   0 roman      (502) staff       (20)     1152 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py
+-rw-r--r--   0 roman      (502) staff       (20)      966 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/vacation.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.122730 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking_schema/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      404 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     5243 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.123422 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/bookings/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      548 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     3898 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/bookings/search.py
+-rw-r--r--   0 roman      (502) staff       (20)      336 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.124050 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/day/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/day/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      365 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/day/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     6732 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/day/day.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.124717 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/types/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/types/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      216 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/types/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      915 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/types/get.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.125118 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/scripts/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/scripts/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      892 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py
+-rw-r--r--   0 roman      (502) staff       (20)     1062 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/setuphandlers.py
+-rw-r--r--   0 roman      (502) staff       (20)     3443 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/testing.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.134461 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/
+-rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1223 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/helpers.py
+-rw-r--r--   0 roman      (502) staff       (20)     3222 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_add_block.py
+-rw-r--r--   0 roman      (502) staff       (20)    24795 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_add_booking.py
+-rw-r--r--   0 roman      (502) staff       (20)     1980 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_add_booking_type.py
+-rw-r--r--   0 roman      (502) staff       (20)    17344 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_available_slots.py
+-rw-r--r--   0 roman      (502) staff       (20)     2011 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_base_slot.py
+-rw-r--r--   0 roman      (502) staff       (20)     4387 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py
+-rw-r--r--   0 roman      (502) staff       (20)     6402 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_booking_info.py
+-rw-r--r--   0 roman      (502) staff       (20)     6901 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_booking_notify.py
+-rw-r--r--   0 roman      (502) staff       (20)     8748 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_booking_schema.py
+-rw-r--r--   0 roman      (502) staff       (20)     8696 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py
+-rw-r--r--   0 roman      (502) staff       (20)     5952 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py
+-rw-r--r--   0 roman      (502) staff       (20)     3088 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
+-rw-r--r--   0 roman      (502) staff       (20)     6317 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_day.py
+-rw-r--r--   0 roman      (502) staff       (20)    10871 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_delete_booking.py
+-rw-r--r--   0 roman      (502) staff       (20)    10361 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+-rw-r--r--   0 roman      (502) staff       (20)     4000 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_gates_overrides.py
+-rw-r--r--   0 roman      (502) staff       (20)     8150 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_move_booking_api.py
+-rw-r--r--   0 roman      (502) staff       (20)     5216 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
+-rw-r--r--   0 roman      (502) staff       (20)    14545 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_pauses_overrides.py
+-rw-r--r--   0 roman      (502) staff       (20)     5029 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
+-rw-r--r--   0 roman      (502) staff       (20)    15081 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazione_events.py
+-rw-r--r--   0 roman      (502) staff       (20)     4861 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+-rw-r--r--   0 roman      (502) staff       (20)     7049 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
+-rw-r--r--   0 roman      (502) staff       (20)      740 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
+-rw-r--r--   0 roman      (502) staff       (20)    19833 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+-rw-r--r--   0 roman      (502) staff       (20)     2485 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_restapi_types_override.py
+-rw-r--r--   0 roman      (502) staff       (20)     9722 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_send_ical.py
+-rw-r--r--   0 roman      (502) staff       (20)     4180 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_setup.py
+-rw-r--r--   0 roman      (502) staff       (20)     3046 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_stringinterp.py
+-rw-r--r--   0 roman      (502) staff       (20)      905 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_utils.py
+-rw-r--r--   0 roman      (502) staff       (20)     6486 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_vacation_api.py
+-rw-r--r--   0 roman      (502) staff       (20)     1198 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py
+-rw-r--r--   0 roman      (502) staff       (20)     2349 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_vocabularies.py
+-rw-r--r--   0 roman      (502) staff       (20)    23517 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
+-rw-r--r--   0 roman      (502) staff       (20)    16547 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/upgrades.py
+-rw-r--r--   0 roman      (502) staff       (20)    10360 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/upgrades.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.135784 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utilities/
+-rw-r--r--   0 roman      (502) staff       (20)       94 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utilities/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     2900 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utilities/dateutils.py
+-rw-r--r--   0 roman      (502) staff       (20)      489 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utilities/email.py
+-rw-r--r--   0 roman      (502) staff       (20)      504 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utilities/log_errors.py
+-rw-r--r--   0 roman      (502) staff       (20)     1118 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utilities/urls.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.136392 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utils/
+-rw-r--r--   0 roman      (502) staff       (20)       67 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utils/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      597 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.139814 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1444 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      607 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/gates.py
+-rw-r--r--   0 roman      (502) staff       (20)     1011 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
+-rw-r--r--   0 roman      (502) staff       (20)      598 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/review_states.py
+-rw-r--r--   0 roman      (502) staff       (20)     1814 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/tipologies.py
+-rw-r--r--   0 roman      (502) staff       (20)      776 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py
+-rw-r--r--   0 roman      (502) staff       (20)     1128 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+-rw-r--r--   0 roman      (502) staff       (20)     2549 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_months.py
+-rw-r--r--   0 roman      (502) staff       (20)     1367 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
+-rw-r--r--   0 roman      (502) staff       (20)      440 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_pause_scheduler.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-12 11:59:54.070653 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/
+-rw-r--r--   0 roman      (502) staff       (20)    60401 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (502) staff       (20)    17548 2024-04-12 11:59:54.000000 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (502) staff       (20)        1 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (502) staff       (20)      295 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/entry_points.txt
+-rw-r--r--   0 roman      (502) staff       (20)       10 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
+-rw-r--r--   0 roman      (502) staff       (20)        1 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/not-zip-safe
+-rw-r--r--   0 roman      (502) staff       (20)      425 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/requires.txt
+-rw-r--r--   0 roman      (502) staff       (20)       10 2024-04-12 11:59:53.000000 redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/top_level.txt
```

### Comparing `redturtle.prenotazioni-2.6.1/APP_IO.txt` & `redturtle.prenotazioni-2.6.2/APP_IO.txt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/CHANGES.rst` & `redturtle.prenotazioni-2.6.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Changelog
 =========
 
 
+2.6.2 (2024-04-12)
+------------------
+
+- Bypass notBeforeDays when using the @available-slots to find the first bookable slot(used by BookingManager).
+  [folix-01]
+
+- Fix day endpoint to show the available scheduling for the same day as start date.
+  [folix-01]
+
+- Manage the user's phone attribute in booking-schema
+  [mamico]
+
+
 2.6.1 (2024-04-02)
 ------------------
 
 - PrenotazioniFolder.max_bookings_allowed constraint (if compiled, the fiscalcode must be required).
   [folix-01]
```

### Comparing `redturtle.prenotazioni-2.6.1/DEVELOP.rst` & `redturtle.prenotazioni-2.6.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/LICENSE.GPL` & `redturtle.prenotazioni-2.6.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/LICENSE.rst` & `redturtle.prenotazioni-2.6.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/PKG-INFO` & `redturtle.prenotazioni-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.6.1
+Version: 2.6.2
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -913,14 +913,27 @@
         .. _List of contributors: https://github.com/RedTurtle/redturtle.prenotazioni/graphs/contributors
         
         
         Changelog
         =========
         
         
+        2.6.2 (2024-04-12)
+        ------------------
+        
+        - Bypass notBeforeDays when using the @available-slots to find the first bookable slot(used by BookingManager).
+          [folix-01]
+        
+        - Fix day endpoint to show the available scheduling for the same day as start date.
+          [folix-01]
+        
+        - Manage the user's phone attribute in booking-schema
+          [mamico]
+        
+        
         2.6.1 (2024-04-02)
         ------------------
         
         - PrenotazioniFolder.max_bookings_allowed constraint (if compiled, the fiscalcode must be required).
           [folix-01]
```

### Comparing `redturtle.prenotazioni-2.6.1/README.rst` & `redturtle.prenotazioni-2.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/docs/conf.py` & `redturtle.prenotazioni-2.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/setup.py` & `redturtle.prenotazioni-2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.prenotazioni",
-    version="2.6.1",
+    version="2.6.2",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/__init__.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/actions/mail.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/actions/mail.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/booker.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/booking_code.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/booking_code.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/conflict.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/conflict.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/ical.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/ical.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/slot.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/adapters/stringinterp.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/base.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/base.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/custom_radio_input.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/custom_radio_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/delete_reservation.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/delete_reservation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/folderfactories.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazione.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazione_add.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazione_add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazione_move.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazione_move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazione_print.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazione_print.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -269,33 +269,36 @@
         for override in overrides:
             override_gates = override.get("gates", []) or gates
             override_week_table = override.get("week_table", []) or week_table
             for gate in override_gates:
                 res[gate] = override_week_table
         return res
 
-    def is_before_allowed_period(self, day):
+    def is_before_allowed_period(self, day, bypass_user_restrictions=False):
         """Returns True if the day is before the first bookable day"""
-        date_limit = self.minimum_bookable_date
+        date_limit = not bypass_user_restrictions and self.minimum_bookable_date or None
+
         if not date_limit:
             return False
         if day <= date_limit.date():
             return True
         return False
 
     @memoize
-    def is_valid_day(self, day):
+    def is_valid_day(self, day, bypass_user_restrictions=False):
         """Returns True if the day is valid"""
         if day < self.first_bookable_day:
             return False
         if self.is_vacation_day(day):
             return False
         if self.last_bookable_day and day > self.last_bookable_day:
             return False
-        if self.is_before_allowed_period(day):
+        if self.is_before_allowed_period(
+            day, bypass_user_restrictions=bypass_user_restrictions
+        ):
             return False
         return self.is_configured_day(day)
 
     @property
     @memoize
     def conflict_manager(self):
         """
@@ -334,21 +337,25 @@
 
     @property
     @memoize
     def base_booking_url(self):
         """Return the base booking url (no parameters) for this context"""
         return "%s/%s" % (self.context.absolute_url(), self.add_view)
 
-    def get_booking_urls(self, day, slot, slot_min_size=0, gate=None):
+    def get_booking_urls(
+        self, day, slot, slot_min_size=0, gate=None, bypass_user_restrictions=False
+    ):
         """Returns, if possible, the booking urls
 
         slot_min_size: seconds
         """
         # we have some conditions to check
-        if not self.is_valid_day(day):
+        if not self.is_valid_day(
+            day, bypass_user_restrictions=bypass_user_restrictions
+        ):
             return []
         if self.maximum_bookable_date and day > self.maximum_bookable_date.date():
             return []
         # date = day.strftime("%Y-%m-%d")
         params = self.remembered_params.copy()
         times = slot.get_values_hr_every(300, slot_min_size=slot_min_size)
         base_url = self.base_booking_url
@@ -367,15 +374,17 @@
                     "class": t.endswith(":00") and "oclock" or None,
                     "booking_date": booking_date,
                     "future": now <= booking_date,
                 }
             )
         return urls
 
-    def get_all_booking_urls_by_gate(self, day, slot_min_size=0):
+    def get_all_booking_urls_by_gate(
+        self, day, slot_min_size=0, bypass_user_restrictions=False
+    ):
         """Get all the booking urls divided by gate
 
         XXX: used only by 'get_all_booking_urls' !!!
 
         slot_min_size: seconds
 
         Return a dict like {
@@ -390,36 +399,45 @@
                 {
                     'title': '08:05',
                  ...
                 ]
             }
         """
         urls = {}
-        if not self.is_valid_day(day):
+        if not self.is_valid_day(
+            day, bypass_user_restrictions=bypass_user_restrictions
+        ):
             return urls
         if self.maximum_bookable_date and day > self.maximum_bookable_date.date():
             return urls
         slots_by_gate = self.get_free_slots(day)
         for gate in slots_by_gate:
             slots = slots_by_gate[gate]
             for slot in slots:
                 slot_urls = self.get_booking_urls(
-                    day, slot, slot_min_size=slot_min_size
+                    day,
+                    slot,
+                    slot_min_size=slot_min_size,
+                    bypass_user_restrictions=bypass_user_restrictions,
                 )
                 urls.setdefault(gate, []).extend(slot_urls)
         return urls
 
-    def get_all_booking_urls(self, day, slot_min_size=0):
+    def get_all_booking_urls(
+        self, day, slot_min_size=0, bypass_user_restrictions=False
+    ):
         """Get all the booking urls
 
         Not divided by gate
 
         slot_min_size: seconds
         """
-        urls_by_gate = self.get_all_booking_urls_by_gate(day, slot_min_size)
+        urls_by_gate = self.get_all_booking_urls_by_gate(
+            day, slot_min_size, bypass_user_restrictions=bypass_user_restrictions
+        )
         urls = {}
         for url in itertools.chain.from_iterable(urls_by_gate.values()):
             urls[url["title"]] = url
         return sorted(urls.values(), key=lambda x: x["title"])
 
     def is_slot_busy(self, day, slot):
         """Check if a slot is busy (i.e. the is no free slot overlapping it)"""
@@ -429,24 +447,28 @@
                 intersection = slot.intersect(free_slot)
                 if intersection:
                     if intersection.lower_value != intersection.upper_value:
                         return False
         return True
 
     @memoize
-    def get_anonymous_booking_url(self, day, slot, slot_min_size=0):
+    def get_anonymous_booking_url(
+        self, day, slot, slot_min_size=0, bypass_user_restrictions=False
+    ):
         """Returns, the the booking url for an anonymous user
 
         Returns the first available/bookable slot/url that fits
         the slot boundaries
 
         slot_min_size: seconds
         """
         # First we check if we have booking urls
-        all_booking_urls = self.get_all_booking_urls(day, slot_min_size)
+        all_booking_urls = self.get_all_booking_urls(
+            day, slot_min_size, bypass_user_restrictions=bypass_user_restrictions
+        )
         if not all_booking_urls:
             # If not the slot can be unavailable or busy
             if self.is_slot_busy(day, slot):
                 return self.busy_slot_booking_url
             else:
                 return self.unavailable_slot_booking_url
         # Otherwise we check if the URL fits the slot boundaries
```

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/prenotazioni_search.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/times-solid.png` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/times-solid.png`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/index.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/stats/booking_stats.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/stats/booking_stats.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/stats/booking_stats.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/stats/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/stats/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/templates/week.pt` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/templates/week.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/vacations.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/vacations.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/viewlets.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/week.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/week.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/widget.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/browser/z3c_custom_widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/pause.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/pause.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazione.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazione_type.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazione_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/prenotazioni_folder.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/content/validators.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/content/validators.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/setuphandlers.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/demo/smsdemo.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/demo/smsdemo.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/events_logger.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/events_logger.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/prenotazione.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/events/prenotazioni_folder.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/events/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/exceptions/booker.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/exceptions/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/indexers/prenotazione.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/indexers/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/interfaces.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/README.md` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/api.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/cli.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/cli.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/io.db` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/io.db`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/monkey.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/rdbms.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/rdbms.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/spec.yaml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/spec.yaml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/io_tools/storage.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/io_tools/storage.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/manual.pot` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/update.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/locales/update.sh` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/locales/update.sh`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/permissions.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/permissions.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/actions.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/default/workflows.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/available_slots/get.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/available_slots/get.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             self.request,
         )
 
         start = self.request.form.get("start", "")
         end = self.request.form.get("end", "")
         past_slots = self.request.form.get("past_slots", False)
         first_available = self.request.form.get("first_available")
+        bypass_user_restrictions = False
 
         if start:
             start = datetime.date.fromisoformat(start)
         else:
             start = datetime.date.today()
 
         if end:
@@ -49,14 +50,15 @@
             "redturtle.prenotazioni: Manage Prenotazioni", obj=self.context
         ):
             end = (
                 self.context.aData
                 and self.context.aData
                 or datetime.date(start.year + 1, start.month, start.day)
             )
+            bypass_user_restrictions = True
         else:
             end = start.replace(day=calendar.monthrange(start.year, start.month)[1])
 
         if start > end:
             msg = self.context.translate(
                 _(
                     "available_slots_wrong_dates",
@@ -73,22 +75,27 @@
         else:
             slot_min_size = 0
 
         response = {
             "@id": f"{self.context.absolute_url()}/@available-slots",
             "items": [],
         }
+
         for n in range(int((end - start).days) + 1):
             booking_date = start + timedelta(n)
             slots = prenotazioni_context_state.get_anonymous_slots(
                 booking_date=booking_date
             )
+
             for slot in slots.get("anonymous_gate", []):
                 info = prenotazioni_context_state.get_anonymous_booking_url(
-                    booking_date, slot, slot_min_size=slot_min_size
+                    booking_date,
+                    slot,
+                    slot_min_size=slot_min_size,
+                    bypass_user_restrictions=bypass_user_restrictions,
                 )
                 if not info.get("url", ""):
                     continue
                 if not past_slots and not info.get("future"):
                     continue
 
                 response["items"].append(json_compatible(info.get("booking_date", "")))
```

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/add.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/delete.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/delete.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/get.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/move.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking/vacation.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking/vacation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py`

 * *Files 9% similar despite different names*

```diff
@@ -92,14 +92,19 @@
             is_readonly = False
 
             if current_user:
                 if field == "email":
                     value = current_user.getProperty("email")
                     # readonly solo se ha un valore
                     is_readonly = bool(value)
+                if field == "phone":
+                    value = current_user.getProperty("phone", "")
+                    # readonly solo se ha un valore (?) non lo lascerei mai readonly permettendo al cittadino
+                    # di modificare il proprio numero di telefono
+                    # is_readonly = bool(value)
                 if field == "fiscalcode":
                     value = current_user.getUserName()
                     is_readonly = True
                 if field == "title":
                     value = current_user.getProperty("fullname")
                     # readonly solo se ha un valore
                     is_readonly = bool(value)
```

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/bookings/search.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/bookings/search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/day/day.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/day/day.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             self.day = date.today()
 
         response = {
             "@id": f"{self.context.absolute_url()}/@day/{self.day.isoformat()}",
         }
 
         # check if date is in the Booking Folder availability dates range
-        if self.context.daData < self.day and (
+        if self.context.daData <= self.day and (
             not self.context.aData or self.context.aData >= self.day
         ):
             response.update(
                 {
                     "bookings": self.get_bookings(),
                     "pauses": self.get_pauses(),
                     "gates": self.get_gates(),
```

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/restapi/services/types/get.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/setuphandlers.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/testing.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/helpers.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_add_block.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_add_block.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_add_booking.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_add_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_add_booking_type.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_add_booking_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_available_slots.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_available_slots.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_base_slot.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_base_slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_booking_info.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_booking_info.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_booking_notify.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_booking_notify.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_booking_schema.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_booking_schema.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_day.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_day.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_delete_booking.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_delete_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_delete_booking_api.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_delete_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_gates_overrides.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_gates_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_move_booking_api.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_move_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_pauses_overrides.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_pauses_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazione_events.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazione_events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_restapi_types_override.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_restapi_types_override.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_send_ical.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_send_ical.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_setup.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_stringinterp.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_utils.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_vacation_api.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_vacation_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_vocabularies.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/tests/test_week_table_overrides.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/tests/test_week_table_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/upgrades.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/upgrades.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utilities/dateutils.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utilities/dateutils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utilities/urls.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utilities/urls.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/configure.zcml` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/gates.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/review_states.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/review_states.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/tipologies.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_months.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_months.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py` & `redturtle.prenotazioni-2.6.2/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/PKG-INFO` & `redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.6.1
+Version: 2.6.2
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -913,14 +913,27 @@
         .. _List of contributors: https://github.com/RedTurtle/redturtle.prenotazioni/graphs/contributors
         
         
         Changelog
         =========
         
         
+        2.6.2 (2024-04-12)
+        ------------------
+        
+        - Bypass notBeforeDays when using the @available-slots to find the first bookable slot(used by BookingManager).
+          [folix-01]
+        
+        - Fix day endpoint to show the available scheduling for the same day as start date.
+          [folix-01]
+        
+        - Manage the user's phone attribute in booking-schema
+          [mamico]
+        
+        
         2.6.1 (2024-04-02)
         ------------------
         
         - PrenotazioniFolder.max_bookings_allowed constraint (if compiled, the fiscalcode must be required).
           [folix-01]
```

### Comparing `redturtle.prenotazioni-2.6.1/src/redturtle.prenotazioni.egg-info/SOURCES.txt` & `redturtle.prenotazioni-2.6.2/src/redturtle.prenotazioni.egg-info/SOURCES.txt`

 * *Files identical despite different names*


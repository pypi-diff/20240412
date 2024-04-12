# Comparing `tmp/sipyconfig-1.2.0.tar.gz` & `tmp/sipyconfig-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipyconfig-1.2.0.tar", last modified: Wed Jul  6 08:31:07 2022, max compression
+gzip compressed data, was "sipyconfig-1.2.1.tar", last modified: Fri Apr 12 21:04:10 2024, max compression
```

## Comparing `sipyconfig-1.2.0.tar` & `sipyconfig-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2022-07-06 08:31:07.444031 sipyconfig-1.2.0/
--rw-r--r--   0 tobias    (1012) familie    (155)    35084 2022-02-03 22:04:07.000000 sipyconfig-1.2.0/LICENSE
--rw-rw-r--   0 tobias    (1012) familie    (155)     1162 2022-07-06 08:31:07.444031 sipyconfig-1.2.0/PKG-INFO
--rw-rw-r--   0 tobias    (1012) familie    (155)      542 2022-02-28 16:14:13.000000 sipyconfig-1.2.0/README.md
--rw-r--r--   0 tobias    (1012) familie    (155)      104 2022-02-03 22:21:27.000000 sipyconfig-1.2.0/pyproject.toml
--rw-rw-r--   0 tobias    (1012) familie    (155)       38 2022-07-06 08:31:07.444031 sipyconfig-1.2.0/setup.cfg
--rw-r--r--   0 tobias    (1012) familie    (155)      953 2022-07-06 08:29:00.000000 sipyconfig-1.2.0/setup.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2022-07-06 08:31:07.428030 sipyconfig-1.2.0/src/
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2022-07-06 08:31:07.444031 sipyconfig-1.2.0/src/sipyconfig/
--rw-r--r--   0 tobias    (1012) familie    (155)      200 2022-02-17 13:33:21.000000 sipyconfig-1.2.0/src/sipyconfig/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)    22569 2022-07-06 08:26:05.000000 sipyconfig-1.2.0/src/sipyconfig/card.py
--rw-r--r--   0 tobias    (1012) familie    (155)     7186 2022-02-03 21:21:15.000000 sipyconfig-1.2.0/src/sipyconfig/comms.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1363 2022-02-17 13:16:55.000000 sipyconfig-1.2.0/src/sipyconfig/crc.py
--rw-r--r--   0 tobias    (1012) familie    (155)     7123 2022-07-06 08:28:21.000000 sipyconfig-1.2.0/src/sipyconfig/enums.py
--rw-r--r--   0 tobias    (1012) familie    (155)    22971 2022-07-06 08:27:35.000000 sipyconfig-1.2.0/src/sipyconfig/station.py
--rw-r--r--   0 tobias    (1012) familie    (155)     3170 2022-05-12 12:32:38.000000 sipyconfig-1.2.0/src/sipyconfig/utils.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2022-07-06 08:31:07.444031 sipyconfig-1.2.0/src/sipyconfig.egg-info/
--rw-rw-r--   0 tobias    (1012) familie    (155)     1162 2022-07-06 08:31:07.000000 sipyconfig-1.2.0/src/sipyconfig.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1012) familie    (155)      417 2022-07-06 08:31:07.000000 sipyconfig-1.2.0/src/sipyconfig.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)        1 2022-07-06 08:31:07.000000 sipyconfig-1.2.0/src/sipyconfig.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)        9 2022-07-06 08:31:07.000000 sipyconfig-1.2.0/src/sipyconfig.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       11 2022-07-06 08:31:07.000000 sipyconfig-1.2.0/src/sipyconfig.egg-info/top_level.txt
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2022-07-06 08:31:07.444031 sipyconfig-1.2.0/test/
--rw-r--r--   0 tobias    (1012) familie    (155)    13082 2022-03-05 14:02:29.000000 sipyconfig-1.2.0/test/test_gui.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2024-04-12 21:04:10.795574 sipyconfig-1.2.1/
+-rw-r--r--   0 tobias    (1012) familie    (155)    35084 2022-02-03 22:04:07.000000 sipyconfig-1.2.1/LICENSE
+-rw-r--r--   0 tobias    (1012) familie    (155)     1186 2024-04-12 21:04:10.795574 sipyconfig-1.2.1/PKG-INFO
+-rw-rw-r--   0 tobias    (1012) familie    (155)      542 2022-02-28 16:14:13.000000 sipyconfig-1.2.1/README.md
+-rw-r--r--   0 tobias    (1012) familie    (155)      104 2022-02-03 22:21:27.000000 sipyconfig-1.2.1/pyproject.toml
+-rw-rw-r--   0 tobias    (1012) familie    (155)       38 2024-04-12 21:04:10.795574 sipyconfig-1.2.1/setup.cfg
+-rw-r--r--   0 tobias    (1012) familie    (155)      953 2024-04-12 21:01:58.000000 sipyconfig-1.2.1/setup.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2024-04-12 21:04:10.795574 sipyconfig-1.2.1/src/
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2024-04-12 21:04:10.795574 sipyconfig-1.2.1/src/sipyconfig/
+-rw-r--r--   0 tobias    (1012) familie    (155)      200 2022-02-17 13:33:21.000000 sipyconfig-1.2.1/src/sipyconfig/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)    23190 2024-04-12 20:56:43.000000 sipyconfig-1.2.1/src/sipyconfig/card.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     7299 2024-04-12 20:56:43.000000 sipyconfig-1.2.1/src/sipyconfig/comms.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1364 2024-04-12 20:56:43.000000 sipyconfig-1.2.1/src/sipyconfig/crc.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     7155 2024-04-12 20:56:43.000000 sipyconfig-1.2.1/src/sipyconfig/enums.py
+-rw-r--r--   0 tobias    (1012) familie    (155)    23517 2024-04-12 21:01:30.000000 sipyconfig-1.2.1/src/sipyconfig/station.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     3182 2024-04-12 20:56:43.000000 sipyconfig-1.2.1/src/sipyconfig/utils.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2024-04-12 21:04:10.795574 sipyconfig-1.2.1/src/sipyconfig.egg-info/
+-rw-r--r--   0 tobias    (1012) familie    (155)     1186 2024-04-12 21:04:10.000000 sipyconfig-1.2.1/src/sipyconfig.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1012) familie    (155)      458 2024-04-12 21:04:10.000000 sipyconfig-1.2.1/src/sipyconfig.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)        1 2024-04-12 21:04:10.000000 sipyconfig-1.2.1/src/sipyconfig.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)        9 2024-04-12 21:04:10.000000 sipyconfig-1.2.1/src/sipyconfig.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       11 2024-04-12 21:04:10.000000 sipyconfig-1.2.1/src/sipyconfig.egg-info/top_level.txt
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2024-04-12 21:04:10.795574 sipyconfig-1.2.1/test/
+-rw-r--r--   0 tobias    (1012) familie    (155)     1050 2022-07-10 00:41:18.000000 sipyconfig-1.2.1/test/test.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1240 2022-07-10 00:51:04.000000 sipyconfig-1.2.1/test/test1.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      486 2022-07-10 00:56:02.000000 sipyconfig-1.2.1/test/test2.py
+-rw-r--r--   0 tobias    (1012) familie    (155)    13253 2024-04-12 16:53:10.000000 sipyconfig-1.2.1/test/test_gui.py
```

### Comparing `sipyconfig-1.2.0/LICENSE` & `sipyconfig-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sipyconfig-1.2.0/PKG-INFO` & `sipyconfig-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: sipyconfig
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python replacement for the functionality of SportIdent Config+
 Home-page: https://gitlab.com/Teigi/sipyconfig
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 4 - Beta
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyserial
 
 # SportIdent Config+ Implementation
 
 A python implementation of the functionality of SPORTident Config+.
 
 Currently only working and tested under Linux.
```

### Comparing `sipyconfig-1.2.0/README.md` & `sipyconfig-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sipyconfig-1.2.0/setup.py` & `sipyconfig-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sipyconfig",
-    version="1.2.0",
+    version="1.2.1",
     author="Teichi",
     author_email="tobias@teichmann.top",
     description="Python replacement for the functionality of SportIdent Config+",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/Teigi/sipyconfig",
     classifiers=[
```

### Comparing `sipyconfig-1.2.0/src/sipyconfig/card.py` & `sipyconfig-1.2.1/src/sipyconfig/card.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,28 +43,29 @@
             except (ValueError, TypeError):
                 self.control_mode = stationmode.UNKNOWN
                 self.siac_mode = siacmode.NO_SIAC
         if auto_detect and (
             self.control_mode is None or
             self.control_mode == stationmode.UNKNOWN
         ):
-            self.control_mode = control_number_to_mode.get(control_number, stationmode.CONTROL)
+            self.control_mode = control_number_to_mode.get(
+                control_number, stationmode.CONTROL)
         if auto_detect and self.control_mode == stationmode.SIAC_SPECIAL:
             self.control_mode = stationmode(control_number)
 
     @classmethod
     def from_bytes(
-            cls,
-            control_number: int,
-            raw_time: bytes,
-            punchdate: int = None,
-            reftime: 'datetime' = None,
-            membytes: 'Optional[bytes]' = None, *,
-            auto_detect: bool = False
-        ) -> 'Punch':
+        cls,
+        control_number: int,
+        raw_time: bytes,
+        punchdate: int = None,
+        reftime: 'datetime' = None,
+        membytes: 'Optional[bytes]' = None, *,
+        auto_detect: bool = False
+    ) -> 'Punch':
         """
         construct Punch class from the byte data
         """
         punchtime = SICard.decode_time(raw_time, punchdate, reftime)
         control_byte = None
         order_number = 0
         if membytes is not None:
@@ -136,14 +137,15 @@
     @staticmethod
     def decode_number(data: 'Union[bytes, List[int]]') -> int:
         """
         Handles decoding the SICard number from bytes. With SICard 5 special case
         """
         if data[0] != 0x00:
             raise SiCardError("Unknown SI-Card!")
+        print([x for x in data[1:4]])
         num = bytes_to_int(data[1:4])
         if num < 500000:
             # SI Card 5
             num2 = bytes_to_int(data[2:4])
             return data[1]*100000 + num2
         return num
 
@@ -211,73 +213,84 @@
     def read_out_data(self, *, no_ack: bool = False) -> None:
         """read out data from SICard"""
         raise NotImplementedError
 
     def process_read_out(self, data: bytes, reftime: 'datetime' = None):
         """process the read out data from a SICard"""
         self._read_at = datetime.now()
-        self._number = self.decode_number([0x00, data[self.CN2], data[self.CN1], data[self.CN0]])
-        self._start_time = self.decode_time(data[self.ST:self.ST+2], data[self.STD] if self.STD != -1 else None, reftime)
-        self._finish_time = self.decode_time(data[self.FT:self.FT+2], data[self.FTD] if self.FTD != -1 else None, reftime)
-        self._check_time = self.decode_time(data[self.CT:self.CT+2], data[self.CTD] if self.CTD != -1 else None, reftime)
+        self._number = self.decode_number(
+            [0x00, data[self.CN2], data[self.CN1], data[self.CN0]])
+        self._start_time = self.decode_time(
+            data[self.ST:self.ST+2], data[self.STD] if self.STD != -1 else None, reftime)
+        self._finish_time = self.decode_time(
+            data[self.FT:self.FT+2], data[self.FTD] if self.FTD != -1 else None, reftime)
+        self._check_time = self.decode_time(
+            data[self.CT:self.CT+2], data[self.CTD] if self.CTD != -1 else None, reftime)
         if self.LT != -1:
-            self._clear_time = self.decode_time(data[self.LT:self.LT+2], data[self.LTD] if self.LTD != -1 else None, reftime)
+            self._clear_time = self.decode_time(
+                data[self.LT:self.LT+2], data[self.LTD] if self.LTD != -1 else None, reftime)
         if self.STR != -1:
-            self._start_reserve = self.decode_time(data[self.STR+2:self.STR+4], data[self.STR], reftime)
+            self._start_reserve = self.decode_time(
+                data[self.STR+2:self.STR+4], data[self.STR], reftime)
         if self.FTR != -1:
-            self._finish_reserve = self.decode_time(data[self.FTR+2:self.FTR+4], data[self.FTR], reftime)
+            self._finish_reserve = self.decode_time(
+                data[self.FTR+2:self.FTR+4], data[self.FTR], reftime)
         if self.LTR != -1:
-            self._clear_reserve = self.decode_time(data[self.LTR+2:self.LTR+4], data[self.LTR], reftime)
+            self._clear_reserve = self.decode_time(
+                data[self.LTR+2:self.LTR+4], data[self.LTR], reftime)
 
         self.process_extra_data(data)
 
         punch_count = data[self.RC]
         if isinstance(self, SI5):
             punch_count -= 1
         if punch_count > self.PM:
             punch_count = self.PM
 
         self._punches = []
         if not isinstance(self, SI5):
             for punch_pointer in range(self.P1, self.P1 + data[self.RC] * self.PL, self.PL):
                 punch_control = data[punch_pointer + self.CN]
-                punch_time = data[punch_pointer + self.PTH:punch_pointer + self.PTL + 1]
+                punch_time = data[punch_pointer +
+                                  self.PTH:punch_pointer + self.PTL + 1]
 
                 punch_date = None
                 if self.PTD != -1:
                     punch_date = data[punch_pointer + self.PTD]
                     punch_control += (punch_date << 2) & ~0xFF
 
-                self.add_punch(Punch.from_bytes(punch_control, punch_time, punch_date, reftime))
+                self.add_punch(Punch.from_bytes(
+                    punch_control, punch_time, punch_date, reftime))
 
     def process_extra_data(self, data: bytes):
         """process any non standard data from the SICard read out"""
         raise NotImplementedError
 
     @classmethod
     def from_auto_send(cls, data: bytes, *, auto_detect_srr: bool = False):
         """create a SI Card object from the data send with auto send."""
         data_new = [x for x in data]
         if data_new[2] == 0x0f:
-            #measures for working with SRR
+            # measures for working with SRR
             data_new[0] = data[0] & 0x7f
             data_new[2] = 0x0
         control_number = bytes_to_int(data_new[:2])
         si_number = cls.decode_number(data_new[2:6])
         time = cls.decode_time(data_new[7:9])
         mem_pointer = data[10:]
         control_byte = mem_pointer[0]
         card: SICard
         if si_number <= 499999:
             card = SI5(data_new[2:6])
         elif 500000 <= si_number <= 999999 or (2003000 <= si_number <= 2003999):
             card = SI6(data_new[2:6])
         else:
             card = SI8To10.switch_types(data_new[2:6])
-        card.add_punch(Punch(control_number, time, control_byte, order_number=mem_pointer[1], auto_detect=auto_detect_srr))
+        card.add_punch(Punch(control_number, time, control_byte,
+                       order_number=mem_pointer[1], auto_detect=auto_detect_srr))
         return card
 
     def add_punch(self, punch: Punch):
         """adds a punch to the list of punches"""
         if not self.punches:
             self._punches = []
         self._punches.append(punch)
@@ -300,21 +313,24 @@
 
             # extract day of week (%7 for sunday = -1)
             day_of_week = (((punchdate & 0b00001110) >> 1) - 1) % 7
 
             if reftime.weekday() == day_of_week and punchtime > timedelta(hours=reftime.hour, minutes=reftime.minute, seconds=reftime.second):
                 reftime -= timedelta(days=7)
             else:
-                reftime -= timedelta(days=(reftime.weekday() - day_of_week) % 7)
+                reftime -= timedelta(days=(reftime.weekday() -
+                                     day_of_week) % 7)
 
-            ref_day = reftime.replace(hour=0, minute=0, second=0, microsecond=0, tzinfo=None)
+            ref_day = reftime.replace(
+                hour=0, minute=0, second=0, microsecond=0, tzinfo=None)
             return ref_day + punchtime
 
         # no punchdate available
-        ref_day = reftime.replace(hour=0, minute=0, second=0, microsecond=0, tzinfo=None)
+        ref_day = reftime.replace(
+            hour=0, minute=0, second=0, microsecond=0, tzinfo=None)
         ref_hour = reftime - ref_day
         t_noon = timedelta(hours=12)
 
         if ref_hour < t_noon:
             # reference time is before noon
             if punchtime < ref_hour:
                 # t is between 0:00 and t_ref
@@ -385,18 +401,21 @@
             if punch_pointer % 16 == 0:
                 # first byte of each block is reserved for punches 31 - 36
                 if data[punch_pointer]:
                     no_time_punches.append(Punch(data[punch_pointer], None))
                 punch_pointer += 1
 
             punch_control = data[punch_pointer + self.CN]
-            punch_time = data[punch_pointer + self.PTH:punch_pointer + self.PTL + 1]
-            punch_date = data[punch_pointer + self.PTD] if self.PTD != -1 else None
+            punch_time = data[punch_pointer +
+                              self.PTH:punch_pointer + self.PTL + 1]
+            punch_date = data[punch_pointer +
+                              self.PTD] if self.PTD != -1 else None
 
-            self.add_punch(Punch.from_bytes(punch_control, punch_time, punch_date, reftime))
+            self.add_punch(Punch.from_bytes(
+                punch_control, punch_time, punch_date, reftime))
             punch_pointer += self.PL
         self.punches.extend(no_time_punches)
 
     def process_extra_data(self, data: bytes):
         pass
 
 
@@ -468,32 +487,36 @@
         super().process_read_out(data, reftime)
 
         self.process_extra_data(data)
 
         if data[:4] == self.SI6_STAR:
             raw_data = bytes([])
 
-            for i in range(2,6):
+            for i in range(2, 6):
                 ret = self._station.send_command(com.GET_SI_6, [i], True)
                 if not isinstance(ret, Command):
                     raise SiError("Can't read Si-Card!")
                 raw_data += ret.data[3:]
 
             for punch_pointer in range(data[self.RC] - self.PM):
                 punch_control = raw_data[punch_pointer + self.CN]
-                punch_time = raw_data[punch_pointer + self.PTH:punch_pointer + self.PTL + 1]
-                punch_date = raw_data[punch_pointer + self.PTD] if self.PTD != -1 else None
+                punch_time = raw_data[punch_pointer +
+                                      self.PTH:punch_pointer + self.PTL + 1]
+                punch_date = raw_data[punch_pointer +
+                                      self.PTD] if self.PTD != -1 else None
 
-                self.add_punch(Punch.from_bytes(punch_control, punch_time, punch_date, reftime))
+                self.add_punch(Punch.from_bytes(
+                    punch_control, punch_time, punch_date, reftime))
                 punch_pointer += self.PL
 
     def process_extra_data(self, data: bytes):
         self._personal_data = {}
         for name, (from_, to_) in self._personal_structure.items():
-            self._personal_data[name] = data[from_:to_+1].decode("ascii", "ignore")
+            self._personal_data[name] = data[from_:to_ +
+                                             1].decode("ascii", "ignore")
 
 
 class SI8To10(SICard):
     """meta class for all SICard 8 and up"""
     _data_name_list: 'Tuple[str, ...]' = ("first_name", "last_name")
 
     def __init__(self, data: 'Union[bytes, List[int]]', station: 'SiUSBStation' = None):
@@ -521,30 +544,31 @@
 
     def read_out_data(self, *, no_ack: bool = False) -> None:
         if not self._station:
             raise AttributeError("SICard needs to be invoked with station!")
 
         raw_data = bytes([])
         for block_number in range(self.BC):
-            ret = self._station.send_command(com.GET_SI_8, [block_number], True)
+            ret = self._station.send_command(
+                com.GET_SI_8, [block_number], True)
             if not isinstance(ret, Command):
                 raise SiError("Can't read Si-Card!")
             raw_data += ret.data[3:]
             if len(raw_data) > self.P1 + self.PL * raw_data[self.RC]:
                 break
 
         self.process_read_out(raw_data)
         if not no_ack:
             self._station.sendACK()
 
     def process_extra_data(self, data: bytes):
         text = data[self.SPD:self.EPD+1].decode("ascii", "ignore").split(";")
 
         self._personal_data = {}
-        for v, k in zip(text, self._data_name_list): # pylint: disable=invalid-name
+        for v, k in zip(text, self._data_name_list):  # pylint: disable=invalid-name
             self._personal_data[k] = v
 
 
 class SI8(SI8To10):
     """SICard 8, numbers 2.000.000 - 2.999.999"""
     CN2 = 0x19
     CN1 = 0x1a
@@ -616,35 +640,40 @@
     PTL = 0x3
     BC = 8
     SPD = 0x20
     EPD = 0x9f
     DOP_M = 0x1C
     DOP_Y = 0x1D
 
-    _data_name_list = ("first_name", "last_name", "sex", "birth", "club", "mail", "phone", "city", "street", "zip", "country")
+    _data_name_list = ("first_name", "last_name", "sex", "birth",
+                       "club", "mail", "phone", "city", "street", "zip", "country")
 
     def process_extra_data(self, data: bytes):
         super().process_extra_data(data)
 
         self._other_data = {
             "production_date": datetime(year=2000+data[self.DOP_Y], month=data[self.DOP_M], day=1)
         }
 
     def write_personal_data(self):
         """apply changes to personal_data dict to the SICard. Max length including separators 128"""
         if not self._station:
             raise AttributeError("SICard needs to be invoked with station!")
 
-        text = ";".join([self._personal_data[x] for x in self._data_name_list]) + ";"
+        text = ";".join([self._personal_data[x]
+                        for x in self._data_name_list]) + ";"
         if len(text) > 128:
             raise ValueError("Length to great maximum 128!")
-        text_bytes = text.encode("ascii", "replace") + b'\xee' * (4 - len(text) % 4)
+        text_bytes = text.encode("ascii", "replace") + \
+            b'\xee' * (4 - len(text) % 4)
         for i in range(0, len(text), 4):
             slice_ = text_bytes[i:i+4]
-            self._station.send_command(com.WRITE_SI_8, bytes([0x08 + i // 4]) + slice_)
+            self._station.send_command(
+                com.WRITE_SI_8, bytes([0x08 + i // 4]) + slice_)
+
 
 class SI10(SI10ToSIAC):
     """SICard 10, numbers 7.000.000 - 7.999.999"""
 
 
 class SI11(SI10ToSIAC):
     """SICard 11, numbers 9.000.000 - 9.999.999"""
@@ -673,8 +702,9 @@
             self._other_data["siac_mode"] = siac_rev[data[self.SIAC_MODE:self.SIAC_MODE+4]]
 
     def write_siac_mode(self, siac_mode: SIAC_BEEP):
         """change blinking mode of the SICard"""
         if not self._station:
             raise AttributeError("SICard needs to be invoked with station!")
 
-        self._station.send_command(com.WRITE_SI_8, bytes([0x73]) + siac_mode.value)
+        self._station.send_command(
+            com.WRITE_SI_8, bytes([0x73]) + siac_mode.value)
```

### Comparing `sipyconfig-1.2.0/src/sipyconfig/comms.py` & `sipyconfig-1.2.1/src/sipyconfig/comms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from typing import Union, List
 from serial import Serial, SerialTimeoutException
 
 from sipyconfig.crc import compute_crc
 from sipyconfig.enums import com, proto, CRCError
 
+
 class ACK():
     """class representing a ACK response"""
 
 
 class NOACK():
     """class representing a NOACK response"""
 
@@ -56,30 +57,33 @@
     def data(self) -> bytes:
         """data of the command"""
         return bytes(self._data)
 
     @data.setter
     def data(self, data: List[int]) -> None:
         if len(data) > 255:
-            raise ValueError("Datastream to big, can only send up to 255 bytes at a time.")
+            raise ValueError(
+                "Datastream to big, can only send up to 255 bytes at a time.")
         self._data = data
         if not self._is_receiving_command:
             self.compute_crc()
 
     def add_data(self, data: Union[int, List[int]]) -> None:
         """append data to this command"""
         if not getattr(self, "_data", None):
             self._data = []
         if isinstance(data, int):
             if self.length + 1 > 255:
-                raise ValueError("Datastream to big, can only send up to 255 bytes at a time.")
+                raise ValueError(
+                    "Datastream to big, can only send up to 255 bytes at a time.")
             self._data.append(data)
         else:
             if self.length + len(data) > 255:
-                raise ValueError("Datastream to big, can only send up to 255 bytes at a time.")
+                raise ValueError(
+                    "Datastream to big, can only send up to 255 bytes at a time.")
             self._data.extend(data)
         if not self._is_receiving_command:
             self.compute_crc()
 
     def compute_crc(self) -> bytes:
         """compute the crc of the currently stored data"""
         self._crc = compute_crc(self.content).to_bytes(2, "big")
@@ -94,29 +98,32 @@
     def crc(self) -> bytes:
         """currently stored crc"""
         return self._crc
 
     @crc.setter
     def crc(self, crc: bytes) -> None:
         if not self._is_receiving_command:
-            raise TypeError("Setting CRC is only possible when command is set receiving!")
+            raise TypeError(
+                "Setting CRC is only possible when command is set receiving!")
         self._crc = crc
 
     @property
     def length(self) -> int:
         """length of the stored data"""
         return len(self._data)
 
     @property
     def packet(self) -> 'bytes':
         """the full byte sequence to be sent to the station, (content + crc / data with DLE)"""
         if self.is_extended_command:
-            packet = bytes([self.command_code, self.length]) + bytes(self.data) + self.crc
+            packet = bytes([self.command_code, self.length]) + \
+                bytes(self.data) + self.crc
         else:
-            packet = bytes([self.command_code]) + bytes(sum([[proto.DLE, x] for x in self.data], []))
+            packet = bytes([self.command_code]) + \
+                bytes(sum([[proto.DLE, x] for x in self.data], []))
         return bytes(self.START_SEQUENCE) + packet + bytes([proto.ETX])
 
     def check_crc(self, crc: 'Union[int, bytes]' = None, content: bytes = None) -> bool:
         """check crc of content, omitted parameters are taken from stored values"""
         if content is None:
             content = self.content
         if crc is None:
@@ -145,15 +152,14 @@
                 seen_dle = True
                 continue
             ret.append(dat)
             seen_dle = False
         return ret
 
 
-
 def receive_basic_command(command_code: int, dev: 'Serial') -> 'Command':
     '''receive command part of the basic protocol,
     structure: STX | command code | parameter/data with DLE | ETX'''
     command = Command(command_code, receiving=True)
     while True:
         byte = dev.read(1)[0]
         if byte == proto.DLE:
@@ -164,15 +170,15 @@
 
 def receive_extended_command(command_code: int, dev: 'Serial') -> 'Command':
     '''receive command part of the extended protocol,
     structure: STX | command code | length byte | parameter/data | CRC1 | CRC0 | ETX'''
     command = Command(command_code, receiving=True)
     length = dev.read(1)[0]
     command.data = dev.read(length)
-    command.crc= dev.read(2)
+    command.crc = dev.read(2)
     if not command.check_crc():
         raise CRCError("CRC does not match!")
     while dev.read(1)[0] != proto.ETX:
         pass
     return command
```

### Comparing `sipyconfig-1.2.0/src/sipyconfig/crc.py` & `sipyconfig-1.2.1/src/sipyconfig/crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 CRC module for communication with SIStations
 """
 
 from typing import Union, List
 
+
 def compute_crc(data: Union[bytes, List[int]]) -> 'int':
     '''compute the CRC by Spec'''
     if isinstance(data, bytes):
         data = [x for x in data]
     i_tmp, ui_tmp1, ui_val = 0, 0, 0
     i = 0
     ui_count = len(data)
```

### Comparing `sipyconfig-1.2.0/src/sipyconfig/enums.py` & `sipyconfig-1.2.1/src/sipyconfig/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 from typing import Dict
 from enum import IntEnum, Enum
 
 
 class SiError(Exception):
     """General Error for the whole module, all other Errors are derived from this class."""
 
+
 class CRCError(SiError):
     """Error for not matching CRC"""
 
+
 class SiCardEventError(SiError):
     """Subclass of this Error are raised, if a SI Card was inserted or removed, while waiting on a command response."""
 
 
 class SiCardInserted(SiCardEventError):
     """raised when a SI Card is inserted into the station while waiting on a command response."""
 
@@ -28,35 +30,35 @@
     """raised when a SI Card is inserted in Auto Send Mode."""
 
 
 class SiCardError(SiError):
     """raised when an Error occurred in parsing the SI Card information."""
 
 
-class misc(IntEnum): # pylint: disable=invalid-name
+class misc(IntEnum):  # pylint: disable=invalid-name
     """enum for miscellaneous values"""
     MODE_DIRECT = 0x4D
     MODE_REMOTE = 0x53
     SIAC_ON = 0x07
     SIAC_OFF = 0x05
 
     DATA_COMMAND_OFFSET = 3
 
 
-class proto(IntEnum): # pylint: disable=invalid-name
+class proto(IntEnum):  # pylint: disable=invalid-name
     """enum for special protocoll characters"""
     STX = 0x02  # Start of text
     ETX = 0x03  # End of text
     ACK = 0x06  # Positive Handshake return
     NAK = 0x15  # Negative Handshake return
     DLE = 0x10  # DeLimitEr for data characters
     WAKEUP = 0xFF  # send to station for wakeup
 
 
-class com(IntEnum): # pylint: disable=invalid-name
+class com(IntEnum):  # pylint: disable=invalid-name
     """enum for all documented command codes"""
     GET_BACK_MEM = 0x81
     SET_SYS_DATA = 0x82
     GET_SYS_DATA = 0x83
     SRR_WRITE = 0xA2
     SRR_READ = 0xA3
     SRR_QUERY = 0xA6
@@ -85,15 +87,15 @@
     SET_MS_MODE_BASIC = 0x70
     SET_BAUDRATE_BASIC = 0x7E
 
 
 com_rev: Dict[int, str] = {v.value: k for k, v in com.__members__.items()}
 
 
-class memaddr(IntEnum): # pylint: disable=invalid-name
+class memaddr(IntEnum):  # pylint: disable=invalid-name
     """enum for all documented system data memory addresses in SI Stations"""
     SERIAL_NO = 0x00
     SRR_CFG = 0x04
     FIRMWARE = 0x05
     BUILD_DATE = 0x08
     MODEL_ID = 0x0B
     MEM_SIZE = 0x0D
@@ -115,15 +117,15 @@
     PROTOCOL_MODE_FLAG = 0x74
     WAKEUP_DATE = 0x75
     WAKEUP_TIME = 0x78
     SLEEP_TIME = 0x7B
     ACTIVE_TIME = 0x7E
 
 
-class memlen(IntEnum): # pylint: disable=invalid-name
+class memlen(IntEnum):  # pylint: disable=invalid-name
     """enum for the length of the values associated with the address described in memaddr"""
     SERIAL_NO = 0x04
     SRR_CFG = 0x01
     FIRMWARE = 0x03
     BUILD_DATE = 0x03
     MODEL_ID = 0x02
     MEM_SIZE = 0x01
@@ -145,15 +147,15 @@
     PROTOCOL_MODE_FLAG = 0x01
     WAKEUP_DATE = 0x03
     WAKEUP_TIME = 0x03
     SLEEP_TIME = 0x03
     ACTIVE_TIME = 0x02
 
 
-class stationmode(IntEnum): # pylint: disable=invalid-name
+class stationmode(IntEnum):  # pylint: disable=invalid-name
     """enum for all supported operating modes of the SI station"""
     CONTROL = 0x02
     START = 0x03
     FINISH = 0x04
     READOUT = 0x05
     CLEAR_OLD = 0x06
     CLEAR = 0x07
@@ -173,28 +175,29 @@
     UNKNOWN = 0xFF
 
 
 mode_rev: Dict[int, str] = {
     v.value: k for k, v in stationmode.__members__.items()}
 
 
-class siacmode(IntEnum): # pylint: disable=invalid-name
+class siacmode(IntEnum):  # pylint: disable=invalid-name
     """enum for different SIAC radio modes"""
-    NO_SIAC=0x00
-    SIAC_SPECIAL=0x10
-    NO_RADIO=0x30
-    LAST_RECORD=0x70
-    ALL_RECORDS=0xb0
-    UNSENT_RECORDS=0xf0
+    NO_SIAC = 0x00
+    SIAC_SPECIAL = 0x10
+    NO_RADIO = 0x30
+    LAST_RECORD = 0x70
+    ALL_RECORDS = 0xb0
+    UNSENT_RECORDS = 0xf0
+
 
 siacmode_rev: Dict[int, str] = {
     v.value: k for k, v in siacmode.__members__.items()}
 
 
-class MODELID(Enum): # pylint: disable=invalid-name
+class MODELID(Enum):  # pylint: disable=invalid-name
     """enum for station model id"""
     SIMSSR1_AP = b'\x6F\x21'
     BSF3 = b'\x80\x03'
     BSF4 = b'\x80\x04'
     BSM4_RS232 = b'\x80\x84'
     BSM6_USB = b'\x80\x86'
     BSF5 = b'\x81\x15'
@@ -232,26 +235,26 @@
 class SETTINGS(IntEnum):
     """enum of the bit mask for the settings byte"""
     OPTICAL_FEEDBACK = 0x01
     ACOUSTIC_FEEDBACK = 0x04
     NUMBER_HIGH_BIT = 0x40
 
 
-class coderange(IntEnum): # pylint: disable=invalid-name
+class coderange(IntEnum):  # pylint: disable=invalid-name
     """suggested code range for different operating modes"""
     READOUT = 15
     PRINTOUT = 11
     CLEAR = 1
     START_FINISH_CHECK_FROM = 2
     START_FINISH_CHECK_TO = 30
     CONTROL_FROM = 31
     CONTROL_TO = 511
 
 
-class defaulttime(IntEnum): # pylint: disable=invalid-name
+class defaulttime(IntEnum):  # pylint: disable=invalid-name
     """"enum for the default/suggested operating times for the operating modes"""
     CLEAR = 4
     CHECK = 4
     START = 4
     CONTROL = 4
     FINISH = 4
     READOUT = 1
@@ -261,22 +264,24 @@
     SIAC_BATTERY = 1
     SIAC_ON = 1
     SIAC_OFF = 1
     SIAC_READOUT = 1
     SIAC_TEST = 12
 
 
-class SIAC_BEEP(Enum): # pylint: disable=invalid-name
+class SIAC_BEEP(Enum):  # pylint: disable=invalid-name
     """enum for the different SIAC feedback (beep) modes"""
     DEFAULT = b'\x18\x00\x05\x4A'
     SHORT = b'\x06\x00\x05\x4A'
     LONG = b'\x30\x00\x05\x4A'
     BLINK_ONLY = b'\x20\x00\x66\x00'
 
-siac_rev: Dict[bytes, str] = {v.value: k for k, v in SIAC_BEEP.__members__.items()}
+
+siac_rev: Dict[bytes, str] = {
+    v.value: k for k, v in SIAC_BEEP.__members__.items()}
 
 """holds the mapping for the SRR autodetect feature, can be modified at runtime if needed"""
 control_number_to_mode: Dict[int, stationmode] = {
     1: stationmode.CLEAR,
     2: stationmode.CHECK,
     3: stationmode.START,
     4: stationmode.FINISH
```

### Comparing `sipyconfig-1.2.0/src/sipyconfig/station.py` & `sipyconfig-1.2.1/src/sipyconfig/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 STANDARD_PORT = "/dev/ttyUSB{0:d}"
 STANDARD_SERIAL_TIMEOUT = 5
 BAUDRATE_EXTENDED = 38400
 BAUDRATE_STANDARD = 4800
 STANDARD_MAX_COMMAND_TRIES = 32
 
+
 class SiUSBStation():
     """main class for interfacing with the SI Station
     NOTE: only stations with extended protocol are currently supported"""
     _dev: 'Serial' = None
     _device_port: str
     _extended_protocol: bool = True
     _direct_mode: Optional[bool] = None
@@ -62,39 +63,41 @@
     _time_read_at: 'datetime'
 
     _command_tries: int = 0
     _serial_timeout: float = STANDARD_SERIAL_TIMEOUT
     _max_command_tries: int = STANDARD_MAX_COMMAND_TRIES
     _currently_waiting: bool = False
 
-    def __init__(self, device: str = None, mode_direct: bool = True) -> None:
+    def __init__(self, device: str | None = None, mode_direct: bool = True) -> None:
         self._sys_data = []
 
         self._init_serial(device)
         self._station_detect_procedure()
         self.set_mode_direct(mode_direct)
         self.get_system_info()
 
-    def _init_serial(self, device: str = None, baudrate: int = BAUDRATE_EXTENDED) -> None:
+    def _init_serial(self, device: str | None = None, baudrate: int = BAUDRATE_EXTENDED) -> None:
         if self._dev:
             self._dev.close()
         if device:
-            self._dev = Serial(device, baudrate=baudrate, timeout=self._serial_timeout)
+            self._dev = Serial(device, baudrate=baudrate,
+                               timeout=self._serial_timeout)
             if self._dev is None:
                 raise SiError("Could not open device!")
             self._device_port = device
             self.flush()
             return
         for i in range(128):
             try:
-                self._dev = Serial(STANDARD_PORT.format(i), baudrate, timeout=self._serial_timeout)
+                self._dev = Serial(STANDARD_PORT.format(
+                    i), baudrate, timeout=self._serial_timeout)
                 self._device_port = STANDARD_PORT.format(i)
                 self.flush()
                 return
-            except SerialException:
+            except (SerialException, BrokenPipeError):
                 continue
         raise SiError("Could not open device!")
 
     def _station_detect_procedure(self) -> bool:
         self._extended_protocol = True
         if self.set_mode_direct():
             return True
@@ -129,50 +132,61 @@
 
     def set_baudrate(self, high_baudrate: bool = True) -> None:
         """set the baudrate of the station to the defined lower (False) or higher (True) baudrate"""
         self.send_command(com.SET_BAUDRATE, [int(high_baudrate)], True)
 
     def get_system_info(self) -> None:
         """retreive the system info from the station"""
-        ret = self.send_command(com.GET_SYS_DATA, [memaddr.MEM_SIZE, memlen.MEM_SIZE], True)
+        ret = self.send_command(
+            com.GET_SYS_DATA, [memaddr.MEM_SIZE, memlen.MEM_SIZE], True)
         if isinstance(ret, Command):
             self._mem_size = ret.data[misc.DATA_COMMAND_OFFSET]
-            ret = self.send_command(com.GET_SYS_DATA, [0x00, self._mem_size], True)
+            ret = self.send_command(
+                com.GET_SYS_DATA, [0x00, self._mem_size], True)
             if isinstance(ret, Command):
-                self._sys_data = [x for x in ret.data[misc.DATA_COMMAND_OFFSET:]]
+                self._sys_data = [
+                    x for x in ret.data[misc.DATA_COMMAND_OFFSET:]]
 
                 cn1, cn0 = ret.data[0], ret.data[1]
                 self._control_number = (cn1 << 8) + cn0
 
-                self._model_id = MODELID(bytes(self._sys_data[memaddr.MODEL_ID:memaddr.MODEL_ID+memlen.MODEL_ID]))
-                self._model_id_str = model_rev.get(self._model_id.value, "UNKNOWN")
+                self._model_id = MODELID(
+                    bytes(self._sys_data[memaddr.MODEL_ID:memaddr.MODEL_ID+memlen.MODEL_ID]))
+                self._model_id_str = model_rev.get(
+                    self._model_id.value, "UNKNOWN")
 
                 self._mode = stationmode(self._sys_data[memaddr.MODE] & 0x3f)
                 if self._mode == stationmode.SIAC_SPECIAL:
                     self._control_number = self._sys_data[memaddr.CONTROL_NUMBER]
-                    self._mode_str = mode_rev.get(self._control_number, "UNKNOWN")
+                    self._mode_str = mode_rev.get(
+                        self._control_number, "UNKNOWN")
                 else:
                     self._mode_str = mode_rev.get(self._mode, "UNKNOWN")
 
                 self._siac_mode = siacmode(self._sys_data[memaddr.MODE] & 0xf0)
-                self._siac_mode_str = siacmode_rev.get(self._siac_mode, "NO_SIAC")
+                self._siac_mode_str = siacmode_rev.get(
+                    self._siac_mode, "NO_SIAC")
 
                 self._setting = self._sys_data[memaddr.SETTINGS_FLAG]
-                self._optical_feedback = bool(self._setting & SETTINGS.OPTICAL_FEEDBACK)
-                self._acoustic_feedback = bool(self._setting & SETTINGS.ACOUSTIC_FEEDBACK)
-                self._control_number_high_bit = bool(self._setting & SETTINGS.NUMBER_HIGH_BIT)
+                self._optical_feedback = bool(
+                    self._setting & SETTINGS.OPTICAL_FEEDBACK)
+                self._acoustic_feedback = bool(
+                    self._setting & SETTINGS.ACOUSTIC_FEEDBACK)
+                self._control_number_high_bit = bool(
+                    self._setting & SETTINGS.NUMBER_HIGH_BIT)
 
                 self._cpc = self._sys_data[memaddr.PROTOCOL_MODE_FLAG]
                 self._cpc_ext_protocol = bool(self._cpc & CPC.EXTENDED_PROTCOL)
                 self._auto_send = bool(self._cpc & CPC.AUTO_SEND)
                 self._handshake = bool(self._cpc & CPC.HANDSHAKE)
                 self._access_password = bool(self._cpc & CPC.ACCESS_PASSWORD)
                 self._read_after_punch = bool(self._cpc & CPC.READ_AFTER_PUNCH)
 
-                self._operating_time = bytes_to_int(self._sys_data[memaddr.ACTIVE_TIME:memaddr.ACTIVE_TIME+memlen.ACTIVE_TIME])
+                self._operating_time = bytes_to_int(
+                    self._sys_data[memaddr.ACTIVE_TIME:memaddr.ACTIVE_TIME+memlen.ACTIVE_TIME])
         self.get_time()
 
     def get_time(self) -> None:
         """get the current time of the station"""
         ret = self.send_command(com.GET_TIME, [], True)
         if isinstance(ret, Command):
             self._time = self._decode_time(ret.data[2:])
@@ -187,15 +201,16 @@
         seconds = bytes_to_int(raw_data[4:6])
         hour = seconds // 3600
         seconds -= hour * 3600
         minute = seconds // 60
         seconds -= minute * 60
         microseconds = int(raw_data[6] * (1e6 / 256))
 
-        ret_time = datetime(year, month, day, hour, minute, seconds, microseconds)
+        ret_time = datetime(year, month, day, hour,
+                            minute, seconds, microseconds)
 
         if (raw_data[3] << 7) & 0xFF:
             ret_time += timedelta(hours=12)
         return ret_time
 
     def set_time(self, time_: 'datetime' = None) -> None:
         """set the current time of the station, if time_ is omitted the current computer time will be set"""
@@ -216,76 +231,86 @@
         seconds = time_.hour * 3600 + time_.minute * 60 + time_.second
         data.extend([x for x in seconds.to_bytes(2, "big")])
         data.append(0x00)
         return bytes(data)
 
     def set_operating_time(self, operating_time: int) -> None:
         """set the operating time span of the station in minutes, (2-5759)"""
-        self.send_command(com.SET_SYS_DATA, bytes([memaddr.ACTIVE_TIME]) + operating_time.to_bytes(2, "big"))
+        self.send_command(com.SET_SYS_DATA, bytes(
+            [memaddr.ACTIVE_TIME]) + operating_time.to_bytes(2, "big"))
         self.get_system_info()
 
     def _splice_control_number(self, sys_data: List[int], num: int) -> List[int]:
         sys_data[memaddr.CONTROL_NUMBER] = num & 0xFF
         sys_data[memaddr.SETTINGS_FLAG] = self._setting | SETTINGS.NUMBER_HIGH_BIT if num > 255 else self._setting & ~SETTINGS.NUMBER_HIGH_BIT
         return sys_data
 
     def set_control_number(self, num: int) -> None:
         """set the control number of the station, supported range (1-511). IMPORTANT: some older SI Chip only support numbers till 255!"""
         if not 0 < num < 512:
             raise ValueError("Only supports values between 1 and 511")
         sys_data = self._splice_control_number(self._sys_data.copy(), num)
-        self.send_command(com.SET_SYS_DATA, [int(memaddr.CONTROL_NUMBER)] + sys_data[memaddr.CONTROL_NUMBER:memaddr.SETTINGS_FLAG+1], True)
+        self.send_command(com.SET_SYS_DATA, [int(
+            memaddr.CONTROL_NUMBER)] + sys_data[memaddr.CONTROL_NUMBER:memaddr.SETTINGS_FLAG+1], True)
         self.get_system_info()
 
     def set_mode(self, mode: stationmode) -> None:
         """set the operating mode of the station"""
         sys_copy = self._sys_data.copy()
         if mode == stationmode.SIAC_TEST:
-            sys_copy = self._splice_control_number(sys_copy, stationmode.SIAC_ON)
+            sys_copy = self._splice_control_number(
+                sys_copy, stationmode.SIAC_ON)
         elif is_siac_special_mode(mode):
             sys_copy = self._splice_control_number(sys_copy, mode)
             mode = stationmode.SIAC_SPECIAL
         if not is_siac_mode(mode):
             self._siac_mode = siacmode.NO_SIAC
-        sys_copy[memaddr.SIAC] = misc.SIAC_ON if is_siac_mode(mode) else misc.SIAC_OFF
+        sys_copy[memaddr.SIAC] = misc.SIAC_ON if is_siac_mode(
+            mode) else misc.SIAC_OFF
         sys_copy[memaddr.MODE] = mode | self.siac_mode
-        self.send_command(com.SET_SYS_DATA, [int(memaddr.SIAC)] + sys_copy[memaddr.SIAC:memaddr.SETTINGS_FLAG+1], True)
+        self.send_command(com.SET_SYS_DATA, [int(
+            memaddr.SIAC)] + sys_copy[memaddr.SIAC:memaddr.SETTINGS_FLAG+1], True)
         self.get_system_info()
 
     def set_siac_mode(self, siac_mode: siacmode) -> None:
         """set SIAC SRR behaviour (only for SIAC_CONTROL, SIAC_START, SIAC_FINISH)"""
         if not is_siac_mode(self.mode):
             raise SiError("Can't set SIAC SRR behaviour for current mode!")
-        self.send_command(com.SET_SYS_DATA, [int(memaddr.MODE), self.mode | siac_mode], True)
+        self.send_command(com.SET_SYS_DATA, [int(
+            memaddr.MODE), self.mode | siac_mode], True)
         self.get_system_info()
 
     def set_protocol_setting(self, setting: CPC, set_val: bool):
         """set a single setting of the protocol settings byte"""
-        sett = apply_bit_mask(self._cpc, setting, set_val << (log2(setting) - 1))
+        sett = apply_bit_mask(self._cpc, setting,
+                              set_val << (log2(setting) - 1))
         if setting in [CPC.AUTO_SEND, CPC.HANDSHAKE]:
             setting = CPC.AUTO_SEND if setting == CPC.HANDSHAKE else CPC.HANDSHAKE
-            sett = apply_bit_mask(sett, setting, int(not set_val) << (log2(setting) - 1))
-        self.send_command(com.SET_SYS_DATA, [memaddr.PROTOCOL_MODE_FLAG, sett], True)
+            sett = apply_bit_mask(sett, setting, int(
+                not set_val) << (log2(setting) - 1))
+        self.send_command(com.SET_SYS_DATA, [
+                          memaddr.PROTOCOL_MODE_FLAG, sett], True)
 
     def set_protocol_settings(self, settings: List[CPC], values: List[int]) -> None:
         """set multiple settings of the protocol settings byte at once. length of settings and values has to be equal"""
         values = [val << log2(sett - 1) for sett, val in zip(settings, values)]
         self.send_command(com.SET_SYS_DATA,
-                        [memaddr.PROTOCOL_MODE_FLAG, apply_bit_mask(self._cpc, array_or([int(x) for x in settings]), array_or(values))], True)
+                          [memaddr.PROTOCOL_MODE_FLAG, apply_bit_mask(self._cpc, array_or([int(x) for x in settings]), array_or(values))], True)
         self.get_system_info()
 
     def set_setting(self, setting: SETTINGS, set_val: bool):
         """set a single setting of the settings byte"""
-        self.send_command(com.SET_SYS_DATA, [memaddr.SETTINGS_FLAG, apply_bit_mask(self._setting, setting, set_val << setting)], True)
+        self.send_command(com.SET_SYS_DATA, [memaddr.SETTINGS_FLAG, apply_bit_mask(
+            self._setting, setting, set_val << setting)], True)
 
     def set_settings(self, settings: List[SETTINGS], values: List[int]) -> None:
         """set multiple settings of the settings byte at once. length of settings and values has to be equal"""
         values = [val << log2(sett - 1) for sett, val in zip(settings, values)]
         self.send_command(com.SET_SYS_DATA,
-                        [memaddr.SETTINGS_FLAG, apply_bit_mask(self._setting, array_or([int(x) for x in settings]), array_or(values))], True)
+                          [memaddr.SETTINGS_FLAG, apply_bit_mask(self._setting, array_or([int(x) for x in settings]), array_or(values))], True)
         self.get_system_info()
 
     def turn_off(self) -> None:
         """Turn off the connected station, is only effective in remote mode (mode_direct = False)"""
         self.send_command(com.TURN_OFF, [], True)
 
     def trigger_feedback(self, num: int = 1) -> bool:
@@ -302,15 +327,16 @@
         self.set_mode(stationmode.READOUT)
         self.set_protocol_setting(CPC.AUTO_SEND, False)
         self.get_system_info()
 
     def ensure_control_readout(self, control_number: int = None, enable_siac: bool = False):
         """ensures that the station is configured to receive SI Punches in Control Mode"""
         self.set_mode_direct(True)
-        self.set_mode(stationmode.SIAC_CONTROL if enable_siac else stationmode.CONTROL)
+        self.set_mode(
+            stationmode.SIAC_CONTROL if enable_siac else stationmode.CONTROL)
         if control_number is not None:
             self.set_control_number(control_number)
         self.set_protocol_setting(CPC.AUTO_SEND, True)
         self.get_system_info()
 
     def wait_for_si_card(self, timeout: float = None, *, no_ack: bool = False, auto_detect_srr: bool = False) -> Optional[SICard]:
         """waits for an SiCard to be inserted, waits a maximum of timeout (infinite if unset),
@@ -332,19 +358,19 @@
             except SiCardAutoSend:
                 return self._si_card
             finally:
                 self._currently_waiting = False
             if timeout is not None and time.time() - invoke_time >= timeout:
                 return None
 
-    def sendACK(self): # pylint: disable=invalid-name
+    def sendACK(self):  # pylint: disable=invalid-name
         """send a ACK packet to the station"""
         self._dev.write([proto.ACK])
 
-    def sendNAK(self): # pylint: disable=invalid-name
+    def sendNAK(self):  # pylint: disable=invalid-name
         """send a NOACK packet to the station"""
         self._dev.write([proto.NAK])
 
     def send_command(self, command_code: com, data: Union[bytes, List[int]], retry: bool = True) -> Union[ACK, NOACK, Command]:
         """send a command to the station with data, if retry = True the command is retried a maximum of max_command_tries if receiving a NOACK response"""
         send_command(command_code, data, self._dev)
         ret = self.receive_command()
@@ -373,15 +399,16 @@
                 raise SiCardInserted("SI-Card insert during command.")
             elif ret.command_code == com.DETECT_SI_8:
                 self._si_card = SI8To10.switch_types(ret.data[2:], self)
                 raise SiCardInserted("SI-Card insert during command.")
             elif ret.command_code == com.SI_REMOVED:
                 raise SiCardRemoved("SI-Card removed during command.")
             elif ret.command_code == com.PUNCH_DATA:
-                self._si_card = SICard.from_auto_send(ret.data, auto_detect_srr=auto_detect_srr)
+                self._si_card = SICard.from_auto_send(
+                    ret.data, auto_detect_srr=auto_detect_srr)
                 raise SiCardAutoSend("SI-Card insert with auto send enabled.")
         return ret
 
     def flush(self, flush_input: bool = True, flush_output: bool = True):
         """flush input and output buffer of the serial interface"""
         if flush_input:
             self._dev.flushInput()
```

### Comparing `sipyconfig-1.2.0/src/sipyconfig/utils.py` & `sipyconfig-1.2.1/src/sipyconfig/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,64 +6,73 @@
 
 from sipyconfig.enums import stationmode
 
 if TYPE_CHECKING:
     from sipyconfig.card import SICard
     from typing import Iterable, List, Union
 
+
 def log2(number: int) -> int:
     """returns length of number in binary without leading zeros"""
     return len(format(number, "b"))
 
+
 def apply_bit_mask(number: int, mask: int, value: int) -> int:
     """sets number to value if mask (works bitwise)"""
     length = max(log2(x) for x in [number, mask, value])
     num_bin = format(number, f"0{length}b")
     mask_bin = format(mask, f"0{length}b")
     value_bin = format(value, f"0{length}b")
     result = "".join(v if int(m) else n for n, m,
                      v in zip(num_bin, mask_bin, value_bin))
     return int(result, 2)
 
+
 def array_or(array: 'List[int]') -> int:
     """return bitwise or of all elements of the list"""
     result = 0
     for num in array:
         result |= num
     return result
 
+
 def is_siac_special_mode(station_mode: int) -> bool:
     """returns True if mode is a SIAC special mode"""
     return station_mode in [stationmode.SIAC_BATTERY_TEST, stationmode.SIAC_ON, stationmode.SIAC_OFF, stationmode.SIAC_RADIO_READOUT, stationmode.SIAC_TEST]
 
+
 def is_siac_mode(station_mode: int) -> bool:
     """returns True if mode is a SIAC mode"""
     return is_siac_special_mode(station_mode) or station_mode in [stationmode.SIAC_CONTROL, stationmode.SIAC_START,
-                                                                stationmode.SIAC_FINISH, stationmode.SIAC_TEST, stationmode.SIAC_SPECIAL]
+                                                                  stationmode.SIAC_FINISH, stationmode.SIAC_TEST, stationmode.SIAC_SPECIAL]
+
 
 def evenhex(num: int) -> str:
     """return hex() of num with leading zeros to make len() even"""
     hex_text = hex(num)[2:]
     if len(hex_text) % 2 != 0:
         return f"0x0{hex_text}"
     return f"0x{hex_text}"
 
+
 def hextoascii(num: int) -> str:
     """return ascii of num if num between 32 and 126 ('normal' character)"""
     if 32 <= num <= 126:
         return chr(num)
     return evenhex(num)
 
+
 def bytes_to_int(data: 'Union[bytes, List[int]]') -> int:
     """return int of bytes"""
     value = 0
     for offset, byte in enumerate([x for x in data][::-1]):
         value += byte << offset*8
     return value
 
+
 def print_si_card(card: 'SICard'):
     """pretty print data stored in an SICard Object"""
     print(f"""
 {card}
 clear:  {card.cleartime}
 check:  {card.checktime}
 start:  {card.starttime}
@@ -77,14 +86,15 @@
 other data:    {card.other_data}
 
 {len(card.punches)} punches:""")
 
     for i, punch in enumerate(card.punches):
         print(f"{i+1:03d} - {punch}")
 
+
 def combine_punches(cards: 'Iterable[SICard]') -> 'List[SICard]':
     """combines all punches of the same card"""
     ret: 'List[SICard]' = []
     for card in cards:
         if len(ret) == 0:
             ret.append(card)
             continue
```

### Comparing `sipyconfig-1.2.0/src/sipyconfig.egg-info/PKG-INFO` & `sipyconfig-1.2.1/src/sipyconfig.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: sipyconfig
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python replacement for the functionality of SportIdent Config+
 Home-page: https://gitlab.com/Teigi/sipyconfig
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 4 - Beta
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyserial
 
 # SportIdent Config+ Implementation
 
 A python implementation of the functionality of SPORTident Config+.
 
 Currently only working and tested under Linux.
```

### Comparing `sipyconfig-1.2.0/test/test_gui.py` & `sipyconfig-1.2.1/test/test_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # pylint: disable=C0114,C0115,C0116,invalid-name,too-few-public-methods,no-name-in-module,attribute-defined-outside-init
 
 from typing import Union, List
 from serial import SerialException, SerialTimeoutException
 
 from PyQt5.QtWidgets import (QApplication, QWidget, QMainWindow, QLabel, QScrollArea,
-                            QCheckBox, QVBoxLayout, QHBoxLayout, QGridLayout, QTabWidget,
-                            QSpinBox, QRadioButton, QPushButton, QButtonGroup, QComboBox,
-                            QLineEdit, QErrorMessage)
+                             QCheckBox, QVBoxLayout, QHBoxLayout, QGridLayout, QTabWidget,
+                             QSpinBox, QRadioButton, QPushButton, QButtonGroup, QComboBox,
+                             QLineEdit, QErrorMessage)
 from PyQt5.QtCore import QThread, pyqtSignal, QTimer, Qt
 from PyQt5.QtGui import QMouseEvent, QIcon
 
 from sipyconfig import SiUSBStation
 from sipyconfig.card import SICard
 from sipyconfig.comms import ACK, NOACK, Command
 from sipyconfig.station import SiError
 from sipyconfig.enums import MODELID, siacmode, stationmode, com, com_rev
 from sipyconfig.utils import is_siac_mode, is_siac_special_mode, evenhex
 
+
 class ReadOutThread(QThread):
     cardRead = pyqtSignal(SICard)
     station: SiUSBStation
     should_stop: bool = False
 
     def setStation(self, station: SiUSBStation):
         self.station = station
@@ -35,14 +36,15 @@
             except SiError:
                 pass
         self.should_stop = False
 
     def setExit(self, do_exit: bool):
         self.should_stop = do_exit
 
+
 class ReadOutWidget(QScrollArea):
     lineSelected = pyqtSignal(int)
     cardSelected = pyqtSignal(SICard)
 
     _cards: List[SICard]
 
     def __init__(self,) -> None:
@@ -64,31 +66,32 @@
             self.main_lay.addWidget(wid, 0, i)
         self.main_lay.setRowStretch(1, 1)
         self.main_lay.setColumnStretch(1, 1)
         self.main_lay.setColumnStretch(3, 1)
         self.main_lay.setColumnStretch(4, 1)
 
     def _addLine(self, data: 'list'):
-        line = self.main_lay.rowCount() # 2
+        line = self.main_lay.rowCount()  # 2
         self.main_lay.setRowStretch(line - 1, 0)
 
         def mouseEvent(ev: QMouseEvent, line: int = line) -> None:
-            if ev.button() == QMouseEvent.LeftButton: # type: ignore
+            if ev.button() == QMouseEvent.LeftButton:  # type: ignore
                 self.lineSelected.emit(line - 1)
 
         widgets = [QLabel(str(line - 1))] + [QLabel(str(dat)) for dat in data]
         for i, wid in enumerate(widgets):
-            wid.mousePressEvent = mouseEvent # type: ignore
+            wid.mousePressEvent = mouseEvent  # type: ignore
             self.main_lay.addWidget(wid, line - 1, i)
         self.main_lay.setRowStretch(line, 1)
 
     def addSiCard(self, card: 'SICard'):
         data = [card.read_at, card.number, "", "", len(card.punches), ""]
         self._addLine(data)
 
+
 class MainWindow(QMainWindow):
 
     def __init__(self, device: str = None) -> None:
         super().__init__()
 
         self.setWindowTitle("SPORTident Py-Config")
         try:
@@ -139,15 +142,16 @@
         self.control_num_wid = QSpinBox()
         self.control_num_wid.setMinimum(1)
         self.control_num_wid.setMaximum(511)
         self.control_lay.addWidget(self.control_num_wid, 2, 1)
 
         self.station_mode_wid = QComboBox()
         self.station_mode_wid.addItems(stationmode.__members__.keys())
-        self.station_mode_wid.currentTextChanged.connect(self.updateGuiStationMode)
+        self.station_mode_wid.currentTextChanged.connect(
+            self.updateGuiStationMode)
         self.control_lay.addWidget(self.station_mode_wid, 3, 0, 1, 2)
 
         self.turn_off_wid = QPushButton("Turn Off")
         self.turn_off_wid.pressed.connect(self.turnOff)
         self.control_lay.addWidget(self.turn_off_wid, 3, 2)
 
         self.siac_mode_wid = QComboBox()
@@ -182,15 +186,16 @@
         self.read_out_sub_lay.addWidget(self.read_out_details)
         self.read_out_details.hide()
         self.read_out_lay.addLayout(self.read_out_sub_lay)
 
         self.read_out_thread = ReadOutThread()
         self.read_out_thread.cardRead.connect(self.read_out_table.addSiCard)
 
-        self.main_wid.currentChanged.connect(lambda x: self.toggleReadOut(False) if x != 1 else '')
+        self.main_wid.currentChanged.connect(
+            lambda x: self.toggleReadOut(False) if x != 1 else '')
 
         self.main_wid.addTab(self.read_out_wid, "Read Out")
 
     def initDebugWid(self):
         self.debug_lay = QGridLayout()
 
         self.debug_command_wid = QComboBox()
@@ -202,15 +207,16 @@
         self.debug_lay.addWidget(self.debug_value_wid, 2, 0)
 
         self.debug_apply_wid = QPushButton("Write!")
         self.debug_apply_wid.pressed.connect(self.debugApply)
         self.debug_lay.addWidget(self.debug_apply_wid, 3, 0)
 
         self.debug_read_output = QLabel()
-        self.debug_read_output.setTextInteractionFlags(Qt.TextSelectableByMouse)
+        self.debug_read_output.setTextInteractionFlags(
+            Qt.TextSelectableByMouse)
         self.debug_lay.addWidget(self.debug_read_output, 4, 0)
         self.debug_read_wid = QPushButton("Read!")
         self.debug_read_wid.pressed.connect(self.debugRead)
         self.debug_lay.addWidget(self.debug_read_wid, 5, 0)
 
         self.debug_lay.setRowStretch(self.debug_lay.rowCount(), 1)
         self.debug_wid = QWidget()
@@ -233,26 +239,30 @@
         except SiError as e:
             self.showError(e)
             return
         except SerialException:
             self.initSerial()
 
         self.control_num_wid.setValue(self.si.control_number)
-        self.control_num_wid.setDisabled(self.si.mode == stationmode.SIAC_SPECIAL or self.si.mode == stationmode.SIAC_TEST)
+        self.control_num_wid.setDisabled(
+            self.si.mode == stationmode.SIAC_SPECIAL or self.si.mode == stationmode.SIAC_TEST)
         self.station_mode_wid.setCurrentText(self.si.mode_string)
         self.siac_mode_wid.setCurrentText(self.si.siac_mode_string)
         self.turn_off_wid.setDisabled(bool(self.si.direct_mode))
 
-        self.control_num_wid.setDisabled(self.si.model_id == MODELID.SIMSSR1_AP)
+        self.control_num_wid.setDisabled(
+            self.si.model_id == MODELID.SIMSSR1_AP)
         self.direct_select.setDisabled(self.si.model_id == MODELID.SIMSSR1_AP)
         self.remote_select.setDisabled(self.si.model_id == MODELID.SIMSSR1_AP)
-        self.station_mode_wid.setDisabled(self.si.model_id == MODELID.SIMSSR1_AP)
+        self.station_mode_wid.setDisabled(
+            self.si.model_id == MODELID.SIMSSR1_AP)
 
     def updateGuiStationMode(self, mode: str):
-        self.control_num_wid.setDisabled(is_siac_special_mode(getattr(stationmode, mode)))
+        self.control_num_wid.setDisabled(
+            is_siac_special_mode(getattr(stationmode, mode)))
         if is_siac_mode(getattr(stationmode, mode)) and not is_siac_special_mode(getattr(stationmode, mode)):
             if not self.siac_mode_wid.isEnabled():
                 self.siac_mode_wid.setDisabled(False)
                 self.siac_mode_wid.setCurrentText("NO_RADIO")
         else:
             self.siac_mode_wid.setCurrentText("NO_SIAC")
             self.siac_mode_wid.setDisabled(True)
@@ -299,42 +309,46 @@
 
     def showError(self, ex: Exception):
         dia = QErrorMessage(self)
         dia.showMessage(str(ex))
 
     def applyChanges(self):
         try:
-            self.si._siac_mode = getattr(siacmode, self.siac_mode_wid.currentText()) # pylint: disable=protected-access
-            self.si.mode = getattr(stationmode, self.station_mode_wid.currentText())
+            self.si._siac_mode = getattr(
+                siacmode, self.siac_mode_wid.currentText())  # pylint: disable=protected-access
+            self.si.mode = getattr(
+                stationmode, self.station_mode_wid.currentText())
             if self.si.mode != stationmode.SIAC_SPECIAL and self.si.mode != stationmode.SIAC_TEST:
                 self.si.control_number = self.control_num_wid.value()
         except SiError as e:
             self.showError(e)
         self.updateGui()
 
     def debugApply(self):
         command = getattr(com, self.debug_command_wid.currentText())
         a = self.debug_value_wid.text()
         if len(a) % 2 != 0:
-            self.showError(ValueError("Need even number of characters to convert to bytes!"))
+            self.showError(ValueError(
+                "Need even number of characters to convert to bytes!"))
             return
-        value = [int(a[x:x+2], 16) for x in range(0,len(a),2)]
+        value = [int(a[x:x+2], 16) for x in range(0, len(a), 2)]
         try:
             self.writeDebugRead(self.si.send_command(command, value, True))
         except SiError as e:
             self.showError(e)
         self.updateGui()
 
     def writeDebugRead(self, ret: Union[ACK, NOACK, Command]):
         if isinstance(ret, ACK):
             self.debug_read_output.setText("ACK")
         elif isinstance(ret, NOACK):
             self.debug_read_output.setText("NOACK")
         else:
-            self.debug_read_output.setText(com_rev.get(ret.command_code, evenhex(ret.command_code)) + " - " + " ".join(evenhex(x) for x in ret.data))
+            self.debug_read_output.setText(com_rev.get(ret.command_code, evenhex(
+                ret.command_code)) + " - " + " ".join(evenhex(x) for x in ret.data))
 
     def debugRead(self):
         try:
             self.writeDebugRead(self.si.receive_command())
         except (SiError, SerialException, SerialTimeoutException) as e:
             self.showError(e)
```


# Comparing `tmp/pyopensky-2.5.tar.gz` & `tmp/pyopensky-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopensky-2.5.tar", max compression
+gzip compressed data, was "pyopensky-2.6.tar", max compression
```

## Comparing `pyopensky-2.5.tar` & `pyopensky-2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     7652 2024-03-19 14:44:03.350002 pyopensky-2.5/license.txt
--rw-r--r--   0        0        0     1596 2024-03-19 14:44:03.350002 pyopensky-2.5/pyproject.toml
--rw-r--r--   0        0        0     1543 2024-03-19 14:44:03.350002 pyopensky-2.5/readme.md
--rw-r--r--   0        0        0       75 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/__init__.py
--rw-r--r--   0        0        0     2390 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/api.py
--rw-r--r--   0        0        0     6841 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/config.py
--rw-r--r--   0        0        0    54747 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/impala.py
--rw-r--r--   0        0        0        0 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/py.typed
--rw-r--r--   0        0        0    14927 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/rest.py
--rw-r--r--   0        0        0     4606 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/s3.py
--rw-r--r--   0        0        0    15012 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/schema.py
--rw-r--r--   0        0        0     1314 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/time.py
--rw-r--r--   0        0        0    32317 2024-03-19 14:44:03.350002 pyopensky-2.5/src/pyopensky/trino.py
--rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 pyopensky-2.5/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-04-12 10:45:35.407092 pyopensky-2.6/license.txt
+-rw-r--r--   0        0        0     1655 2024-04-12 10:45:35.407092 pyopensky-2.6/pyproject.toml
+-rw-r--r--   0        0        0     1588 2024-04-12 10:45:35.407092 pyopensky-2.6/readme.md
+-rw-r--r--   0        0        0       75 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/__init__.py
+-rw-r--r--   0        0        0     2390 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/api.py
+-rw-r--r--   0        0        0     6841 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/config.py
+-rw-r--r--   0        0        0    54747 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/impala.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/py.typed
+-rw-r--r--   0        0        0    14927 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/rest.py
+-rw-r--r--   0        0        0     4606 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/s3.py
+-rw-r--r--   0        0        0    16683 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/schema.py
+-rw-r--r--   0        0        0     1314 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/time.py
+-rw-r--r--   0        0        0    34748 2024-04-12 10:45:35.407092 pyopensky-2.6/src/pyopensky/trino.py
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 pyopensky-2.6/PKG-INFO
```

### Comparing `pyopensky-2.5/license.txt` & `pyopensky-2.6/license.txt`

 * *Files identical despite different names*

### Comparing `pyopensky-2.5/pyproject.toml` & `pyopensky-2.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "pyopensky"
-version = "2.5"
+version = "2.6"
 description = "A Python interface for OpenSky database"
+repository = "https://github.com/open-aviation/pyopensky/"
 authors = ["Xavier Olive <git@xoolive.org>", "Junzi Sun <j.sun-1@tudelft.nl>"]
 license = "MIT"
 readme = "readme.md"
 include = [
     "license.txt",
     "py.typed",
 ]
```

### Comparing `pyopensky-2.5/readme.md` & `pyopensky-2.6/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyopensky
 
 The `pyopensky` Python library provides functions to download data from the OpenSky Network live API and historical databases. It aims at making ADS-B and Mode S data from OpenSky easily accessible in the Python programming environment.
 
-Full documentation on https://open-aviation.github.io/pyopensky
+Full documentation on [https://open-aviation.github.io/pyopensky](https://open-aviation.github.io/pyopensky)
 
 ## Installation
 
 ```sh
 pip install pyopensky
 ```
```

### Comparing `pyopensky-2.5/src/pyopensky/api.py` & `pyopensky-2.6/src/pyopensky/api.py`

 * *Files identical despite different names*

### Comparing `pyopensky-2.5/src/pyopensky/config.py` & `pyopensky-2.6/src/pyopensky/config.py`

 * *Files identical despite different names*

### Comparing `pyopensky-2.5/src/pyopensky/impala.py` & `pyopensky-2.6/src/pyopensky/impala.py`

 * *Files identical despite different names*

### Comparing `pyopensky-2.5/src/pyopensky/rest.py` & `pyopensky-2.6/src/pyopensky/rest.py`

 * *Files identical despite different names*

### Comparing `pyopensky-2.5/src/pyopensky/s3.py` & `pyopensky-2.6/src/pyopensky/s3.py`

 * *Files identical despite different names*

### Comparing `pyopensky-2.5/src/pyopensky/schema.py` & `pyopensky-2.6/src/pyopensky/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,14 +63,25 @@
         if isinstance(value, (str, datetime)):
             value = pd.to_datetime(value, utc=True)
         if isinstance(value, pd.Timestamp):
             return float(value.timestamp())
         return super().process_bind_param(value, dialect)
 
 
+class AddressString(TypeDecorator[str]):
+    """Automatic coercing of icao24 addresses into low characters."""
+
+    impl = String
+
+    def process_bind_param(self, value: str | None, dialect: Dialect) -> Any:
+        if isinstance(value, str):
+            return value.lower()
+        return super().process_bind_param(value, dialect)
+
+
 class CallsignString(TypeDecorator[str]):
     """Automatic coercing of callsigns into 8-char left padded strings.
 
     Callsigns are decoded as 8 character strings, filled with spaces if needed.
     In practice, we trim the remaining spaces at the end of a callsign.
 
     When binding parameters, callsigns should be fit into 8 characters only when
@@ -118,15 +129,15 @@
     def __post_init__(self) -> None:
         if isinstance(self.time, int):
             self.time = pd.Timestamp(self.time, unit="s", tz="utc")
 
 
 @dataclass
 class AirportCandidateRow:
-    icao24: str
+    icao24: Address
     horizdistance: int
     vertdistance: int
 
 
 class TrackType(TypeDecorator[List[Dict[str, Any]]]):
     impl = ARRAY(String)
 
@@ -176,31 +187,33 @@
 ## For some types, the conversion is automatic (see `type_annotation_map`)
 
 AirportCandidates = List[AirportCandidateRow]
 Track = List[TrackRow]
 Sensors = List[SensorRow]
 
 Callsign = Annotated[str, mapped_column(CallsignString)]
+Address = Annotated[str, mapped_column(AddressString)]
 
 
 class Base(DeclarativeBase):
     type_annotation_map: ClassVar[dict[Any, Any]] = {
         pd.Timestamp: UTCTimestampInteger,
         AirportCandidates: AirportCandidateType,
         Track: TrackType,
         Callsign: CallsignString,
+        Address: AddressString,
         Sensors: SensorsType,
     }
 
 
 class StateVectorsData4(Base):
     __tablename__ = "state_vectors_data4"
 
     time: Mapped[pd.Timestamp]
-    icao24: Mapped[str]
+    icao24: Mapped[Address]
     lat: Mapped[float]
     lon: Mapped[float]
     velocity: Mapped[float]
     heading: Mapped[float]
     vertrate: Mapped[float]
     callsign: Mapped[Callsign]
     onground: Mapped[bool]
@@ -214,15 +227,15 @@
     serials: Mapped[List[int]] = mapped_column(ARRAY(Integer))  # TODO
     hour: Mapped[pd.Timestamp] = mapped_column(primary_key=True)
 
 
 class FlightsData4(Base):
     __tablename__ = "flights_data4"
 
-    icao24: Mapped[str]
+    icao24: Mapped[Address]
     firstseen: Mapped[pd.Timestamp]
     estdepartureairport: Mapped[str]
     lastseen: Mapped[pd.Timestamp]
     estarrivalairport: Mapped[str]
     callsign: Mapped[Callsign]
     track: Mapped[Track]
     estdepartureairporthorizdistance: Mapped[int]
@@ -239,15 +252,15 @@
     #   - we still need one column with a primary key
     day: Mapped[pd.Timestamp] = mapped_column(primary_key=True)
 
 
 class FlightsData5(Base):
     __tablename__ = "flights_data5"
 
-    icao24: Mapped[str]
+    icao24: Mapped[Address]
     firstseen: Mapped[pd.Timestamp]
     estdepartureairport: Mapped[str]
     lastseen: Mapped[pd.Timestamp]
     estarrivalairport: Mapped[str]
     callsign: Mapped[Callsign]
     track: Mapped[Track]
     estdepartureairporthorizdistance: Mapped[int]
@@ -276,25 +289,15 @@
 
 class RawTable(Protocol):
     sensors: Mapped[Sensors]
     rawmsg: Mapped[str]
     mintime: Mapped[pd.Timestamp]
     maxtime: Mapped[pd.Timestamp]
     msgcount: Mapped[int]
-    icao24: Mapped[str]
-    message: Mapped[str]
-    isid: Mapped[bool]
-    flightstatus: Mapped[int]
-    downlinkrequest: Mapped[int]
-    utilitymsg: Mapped[int]
-    interrogatorid: Mapped[int]
-    identifierdesignator: Mapped[int]
-    valuecode: Mapped[int]
-    altitude: Mapped[float]
-    identity: Mapped[str]
+    icao24: Mapped[Address]
 
     # Whatever, we pick this one as primary key BUT
     #   - this is not true
     #   - we still need one column with a primary key
     hour: Mapped[pd.Timestamp] = mapped_column(primary_key=True)
 
 
@@ -302,15 +305,15 @@
     __tablename__ = "acas_data4"
 
     sensors: Mapped[Sensors]
     rawmsg: Mapped[str]
     mintime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     maxtime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     msgcount: Mapped[int]
-    icao24: Mapped[str]
+    icao24: Mapped[Address]
     message: Mapped[str]
     isid: Mapped[bool]
     flightstatus: Mapped[int]
     downlinkrequest: Mapped[int]
     utilitymsg: Mapped[int]
     interrogatorid: Mapped[int]
     identifierdesignator: Mapped[int]
@@ -328,15 +331,15 @@
     __tablename__ = "allcall_replies_data4"
 
     sensors: Mapped[Sensors]
     rawmsg: Mapped[str]
     mintime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     maxtime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     msgcount: Mapped[int]
-    icao24: Mapped[str]
+    icao24: Mapped[Address]
     message: Mapped[str]
     isid: Mapped[bool]
     flightstatus: Mapped[int]
     downlinkrequest: Mapped[int]
     utilitymsg: Mapped[int]
     interrogatorid: Mapped[int]
     identifierdesignator: Mapped[int]
@@ -354,24 +357,17 @@
     __tablename__ = "identification_data4"
 
     sensors: Mapped[Sensors]
     rawmsg: Mapped[str]
     mintime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     maxtime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     msgcount: Mapped[int]
-    icao24: Mapped[str]
-    message: Mapped[str]
-    isid: Mapped[bool]
-    flightstatus: Mapped[int]
-    downlinkrequest: Mapped[int]
-    utilitymsg: Mapped[int]
-    interrogatorid: Mapped[int]
-    identifierdesignator: Mapped[int]
-    valuecode: Mapped[int]
-    altitude: Mapped[float]
+    icao24: Mapped[Address]
+    emittercategory: Mapped[int]
+    ftc: Mapped[int]
     identity: Mapped[str]
 
     # Whatever, we pick this one as primary key BUT
     #   - this is not true
     #   - we still need one column with a primary key
     hour: Mapped[pd.Timestamp] = mapped_column(primary_key=True)
 
@@ -381,24 +377,41 @@
 
     sensors: Mapped[Sensors]
     rawmsg: Mapped[str]
     mintime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     maxtime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     msgcount: Mapped[int]
     icao24: Mapped[str]
-    message: Mapped[str]
-    isid: Mapped[bool]
-    flightstatus: Mapped[int]
-    downlinkrequest: Mapped[int]
-    utilitymsg: Mapped[int]
-    interrogatorid: Mapped[int]
-    identifierdesignator: Mapped[int]
-    valuecode: Mapped[int]
-    altitude: Mapped[float]
-    identity: Mapped[str]
+    subtypecode: Mapped[int]
+    unknowncapcode: Mapped[bool]
+    unknownopcode: Mapped[bool]
+    hasoperationaltcas: Mapped[int]
+    has1090esin: Mapped[bool]
+    supportsairreferencedvelocity: Mapped[int]
+    haslowtxpower: Mapped[int]
+    supportstargetstatereport: Mapped[int]
+    supportstargetchangereport: Mapped[int]
+    hasuatin: Mapped[bool]
+    nacv: Mapped[int]
+    nicsupplementc: Mapped[int]
+    hastcasresolutionadvisory: Mapped[bool]
+    hasactiveidentswitch: Mapped[bool]
+    usessingleantenna: Mapped[bool]
+    systemdesignassurance: Mapped[int]
+    gpsantennaoffset: Mapped[int]
+    airplanelength: Mapped[int]
+    airplanewidth: Mapped[float]
+    version: Mapped[int]
+    nicsupplementa: Mapped[bool]
+    positionnac: Mapped[float]
+    geometricverticalaccuracy: Mapped[int]
+    sourceintegritylevel: Mapped[int]
+    barometricaltitudeintegritycode: Mapped[int]
+    trackheadinginfo: Mapped[int]
+    horizontalreferencedirection: Mapped[bool]
 
     # Whatever, we pick this one as primary key BUT
     #   - this is not true
     #   - we still need one column with a primary key
     hour: Mapped[pd.Timestamp] = mapped_column(primary_key=True)
 
 
@@ -406,15 +419,15 @@
     __tablename__ = "position_data4"
 
     sensors: Mapped[Sensors]
     rawmsg: Mapped[str]
     mintime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     maxtime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     msgcount: Mapped[int]
-    icao24: Mapped[str]
+    icao24: Mapped[Address]
     nicsuppla: Mapped[bool]
     hcr: Mapped[float]
     nic: Mapped[int]
     survstatus: Mapped[int]
     nicsupplb: Mapped[bool]
     odd: Mapped[bool]
     baroalt: Mapped[bool]
@@ -438,15 +451,15 @@
     __tablename__ = "rollcall_replies_data4"
 
     sensors: Mapped[Sensors]
     rawmsg: Mapped[str]
     mintime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     maxtime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     msgcount: Mapped[int]
-    icao24: Mapped[str]
+    icao24: Mapped[Address]
     message: Mapped[str]
     isid: Mapped[bool]
     flightstatus: Mapped[int]
     downlinkrequest: Mapped[int]
     utilitymsg: Mapped[int]
     interrogatorid: Mapped[int]
     identifierdesignator: Mapped[int]
@@ -464,23 +477,54 @@
     __tablename__ = "velocity_data4"
 
     sensors: Mapped[Sensors]
     rawmsg: Mapped[str]
     mintime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     maxtime: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
     msgcount: Mapped[int]
-    icao24: Mapped[str]
-    message: Mapped[str]
-    isid: Mapped[bool]
-    flightstatus: Mapped[int]
-    downlinkrequest: Mapped[int]
-    utilitymsg: Mapped[int]
-    interrogatorid: Mapped[int]
-    identifierdesignator: Mapped[int]
-    valuecode: Mapped[int]
-    altitude: Mapped[float]
-    identity: Mapped[str]
+    icao24: Mapped[Address]
+    supersonic: Mapped[bool]
+    intentchange: Mapped[bool]
+    ifrcapability: Mapped[bool]
+    nac: Mapped[int]
+    ewvelocity: Mapped[float]
+    nsvelocity: Mapped[float]
+    baro: Mapped[bool]
+    vertrate: Mapped[float]
+    geominurbaro: Mapped[float]  # typo confirmed
+    heading: Mapped[float]
+    velocity: Mapped[float]
+
+    # Whatever, we pick this one as primary key BUT
+    #   - this is not true
+    #   - we still need one column with a primary key
+    hour: Mapped[pd.Timestamp] = mapped_column(primary_key=True)
+
+
+class FlarmRaw(Base):
+    __tablename__ = "flarm_raw"
+
+    sensortype: Mapped[str]
+    sensorlatitude: Mapped[float]
+    sensorlongitude: Mapped[float]
+    sensoraltitude: Mapped[int]
+    timeatserver: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
+    timeatsensor: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
+    timestamp: Mapped[pd.Timestamp] = mapped_column(UTCTimestampFloat)
+    rawmessage: Mapped[str]
+    crc: Mapped[str]
+    rawsoftmessage: Mapped[str]
+    sensorname: Mapped[str]
+    ntperror: Mapped[float]
+    userfreqcorrection: Mapped[float]
+    autofreqcorrection: Mapped[float]
+    frequency: Mapped[float]
+    channel: Mapped[int]
+    snrdetector: Mapped[float]
+    snrdemodulator: Mapped[float]
+    typeogn: Mapped[bool]
+    crccorrect: Mapped[bool]
 
     # Whatever, we pick this one as primary key BUT
     #   - this is not true
     #   - we still need one column with a primary key
     hour: Mapped[pd.Timestamp] = mapped_column(primary_key=True)
```

### Comparing `pyopensky-2.5/src/pyopensky/time.py` & `pyopensky-2.6/src/pyopensky/time.py`

 * *Files identical despite different names*

### Comparing `pyopensky-2.5/src/pyopensky/trino.py` & `pyopensky-2.6/src/pyopensky/trino.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from trino.sqlalchemy import URL
 
 import pandas as pd
 
 from .api import HasBounds, OpenSkyDBAPI
 from .config import cache_path, trino_password, trino_username
 from .schema import (
+    FlarmRaw,
     FlightsData4,
     FlightsData5,
     RawTable,
     RollcallRepliesData4,
     StateVectorsData4,
 )
 from .time import timelike, to_datetime
@@ -379,14 +380,15 @@
         bounds: None
         | str
         | HasBounds
         | tuple[float, float, float, float] = None,
         departure_airport: None | str = None,
         arrival_airport: None | str = None,
         airport: None | str = None,
+        time_buffer: None | str | pd.Timedelta = None,
         cached: bool = True,
         compress: bool = False,
         limit: None | int = None,
         selected_columns: tuple[InstrumentedAttribute[Any] | str, ...] = (),
         **kwargs: Any,
     ) -> None | pd.DataFrame:
         """Get Traffic from the OpenSky Trino database.
@@ -431,14 +433,18 @@
             airport. Selects flights departing from the airport between the two
             timestamps;
         :param arrival_airport: a string for the ICAO identifier of the airport.
             Selects flights arriving at the airport between the two timestamps;
         :param airport: a string for the ICAO identifier of the airport. Selects
             flights departing from or arriving at the airport between the two
             timestamps;
+        :param time_buffer: (default: None) time buffer used to extend time
+            bounds for flights in the OpenSky flight tables: requests will get
+            flights between ``start - time_buffer`` and ``stop + time_buffer``.
+            If no airport is specified, the parameter is ignored.
 
         .. warning::
 
             - See :meth:`pyopensky.trino.flightlist` if you do not need any
               trajectory information.
             - If both departure_airport and arrival_airport are set, requested
               timestamps match the arrival time;
@@ -515,26 +521,34 @@
                 airport,
                 FlightsData4.estdepartureairport,
                 FlightsData4.estarrivalairport,
             )
 
             flight_query = flight_table.subquery()
             fd4 = aliased(FlightsData4, alias=flight_query, adapt_on_names=True)
-            stmt = (
-                select(StateVectorsData4)
-                .join(
-                    flight_query,
-                    (fd4.icao24 == StateVectorsData4.icao24)
-                    & (fd4.callsign == StateVectorsData4.callsign),
-                )
-                .where(
+
+            if isinstance(time_buffer, str):
+                time_buffer = pd.Timedelta(time_buffer)
+
+            stmt = select(StateVectorsData4).join(
+                flight_query,
+                (fd4.icao24 == StateVectorsData4.icao24)
+                & (fd4.callsign == StateVectorsData4.callsign),
+            )
+
+            if time_buffer is None:
+                stmt = stmt.where(
                     StateVectorsData4.time >= fd4.firstseen,
                     StateVectorsData4.time <= fd4.lastseen,
                 )
-            )
+            else:
+                stmt = stmt.where(
+                    StateVectorsData4.time >= (fd4.firstseen - time_buffer),
+                    StateVectorsData4.time <= (fd4.lastseen + time_buffer),
+                )
 
         stmt = self.stmt_where_str(stmt, icao24, StateVectorsData4.icao24)
         stmt = self.stmt_where_str(stmt, callsign, StateVectorsData4.callsign)
 
         if bounds is not None:
             if isinstance(bounds, str):
                 from cartes.osm import Nominatim
@@ -602,14 +616,71 @@
 
         if limit is not None:
             stmt = stmt.limit(limit)
 
         res = self.query(stmt, cached=cached, compress=compress)
 
         if res.shape[0] == 0:
+            return None
+
+        return res
+
+    def flarm(
+        self,
+        start: timelike,
+        stop: None | timelike = None,
+        *args: ColumnExpressionArgument[bool],
+        sensor_name: None | str | list[str] = None,
+        cached: bool = True,
+        compress: bool = False,
+        limit: None | int = None,
+        correct_only: bool = True,
+        extra_columns: tuple[InstrumentedAttribute[Any], ...] = (),
+        **kwargs: Any,
+    ) -> None | pd.DataFrame:
+        start_ts = to_datetime(start)
+        stop_ts = (
+            to_datetime(stop)
+            if stop is not None
+            else start_ts + pd.Timedelta("1d")
+        )
+        stmt = select(FlarmRaw).with_only_columns(
+            FlarmRaw.sensoraltitude,
+            FlarmRaw.sensorlatitude,
+            FlarmRaw.sensorlongitude,
+            FlarmRaw.sensorname,
+            FlarmRaw.timestamp,
+            FlarmRaw.timeatserver,
+            FlarmRaw.timeatsensor,
+            FlarmRaw.rawmessage,
+            *extra_columns,
+        )
+        if correct_only:
+            stmt = stmt.where(FlarmRaw.crccorrect)
+            stmt = stmt.where(FlarmRaw.rawmessage.is_not(None))
+
+        if sensor_name is not None:
+            stmt = self.stmt_where_str(stmt, sensor_name, FlarmRaw.sensorname)
+
+        for condition in args:
+            stmt = stmt.where(condition)
+
+        stmt = stmt.where(
+            FlarmRaw.timestamp >= start_ts,
+            FlarmRaw.timestamp <= stop_ts,
+            FlarmRaw.hour >= start_ts.floor("1h"),
+            FlarmRaw.hour < stop_ts.ceil("1h"),
+        )
+
+        if limit is not None:
+            stmt = stmt.limit(limit)
+
+        res = self.query(stmt, cached=cached, compress=compress)
+
+        if res.shape[0] == 0:
             return None
 
         return res
 
     def rawdata(
         self,
         start: timelike,
```

### Comparing `pyopensky-2.5/PKG-INFO` & `pyopensky-2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pyopensky
-Version: 2.5
+Version: 2.6
 Summary: A Python interface for OpenSky database
+Home-page: https://github.com/open-aviation/pyopensky/
 License: MIT
 Author: Xavier Olive
 Author-email: git@xoolive.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -17,21 +18,22 @@
 Requires-Dist: pandas (>=1.5)
 Requires-Dist: paramiko (>=2.7)
 Requires-Dist: pyarrow (>=11.0.0)
 Requires-Dist: pyjwt (>=2.7.0)
 Requires-Dist: tqdm (>=4.65.0)
 Requires-Dist: trino[sqlalchemy] (>=0.322)
 Requires-Dist: typing-extensions (>=4.5.0)
+Project-URL: Repository, https://github.com/open-aviation/pyopensky/
 Description-Content-Type: text/markdown
 
 # pyopensky
 
 The `pyopensky` Python library provides functions to download data from the OpenSky Network live API and historical databases. It aims at making ADS-B and Mode S data from OpenSky easily accessible in the Python programming environment.
 
-Full documentation on https://open-aviation.github.io/pyopensky
+Full documentation on [https://open-aviation.github.io/pyopensky](https://open-aviation.github.io/pyopensky)
 
 ## Installation
 
 ```sh
 pip install pyopensky
 ```
```


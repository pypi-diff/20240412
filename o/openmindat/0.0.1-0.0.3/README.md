# Comparing `tmp/openmindat-0.0.1.tar.gz` & `tmp/openmindat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmindat-0.0.1.tar", last modified: Fri Dec 15 07:09:38 2023, max compression
+gzip compressed data, was "openmindat-0.0.3.tar", last modified: Fri Apr 12 00:57:44 2024, max compression
```

## Comparing `openmindat-0.0.1.tar` & `openmindat-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2023-12-15 07:09:38.556135 openmindat-0.0.1/
--rw-r--r--   0 blc        (501) staff       (20)    11357 2023-09-28 23:58:40.000000 openmindat-0.0.1/LICENSE
--rw-r--r--   0 blc        (501) staff       (20)       17 2023-12-15 00:59:03.000000 openmindat-0.0.1/MANIFEST.in
--rw-r--r--   0 blc        (501) staff       (20)     3153 2023-12-15 07:09:38.555928 openmindat-0.0.1/PKG-INFO
--rw-r--r--   0 blc        (501) staff       (20)     2558 2023-12-15 07:06:59.000000 openmindat-0.0.1/README.md
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2023-12-15 07:09:38.554345 openmindat-0.0.1/openmindat/
--rw-r--r--   0 blc        (501) staff       (20)     3643 2023-12-14 23:36:46.000000 openmindat-0.0.1/openmindat/__init__.py
--rw-r--r--   0 blc        (501) staff       (20)    38755 2023-12-14 23:40:15.000000 openmindat-0.0.1/openmindat/geomaterials.py
--rw-r--r--   0 blc        (501) staff       (20)     2613 2023-12-14 23:36:54.000000 openmindat-0.0.1/openmindat/geomaterials_search.py
--rw-r--r--   0 blc        (501) staff       (20)    11277 2023-12-15 00:14:49.000000 openmindat-0.0.1/openmindat/localities.py
--rw-r--r--   0 blc        (501) staff       (20)     5934 2023-12-15 06:51:54.000000 openmindat-0.0.1/openmindat/mindat_api.py
--rw-r--r--   0 blc        (501) staff       (20)     8608 2023-12-14 23:37:08.000000 openmindat-0.0.1/openmindat/minerals_ima.py
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2023-12-15 07:09:38.555696 openmindat-0.0.1/openmindat.egg-info/
--rw-r--r--   0 blc        (501) staff       (20)     3153 2023-12-15 07:09:38.000000 openmindat-0.0.1/openmindat.egg-info/PKG-INFO
--rw-r--r--   0 blc        (501) staff       (20)      401 2023-12-15 07:09:38.000000 openmindat-0.0.1/openmindat.egg-info/SOURCES.txt
--rw-r--r--   0 blc        (501) staff       (20)        1 2023-12-15 07:09:38.000000 openmindat-0.0.1/openmindat.egg-info/dependency_links.txt
--rw-r--r--   0 blc        (501) staff       (20)        1 2023-12-15 07:09:38.000000 openmindat-0.0.1/openmindat.egg-info/not-zip-safe
--rw-r--r--   0 blc        (501) staff       (20)        9 2023-12-15 07:09:38.000000 openmindat-0.0.1/openmindat.egg-info/requires.txt
--rw-r--r--   0 blc        (501) staff       (20)       11 2023-12-15 07:09:38.000000 openmindat-0.0.1/openmindat.egg-info/top_level.txt
--rw-r--r--   0 blc        (501) staff       (20)       38 2023-12-15 07:09:38.556190 openmindat-0.0.1/setup.cfg
--rw-r--r--   0 blc        (501) staff       (20)     1039 2023-12-15 07:07:33.000000 openmindat-0.0.1/setup.py
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-12 00:57:44.107414 openmindat-0.0.3/
+-rw-r--r--   0 blc        (501) staff       (20)    11357 2023-09-28 23:58:40.000000 openmindat-0.0.3/LICENSE
+-rw-r--r--   0 blc        (501) staff       (20)      136 2024-04-09 06:30:41.000000 openmindat-0.0.3/MANIFEST.in
+-rw-r--r--   0 blc        (501) staff       (20)     4911 2024-04-12 00:57:44.107139 openmindat-0.0.3/PKG-INFO
+-rw-r--r--   0 blc        (501) staff       (20)     4375 2024-04-12 00:56:04.000000 openmindat-0.0.3/README.md
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-12 00:57:44.104996 openmindat-0.0.3/openmindat/
+-rw-r--r--   0 blc        (501) staff       (20)     4506 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/__init__.py
+-rw-r--r--   0 blc        (501) staff       (20)     8088 2024-04-12 00:35:16.000000 openmindat-0.0.3/openmindat/countries.py
+-rw-r--r--   0 blc        (501) staff       (20)     5384 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/dana8.py
+-rw-r--r--   0 blc        (501) staff       (20)    46983 2024-04-12 00:27:42.000000 openmindat-0.0.3/openmindat/geomaterials.py
+-rw-r--r--   0 blc        (501) staff       (20)     3810 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/geomaterials_search.py
+-rw-r--r--   0 blc        (501) staff       (20)    16008 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/localities.py
+-rw-r--r--   0 blc        (501) staff       (20)     8328 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/localities_age.py
+-rw-r--r--   0 blc        (501) staff       (20)     8369 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/localities_status.py
+-rw-r--r--   0 blc        (501) staff       (20)     8330 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/localities_type.py
+-rw-r--r--   0 blc        (501) staff       (20)     4465 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/locgeoregion2.py
+-rw-r--r--   0 blc        (501) staff       (20)     3873 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/locobject.py
+-rw-r--r--   0 blc        (501) staff       (20)    11800 2024-04-12 00:35:16.000000 openmindat-0.0.3/openmindat/mindat_api.py
+-rw-r--r--   0 blc        (501) staff       (20)    13419 2024-04-12 00:36:48.000000 openmindat-0.0.3/openmindat/minerals_ima.py
+-rw-r--r--   0 blc        (501) staff       (20)     5848 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/nickel_strunz.py
+-rw-r--r--   0 blc        (501) staff       (20)     3126 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/photo_count.py
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-12 00:57:44.106683 openmindat-0.0.3/openmindat.egg-info/
+-rw-r--r--   0 blc        (501) staff       (20)     4911 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/PKG-INFO
+-rw-r--r--   0 blc        (501) staff       (20)      642 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/SOURCES.txt
+-rw-r--r--   0 blc        (501) staff       (20)        1 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/dependency_links.txt
+-rw-r--r--   0 blc        (501) staff       (20)        1 2024-03-09 23:51:57.000000 openmindat-0.0.3/openmindat.egg-info/not-zip-safe
+-rw-r--r--   0 blc        (501) staff       (20)       16 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/requires.txt
+-rw-r--r--   0 blc        (501) staff       (20)       11 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/top_level.txt
+-rw-r--r--   0 blc        (501) staff       (20)       38 2024-04-12 00:57:44.107507 openmindat-0.0.3/setup.cfg
+-rw-r--r--   0 blc        (501) staff       (20)     1058 2024-04-12 00:52:52.000000 openmindat-0.0.3/setup.py
```

### Comparing `openmindat-0.0.1/LICENSE` & `openmindat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.1/openmindat/__init__.py` & `openmindat-0.0.3/openmindat/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,16 +34,34 @@
         >>> gr.elements_exc("Au,Ag")
         >>> gr.saveto("/path/to/geomaterials_data")
         
 Press q to quit.
 """
 from . import mindat_api
 from .minerals_ima import MineralsIMARetriever
+from .minerals_ima import MineralsIdRetriever
 from .geomaterials_search import GeomaterialSearchRetriever
 from .geomaterials import GeomaterialRetriever
+from .geomaterials import GeomaterialIdRetriever
+from .geomaterials import GeomaterialDictRetriever
+from .localities import LocalitiesRetriever
+from .localities import LocalitiesIdRetriever
+from .localities_age import LocalitiesAgeRetriever
+from .localities_age import LocalitiesAgeIdRetriever
+from .localities_status import LocalitiesStatusRetriever
+from .localities_status import LocalitiesStatusIdRetriever
+from .localities_type import LocalitiesTypeRetriever
+from .localities_type import LocalitiesTypeIdRetriever
+from .locgeoregion2 import GeoRegionRetriever
+from .locobject import LocobjectRetriever
+from .countries import CountriesListRetriever
+from .countries import CountriesIdRetriever
+from .dana8 import DanaRetriever
+from .nickel_strunz import StrunzRetriever
+from .photo_count import PhotoCountRetriever
 
 if __name__ == "__main__":
     # --------------------------------------------
     # Use case 1: Search for a geomaterial by name
     
     # Check the docstring for GeomaterialSearchRetriever for more information
     help(MineralsIMARetriever)
```

### Comparing `openmindat-0.0.1/openmindat/geomaterials.py` & `openmindat-0.0.3/openmindat/geomaterials.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from . import mindat_api
 from datetime import datetime
 
 class GeomaterialRetriever:
     """
     This module provides the GeomaterialRetriever class for retrieving geomaterial data from the Mindat API. This class offers various methods to specify query parameters for filtering and retrieving detailed information about geomaterials, such as minerals and rocks.
+    For more information visit: https://api.mindat.org/schema/redoc/#tag/geomaterials
 
     The class allows for setting parameters like birifrigence, cleavage type, color, crystal system, density, diaphaneity, chemical elements inclusion or exclusion, entry types, optical properties, and more. It provides flexibility through method chaining and supports saving the query results either to a specified directory or to the current directory.
 
     Usage:
         >>> gr = GeomaterialRetriever()
         >>> gr.cleavagetype('Distinct/Good').colour('blue').crystal_system(["Amorphous", "Hexagonal"]).save()
         >>> gr.density_max('9').density_min(8).save()
 
     Press q to quit.
     """
     
     def __init__(self) -> None:
+        self.end_point = 'geomaterials'
         self._params = {}
         self._init_params()
          # Flag to indicate if the geomaterials have been retrieved
 
     def _init_params(self):
         self._params.clear()
         self._params.update({'format': 'json'})
@@ -1240,55 +1242,316 @@
         '''
         self._params.update({
             'varietyof': VARIETYOF
         })
 
         return self
 
-    def saveto(self, OUTDIR = ''):
+    def saveto(self, OUTDIR = '', FILE_NAME = ''):
         '''
         Executes the query to retrieve the list of geomaterials and saves the results to a specified directory.
 
         Args:
             OUTDIR (str): The directory path where the retrieved geomaterials will be saved. If not provided, the current directory will be used.
+            FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
 
         Returns:
             None
 
         Example:
             >>> gr = GeomaterialRetriever()
-            >>> gr.saveto("/path/to/directory")
+            >>> gr.density_min(3.25).saveto("/path/to/directory")
 
         '''
 
         print("Retrieving geomaterials. This may take a while... ")
        
         params = self._params
         end_point = 'geomaterials'
         outdir = OUTDIR
+        file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_list(params, end_point, outdir)
+        ma.get_mindat_list(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
 
-    def save(self):
+    def save(self, FILE_NAME = ''):
         '''
         Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
 
+        Args:
+            FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+
         Returns:
             None
 
         Example:
             >>> gr = GeomaterialRetriever()
-            >>> gr.save()
+            >>> gr.density_min(3.25).save()
+
+        '''
+        file_name = FILE_NAME
+        
+        self.saveto('', file_name)
+        
+
+    def get_list(self):
+        '''
+        Executes the query to retrieve the list of geomaterials and returns the json object.
+
+        Returns:
+            list of dictionaries.
+
+        Example:
+            >>> gr = GeomaterialRetriever()
+            >>> geoObject = gr.density_min(3.25).get_list()
+
+        '''
+        
+        print("Retrieving geomaterials. This may take a while... ")
+       
+        params = self._params
+        end_point = self.end_point
+        
+        #clears params for next get statement     
+        self._init_params()
+        
+        ma = mindat_api.MindatApi()
+        return ma.get_mindat_list_object(params, end_point)
+
+
+class GeomaterialIdRetriever:
+    """
+    This module provides the GeomaterialIdRetriever class for returning geomaterial by id
+    For more information visit: https://api.mindat.org/schema/redoc/#tag/geomaterials/operation/geomaterials_retrieve
+
+    Usage:
+        >>> gir = GeomaterialIdRetriever()
+        >>> gir.id(5).save
+
+    Attributes:
+        id (int): An int to store id parameter.
+    """
+    
+    def __init__(self):
+        self.end_point = "geomaterials"
+        self.sub_endpoint = '0'
+        
+        self._params = {}
+        self._init_params()
+
+    def _init_params(self):
+        self._params.clear()
+        self._params = {'format': 'json'}
+
+    #ask about if this option of addint variety to this endpoint is a good idea
+    def id(self, ID, VARIETIES = None):
+        '''
+        Returns locality with matching id
+
+        Args:
+            id (INT): The locality id.
+            variety: optional toggle returning varieties with 'y', leave empty if varieties aren't wanted
+
+        Returns:
+            self: The GeomaterialIdRetriever() object.
+
+        Example:
+            >>> gir = GeomaterialIdRetriever()
+            >>> gir.id(2)
+            >>> gir.save()
+        '''
+        
+        try:
+            ID = int(ID)
+        except ValueError:
+            raise ValueError("Invalid input. ID must be a valid integer.")
+        
+        id = str(ID)
+        varieties = VARIETIES
+        
+        if varieties == 'y':
+            self.sub_endpoint = '/'.join([id, 'varieties'])
+        elif varieties != None:
+            raise ValueError(f"Invalid input for 'varieties': {varieties}")
+        else:
+            self.sub_endpoint = id
+        
+        return self
+    
+    def saveto(self, OUTDIR = '', FILE_NAME = ''):
+        '''
+            Executes the query to retrieve the Geomaterials with keywords and saves the results to a specified directory.
+
+            Args:
+                OUTDIR (str): The directory path where the retrieved Geomaterials will be saved. If not provided, the current directory will be used.
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+
+            Returns:
+                None
+
+            Example:
+                >>> gir = GeomaterialIdRetriever()
+                >>> gir.id(5).saveto("/path/to/directory", "geo5")
+        '''
+
+        print("Retrieving Geomaterials. This may take a while... ")
+
+        params = self._params
+        end_point = '/'.join([self.end_point, self.sub_endpoint])
+        outdir = OUTDIR
+        file_name = FILE_NAME
+
+        ma = mindat_api.MindatApi()
+        ma.get_mindat_item(params, end_point, outdir, file_name)
+
+        # reset the query parameters in case the user wants to make another query
+        self._init_params()
+    
+    def save(self, FILE_NAME = ''):
+        '''
+            Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
+
+            Args:
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+            
+            Returns:
+                None
+
+            Example:
+                >>> gir = GeomaterialIdRetriever()
+                >>> gir.id(5).save()
+        '''
+        file_name = FILE_NAME
+        
+        self.saveto('', file_name)
+        
+    def get_list(self):
+        '''
+        Executes the query to retrieve geomaterial with a corresponding id and returns a dictionary.
+
+        Returns:
+            List of DIctionaries.
+
+        Example:
+            >>> gir = GeomaterialIdRetriever()
+            >>> geo5 = gir.id(5).get_list()
 
         '''
-        self.saveto()
+        
+        print("Retrieving geomaterials. This may take a while... ")
+       
+        params = self._params
+        end_point = '/'.join([self.end_point, self.sub_endpoint])
+        
+        #clears params for next get statement     
+        self._init_params()
+        
+        ma = mindat_api.MindatApi()
+        return [ma.get_mindat_dict(params, end_point)]
+        
+        
+        
+        #NOT YET WORKING, check in to see if it returns list vs item
+class GeomaterialDictRetriever:
+    """
+    This module provides the GeomaterialDictRetriever class for returning geomaterial Dictionaries
+    For more information visit: https://api.mindat.org/schema/redoc/#tag/geomaterials/operation/geomaterials_dict_retrieve
+
+    Usage:
+        >>> gdr = GeomaterialDictRetriever()
+        >>> gdr.id(5)
+
+    Attributes:
+        id (int): An int to store id parameter.
+    """ 
+    
+    def __init__(self):
+        self.end_point = 'geomaterials/dict'
+        self.sub_endpoint = '0'
+        
+        self._params = {}
+        self._init_params()
+
+    def _init_params(self):
+        self._params.clear()
+        self._params = {'format': 'json'}
+    
+    def saveto(self, OUTDIR = '', FILE_NAME = ''):
+        '''
+            Executes the query to retrieve the Geomaterials with keywords and saves the results to a specified directory.
+
+            Args:
+                OUTDIR (str): The directory path where the retrieved Geomaterials will be saved. If not provided, the current directory will be used.
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+
+            Returns:
+                None
 
+            Example:
+                >>> gdr = GeomaterialDictRetriever()
+                >>> gdr.saveto("/path/to/directory", "geoDict")
+        '''
+
+        print("Retrieving Geomaterials. This may take a while... ")
+
+        params = self._params
+        end_point = self.end_point
+        outdir = OUTDIR
+        file_name = FILE_NAME
+
+        ma = mindat_api.MindatApi()
+        ma.get_mindat_item(params, end_point, outdir, file_name)
+
+        # reset the query parameters in case the user wants to make another query
+        self._init_params()
+    
+    def save(self, FILE_NAME = ''):
+        '''
+            Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
+
+            Args:
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+            
+            Returns:
+                None
+
+            Example:
+                >>> gdr = GeomaterialDictRetriever()
+                >>> gdr.save()
+        '''
+        file_name = FILE_NAME
+        
+        self.saveto('', file_name)   
+        
+    def get_list(self):
+        '''
+        Executes the query to retrieve the dictionary of geomaterials.
+
+        Returns:
+            dictionary.
+
+        Example:
+            >>> gdr = GeomaterialDictRetriever()
+            >>> geoDict = gdr.get_list()
+
+        '''
+        
+        print("Retrieving geomaterials. This may take a while... ")
+       
+        params = self._params
+        end_point = self.end_point
+        
+        #clears params for next get statement     
+        self._init_params()
+        
+        ma = mindat_api.MindatApi()
+        return [ma.get_mindat_dict(params, end_point)]
+        
 
 if __name__ == '__main__':
     gr = GeomaterialRetriever()
     # gr.cleavagetype('Distinct/Good').colour('blue').crystal_system(["Amorphous", "Hexagonal"]).save()
     gr.id__in("3337, 114").save()
     # print(gr.density_max('9').density_min(8).ordering('-name')._params)
```

### Comparing `openmindat-0.0.1/openmindat/geomaterials_search.py` & `openmindat-0.0.3/openmindat/geomaterials_search.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from . import mindat_api
 
 class GeomaterialSearchRetriever:
     """
     A class to facilitate the retrieval of geomaterial data from the Mindat API using search keywords. It enables users to construct queries based on specific keywords and offers functionality to save the retrieved data.
+    For more information visit: https://api.mindat.org/schema/redoc/#tag/geomaterials_search
 
     Methods:
         geomaterials_search(KEYWORDS): Updates the search query with specified keywords.
         saveto(OUTDIR): Executes the search query and saves the data to a specified directory.
         save(): Executes the search query and saves the data to the current directory.
 
     Usage:
         >>> gsr = GeomaterialSearchRetriever()
         >>> gsr.geomaterials_search("quartz, green, hexagonal").save()
 
     Press q to quit.
     """
     def __init__(self):
        self._params = {}
+       self.end_point = 'geomaterials_search'
     
     def _init_params(self):
         self._params.clear()
         self._params = {'format': 'json'}
 
     def geomaterials_search(self, KEYWORDS):
         '''
@@ -29,51 +31,81 @@
         Args:
             KEYWORDS (str): A string containing the keywords to search for. 
 
         Returns:
             self: The GeomaterialRetriever object, allowing for method chaining.
 
         Example:
-            >>> gr = GeomaterialRetriever()
-            >>> gr.geomaterials_search("quartz, green, hexagonal")
-            >>> gr.save()
-'''
+            >>> gsr = GeomaterialSearchRetriever()
+            >>> gsr.geomaterials_search("quartz, green, hexagonal")
+            >>> gsr.save()
+        '''
         keywords = KEYWORDS
         self._params.update({'q': keywords})
         return self
     
-    def saveto(self, OUTDIR = ''):
+    def saveto(self, OUTDIR = '', FILE_NAME = ''):
         '''
             Executes the query to retrieve the geomaterials with keywords and saves the results to a specified directory.
 
             Args:
                 OUTDIR (str): The directory path where the retrieved geomaterials will be saved. If not provided, the current directory will be used.
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
 
             Returns:
                 None
         '''
-
         print("Retrieving geomaterials. This may take a while... ")
         
         params = self._params
-        end_point = 'geomaterials_search'
+        end_point = self.end_point
         outdir = OUTDIR
+        file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_search(params, end_point, outdir)
+        ma.get_mindat_search(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
 
-    def save(self):
+    def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
 
+            Args:
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+
             Returns:
                 None
         '''
-        self.saveto()
+        file_name = FILE_NAME
+        
+        self.saveto('', file_name)
+        
+    def get_list(self):
+        '''
+        Executes the query to retrieve the geomaterial search data as a dictionary.
+
+        Returns:
+            List of dictionaries.
+
+        Example:
+            >>> gsr = geomaterialSeachRetriever()
+            >>> greenQuarts = gsr.geomaterial_search("quartz, green").get_list()
+
+        '''
+        
+        print("Retrieving geomaterial search. This may take a while... ")
+       
+        params = self._params
+        end_point = self.end_point
+        
+        #clears params for next get statement     
+        self._init_params()
+        
+        ma = mindat_api.MindatApi()
+        return [ma.get_mindat_dict(params, end_point)]
 
 
 if __name__ == '__main__':
     gsr = GeomaterialSearchRetriever()
     gsr.geomaterials_search("quartz, green, hexagonal").save()
```

### Comparing `openmindat-0.0.1/openmindat/localities.py` & `openmindat-0.0.3/openmindat/localities.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from . import mindat_api
 from datetime import datetime
 
 class LocalitiesRetriever:
     """
     This module provides the LocalitiesRetriever class for querying locality data from the Mindat API. The class enables users to construct queries based on various parameters such as country, description, included/excluded elements, and more. It supports method chaining for the flexible combination of query parameters and offers functionality to save the queried data either to a specified directory or the current directory.
+    For more information visit: https://api.mindat.org/schema/redoc/#tag/localities
 
     Usage:
         >>> lr = LocalitiesRetriever()
         >>> lr.country("France").description("quartz").saveto("/path/to/directory")
 
     Attributes:
         _params (dict): A dictionary to store query parameters.
@@ -29,14 +30,15 @@
         save(): Executes the query and saves the results to the current directory.
 
     Press q to quit.
     """
 
     def __init__(self):
         self._params = {}
+        self.end_point = 'localities'
         self._init_params()
 
     def _init_params(self):
         self._params.clear()
         self._params = {'format': 'json'}
         self.page_size(1500)
 
@@ -327,51 +329,204 @@
 
         self._params.update({
             'updated_at': DATE_STR
         })
 
         return self
     
-    def saveto(self, OUTDIR=''):
+    def saveto(self, OUTDIR = '', FILE_NAME = ''):
         '''
-            Executes the query to retrieve the geomaterials with keywords and saves the results to a specified directory.
+            Executes the query to retrieve the localities with keywords and saves the results to a specified directory.
 
             Args:
-                OUTDIR (str): The directory path where the retrieved geomaterials will be saved. If not provided, the current directory will be used.
+                OUTDIR (str): The directory path where the retrieved localities will be saved. If not provided, the current directory will be used.
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
 
             Returns:
                 None
 
             Example:
                 >>> lr = LocalitiesRetriever()
-                >>> lr.saveto("/path/to/directory")
+                >>> lr.saveto("/path/to/directory", "france")
         '''
 
         print("Retrieving localities. This may take a while... ")
 
         params = self._params
-        end_point = 'localities'
+        end_point = self.end_point
         outdir = OUTDIR
+        file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_list(params, end_point, outdir)
+        ma.get_mindat_list(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
     
-    def save(self):
+    def save(self, FILE_NAME = ''):
         '''
-            Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
+            Executes the query to retrieve the list of localities and saves the results to the current directory.
 
+            Args:
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+            
             Returns:
                 None
 
             Example:
                 >>> lr = LocalitiesRetriever()
                 >>> lr.save()
         '''
-        self.saveto()
+        file_name = FILE_NAME
+        
+        self.saveto('', file_name)
+        
+    def get_list(self):
+        '''
+        Executes the query to retrieve the list of localities and returns the json object.
+
+        Returns:
+            list of dictionaries.
 
+        Example:
+            >>> lr = LocalitiesRetriever()
+            >>> france = lr.country('France').get_list()
+
+        '''
+        
+        print("Retrieving localities. This may take a while... ")
+       
+        params = self._params
+        end_point = self.end_point
+        
+        #clears params for next get statement     
+        self._init_params()
+        
+        ma = mindat_api.MindatApi()
+        return ma.get_mindat_list_object(params, end_point)
+        
+        
+class LocalitiesIdRetriever:
+    """
+    This module provides the LocalitiesIdRetriever class for returning localities by id
+    For more information visit: https://api.mindat.org/schema/redoc/#tag/localities/operation/localities_retrieve
+
+    Usage:
+        >>> lir = LocalitiesIdRetriever()
+        >>> lir.id(5)
+
+    Attributes:
+        id (int): An int to store id parameter.
+    """
+    
+    def __init__(self):
+        self.end_point = 'localities'
+        self.sub_endpoint = '0'
+        
+        self._params = {}
+        self._init_params()
+
+    def _init_params(self):
+        self._params.clear()
+        self._params = {'format': 'json'}
+
+    def id(self, ID):
+        '''
+        Returns locality with matching id
+
+        Args:
+            id (INT): The locality id.
+
+        Returns:
+            self: The LocalitiesIdRetriever() object.
+
+        Example:
+            >>> lir = LocalitiesIdRetriever()
+            >>> lir.id(2)
+            >>> lir.save()
+        '''
+        
+        try:
+            ID = int(ID)
+        except ValueError:
+            raise ValueError("Invalid input. ID must be a valid integer.")
+        
+        id = str(ID)
+        
+        self.sub_endpoint = id
+        
+        return self
+    
+    def saveto(self, OUTDIR = '', FILE_NAME = ''):
+        '''
+            Executes the query to retrieve the localities with keywords and saves the results to a specified directory.
+
+            Args:
+                OUTDIR (str): The directory path where the retrieved localities will be saved. If not provided, the current directory will be used.
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+
+            Returns:
+                None
+
+            Example:
+                >>> lir = LocalitiesIdRetriever()
+                >>> lir.saveto("/path/to/directory", "france")
+        '''
+
+        print("Retrieving localities. This may take a while... ")
+
+        params = self._params
+        end_point = '/'.join([self.end_point, self.sub_endpoint])
+        outdir = OUTDIR
+        file_name = FILE_NAME
+
+        ma = mindat_api.MindatApi()
+        ma.get_mindat_item(params, end_point, outdir, file_name)
+
+        # reset the query parameters in case the user wants to make another query
+        self._init_params()
+    
+    def save(self, FILE_NAME = ''):
+        '''
+            Executes the query to retrieve the list of localities and saves the results to the current directory.
+
+            Args:
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+            
+            Returns:
+                None
+
+            Example:
+                >>> lir = LocalitiesIdRetriever()
+                >>> lir.save()
+        '''
+        file_name = FILE_NAME
+        
+        self.saveto('', file_name)
+        
+    def get_list(self):
+        '''
+        Executes the query to retrieve locality with a corresponding id and returns a dictionary.
+
+        Returns:
+            List of Dictionaries.
+
+        Example:
+                >>> lir = localitiesIdRetriever()
+                >>> locality5 = lir.id(5).get_list()
+
+        '''
+        
+        print("Retrieving localities. This may take a while... ")
+       
+        params = self._params
+        end_point = '/'.join([self.end_point, self.sub_endpoint])
+        
+        #clears params for next get statement     
+        self._init_params()
+        
+        ma = mindat_api.MindatApi()
+        return [ma.get_mindat_dict(params, end_point)]
 
 if __name__ == '__main__':
     lr = LocalitiesRetriever()
     lr.country("UK").save()
```

### Comparing `openmindat-0.0.1/openmindat/minerals_ima.py` & `openmindat-0.0.3/openmindat/minerals_ima.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from . import mindat_api
 from datetime import datetime
 
 class MineralsIMARetriever:
     '''
     A class for querying mineral data from the Mindat API. It supports various query parameters such as mineral IDs, IMA status, fields selection, and pagination. The class enables method chaining for building complex queries and provides functionalities to save the queried data either to a specified directory or the current directory.
+    For more information visit: https://api.mindat.org/schema/redoc/#tag/minerals_ima
 
     Usage:
         >>> mir = MineralsIMARetriever()
         >>> mir.ima(1).fields("id,name,ima_formula").saveto("/path/to/directory")
 
     Press q to quit.
     '''
     def __init__(self):
+        self.end_point = 'minerals_ima'
         self._params = {}
+        self._init_params()
 
     def _init_params(self):
         self._params.clear()
         self._params = {'format': 'json'}
+        self.page_size(1500)
 
     def expand(self, EXPAND_FIELDS):
         '''
         Expand the query to include related minerals and select specific fields to expand.
 
         Args:
             EXPAND_FIELDS(list[str] or str): The fields to expand. Valid options are:
@@ -245,51 +249,205 @@
 
         self._params.update({
             'updated_at': DATE_STR
         })
 
         return self
     
-    def saveto(self, OUTDIR=''):
+    def saveto(self, OUTDIR='', FILE_NAME = ''):
         '''
             Executes the query to retrieve the geomaterials with keywords and saves the results to a specified directory.
 
             Args:
                 OUTDIR (str): The directory path where the retrieved geomaterials will be saved. If not provided, the current directory will be used.
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
 
             Returns:
                 None
 
             Example:
                 >>> mir = MineralsIMARetriever()
                 >>> mir.saveto("/path/to/directory")
         '''
 
         print("Retrieving geomaterials. This may take a while... ")
 
         params = self._params
-        end_point = 'minerals_ima'
+        end_point = self.end_point
         outdir = OUTDIR
+        file_name = FILE_NAME
 
         ma = mindat_api.MindatApi()
-        ma.get_mindat_list(params, end_point, outdir)
+        ma.get_mindat_list(params, end_point, outdir, file_name)
 
         # reset the query parameters in case the user wants to make another query
         self._init_params()
     
-    def save(self):
+    def save(self, FILE_NAME = ''):
         '''
             Executes the query to retrieve the list of geomaterials and saves the results to the current directory.
 
+            Args:
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+                
             Returns:
                 None
 
             Example:
                 >>> mir = MineralsIMARetriever()
                 >>> mir.save()
         '''
-        self.saveto()
+        file_name = FILE_NAME
+        
+        self.saveto('', file_name)
+        
+    def get_list(self):
+        '''
+        Executes the query to retrieve the list of mineral data and returns the json object.
+
+        Returns:
+            list of dictionaries.
+
+        Example:
+                >>> mir = MineralsIMARetriever()
+                >>> quartsIMA = mir.q('quartz').get_list()
+
+        '''
+        
+        print("Retrieving minerals. This may take a while... ")
+       
+        params = self._params
+        end_point = self.end_point
+        
+        #clears params for next get statement     
+        self._init_params()
+        
+        ma = mindat_api.MindatApi()
+        return ma.get_mindat_list_object(params, end_point)
+        
+        
+class MineralsIdRetriever:
+    """
+    This module provides the MineralsIdRetriever class for returning Minerals by id
+    For more information visit: https://api.mindat.org/schema/redoc/#tag/minerals_ima/operation/minerals_ima_retrieve
+
+    Usage:
+        >>> midr = MineralsIdRetriever()
+        >>> midr.id(5)
+
+    Attributes:
+        id (int): An int to store id parameter.
+    """
+    
+    def __init__(self):
+        self.end_point = 'minerals_ima'
+        self.sub_endpoint = '0'
+        
+        self._params = {}
+        self._init_params()
+
+    def _init_params(self):
+        self._params.clear()
+        self._params = {'format': 'json'}
+
+    def id(self, ID):
+        '''
+        Returns locality with matching id
+
+        Args:
+            id (INT): The locality id.
+
+        Returns:
+            self: The MineralsIdRetriever() object.
+
+        Example:
+            >>> midr = MineralsIdRetriever()
+            >>> midr.id(2)
+            >>> midr.save()
+        '''
+        
+        try:
+            ID = int(ID)
+        except ValueError:
+            raise ValueError("Invalid input. ID must be a valid integer.")
+        
+        id = str(ID)
+        
+        self.sub_endpoint = id
+        
+        return self
+    
+    def saveto(self, OUTDIR = '', FILE_NAME = ''):
+        '''
+            Executes the query to retrieve the Minerals with keywords and saves the results to a specified directory.
+
+            Args:
+                OUTDIR (str): The directory path where the retrieved Minerals will be saved. If not provided, the current directory will be used.
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+
+            Returns:
+                None
+
+            Example:
+                >>> midr = MineralsIdRetriever()
+                >>> midr.id(3).saveto("/path/to/directory", "Mineral_ima_id")
+        '''
+
+        print("Retrieving Minerals. This may take a while... ")
+
+        params = self._params
+        end_point = '/'.join([self.end_point, self.sub_endpoint])
+        outdir = OUTDIR
+        file_name = FILE_NAME
+
+        ma = mindat_api.MindatApi()
+        ma.get_mindat_item(params, end_point, outdir, file_name)
+
+        # reset the query parameters in case the user wants to make another query
+        self._init_params()
+    
+    def save(self, FILE_NAME = ''):
+        '''
+            Executes the query to retrieve the list of minerals and saves the results to the current directory.
+
+            Args:
+                FILE_NAME (str): An optional file name, if no input is given it uses the end point as a name
+            
+            Returns:
+                None
+
+            Example:
+                >>> midr = MineralsIdRetriever()
+                >>> midr.id(3).save()
+        '''
+        file_name = FILE_NAME
+        
+        self.saveto('', file_name)
+        
+    def get_list(self):
+        '''
+        Executes the query to retrieve mineral IMA status with a corresponding id and returns a dictionary.
+
+        Returns:
+            List of Dictionaries.
+
+        Example:
+                >>> midr = MineralsIdRetriever()
+                >>> ima9 = midr.id(9).get_list()
+
+        '''
+        
+        print("Retrieving minerals. This may take a while... ")
+       
+        params = self._params
+        end_point = '/'.join([self.end_point, self.sub_endpoint])
+        
+        #clears params for next get statement     
+        self._init_params()
+        
+        ma = mindat_api.MindatApi()
+        return [ma.get_mindat_dict(params, end_point)]
 
 
 if __name__ == '__main__':
     mir = MineralsIMARetriever()
     mir.ima('1').saveto()
```

### Comparing `openmindat-0.0.1/setup.py` & `openmindat-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name='openmindat',
-      version='0.0.1',
+      version='0.0.3',
       description='An alpha version for OpenMindat package',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: Apache Software License',
         "Programming Language :: Python :: 3",
@@ -21,10 +21,11 @@
       url='https://github.com/ChuBL/OpenMindat',
       author='Jiyin Zhang',
       author_email='jiyinz@uidaho.edu',
       license='Apache Software License',
       packages=['openmindat'],
       install_requires=[
           'requests',
+          'PyYAML'
       ],
       include_package_data=True,
       zip_safe=False)
```


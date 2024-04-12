# Comparing `tmp/edgarquery-0.0.58.tar.gz` & `tmp/edgarquery-0.0.59.tar.gz`

## Comparing `edgarquery-0.0.58.tar` & `edgarquery-0.0.59.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 edgarquery-0.0.58/genusage.sh
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 edgarquery-0.0.58/notes.txt
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.58/scripts/edgarquery.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.58/scripts/edgartickerstocsv.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/__about__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/__init__.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/concepts.sh
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/ebquery.py
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcikperson.py
--rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcompanyconcepttocsv.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcompanyfactsshow.py
--rwxr-xr-x   0        0        0     5961 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcompanyfactstocsv.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcompanyfactsziptocsv.py
--rw-r--r--   0        0        0     8602 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarlatest10K.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarlatestsubmissions.py
--rwxr-xr-x   0        0        0    15138 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarquery.py
--rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarsubmissions.py
--rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarsubmissionsziptocsv.py
--rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgartickerstocsv.py
--rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarxbrlframestocsv.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/sedfile
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/tickerd.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/__init__.py
--rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/p.sh
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/s.sh
--rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/x.sh
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/y.sh
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.58/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.58/LICENSE.txt
--rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 edgarquery-0.0.58/README.md
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 edgarquery-0.0.58/pyproject.toml
--rw-r--r--   0        0        0     9421 2020-02-02 00:00:00.000000 edgarquery-0.0.58/PKG-INFO
+-rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 edgarquery-0.0.59/genusage.sh
+-rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 edgarquery-0.0.59/notes.txt
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.59/scripts/edgarquery.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.59/scripts/edgartickerstocsv.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/__about__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/__init__.py
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/concepts.sh
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/ebquery.py
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcikperson.py
+-rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcompanyconcepttocsv.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcompanyfactsshow.py
+-rwxr-xr-x   0        0        0     5961 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcompanyfactstocsv.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcompanyfactsziptocsv.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarlatest10K.py
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarlatestsubmissions.py
+-rwxr-xr-x   0        0        0    15138 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarquery.py
+-rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarsubmissions.py
+-rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarsubmissionsziptocsv.py
+-rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgartickerstocsv.py
+-rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarxbrlframestocsv.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/sedfile
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/tickerd.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/__init__.py
+-rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/p.sh
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/s.sh
+-rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/x.sh
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/y.sh
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.59/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.59/LICENSE.txt
+-rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 edgarquery-0.0.59/README.md
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 edgarquery-0.0.59/pyproject.toml
+-rw-r--r--   0        0        0     9421 2020-02-02 00:00:00.000000 edgarquery-0.0.59/PKG-INFO
```

### Comparing `edgarquery-0.0.58/genusage.sh` & `edgarquery-0.0.59/genusage.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/notes.txt` & `edgarquery-0.0.59/notes.txt`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/scripts/edgarquery.py` & `edgarquery-0.0.59/scripts/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/ebquery.py` & `edgarquery-0.0.59/src/edgarquery/ebquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarcikperson.py` & `edgarquery-0.0.59/src/edgarquery/edgarcikperson.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarcompanyconcepttocsv.py` & `edgarquery-0.0.59/src/edgarquery/edgarcompanyconcepttocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarcompanyfactsshow.py` & `edgarquery-0.0.59/src/edgarquery/edgarcompanyfactsshow.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarcompanyfactstocsv.py` & `edgarquery-0.0.59/src/edgarquery/edgarcompanyfactstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarcompanyfactsziptocsv.py` & `edgarquery-0.0.59/src/edgarquery/edgarcompanyfactsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarlatest10K.py` & `edgarquery-0.0.59/src/edgarquery/edgarlatest10K.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,21 +194,21 @@
             # self.storequery(resp, tf=ofn)
             print('\tSEARCHING: %s' % (url) )
             tktbl = self.dogrep(cik, ofn)
             if tktbl:
                 tkurl = self.get10kfromhtml(cik, tktbl, link, directory)
                 if link:
                     print(tkurl)
+                if show:
+                    webbrowser.open(tkurl)
                 if directory:
                     tkresp = self.uq.query(tkurl, self.hdr)
                     ofn = os.path.join(directory, 'CIK%s.10-K.htm' %\
                         (cik.zfill(10) ) )
                     self.uq.storequery(tkresp, ofn)
-                    if show:
-                        webbrowser.open('file://%s' % (ofn) )
                 return
 
 
 # if __name__ == '__main__':
 def main():
     LT = EDGARLatest10K()
```

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarlatestsubmissions.py` & `edgarquery-0.0.59/src/edgarquery/edgarlatestsubmissions.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarquery.py` & `edgarquery-0.0.59/src/edgarquery/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarsubmissions.py` & `edgarquery-0.0.59/src/edgarquery/edgarsubmissions.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarsubmissionsziptocsv.py` & `edgarquery-0.0.59/src/edgarquery/edgarsubmissionsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgartickerstocsv.py` & `edgarquery-0.0.59/src/edgarquery/edgartickerstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/edgarxbrlframestocsv.py` & `edgarquery-0.0.59/src/edgarquery/edgarxbrlframestocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/src/edgarquery/tickerd.py` & `edgarquery-0.0.59/src/edgarquery/tickerd.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/tests/p.sh` & `edgarquery-0.0.59/tests/p.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/tests/x.sh` & `edgarquery-0.0.59/tests/x.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/LICENSE.txt` & `edgarquery-0.0.59/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/README.md` & `edgarquery-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/pyproject.toml` & `edgarquery-0.0.59/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.58/PKG-INFO` & `edgarquery-0.0.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgarquery
-Version: 0.0.58
+Version: 0.0.59
 Summary: Downloads various SEC EDGAR files by CIK or ticker.  companyfactsshow displays company facts in your browser
 Project-URL: Documentation, https://github.com/dfwcnj/edgarquery#readme
 Project-URL: Issues, https://github.com/dfwcnj/edgarquery/issues
 Project-URL: Source, https://github.com/dfwcnj/edgarquery
 Author-email: Don Caldwell <dfwcnj@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```


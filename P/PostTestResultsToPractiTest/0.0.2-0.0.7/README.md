# Comparing `tmp/posttestresultstopractitest-0.0.2.tar.gz` & `tmp/posttestresultstopractitest-0.0.7.tar.gz`

## Comparing `posttestresultstopractitest-0.0.2.tar` & `posttestresultstopractitest-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/userInputs.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/ClonePTTestSet.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/GetConfigValues.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/GetPTProjectId.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/GetPTTestSetId.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/Orchestrator.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/PT_APIRequest.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/LICENSE
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/userInputs.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/ClonePTTestSet.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/Constants.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/CreatePTInstance.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/CreatePTTestSet.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/EnumClass.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/GetConfigValues.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/GetPTInstance.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/GetPTProjectId.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/GetPTTest.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/GetPTTestSetId.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/Orchestrator.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/PT_APIRequest.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/PostTestResults.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/tests/mainEntrance.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/README.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.7/PKG-INFO
```

### Comparing `posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/ClonePTTestSet.py` & `posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/ClonePTTestSet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import json
-from src.PostTestResultsToPractiTest import PT_APIRequest
-from src.PostTestResultsToPractiTest import GetConfigValues
-from src.PostTestResultsToPractiTest import GetPTProjectId
-from src.PostTestResultsToPractiTest import GetPTTestSetId
+from PostTestResultsToPractiTest import PT_APIRequest
+from PostTestResultsToPractiTest import GetConfigValues
+from PostTestResultsToPractiTest import GetPTProjectId
+from PostTestResultsToPractiTest import Constants
 
 def ClonePTTestSet(testSetIdTocloneFrom):
     GetConfigValues.GetConfigValues()
     projectId = GetPTProjectId.RetrieveProjectId()
     
     jsonData = json.dumps({"data":{"type":"sets","attributes":{"name":GetConfigValues.PTTestsetName_New,"priority":"highest"}}})
     
-    res = PT_APIRequest.sendRequest(GetConfigValues.PT_API_BaseURL + "/projects/" + projectId +"/sets/" + testSetIdTocloneFrom + "/clone.json", "post", jsonData)
+    res = PT_APIRequest.sendRequest(Constants.PT_API_BASEURL + "/projects/" + projectId +"/sets/" + testSetIdTocloneFrom + "/clone.json", "post", jsonData)
     #print (res.status_code)
     #print (res.text)
     #print (res.content)
     if res.status_code == 200:
         responseData = json.loads(res.content)
         #print(type(testSets))
 
         data = responseData['data']
    
         newTestSetId = data['id']
-        print ("new test set id: " + newTestSetId)
+        print ("TestSetName:", GetConfigValues.PTTestsetName_New, "-->New test set id: " + newTestSetId)
         return newTestSetId
     else:
-        raise Exception ("Call to clone test set was unsucessful with status code", res.status_code)
+        raise Exception ("Call to clone test set was unsuccessful with status code", res.status_code)
```

### Comparing `posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/GetPTTestSetId.py` & `posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/GetPTTestSetId.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 import json
-from src.PostTestResultsToPractiTest import PT_APIRequest
-from src.PostTestResultsToPractiTest import GetConfigValues
-from src.PostTestResultsToPractiTest import GetPTProjectId
+from PostTestResultsToPractiTest import PT_APIRequest
+from PostTestResultsToPractiTest import GetConfigValues
+from PostTestResultsToPractiTest import GetPTProjectId
+from PostTestResultsToPractiTest import Constants
 
-def RetrieveTestSetId():
+def RetrieveTestSetId(testSetName):
     GetConfigValues.GetConfigValues()
     projectId = GetPTProjectId.RetrieveProjectId()
     
-    res = PT_APIRequest.getRequest(GetConfigValues.PT_API_BaseURL + "/projects/" + projectId + "/sets.json?name_exact=" + GetConfigValues.PTTestsetName_ToCloneFrom)
+    res = PT_APIRequest.getRequest(Constants.PT_API_BASEURL + "/projects/" + projectId + "/sets.json?name_exact=" + testSetName)
 
-    #print (res.status_code)
-    #print (res.text)
-    #print (res.content)
     if res.status_code == 200:
         testSets = json.loads(res.content)
-        #print(type(testSets))
-
         testSet = testSets['data']
 
-        myTestSetData = list(filter(lambda myData:myData['attributes']['name']==GetConfigValues.PTTestsetName_ToCloneFrom, testSet)) 
+        myTestSetData = list(filter(lambda myData:myData['attributes']['name']==testSetName, testSet)) 
         
         if len(myTestSetData) != 0:
             myTestSetId = myTestSetData[0]['id']
-            print (myTestSetId)
+            print (testSetName, "--> Test set id:", myTestSetId)
             return myTestSetId
         else:
-            raise Exception ("No matching test set of " + GetConfigValues.PTTestsetName_ToCloneFrom + "is found")
+            print ("No matching test set of " + testSetName + " is found")
+            return None
     else:
-        raise Exception ("Call to get test set was unsucessful with status code", res.status_code)
+        raise Exception ("Call to get test set was unsuccessful with status code", res.status_code)
+
+def RetrieveTestSetWithVersion(testSetName: str, releaseVersion: str) -> int:
+    """Retrieve test set id given a name and version.
+
+    :param testSetName: Test set name to filter by.
+    :param releaseVersion: Release version for test set run.
+    :return: PractiTest test set id.
+    """
+    GetConfigValues.GetConfigValues()
+    projectId = GetPTProjectId.RetrieveProjectId()
+    
+    res = PT_APIRequest.getRequest(Constants.PT_API_BASEURL + "/projects/" + projectId + "/sets.json?name_exact=" + testSetName)
+
+    if res.status_code == 200:
+        testSets = json.loads(res.content)
+        testSet = testSets['data']
 
-#retrieveProjectId()
+        myTestSetData = list(filter(lambda myData:myData['attributes']['version']==releaseVersion, testSet)) 
+        
+        if len(myTestSetData) != 0:
+            myTestSetId = myTestSetData[0]['id']
+            return myTestSetId
+        else:
+            return None
+    else:
+        raise Exception ("Call to get test set was unsuccessful with status code", res.status_code)
```

### Comparing `posttestresultstopractitest-0.0.2/src/PostTestResultsToPractiTest/PT_APIRequest.py` & `posttestresultstopractitest-0.0.7/src/PostTestResultsToPractiTest/PT_APIRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import requests
-from src.PostTestResultsToPractiTest import GetConfigValues
-from requests.auth import AuthBase
+from PostTestResultsToPractiTest import GetConfigValues
 
 def getRequest(url):
     res = requests.get(url, auth=('',GetConfigValues.PT_Token))
     return res
 
 def sendRequest(url, putOrPostMethod, jsonData):
     if putOrPostMethod.lower() == "put":
```

### Comparing `posttestresultstopractitest-0.0.2/LICENSE` & `posttestresultstopractitest-0.0.7/LICENSE`

 * *Files identical despite different names*


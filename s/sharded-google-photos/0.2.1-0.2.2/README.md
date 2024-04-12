# Comparing `tmp/sharded_google_photos-0.2.1.tar.gz` & `tmp/sharded_google_photos-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharded_google_photos-0.2.1.tar", max compression
+gzip compressed data, was "sharded_google_photos-0.2.2.tar", max compression
```

## Comparing `sharded_google_photos-0.2.1.tar` & `sharded_google_photos-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2024-03-18 17:48:51.353682 sharded_google_photos-0.2.1/LICENSE
--rw-r--r--   0        0        0     4795 2024-04-03 03:34:24.298488 sharded_google_photos-0.2.1/README.md
--rw-r--r--   0        0        0      780 2024-04-03 23:10:55.108775 sharded_google_photos-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      464 2024-03-20 07:05:33.524175 sharded_google_photos-0.2.1/sharded_google_photos/backup/diffs_splitter.py
--rw-r--r--   0        0        0     8761 2024-03-29 18:32:42.111368 sharded_google_photos-0.2.1/sharded_google_photos/backup/gphotos_backup.py
--rw-r--r--   0        0        0      551 2024-03-27 17:57:15.555272 sharded_google_photos-0.2.1/sharded_google_photos/backup/gphotos_uploader.py
--rw-r--r--   0        0        0     2532 2024-04-02 06:21:34.945407 sharded_google_photos-0.2.1/sharded_google_photos/backup/media_item_repository.py
--rw-r--r--   0        0        0     2841 2024-03-27 17:57:15.558065 sharded_google_photos-0.2.1/sharded_google_photos/backup/shared_album_repository.py
--rw-r--r--   0        0        0     2193 2024-03-27 17:57:15.559288 sharded_google_photos-0.2.1/sharded_google_photos/cleanup/gphotos_cleaner.py
--rw-r--r--   0        0        0     6168 2024-04-03 23:06:18.951870 sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_album_client.py
--rw-r--r--   0        0        0     4306 2024-04-01 07:46:11.129212 sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_client.py
--rw-r--r--   0        0        0     8990 2024-04-03 23:09:52.803576 sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_mediaitem_client.py
--rw-r--r--   0        0        0     1721 2024-03-27 17:57:15.565065 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_album_client.py
--rw-r--r--   0        0        0     1540 2024-03-27 17:57:15.566785 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_client.py
--rw-r--r--   0        0        0     1197 2024-03-27 17:57:15.567903 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py
--rw-r--r--   0        0        0     9185 2024-03-27 17:57:15.569275 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_repository.py
--rw-r--r--   0        0        0      616 2024-03-29 18:32:42.115559 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 sharded_google_photos-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-18 17:48:51.353682 sharded_google_photos-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4911 2024-04-12 00:24:04.266588 sharded_google_photos-0.2.2/README.md
+-rw-r--r--   0        0        0      780 2024-04-12 00:24:08.844577 sharded_google_photos-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      464 2024-04-11 21:04:01.535822 sharded_google_photos-0.2.2/sharded_google_photos/backup/diffs_splitter.py
+-rw-r--r--   0        0        0     9209 2024-04-12 00:24:04.267735 sharded_google_photos-0.2.2/sharded_google_photos/backup/gphotos_backup.py
+-rw-r--r--   0        0        0      551 2024-03-27 17:57:15.555272 sharded_google_photos-0.2.2/sharded_google_photos/backup/gphotos_uploader.py
+-rw-r--r--   0        0        0     2782 2024-04-12 00:24:04.268961 sharded_google_photos-0.2.2/sharded_google_photos/backup/media_item_repository.py
+-rw-r--r--   0        0        0     2841 2024-03-27 17:57:15.558065 sharded_google_photos-0.2.2/sharded_google_photos/backup/shared_album_repository.py
+-rw-r--r--   0        0        0     2193 2024-03-27 17:57:15.559288 sharded_google_photos-0.2.2/sharded_google_photos/cleanup/gphotos_cleaner.py
+-rw-r--r--   0        0        0     6453 2024-04-12 00:24:04.271074 sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_album_client.py
+-rw-r--r--   0        0        0     4306 2024-04-11 20:37:57.786024 sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_client.py
+-rw-r--r--   0        0        0     9122 2024-04-12 00:24:04.272729 sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_mediaitem_client.py
+-rw-r--r--   0        0        0     1721 2024-03-27 17:57:15.565065 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_album_client.py
+-rw-r--r--   0        0        0     1540 2024-03-27 17:57:15.566785 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_client.py
+-rw-r--r--   0        0        0     1197 2024-03-27 17:57:15.567903 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py
+-rw-r--r--   0        0        0     9185 2024-03-27 17:57:15.569275 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_repository.py
+-rw-r--r--   0        0        0      616 2024-03-29 18:32:42.115559 sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py
+-rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 sharded_google_photos-0.2.2/PKG-INFO
```

### Comparing `sharded_google_photos-0.2.1/LICENSE` & `sharded_google_photos-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/README.md` & `sharded_google_photos-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,33 @@
+Metadata-Version: 2.1
+Name: sharded-google-photos
+Version: 0.2.2
+Summary: A tool to shard photos across multiple Google Photo accounts
+License: GNU General Public License v3.0
+Author: Emilio K
+Author-email: e.kartonoe@gmail.com
+Requires-Python: >=3.12,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: google-api-python-client (>=2.122.0,<3.0.0)
+Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
+Requires-Dist: python-magic (>=0.4.27,<0.5.0)
+Description-Content-Type: text/markdown
+
 # Sharded-Google-Photos
 
 ## Description
 
 Running out of space in your Google Photos account? Wish you can upload an unlimited number of photos on Google Photos? Now you can! With this Python library, you can upload your photos to multiple Google Photo Accounts and then share those albums to your main Google Photos account. That way, you get to see all of your photos on one main Google Photos account.
 
 It works like this:
 
-1. Let's say you have three Google Accounts.
+1. Let's say you have three Google Accounts. Create an OAuth2 to interact with Google Photos and Google Drive.
 
 2. Install `libmagic`
 
 3. Install the package by running `pip install sharded-google-photos`.
 
 4. Import the following code in your `main.py` app:
 
@@ -28,56 +45,58 @@
 
     backup_client = GPhotosBackup(clients)
     ```
 
 5. To upload four photos from two folders, run the following:
 
     ```python
-    new_album_uris = backup_client.backup([
-        {
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/2.jpg",
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/3.jpg",
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/4.jpg",
-        }
-    ])
+    new_album_uris = backup_client.backup(
+        [
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg" },
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/2.jpg" },
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/3.jpg" },
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/4.jpg" },
+        ]
+    )
     print(new_album_uris)
     ```
 
     What will happen is that it will:
 
     1. A shared read-only album `Archives/Photos/2022/Trip to California` will be made in some Google Photos account with the most amount of space available.
 
     2. A shared read-only album `Archives/Photos/2022/Trip to Toronto` will be made in some Google Photos account with the second most amount of space available.
 
     3. Photos `1.jpg`, and `2.jpg` will be in the `Archives/Photos/2022/Trip to California` album.
 
     4. Photos `3.jpg`, and `4.jpg` will be in the `Archives/Photos/2022/Trip to Toronto` album.
 
-    3. The url to those new albums will be in `new_album_uris` that you can share to.
+    5. The url to those new albums will be in `new_album_uris` that you can share to.
 
 6. To update a file in a folder, run the following:
 
     ```python
-    backup_client.backup([
-        {
-            "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
-        }
-    ])
+    backup_client.backup(
+        [
+            { "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg" },
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg" },
+        ]
+    )
     ```
 
 7. To delete a file in a folder, run the following:
 
     ```python
-    backup_client.backup([
-        {
-            "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
-        }
-    ])
+    backup_client.backup(
+        [
+            {
+                "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
+            }
+        ]
+    )
     ```
 
     Note: it is not possible for the Google Photos API to actually delete a photo from Google Photos. Instead, you can clean your Google Photo accounts by putting all album-less photos into a "Trash" album by running the following script:
 
     ```python
     from sharded_google_photos.cleanup.gphotos_cleaner import GPhotosCleaner
 
@@ -143,7 +162,8 @@
 ### Credits
 
 Emilio Kartono, who made the entire project.
 
 ### License
 
 This project is protected under the GNU licence. Please refer to the LICENSE.txt for more information.
+
```

### Comparing `sharded_google_photos-0.2.1/pyproject.toml` & `sharded_google_photos-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sharded-google-photos"
-version = "0.2.1"
+version = "0.2.2"
 description = "A tool to shard photos across multiple Google Photo accounts"
 authors = ["Emilio K <e.kartonoe@gmail.com>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/backup/gphotos_backup.py` & `sharded_google_photos-0.2.2/sharded_google_photos/backup/gphotos_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,24 @@
 from .shared_album_repository import SharedAlbumRepository
 from .media_item_repository import MediaItemRepository
 from .gphotos_uploader import GPhotosUploader
 
 logger = logging.getLogger(__name__)
 
 
+class NoAvailableSpaceInExistingAlbumException(Exception):
+    """Exception raised when there is no space in an existing album"""
+
+    def __init__(self, client_idx: int, album_id: str, album_title: str):
+        super().__init__(f"Need to move {album_title} out of {client_idx}")
+        self.client_idx = client_idx
+        self.album_id = album_id
+        self.album_title = album_title
+
+
 class GPhotosBackup:
     def __init__(self, gphoto_clients: list[GPhotosClient]):
         self.gphoto_clients = gphoto_clients
 
     def backup(self, diffs):
         # Insert new metadata in the diffs
         new_diffs = self.add_new_metadata(diffs)
@@ -133,15 +143,17 @@
                 chunked_new_diffs[album_title].get("+", [])
             )
 
             album = shared_album_repository.get_album_from_title(album_title)
             client_idx = album["client_idx"]
 
             if space_remaining[client_idx] - space_needed <= 0:
-                raise Exception(f"Need to move {album_title} out of {client_idx}")
+                raise NoAvailableSpaceInExistingAlbumException(
+                    client_idx, album["id"], album_title
+                )
 
             space_remaining[client_idx] -= space_needed
             results[album_title] = {
                 "album": album,
                 "client_idx": client_idx,
                 "is_new_album": False,
             }
```

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/backup/gphotos_uploader.py` & `sharded_google_photos-0.2.2/sharded_google_photos/backup/gphotos_uploader.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/backup/media_item_repository.py` & `sharded_google_photos-0.2.2/sharded_google_photos/backup/media_item_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,26 +38,32 @@
         media_id = self.file_name_to_media_ids[file_name]
         return self.media_id_to_obj[media_id]
 
     def get_num_media_items(self):
         return len(self.media_id_to_obj)
 
     def remove_media_items(self, media_ids):
+        MAX_REMOVE_ITEMS_LENGTH_PER_CALL = 50
+
         if len(media_ids) == 0:
             return
 
         for media_id in media_ids:
             if media_id not in self.media_id_to_obj:
                 raise Exception("Media item is not found")
 
             media_item = self.media_id_to_obj[media_id]
             del self.media_id_to_obj[media_id]
             del self.file_name_to_media_ids[media_item["filename"]]
 
-        self.gphoto_client.albums().remove_photos_from_album(self.album_id, media_ids)
+        for i in range(0, len(media_ids), MAX_REMOVE_ITEMS_LENGTH_PER_CALL):
+            chunked_media_ids = media_ids[i : i + MAX_REMOVE_ITEMS_LENGTH_PER_CALL]
+            self.gphoto_client.albums().remove_photos_from_album(
+                self.album_id, chunked_media_ids
+            )
 
         logger.debug(f"Media items removed from album {self.album_id}: {media_ids}")
 
     def add_uploaded_photos(self, upload_tokens):
         if len(upload_tokens) == 0:
             logger.debug("No uploaded tokens to add")
             return
```

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/backup/shared_album_repository.py` & `sharded_google_photos-0.2.2/sharded_google_photos/backup/shared_album_repository.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/cleanup/gphotos_cleaner.py` & `sharded_google_photos-0.2.2/sharded_google_photos/cleanup/gphotos_cleaner.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_album_client.py` & `sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_album_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,109 @@
 import json
 import logging
 import backoff
 from requests.exceptions import RequestException
 
 from google.auth.transport.requests import AuthorizedSession
+from google.auth.transport import DEFAULT_RETRYABLE_STATUS_CODES
 
 logger = logging.getLogger(__name__)
 
 
+def fatal_code(e):
+    return e.response.status_code not in DEFAULT_RETRYABLE_STATUS_CODES
+
+
 class GPhotosAlbumClient:
     def __init__(self, session: AuthorizedSession):
         self._session = session
 
     def list_shared_albums(self, exclude_non_app_created_data: bool = False):
         logger.debug("Listing albums")
 
         albums = []
         cur_page_token = None
         while True:
-            res = self._list_shared_albums_in_pages(
+            res_body = self._list_shared_albums_in_pages(
                 cur_page_token, exclude_non_app_created_data
             )
-            res_body = res.json()
 
             if "sharedAlbums" not in res_body:
                 break
 
             albums += res_body["sharedAlbums"]
 
             if "nextPageToken" in res_body:
                 cur_page_token = res_body["nextPageToken"]
             else:
                 break
 
         return albums
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def _list_shared_albums_in_pages(
         self, page_token: str | None, exclude_non_app_created_data: bool
     ):
         uri = "https://photoslibrary.googleapis.com/v1/sharedAlbums"
         params = {
             "pageToken": page_token,
             "excludeNonAppCreatedData": exclude_non_app_created_data,
         }
         res = self._session.get(uri, params=params)
         res.raise_for_status()
-        return res
+
+        return res.json()
 
     def list_albums(self, exclude_non_app_created_data: bool = False):
         logger.debug("Listing albums")
 
         albums = []
         cur_page_token = None
         while True:
-            res = self._list_albums_in_pages(
+            res_json = self._list_albums_in_pages(
                 cur_page_token, exclude_non_app_created_data
             )
-            res_json = res.json()
 
             if "albums" not in res_json:
                 break
 
             albums += res_json["albums"]
 
             if "nextPageToken" in res_json:
                 cur_page_token = res_json["nextPageToken"]
             else:
                 break
 
         return albums
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def _list_albums_in_pages(
         self, page_token: str | None, exclude_non_app_created_data: bool
     ):
         uri = "https://photoslibrary.googleapis.com/v1/albums"
         params = {
             "pageToken": page_token,
             "excludeNonAppCreatedData": exclude_non_app_created_data,
         }
         res = self._session.get(uri, params=params)
         res.raise_for_status()
+        return res.json()
 
-        return res
-
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def create_album(self, album_name: str):
         logger.debug(f"Creating album {album_name}")
 
         request_body = json.dumps({"album": {"title": album_name}})
         uri = "https://photoslibrary.googleapis.com/v1/albums"
         res = self._session.post(uri, request_body)
         res.raise_for_status()
 
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def update_album(
         self, album_id: str, new_title: str = None, new_cover_media_item_id: str = None
     ):
         uri = f"https://photoslibrary.googleapis.com/v1/albums/{album_id}"
 
         if new_title is not None and new_cover_media_item_id is not None:
             uri += "?updateMask=title&updateMask=coverPhotoMediaItemId"
@@ -111,15 +114,15 @@
 
         request = {"title": new_title, "coverPhotoMediaItemId": new_cover_media_item_id}
         res = self._session.patch(uri, json.dumps(request))
         res.raise_for_status()
 
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def share_album(
         self,
         album_id: str,
         is_collaborative: bool = False,
         is_commentable: bool = False,
     ):
         logger.debug(f"Sharing album {album_id}")
@@ -136,47 +139,47 @@
             album_id
         )
         res = self._session.post(uri, request_body)
         res.raise_for_status()
 
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def join_album(self, share_token: str):
         logger.debug(f"Joining shared album {share_token}")
 
         request_body = json.dumps({"shareToken": share_token})
         uri = "https://photoslibrary.googleapis.com/v1/sharedAlbums:join"
         res = self._session.post(uri, request_body)
         res.raise_for_status()
 
         return res.json()
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def unshare_album(self, album_id: str):
         logger.debug(f"Unsharing shared album {album_id}")
 
         uri = "https://photoslibrary.googleapis.com/v1/albums/{0}:unshare".format(
             album_id
         )
         res = self._session.post(uri)
         res.raise_for_status()
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def add_photos_to_album(self, album_id: str, media_item_ids: list[str]):
         logger.debug(f"Add photos to album {album_id} {media_item_ids}")
 
         request_body = json.dumps({"mediaItemIds": media_item_ids})
         uri = "https://photoslibrary.googleapis.com/v1/albums/{0}:batchAddMediaItems".format(
             album_id
         )
         res = self._session.post(uri, request_body)
         res.raise_for_status()
 
-    @backoff.on_exception(backoff.expo, (RequestException))
+    @backoff.on_exception(backoff.expo, (RequestException), giveup=fatal_code)
     def remove_photos_from_album(self, album_id: str, media_item_ids: list[str]):
         logger.debug(f"Removing photos from album {album_id} {media_item_ids}")
 
         request_body = json.dumps({"mediaItemIds": media_item_ids})
         uri = "https://photoslibrary.googleapis.com/v1/albums/{0}:batchRemoveMediaItems".format(
             album_id
         )
```

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_client.py` & `sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_mediaitem_client.py` & `sharded_google_photos-0.2.2/sharded_google_photos/shared/gphotos_mediaitem_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,17 @@
         mime_type = self._get_mime_type(photo_file_path)
         file_size_in_bytes = os.stat(photo_file_path).st_size
 
         logger.debug(
             f"Uploading in chunks with mime_type {mime_type} and file size {file_size_in_bytes}"
         )
 
-        res_1 = self._initialize_chunked_upload(mime_type, file_size_in_bytes)
+        res_1 = self._initialize_chunked_upload(
+            mime_type, file_name, file_size_in_bytes
+        )
         upload_url = res_1.headers["X-Goog-Upload-URL"]
         chunk_size = int(res_1.headers["X-Goog-Upload-Chunk-Granularity"])
 
         logger.debug(f"Obtained upload url and chunk size: {upload_url} {chunk_size}")
 
         with open(photo_file_path, "rb") as file_obj:
             cur_offset = 0
@@ -222,19 +224,22 @@
 
                 chunk = next_chunk
 
         logger.debug(f"Chunk uploading finished: {photo_file_path}")
         return upload_token
 
     @backoff.on_exception(backoff.expo, (RequestException))
-    def _initialize_chunked_upload(self, mime_type: str, file_size_in_bytes: int):
+    def _initialize_chunked_upload(
+        self, mime_type: str, file_name: str, file_size_in_bytes: int
+    ):
         self._session.headers["Content-Length"] = "0"
         self._session.headers["X-Goog-Upload-Command"] = "start"
         self._session.headers["X-Goog-Upload-Content-Type"] = mime_type
         self._session.headers["X-Goog-Upload-Protocol"] = "resumable"
+        self._session.headers["X-Goog-Upload-File-Name"] = file_name
         self._session.headers["X-Goog-Upload-Raw-Size"] = str(file_size_in_bytes)
 
         res = self._session.post("https://photoslibrary.googleapis.com/v1/uploads")
         res.raise_for_status()
 
         return res
```

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_album_client.py` & `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_album_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_client.py` & `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py` & `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_repository.py` & `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/fake_gphotos_repository.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py` & `sharded_google_photos-0.2.2/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.1/PKG-INFO` & `sharded_google_photos-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-Metadata-Version: 2.1
-Name: sharded-google-photos
-Version: 0.2.1
-Summary: A tool to shard photos across multiple Google Photo accounts
-License: GNU General Public License v3.0
-Author: Emilio K
-Author-email: e.kartonoe@gmail.com
-Requires-Python: >=3.12,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: google-api-python-client (>=2.122.0,<3.0.0)
-Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
-Requires-Dist: python-magic (>=0.4.27,<0.5.0)
-Description-Content-Type: text/markdown
-
 # Sharded-Google-Photos
 
 ## Description
 
 Running out of space in your Google Photos account? Wish you can upload an unlimited number of photos on Google Photos? Now you can! With this Python library, you can upload your photos to multiple Google Photo Accounts and then share those albums to your main Google Photos account. That way, you get to see all of your photos on one main Google Photos account.
 
 It works like this:
 
-1. Let's say you have three Google Accounts.
+1. Let's say you have three Google Accounts. Create an OAuth2 to interact with Google Photos and Google Drive.
 
 2. Install `libmagic`
 
 3. Install the package by running `pip install sharded-google-photos`.
 
 4. Import the following code in your `main.py` app:
 
@@ -45,56 +28,58 @@
 
     backup_client = GPhotosBackup(clients)
     ```
 
 5. To upload four photos from two folders, run the following:
 
     ```python
-    new_album_uris = backup_client.backup([
-        {
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/2.jpg",
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/3.jpg",
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/4.jpg",
-        }
-    ])
+    new_album_uris = backup_client.backup(
+        [
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg" },
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/2.jpg" },
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/3.jpg" },
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/4.jpg" },
+        ]
+    )
     print(new_album_uris)
     ```
 
     What will happen is that it will:
 
     1. A shared read-only album `Archives/Photos/2022/Trip to California` will be made in some Google Photos account with the most amount of space available.
 
     2. A shared read-only album `Archives/Photos/2022/Trip to Toronto` will be made in some Google Photos account with the second most amount of space available.
 
     3. Photos `1.jpg`, and `2.jpg` will be in the `Archives/Photos/2022/Trip to California` album.
 
     4. Photos `3.jpg`, and `4.jpg` will be in the `Archives/Photos/2022/Trip to Toronto` album.
 
-    3. The url to those new albums will be in `new_album_uris` that you can share to.
+    5. The url to those new albums will be in `new_album_uris` that you can share to.
 
 6. To update a file in a folder, run the following:
 
     ```python
-    backup_client.backup([
-        {
-            "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
-            "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
-        }
-    ])
+    backup_client.backup(
+        [
+            { "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg" },
+            { "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg" },
+        ]
+    )
     ```
 
 7. To delete a file in a folder, run the following:
 
     ```python
-    backup_client.backup([
-        {
-            "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
-        }
-    ])
+    backup_client.backup(
+        [
+            {
+                "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
+            }
+        ]
+    )
     ```
 
     Note: it is not possible for the Google Photos API to actually delete a photo from Google Photos. Instead, you can clean your Google Photo accounts by putting all album-less photos into a "Trash" album by running the following script:
 
     ```python
     from sharded_google_photos.cleanup.gphotos_cleaner import GPhotosCleaner
 
@@ -160,8 +145,7 @@
 ### Credits
 
 Emilio Kartono, who made the entire project.
 
 ### License
 
 This project is protected under the GNU licence. Please refer to the LICENSE.txt for more information.
-
```


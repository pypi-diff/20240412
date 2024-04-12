# Comparing `tmp/twikit-1.4.6.tar.gz` & `tmp/twikit-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.4.6.tar", last modified: Tue Apr  9 12:10:32 2024, max compression
+gzip compressed data, was "twikit-1.4.7.tar", last modified: Fri Apr 12 13:44:07 2024, max compression
```

## Comparing `twikit-1.4.6.tar` & `twikit-1.4.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 12:10:32.339234 twikit-1.4.6/
--rw-rw-rw-   0        0        0     1079 2024-04-06 11:03:16.000000 twikit-1.4.6/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-09 12:10:32.335246 twikit-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-08 13:45:07.000000 twikit-1.4.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 12:10:32.339234 twikit-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-08 07:44:57.000000 twikit-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:10:32.268418 twikit-1.4.6/twikit/
--rw-rw-rw-   0        0        0      469 2024-04-09 12:01:19.000000 twikit-1.4.6/twikit/__init__.py
--rw-rw-rw-   0        0        0   110719 2024-04-09 11:44:57.000000 twikit-1.4.6/twikit/client.py
--rw-rw-rw-   0        0        0     2380 2024-04-06 04:29:07.000000 twikit-1.4.6/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-08 14:07:28.000000 twikit-1.4.6/twikit/group.py
--rw-rw-rw-   0        0        0     1913 2024-04-06 04:28:27.000000 twikit-1.4.6/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-08 13:03:12.000000 twikit-1.4.6/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-06 13:37:31.000000 twikit-1.4.6/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-06 13:37:50.000000 twikit-1.4.6/twikit/notification.py
--rw-rw-rw-   0        0        0     1070 2024-04-08 13:03:49.000000 twikit-1.4.6/twikit/trend.py
--rw-rw-rw-   0        0        0    19984 2024-04-09 11:44:08.000000 twikit-1.4.6/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:10:32.332248 twikit-1.4.6/twikit/twikit_async/
--rw-rw-rw-   0        0        0      421 2024-04-09 12:01:28.000000 twikit-1.4.6/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   112712 2024-04-09 11:53:31.000000 twikit-1.4.6/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.6/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-08 14:09:21.000000 twikit-1.4.6/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     1955 2024-04-06 04:28:33.000000 twikit-1.4.6/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-08 13:08:52.000000 twikit-1.4.6/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-06 13:49:04.000000 twikit-1.4.6/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-06 13:49:28.000000 twikit-1.4.6/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-06 13:49:39.000000 twikit-1.4.6/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    20105 2024-04-09 11:54:15.000000 twikit-1.4.6/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14677 2024-04-08 13:10:20.000000 twikit-1.4.6/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-06 13:55:17.000000 twikit-1.4.6/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14454 2024-04-08 13:05:19.000000 twikit-1.4.6/twikit/user.py
--rw-rw-rw-   0        0        0    21711 2024-04-09 11:20:05.000000 twikit-1.4.6/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:10:32.287366 twikit-1.4.6/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-09 12:10:32.000000 twikit-1.4.6/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-04-09 12:10:32.000000 twikit-1.4.6/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 12:10:32.000000 twikit-1.4.6/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-09 12:10:32.000000 twikit-1.4.6/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 12:10:32.000000 twikit-1.4.6/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 13:44:07.539001 twikit-1.4.7/
+-rw-rw-rw-   0        0        0     1079 2024-04-06 11:03:16.000000 twikit-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-12 13:44:07.536010 twikit-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-08 13:45:07.000000 twikit-1.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:44:07.539001 twikit-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-08 07:44:57.000000 twikit-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:44:07.463204 twikit-1.4.7/twikit/
+-rw-rw-rw-   0        0        0      509 2024-04-12 13:42:19.000000 twikit-1.4.7/twikit/__init__.py
+-rw-rw-rw-   0        0        0   112236 2024-04-12 13:32:55.000000 twikit-1.4.7/twikit/client.py
+-rw-rw-rw-   0        0        0     2380 2024-04-06 04:29:07.000000 twikit-1.4.7/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-08 14:07:28.000000 twikit-1.4.7/twikit/group.py
+-rw-rw-rw-   0        0        0     1913 2024-04-06 04:28:27.000000 twikit-1.4.7/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-08 13:03:12.000000 twikit-1.4.7/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-06 13:37:31.000000 twikit-1.4.7/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-06 13:37:50.000000 twikit-1.4.7/twikit/notification.py
+-rw-rw-rw-   0        0        0     1070 2024-04-08 13:03:49.000000 twikit-1.4.7/twikit/trend.py
+-rw-rw-rw-   0        0        0    20706 2024-04-12 09:14:00.000000 twikit-1.4.7/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:44:07.533018 twikit-1.4.7/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      461 2024-04-10 11:59:51.000000 twikit-1.4.7/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   114259 2024-04-12 13:16:46.000000 twikit-1.4.7/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.7/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-08 14:09:21.000000 twikit-1.4.7/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     1955 2024-04-06 04:28:33.000000 twikit-1.4.7/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-08 13:08:52.000000 twikit-1.4.7/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-06 13:49:04.000000 twikit-1.4.7/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-06 13:49:28.000000 twikit-1.4.7/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-06 13:49:39.000000 twikit-1.4.7/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    20105 2024-04-09 11:54:15.000000 twikit-1.4.7/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14677 2024-04-08 13:10:20.000000 twikit-1.4.7/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-06 13:55:17.000000 twikit-1.4.7/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14454 2024-04-08 13:05:19.000000 twikit-1.4.7/twikit/user.py
+-rw-rw-rw-   0        0        0    21797 2024-04-12 12:58:43.000000 twikit-1.4.7/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:44:07.483150 twikit-1.4.7/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.4.6/LICENSE` & `twikit-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/PKG-INFO` & `twikit-1.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.6
+Version: 1.4.7
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.6/README.md` & `twikit-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/setup.py` & `twikit-1.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/client.py` & `twikit-1.4.7/twikit/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -726,14 +726,59 @@
         response = self.http.get(
             Endpoint.UPLOAD_MEDIA,
             params=params,
             headers=self._base_headers
         ).json()
         return response
 
+    def create_media_metadata(
+        self,
+        media_id: str,
+        alt_text: str | None = None,
+        sensitive_warning: list[
+            Literal['adult_content', 'graphic_violence', 'other']] = None
+    ) -> Response:
+        """
+        Adds metadata to uploaded media.
+
+        Parameters
+        ----------
+        media_id : :class:`str`
+            The media id for which to create metadata.
+        alt_text : :class:`str` | None, default=None
+            Alternative text for the media.
+        sensitive_warning : list{'adult_content', 'graphic_violence', 'other'}
+            A list of sensitive content warnings for the media.
+
+        Returns
+        -------
+        :class:`httpx.Response`
+            Response returned from twitter api.
+
+        Examples
+        --------
+        >>> media_id = client.upload_media('media.jpg')
+        >>> client.create_media_metadata(
+        ...     media_id,
+        ...     alt_text='This is a sample media',
+        ...     sensitive_warning=['other']
+        ... )
+        >>> client.create_tweet(media_ids=[media_id])
+        """
+        data = {'media_id': media_id}
+        if alt_text is not None:
+            data['alt_text'] = {'text': alt_text}
+        if sensitive_warning is not None:
+            data['sensitive_media_warning'] = sensitive_warning
+        return self.http.post(
+            Endpoint.CREATE_MEDIA_METADATA,
+            json=data,
+            headers=self._base_headers
+        )
+
     def create_poll(
         self,
         choices: list[str],
         duration_minutes: int
     ) -> str:
         """
         Creates a poll and returns card-uri.
@@ -1477,15 +1522,15 @@
         response = self.http.get(
             Endpoint.FETCH_COMMUNITY_NOTE,
             params=params,
             headers=self._base_headers
         ).json()
         note_data = response['data']['birdwatch_note_by_rest_id']
         if 'data_v1' not in note_data:
-            raise TwitterException(f'Invalid user id: {note_id}')
+            raise TwitterException(f'Invalid note id: {note_id}')
         return CommunityNote(
             self, note_data
         )
 
     def get_user_tweets(
         self,
         user_id: str,
```

### Comparing `twikit-1.4.6/twikit/errors.py` & `twikit-1.4.7/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/group.py` & `twikit-1.4.7/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/http.py` & `twikit-1.4.7/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/list.py` & `twikit-1.4.7/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/message.py` & `twikit-1.4.7/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/notification.py` & `twikit-1.4.7/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/trend.py` & `twikit-1.4.7/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/tweet.py` & `twikit-1.4.7/twikit/tweet.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,14 +433,36 @@
             Response returned from twitter api.
         """
         return self._client.delete_scheduled_tweet(self.id)
 
     def __repr__(self) -> str:
         return f'<ScheduledTweet id="{self.id}">'
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, ScheduledTweet) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self == __value
+
+
+class TweetTombstone:
+    def __init__(self, client: Client, tweet_id: str, data: dict) -> None:
+        self._client = client
+        self.id = tweet_id
+        self.text: str = data['text']['text']
+
+    def __repr__(self) -> str:
+        return f'<TweetTombstone id="{self.id}">'
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, TweetTombstone) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self == __value
+
 
 class Poll:
     """Represents a poll associated with a tweet.
 
     Attributes
     ----------
     tweet : :class:`Tweet`
```

### Comparing `twikit-1.4.6/twikit/twikit_async/client.py` & `twikit-1.4.7/twikit/twikit_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -739,14 +739,59 @@
         response = (await self.http.get(
             Endpoint.UPLOAD_MEDIA,
             params=params,
             headers=self._base_headers
         )).json()
         return response
 
+    async def create_media_metadata(
+        self,
+        media_id: str,
+        alt_text: str | None = None,
+        sensitive_warning: list[
+            Literal['adult_content', 'graphic_violence', 'other']] = None
+    ) -> Response:
+        """
+        Adds metadata to uploaded media.
+
+        Parameters
+        ----------
+        media_id : :class:`str`
+            The media id for which to create metadata.
+        alt_text : :class:`str` | None, default=None
+            Alternative text for the media.
+        sensitive_warning : list{'adult_content', 'graphic_violence', 'other'}
+            A list of sensitive content warnings for the media.
+
+        Returns
+        -------
+        :class:`httpx.Response`
+            Response returned from twitter api.
+
+        Examples
+        --------
+        >>> media_id = await client.upload_media('media.jpg')
+        >>> await client.create_media_metadata(
+        ...     media_id,
+        ...     alt_text='This is a sample media',
+        ...     sensitive_warning=['other']
+        ... )
+        >>> await client.create_tweet(media_ids=[media_id])
+        """
+        data = {'media_id': media_id}
+        if alt_text is not None:
+            data['alt_text'] = {'text': alt_text}
+        if sensitive_warning is not None:
+            data['sensitive_media_warning'] = sensitive_warning
+        return await self.http.post(
+            Endpoint.CREATE_MEDIA_METADATA,
+            json=data,
+            headers=self._base_headers
+        )
+
     async def create_poll(
         self,
         choices: list[str],
         duration_minutes: int
     ) -> str:
         """
         Creates a poll and returns card-uri.
```

### Comparing `twikit-1.4.6/twikit/twikit_async/errors.py` & `twikit-1.4.7/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/group.py` & `twikit-1.4.7/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/http.py` & `twikit-1.4.7/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/list.py` & `twikit-1.4.7/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/message.py` & `twikit-1.4.7/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/notification.py` & `twikit-1.4.7/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/trend.py` & `twikit-1.4.7/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/tweet.py` & `twikit-1.4.7/twikit/twikit_async/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/user.py` & `twikit-1.4.7/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/twikit_async/utils.py` & `twikit-1.4.7/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/user.py` & `twikit-1.4.7/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.6/twikit/utils.py` & `twikit-1.4.7/twikit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     """
     LOGIN_FLOW = 'https://api.twitter.com/1.1/onboarding/task.json'
     LOGOUT = 'https://api.twitter.com/1.1/account/logout.json'
     CREATE_TWEET = 'https://twitter.com/i/api/graphql/SiM_cAu83R0wnrpmKQQSEw/CreateTweet'
     DELETE_TWEET = 'https://twitter.com/i/api/graphql/VaenaVgh5q5ih7kvyVjgtg/DeleteTweet'
     SEARCH_TIMELINE = 'https://twitter.com/i/api/graphql/flaR-PUMshxFWZWPNpq4zA/SearchTimeline'
     UPLOAD_MEDIA = 'https://upload.twitter.com/i/media/upload.json'
+    CREATE_MEDIA_METADATA = 'https://api.twitter.com/1.1/media/metadata/create.json'
     GUEST_TOKEN = 'https://api.twitter.com/1.1/guest/activate.json'
     CREATE_CARD = 'https://caps.twitter.com/v2/cards/create.json'
     USER_BY_SCREEN_NAME = 'https://twitter.com/i/api/graphql/NimuplG1OB7Fd2btCLdBOw/UserByScreenName'
     USER_BY_REST_ID = 'https://twitter.com/i/api/graphql/tD8zKvQzwY3kdx5yz6YmOw/UserByRestId'
     USER_TWEETS = 'https://twitter.com/i/api/graphql/QWF3SzpHmykQHsQMixG0cg/UserTweets'
     USER_TWEETS_AND_REPLIES = 'https://twitter.com/i/api/graphql/vMkJyzx1wdmvOeeNG0n6Wg/UserTweetsAndReplies'
     USER_MEDIA = 'https://twitter.com/i/api/graphql/2tLOJWwGuCTytDrGBg8VwQ/UserMedia'
```

### Comparing `twikit-1.4.6/twikit.egg-info/PKG-INFO` & `twikit-1.4.7/twikit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.6
+Version: 1.4.7
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.6/twikit.egg-info/SOURCES.txt` & `twikit-1.4.7/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


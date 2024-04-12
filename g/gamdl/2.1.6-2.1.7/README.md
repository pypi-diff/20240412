# Comparing `tmp/gamdl-2.1.6.tar.gz` & `tmp/gamdl-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.1.6.tar` & `gamdl-2.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       17 2024-04-10 22:05:31.703859 gamdl-2.1.6/.github/FUNDING.yml
--rw-r--r--   0        0        0     1137 2024-04-10 22:05:31.703859 gamdl-2.1.6/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-10 22:05:31.703859 gamdl-2.1.6/.gitignore
--rw-r--r--   0        0        0    11844 2024-04-10 22:05:31.703859 gamdl-2.1.6/README.md
--rw-r--r--   0        0        0       22 2024-04-10 22:05:31.703859 gamdl-2.1.6/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-10 22:05:31.703859 gamdl-2.1.6/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-10 22:05:31.703859 gamdl-2.1.6/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26576 2024-04-10 22:05:31.703859 gamdl-2.1.6/gamdl/cli.py
--rw-r--r--   0        0        0     5580 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/constants.py
--rw-r--r--   0        0        0    12691 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader.py
--rw-r--r--   0        0        0    10392 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2254 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader_post.py
--rw-r--r--   0        0        0    13976 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3865 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      817 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/models.py
--rw-r--r--   0        0        0      560 2024-04-10 22:05:31.707859 gamdl-2.1.6/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-10 22:05:31.707859 gamdl-2.1.6/requirements.txt
--rw-r--r--   0        0        0    12319 1970-01-01 00:00:00.000000 gamdl-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-12 21:07:37.058617 gamdl-2.1.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1137 2024-04-12 21:07:37.058617 gamdl-2.1.7/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-12 21:07:37.058617 gamdl-2.1.7/.gitignore
+-rw-r--r--   0        0        0    11960 2024-04-12 21:07:37.058617 gamdl-2.1.7/README.md
+-rw-r--r--   0        0        0       22 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26706 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/cli.py
+-rw-r--r--   0        0        0     5580 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/constants.py
+-rw-r--r--   0        0        0    12691 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader.py
+-rw-r--r--   0        0        0    10566 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2254 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    14069 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3865 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      817 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-12 21:07:37.058617 gamdl-2.1.7/gamdl/models.py
+-rw-r--r--   0        0        0      592 2024-04-12 21:07:37.058617 gamdl-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-12 21:07:37.058617 gamdl-2.1.7/requirements.txt
+-rw-r--r--   0        0        0    12467 1970-01-01 00:00:00.000000 gamdl-2.1.7/PKG-INFO
```

### Comparing `gamdl-2.1.6/.github/workflows/main.yml` & `gamdl-2.1.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/README.md` & `gamdl-2.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,29 @@
     * Binaries can be obtained from here: https://www.bento4.com/downloads/.
  
 ## Installation
 1. Install the package `gamdl` using pip
     ```bash
     pip install gamdl
     ```
-2. Place your cookies in the same directory you will run gamdl from and name it as `cookies.txt`
+2. Place your cookies file in the directory from which you will be running gamdl and name it `cookies.txt`.
 
 ## Usage
+```bash
+gamdl [OPTIONS] URLS...
+```
+
+### Examples
 * Download a song
     ```bash
-    gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1626265761?i=1626265765"
+    gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1624945511?i=1624945512"
     ```
 * Download an album
     ```bash
-    gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1626265761"
+    gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1624945511"
     ```
 
 ## Configuration
 You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
 | Command line argument / Config file key                         | Description                                                                  | Default value                                |
 | --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
 | `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
@@ -144,30 +149,30 @@
 * `aac-downmix`
 * `aac-he-binaural`
 * `aac-he-downmix`
 * `atmos`
 * `ac3`
 * `alac`
 * `ask`
-    * When using this option, the script will ask you which **non-legacy** codec to use that is available for the song.
+    * When using this option, gamdl will ask you which **non-legacy** codec to use that is available for the song.
 
 **Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
 * `h264-best` (with AAC 256kbps, up to 1080p)
 * `h265-best` (With AAC 256kpbs, up to 2160p)
 * `ask`
-    * When using this option, the script will ask you which audio and video codec to use.
+    * When using this option, gamdl will ask you which audio and video codec to use that is available for the music video.
   
 ### Post videos/extra videos qualities
 The following qualities are available:
 * `best` (with AAC 256kbps, up to 1080p)
 * `ask`
-    * When using this option, the script will ask you which video quality to use.
+    * When using this option, gamdl will ask you which video quality to use that is available for the video.
 
 Post videos doesn't require remuxing and are limited to `ytdlp` download mode.
 
 ### Synced lyrics formats
 The following synced lyrics formats are available:
 * `lrc`
 * `srt`
```

### Comparing `gamdl-2.1.6/gamdl/apple_music_api.py` & `gamdl-2.1.7/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/gamdl/cli.py` & `gamdl-2.1.7/gamdl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,17 @@
     logging.basicConfig(
         format="[%(levelname)-8s %(asctime)s] %(message)s",
         datefmt="%H:%M:%S",
     )
     logger = logging.getLogger(__name__)
     logger.setLevel(log_level)
     logger.debug("Starting downloader")
+    if not cookies_path.exists():
+        logger.critical(X_NOT_FOUND_STRING.format("Cookies file", cookies_path))
+        return
     apple_music_api = AppleMusicApi(
         cookies_path,
         language=language,
     )
     itunes_api = ItunesApi(
         apple_music_api.storefront,
         apple_music_api.language,
```

### Comparing `gamdl-2.1.6/gamdl/constants.py` & `gamdl-2.1.7/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/gamdl/downloader.py` & `gamdl-2.1.7/gamdl/downloader.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/gamdl/downloader_music_video.py` & `gamdl-2.1.7/gamdl/downloader_music_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,15 @@
                 self.downloader.mp4decrypt_path_full,
                 encrypted_path,
                 "--key",
                 f"1:{decryption_key}",
                 decrypted_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def remux_mp4box(
         self,
         decrypted_path_audio: Path,
         decrypted_path_video: Path,
         fixed_path: Path,
@@ -247,14 +248,15 @@
                 decrypted_path_video,
                 "-itags",
                 "artist=placeholder",
                 "-new",
                 fixed_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def remux_ffmpeg(
         self,
         decrypted_path_video: Path,
         decrypte_path_audio: Path,
         fixed_path: Path,
@@ -281,14 +283,15 @@
                 "-c",
                 "copy",
                 "-c:s",
                 "mov_text",
                 fixed_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def remux(
         self,
         decrypted_path_video: Path,
         decrypted_path_audio: Path,
         remuxed_path: Path,
```

### Comparing `gamdl-2.1.6/gamdl/downloader_post.py` & `gamdl-2.1.7/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/gamdl/downloader_song.py` & `gamdl-2.1.7/gamdl/downloader_song.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,17 @@
     def get_lyrics(self, track_metadata: dict) -> Lyrics:
         if not track_metadata["attributes"]["hasLyrics"]:
             return Lyrics()
         elif track_metadata.get("relationships") is None:
             track_metadata = self.downloader.apple_music_api.get_song(
                 track_metadata["id"]
             )
-        if track_metadata["relationships"]["lyrics"]["data"]:
+        if track_metadata["relationships"]["lyrics"]["data"] and track_metadata[
+            "relationships"
+        ]["lyrics"]["data"][0].get("attributes"):
             return self._get_lyrics(
                 track_metadata["relationships"]["lyrics"]["data"][0]["attributes"][
                     "ttml"
                 ]
             )
         else:
             return Lyrics()
@@ -199,17 +201,17 @@
         index = 1
         for div in lyrics_ttml_et.iter("{http://www.w3.org/ns/ttml}div"):
             for p in div.iter("{http://www.w3.org/ns/ttml}p"):
                 if p.text is not None:
                     lyrics.unsynced += p.text + "\n"
                 if p.attrib.get("begin"):
                     if self.synced_lyrics_format == SyncedLyricsFormat.LRC:
-                        lyrics.synced += f"{self.get_lyrics_synced_line_lrc(p.attrib.get('begin'), p.text)}\n"
+                        lyrics.synced += f"{self.get_lyrics_synced_line_lrc(p.attrib.get('begin'), p.text)}"
                     elif self.synced_lyrics_format == SyncedLyricsFormat.SRT:
-                        lyrics.synced += f"{self.get_lyrics_synced_line_srt(index, p.attrib.get('begin'), p.attrib.get('end'), p.text)}\n"
+                        lyrics.synced += f"{self.get_lyrics_synced_line_srt(index, p.attrib.get('begin'), p.attrib.get('end'), p.text)}"
                     elif self.synced_lyrics_format == SyncedLyricsFormat.TTML:
                         if not lyrics.synced:
                             lyrics.synced = minidom.parseString(
                                 lyrics_ttml
                             ).toprettyxml()
                         continue
                     lyrics.synced += "\n"
```

### Comparing `gamdl-2.1.6/gamdl/downloader_song_legacy.py` & `gamdl-2.1.7/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/gamdl/enums.py` & `gamdl-2.1.7/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/gamdl/hardcoded_wvd.py` & `gamdl-2.1.7/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/gamdl/itunes_api.py` & `gamdl-2.1.7/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.6/pyproject.toml` & `gamdl-2.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gamdl"
-description = "Download Apple Music songs/music videos/albums/playlists"
+description = "A Python script to download Apple Music songs/music videos/albums/playlists/post videos."
 requires-python = ">=3.8"
 authors = [{ name = "glomatico" }]
 dependencies = [
     "ciso8601",
     "click",
     "m3u8",
     "tabulate",
```

### Comparing `gamdl-2.1.6/PKG-INFO` & `gamdl-2.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.1.6
-Summary: Download Apple Music songs/music videos/albums/playlists
+Version: 2.1.7
+Summary: A Python script to download Apple Music songs/music videos/albums/playlists/post videos.
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: m3u8
 Requires-Dist: tabulate
@@ -42,24 +42,29 @@
     * Binaries can be obtained from here: https://www.bento4.com/downloads/.
  
 ## Installation
 1. Install the package `gamdl` using pip
     ```bash
     pip install gamdl
     ```
-2. Place your cookies in the same directory you will run gamdl from and name it as `cookies.txt`
+2. Place your cookies file in the directory from which you will be running gamdl and name it `cookies.txt`.
 
 ## Usage
+```bash
+gamdl [OPTIONS] URLS...
+```
+
+### Examples
 * Download a song
     ```bash
-    gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1626265761?i=1626265765"
+    gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1624945511?i=1624945512"
     ```
 * Download an album
     ```bash
-    gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1626265761"
+    gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1624945511"
     ```
 
 ## Configuration
 You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
 | Command line argument / Config file key                         | Description                                                                  | Default value                                |
 | --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
 | `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
@@ -161,30 +166,30 @@
 * `aac-downmix`
 * `aac-he-binaural`
 * `aac-he-downmix`
 * `atmos`
 * `ac3`
 * `alac`
 * `ask`
-    * When using this option, the script will ask you which **non-legacy** codec to use that is available for the song.
+    * When using this option, gamdl will ask you which **non-legacy** codec to use that is available for the song.
 
 **Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
 * `h264-best` (with AAC 256kbps, up to 1080p)
 * `h265-best` (With AAC 256kpbs, up to 2160p)
 * `ask`
-    * When using this option, the script will ask you which audio and video codec to use.
+    * When using this option, gamdl will ask you which audio and video codec to use that is available for the music video.
   
 ### Post videos/extra videos qualities
 The following qualities are available:
 * `best` (with AAC 256kbps, up to 1080p)
 * `ask`
-    * When using this option, the script will ask you which video quality to use.
+    * When using this option, gamdl will ask you which video quality to use that is available for the video.
 
 Post videos doesn't require remuxing and are limited to `ytdlp` download mode.
 
 ### Synced lyrics formats
 The following synced lyrics formats are available:
 * `lrc`
 * `srt`
```


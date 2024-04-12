# Comparing `tmp/pispy-client-0.4.0.tar.gz` & `tmp/pispy-client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pispy-client-0.4.0.tar", last modified: Wed Apr 10 14:13:00 2024, max compression
+gzip compressed data, was "pispy-client-0.5.0.tar", last modified: Fri Apr 12 15:22:32 2024, max compression
```

## Comparing `pispy-client-0.4.0.tar` & `pispy-client-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,23 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 14:13:00.799626 pispy-client-0.4.0/
--rw-r--r--   0 davep      (501) staff       (20)     2403 2024-04-10 14:13:00.799572 pispy-client-0.4.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     1108 2024-04-10 13:45:14.000000 pispy-client-0.4.0/README.md
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 14:13:00.797122 pispy-client-0.4.0/pispy/
--rw-r--r--   0 davep      (501) staff       (20)      403 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      378 2024-04-10 13:45:14.000000 pispy-client-0.4.0/pispy/__main__.py
--rw-r--r--   0 davep      (501) staff       (20)     1209 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/app.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 14:13:00.797579 pispy-client-0.4.0/pispy/data/
--rw-r--r--   0 davep      (501) staff       (20)      371 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/data/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     7438 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/data/package.py
--rw-r--r--   0 davep      (501) staff       (20)     1856 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/data/stats.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2024-04-10 13:45:14.000000 pispy-client-0.4.0/pispy/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 14:13:00.798006 pispy-client-0.4.0/pispy/screens/
--rw-r--r--   0 davep      (501) staff       (20)      356 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/screens/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     2615 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/screens/lookup.py
--rw-r--r--   0 davep      (501) staff       (20)     1092 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/screens/stats.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 14:13:00.798473 pispy-client-0.4.0/pispy/widgets/
--rw-r--r--   0 davep      (501) staff       (20)      373 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/widgets/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     8761 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/widgets/package_info.py
--rw-r--r--   0 davep      (501) staff       (20)     1880 2024-04-10 14:03:43.000000 pispy-client-0.4.0/pispy/widgets/top_by_size.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-10 14:13:00.799363 pispy-client-0.4.0/pispy_client.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     2403 2024-04-10 14:13:00.000000 pispy-client-0.4.0/pispy_client.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      539 2024-04-10 14:13:00.000000 pispy-client-0.4.0/pispy_client.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-10 14:13:00.000000 pispy-client-0.4.0/pispy_client.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       45 2024-04-10 14:13:00.000000 pispy-client-0.4.0/pispy_client.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       22 2024-04-10 14:13:00.000000 pispy-client-0.4.0/pispy_client.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)        6 2024-04-10 14:13:00.000000 pispy-client-0.4.0/pispy_client.egg-info/top_level.txt
--rw-r--r--   0 davep      (501) staff       (20)      124 2024-04-10 14:08:22.000000 pispy-client-0.4.0/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1404 2024-04-10 14:13:00.799885 pispy-client-0.4.0/setup.cfg
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.658897 pispy-client-0.5.0/
+-rw-r--r--   0 davep      (501) staff       (20)     2403 2024-04-12 15:22:32.658781 pispy-client-0.5.0/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     1108 2024-04-10 13:45:14.000000 pispy-client-0.5.0/README.md
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.656562 pispy-client-0.5.0/pispy/
+-rw-r--r--   0 davep      (501) staff       (20)      403 2024-04-12 15:20:43.000000 pispy-client-0.5.0/pispy/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      378 2024-04-10 13:45:14.000000 pispy-client-0.5.0/pispy/__main__.py
+-rw-r--r--   0 davep      (501) staff       (20)     1935 2024-04-12 09:50:20.000000 pispy-client-0.5.0/pispy/app.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.656816 pispy-client-0.5.0/pispy/data/
+-rw-r--r--   0 davep      (501) staff       (20)      331 2024-04-11 08:19:00.000000 pispy-client-0.5.0/pispy/data/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     7041 2024-04-12 15:02:03.000000 pispy-client-0.5.0/pispy/data/package.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2024-04-10 13:45:14.000000 pispy-client-0.5.0/pispy/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.657079 pispy-client-0.5.0/pispy/widgets/
+-rw-r--r--   0 davep      (501) staff       (20)      325 2024-04-11 08:19:00.000000 pispy-client-0.5.0/pispy/widgets/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     8776 2024-04-12 15:20:26.000000 pispy-client-0.5.0/pispy/widgets/package_info.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-12 15:22:32.658211 pispy-client-0.5.0/pispy_client.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     2403 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      417 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       45 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       22 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)        6 2024-04-12 15:22:32.000000 pispy-client-0.5.0/pispy_client.egg-info/top_level.txt
+-rw-r--r--   0 davep      (501) staff       (20)      124 2024-04-11 08:19:00.000000 pispy-client-0.5.0/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1404 2024-04-12 15:22:32.659229 pispy-client-0.5.0/setup.cfg
```

### Comparing `pispy-client-0.4.0/PKG-INFO` & `pispy-client-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pispy-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A terminal-based Python package index inspector
 Home-page: https://github.com/davep/pispy
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `pispy-client-0.4.0/README.md` & `pispy-client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pispy-client-0.4.0/pispy/data/package.py` & `pispy-client-0.5.0/pispy/data/package.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,80 +13,80 @@
 ##############################################################################
 def _get(
     payload: dict[str, dict[str, Any]], via: str, value: str, default: Any = ""
 ) -> Any:
     """Get some data, default if it isn't there or is `None`.
 
     Args:
-        payload (dict[ str, dict[ str, Any ] ]): The payload from the API.
-        via (str): The child collection to get the value via.
-        value (str): The value to get.
-        default (Any, optional): The default to use.
+        payload: The payload from the API.
+        via: The child collection to get the value via.
+        value: The value to get.
+        default: The default to use.
 
     Returns:
-        Any: The value found, or the default.
+        The value found, or the default.
 
     Note:
         The default is used if `value` can't be found, or if it is `None`.
     """
     return default if (result := payload.get(via, {}).get(value)) is None else result
 
 
 ##############################################################################
 class PackageURL(NamedTuple):
     """A package's release URL data."""
 
     comment_text: str
-    """str: The comment text for the URL."""
+    """The comment text for the URL."""
 
     digests: dict[str, str]
-    """dict[ str, str ]: The digests for the URL."""
+    """The digests for the URL."""
 
     downloads: int
-    """int: The number of downloads for the URL."""
+    """The number of downloads for the URL."""
 
     filename: str
-    """str: The filename for the URL."""
+    """The filename for the URL."""
 
     has_sig: bool
-    """bool: Does the URL have a signature?"""
+    """Does the URL have a signature?"""
 
     md5_digest: str
-    """str: The MD5 digest for the URL."""
+    """The MD5 digest for the URL."""
 
     packagetype: str
-    """str: The type of package."""
+    """The type of package."""
 
     python_version: str
-    """str: The version of package for this URL."""
+    """The version of package for this URL."""
 
     size: int
-    """int: The size of the download at this URL."""
+    """The size of the download at this URL."""
 
     upload_time_iso_8601: str
-    """str: The upload time of the URL in ISo 8601 format."""
+    """The upload time of the URL in ISo 8601 format."""
 
     url: str
-    """str: The URL itself."""
+    """The URL itself."""
 
     yanked: bool
-    """bool: Has this URL been yanked?"""
+    """Has this URL been yanked?"""
 
     yanked_reason: str
-    """str: The reason for the yank, if the URL has been yanked."""
+    """The reason for the yank, if the URL has been yanked."""
 
     @classmethod
     def from_json(cls, data: dict[str, Any]) -> "PackageURL":
         """Get package URL information from the given data.
 
         Args:
-            data (dict[ str, Any ]): The URL data.
+            data: The URL data.
 
         Returns:
-            PackageURL: An instance of a `PackageURL` class.
+            An instance of a `PackageURL` class.
         """
         url = partial(_get, {"url": data}, "url")
         return cls(
             comment_text=url("comment_text"),
             digests=url("digests", {}),
             downloads=url("downloads", 0),
             filename=url("filename"),
@@ -103,101 +103,100 @@
 
 
 ##############################################################################
 class Package(NamedTuple):
     """A Package in PyPi."""
 
     author: str
-    """str: The author of the package."""
+    """The author of the package."""
 
     author_email: str
-    """str: The email address of the author."""
+    """The email address of the author."""
 
     bugtrack_url: str
-    """str: The URL for the package's bug tracker."""
+    """The URL for the package's bug tracker."""
 
     classifiers: list[str]
-    """list[ str ]: The list of classifiers for the package."""
+    """The list of classifiers for the package."""
 
     description: str
-    """str: The description for the package."""
+    """The description for the package."""
 
     description_content_type: str
-    """str: The content type of the description."""
+    """The content type of the description."""
 
     docs_url: str
-    """str: The URL for the packages documentation."""
+    """The URL for the packages documentation."""
 
     download_url: str
-    """str: The URL to download the package."""
+    """The URL to download the package."""
 
     homepage: str
-    """str: The homepage for the package."""
+    """The homepage for the package."""
 
     keywords: list[str]
-    """list[ str ]: The keywords for the package."""
+    """The keywords for the package."""
 
     license: str
-    """str: The licence for the package."""
+    """The licence for the package."""
 
     maintainer: str
-    """str: The name of the maintainer of the package."""
+    """The name of the maintainer of the package."""
 
     maintainer_email: str
-    """str: The email address of the maintainer of the package."""
+    """The email address of the maintainer of the package."""
 
     name: str
-    """str: The name of the package."""
+    """The name of the package."""
 
     package_url: str
-    """str: The URL for the package."""
+    """The URL for the package."""
 
     platform: str
-    """str: The platform for the package."""
+    """The platform for the package."""
 
     project_url: str
-    """str: The URL of the project for the package."""
+    """The URL of the project for the package."""
 
     project_urls: dict[str, str]
-    """dict[ str, str ]: The URLs for the project associated with the package."""
+    """The URLs for the project associated with the package."""
 
     release_url: str
-    """str: The URL of the latest release of the package."""
+    """The URL of the latest release of the package."""
 
     requires_dist: list[str]
-    """list[ str ]: The requirements for the distribution of the package."""
+    """The requirements for the distribution of the package."""
 
     requires_python: str
-    """str: The version of Python required for the package."""
+    """The version of Python required for the package."""
 
     summary: str
-    """str: The summary of the package."""
+    """The summary of the package."""
 
     version: str
-    """str: The version of the package."""
+    """The version of the package."""
 
     yanked: bool
-    """bool: Has the package been yanked?"""
+    """Has the package been yanked?"""
 
     yanked_reason: str
-    """str: The reason for the yank, if the package has been yanked."""
+    """The reason for the yank, if the package has been yanked."""
 
     urls: list[PackageURL]
-    """list[ URL ]: The URLs for this package."""
+    """The URLs for this package."""
 
     @classmethod
     async def from_pypi(cls, package: str) -> tuple[bool, "Package"]:
         """Get information on the given package from PyPi.
 
         Args:
-            package (str): The name of the package to get data for.
+            package: The name of the package to get data for.
 
         Returns:
-            tuple[ bool, Package ]: A flag to say if the package was found
-                and package data.
+            A flag to say if the package was found and package data.
         """
 
         async with httpx.AsyncClient() as client:
 
             # Get the package's data from the API.
             resp = await client.get(
                 f"https://pypi.org/pypi/{package}/json", follow_redirects=True
@@ -215,17 +214,17 @@
                 author_email=info("author_email"),
                 bugtrack_url=info("bugtrack_url"),
                 classifiers=info("classifiers", []),
                 description=info("description"),
                 description_content_type=info("description_content_type"),
                 docs_url=info("docs_url"),
                 download_url=info("download_url"),
-                homepage=info("homepage"),
+                homepage=info("home_page"),
                 keywords=info("keywords").split(),
-                license=info("licence"),
+                license=info("license"),
                 maintainer=info("maintainer"),
                 maintainer_email=info("maintainer_email"),
                 name=info("name"),
                 package_url=info("package_url"),
                 platform=info("platform"),
                 project_url=info("project_url"),
                 project_urls=info("project_urls", {}),
```

### Comparing `pispy-client-0.4.0/pispy/widgets/package_info.py` & `pispy-client-0.5.0/pispy/widgets/package_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,286 +1,274 @@
 """Provides a widget that shows package information."""
 
 ##############################################################################
 # Python imports.
-from typing import Any, Iterator
+from functools import singledispatch
+from typing import Any, Callable, Iterator
+from webbrowser import open as visit_url
+
+##############################################################################
+# Package resources imports.
 from pkg_resources import parse_requirements
 
 ##############################################################################
 # Textual imports.
 from textual.app import ComposeResult
-from textual.containers import Vertical
+from textual.containers import Vertical, VerticalScroll
+from textual.widget import Widget
 from textual.widgets import Label, Markdown
 
 ##############################################################################
-# Rich imports.
-from rich.console import RenderableType
-
-##############################################################################
 # Local imports.
 from ..data import Package, PackageURL
 
 
 ##############################################################################
 class Title(Label):
     """A title for an item of package information."""
 
     DEFAULT_CSS = """
     Title {
         background: $panel-lighten-3;
         text-style: bold;
-        width: 100%;
+        width: 1fr;
     }
     """
-    """str: The defaults styles."""
+    """The defaults styles."""
 
     def __init__(self, text: str) -> None:
         """Initialise the title.
 
         Args:
-            text (str): The title.
+            text: The title.
         """
         super().__init__(f"{text}:")
 
 
 ##############################################################################
 class Value(Label):
     """A value for an item of package information."""
 
     DEFAULT_CSS = """
     Value {
         background: $panel;
         padding-bottom: 1;
-        width: 100%;
-    }
-
-    Value.none {
-        color: $text-muted;
+        width: 1fr;
     }
     """
-    """str: The default styles."""
-
-    def __init__(self, value: RenderableType, *args: Any, **kwargs: Any) -> None:
-        """Initialise the value.
-
-        Args:
-            value (RenderableType): The value.
-        """
-        super().__init__(
-            value or "None", *args, classes=("none" if not value else ""), **kwargs
-        )
 
 
 ##############################################################################
-class URL(Markdown):
+class URL(Label):
     """A URL for an item of package information."""
 
     DEFAULT_CSS = """
     URL {
         background: $panel;
-        margin: 0;
+        padding-bottom: 1;
+        width: 1fr;
     }
     """
 
     def __init__(self, url: str) -> None:
         """Initialise the URL.
 
         Args:
-            url (str): The URL.
+            url: The URL.
         """
-        super().__init__(f"<{url}>" if url else "*None*")
+        super().__init__(f"[@click=visit('{url}')]{url}[/]")
+
+    def action_visit(self, url: str) -> None:
+        """Visit the given URL.
+
+        Args:
+           url: The URL to visit.
+        """
+        visit_url(url)
+
+
+##############################################################################
+@singledispatch
+def maybe_show(
+    title: str, value: Any, widget: Callable[[Any], Widget]
+) -> Iterator[Widget]:
+    """Maybe show a value with a given title.
+
+    Args:
+        title: The title for the value to show.
+        value: The value to show.
+        widget: The type of widget to show the value.
+
+    Yields:
+        The widgets required to show the value.
+    """
+    yield Title(title)
+    yield widget(value)
+
+
+##############################################################################
+@maybe_show.register
+def _(title: str, value: None, widget: Callable[[Any], Widget]) -> Iterator[Widget]:
+    """Show noting when the value is `None`."""
+    del title, value, widget
+    yield from ()
+
+
+##############################################################################
+@maybe_show.register
+def _(title: str, value: str, widget: Callable[[Any], Widget]) -> Iterator[Widget]:
+    """Maybe show a string value."""
+    if value:
+        yield Title(title)
+        yield widget(value)
+
+
+##############################################################################
+def widgets_for(*values: tuple[str, Any, Callable[[Any], Widget]]) -> Iterator[Widget]:
+    """Generate the widgets needed to show the given values.
+
+    Args:
+        values: The collection of values to show.
+
+    Yields:
+        The widgets required to show the values.
+    """
+    for title, value, display in values:
+        yield from maybe_show(title, value, display)
 
 
 ##############################################################################
 class PackageURLData(Vertical):
     """Widget for displaying data about a package URL."""
 
     DEFAULT_CSS = """
     PackageURLData {
         height: auto;
-        margin: 1 2;
         border: solid $accent;
         background: $panel;
     }
     """
 
     def __init__(self, url: PackageURL, *args: Any, **kwargs: Any) -> None:
         """Initialise the package URL widget.
 
         Args:
-            url (PackageURL): The package URL to display the data for.
+            url: The package URL to display the data for.
         """
         super().__init__(*args, **kwargs)
         self._url = url
 
-    @staticmethod
-    def digests(digest_data: dict[str, str]) -> Iterator[Title | Value]:
-        """Generate the widgets for displaying digest items.
-
-        Args:
-            digest_data (dict[ str, str]): The digest data for the URL.
-
-        Yields:
-            Title | Value: The widgets for displaying the data.
-        """
-        for name, value in digest_data.items():
-            yield Title(name)
-            yield Value(value)
-
     def compose(self) -> ComposeResult:
         """Compose the package URL display.
 
         Returns:
-            ComposeResult: The package URL data layout.
+            The package URL data layout.
         """
-        yield Title("URL")
-        yield URL(self._url.url)
-        yield Title("Package Type")
-        yield Value(self._url.packagetype)
-        yield Title("Python Version")
-        yield Value(self._url.python_version)
-        yield Title("Size")
-        yield Value(f"{self._url.size:,}")
-        yield Title("MD5 Digest")
-        yield Value(self._url.md5_digest)
-        yield Title("Uploaded")
-        yield Value(self._url.upload_time_iso_8601)
-        yield Title("Has Signature")
-        yield Value("Yes" if self._url.has_sig else "No")
-        yield Title("Downloads")
-        yield Value(f"{self._url.downloads:,}")
-        yield Title("Comments")
-        yield Value(self._url.comment_text)
-        yield from self.digests(self._url.digests)
-        yield Title("Yanked Reason")
-        yield Value("Yes" if self._url.yanked else "No")
-        yield Title("Yanked Reason")
-        yield Value(self._url.yanked_reason)
+        yield from widgets_for(
+            ("URL", self._url.url, URL),
+            ("Package Type", self._url.packagetype, Value),
+            ("Python Version", self._url.python_version, Value),
+            ("Size", f"{self._url.size:,}", Value),
+            ("MD5 Digest", self._url.md5_digest, Value),
+            ("Uploaded", self._url.upload_time_iso_8601, Value),
+            ("Has Signature", "Yes" if self._url.has_sig else "No", Value),
+            ("Downloads", f"{self._url.downloads:,}", Value),
+            ("Comments", self._url.comment_text, Value),
+            *((name, value, Value) for name, value in self._url.digests.items()),
+            ("Yanked", "Yes" if self._url.yanked else "No", Value),
+            ("Yanked Reason", self._url.yanked_reason, Value),
+        )
 
 
 ##############################################################################
-class PackageInfo(Vertical, can_focus=True):
+class PackageInfo(VerticalScroll):
     """Widget for displaying package information."""
 
     DEFAULT_CSS = """
     PackageInfo {
-        border: tall $primary;
+        border: tall $background;
         height: 1fr;
-    }
-
-    PackageInfo:focus {
-        border: tall $accent;
-    }
+        padding: 0 1;
 
-    PackageInfo Label.error {
-        color: red;
-        text-style: bold;
+        &:focus {
+            border: tall $accent;
+        }
+
+        Label.error {
+            color: red;
+            text-style: bold;
+        }
     }
     """
 
-    async def clear(self) -> None:
-        """Clear the content of the widget."""
-        await self.query("PackageInfo > * ").remove()
-
-    @staticmethod
-    def project_urls(urls: dict[str, str]) -> Iterator[Title | URL]:
-        """Generate title/URL widgets from the project's URLs.
-
-        Args:
-            urls (dict[ str, str]): The project URLs.
-
-        Yields:
-            Title | URL: A title or a URL.
-        """
-        for title, url in urls.items():
-            yield Title(title)
-            yield URL(url)
-
-    @staticmethod
-    def package_urls(urls: list[PackageURL]) -> Iterator[Title | PackageURLData]:
-        for package in urls:
-            yield Title(package.filename)
-            yield PackageURLData(package)
-
     async def show(self, package_name: str) -> None:
         """Show the package information for the given package.
 
         Args:
-            package_name (str): The name of the package to lookup and show
+            package_name: The name of the package to lookup and show
         """
 
         # Don't bother trying to do anything if there isn't actually a name.
         if not package_name.strip():
             return
 
         # Clear any previous content.
-        await self.clear()
+        await self.remove_children()
 
         # Download the data for the package.
         found, package = await Package.from_pypi(package_name)
 
         # If we found it...
         if found:
-            # ...populate the output.
             await self.mount(
-                Title("Name"),
-                Value(package.name),
-                Title("Version"),
-                Value(package.version),
-                Title("Summary"),
-                Value(package.summary),
-                Title("URL"),
-                URL(package.package_url),
-                Title("Author"),
-                Value(package.author),
-                Title("Email"),
-                Value(package.author_email),
-                Title("Bug Track URL"),
-                URL(package.bugtrack_url),
-                Title("Classifiers"),
-                Value("\n".join(package.classifiers)),
-                Title("Description"),
-                (
-                    Markdown(package.description)
-                    if package.description_content_type == "text/markdown"
-                    else Value(package.description)
-                ),
-                Title("Documentation URL"),
-                URL(package.docs_url),
-                Title("Download URL"),
-                URL(package.download_url),
-                Title("Homepage"),
-                URL(package.homepage),
-                Title("Keywords"),
-                Value(", ".join(package.keywords)),
-                Title("License"),
-                Value(package.license),
-                Title("Maintainer"),
-                Value(package.maintainer),
-                Title("Email"),
-                Value(package.maintainer_email),
-                Title("Platform"),
-                Value(package.platform),
-                Title("Project URL"),
-                URL(package.project_url),
-                *self.project_urls(package.project_urls),
-                Title("Release URL"),
-                URL(package.release_url),
-                Title("Requires"),
-                Value(
-                    ", ".join(
-                        f"[@click=screen.lookup('{pkg.project_name}')]{pkg.project_name}[/]"
-                        for pkg in parse_requirements(package.requires_dist)
-                    )
-                ),
-                Title("Yanked"),
-                Value("Yes" if package.yanked else "No"),
-                Title("Yanked Reason"),
-                Value(package.yanked_reason),
-                *self.package_urls(package.urls),
+                *widgets_for(
+                    ("Name", package.name, Value),
+                    ("Version", package.version, Value),
+                    ("Summary", package.summary, Value),
+                    ("URL", package.package_url, URL),
+                    ("Author", package.author, Value),
+                    ("Email", package.author_email, Value),
+                    ("Bug Track URL", package.bugtrack_url, URL),
+                    ("Classifiers", "\n".join(package.classifiers), Value),
+                    (
+                        "Description",
+                        package.description,
+                        Markdown
+                        if package.description_content_type == "text/markdown"
+                        else Value,
+                    ),
+                    ("Documentation URL", package.docs_url, URL),
+                    ("Download URL", package.download_url, URL),
+                    ("Homepage", package.homepage, URL),
+                    ("Keywords", ", ".join(package.keywords), Value),
+                    ("License", package.license, Value),
+                    ("Maintainer", package.maintainer, Value),
+                    ("Email", package.maintainer_email, Value),
+                    ("Platform", package.platform, Value),
+                    ("Project URL", package.project_url, URL),
+                    *(
+                        (title, value, URL)
+                        for title, value in package.project_urls.items()
+                    ),
+                    ("Release URL", package.release_url, URL),
+                    (
+                        "Requires",
+                        ", ".join(
+                            f"[@click=screen.lookup('{pkg.project_name}')]{pkg.project_name}[/]"
+                            for pkg in parse_requirements(package.requires_dist)
+                        ),
+                        Value,
+                    ),
+                    ("Yanked", "Yes" if package.yanked else "No", Value),
+                    ("Yanked Reason", package.yanked_reason, Value),
+                    *(
+                        (package.filename, package, PackageURLData)
+                        for package in package.urls
+                    ),
+                )
             )
         else:
             # Report that we didn't find it.
-            await self.query_one(PackageInfo).mount(Label("Not found", classes="error"))
+            await self.mount(Label("Not found", classes="error"))
 
 
 ### package_info.py ends here
```

### Comparing `pispy-client-0.4.0/pispy_client.egg-info/PKG-INFO` & `pispy-client-0.5.0/pispy_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pispy-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A terminal-based Python package index inspector
 Home-page: https://github.com/davep/pispy
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `pispy-client-0.4.0/setup.cfg` & `pispy-client-0.5.0/setup.cfg`

 * *Files identical despite different names*


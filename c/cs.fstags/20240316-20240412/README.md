# Comparing `tmp/cs.fstags-20240316.tar.gz` & `tmp/cs.fstags-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.fstags-20240316.tar", last modified: Sat Mar 16 06:49:13 2024, max compression
+gzip compressed data, was "cs.fstags-20240412.tar", last modified: Fri Apr 12 05:44:48 2024, max compression
```

## Comparing `cs.fstags-20240316.tar` & `cs.fstags-20240412.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:49:13.634719 cs.fstags-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)      148 2024-03-16 06:48:39.000000 cs.fstags-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    21183 2024-03-16 06:49:13.634411 cs.fstags-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    37249 2024-03-16 06:48:50.000000 cs.fstags-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:49:13.625918 cs.fstags-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:49:13.626233 cs.fstags-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:49:13.631244 cs.fstags-20240316/lib/python/cs/
--rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-03-16 06:48:39.000000 cs.fstags-20240316/lib/python/cs/fstags.1
--rw-r--r--   0 cameron    (501) cameron    (502)     7052 2024-03-16 06:48:19.000000 cs.fstags-20240316/lib/python/cs/fstags.1.md
--rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-03-16 06:48:39.000000 cs.fstags-20240316/lib/python/cs/fstags.5
--rw-r--r--   0 cameron    (501) cameron    (502)    17938 2024-03-16 06:48:19.000000 cs.fstags-20240316/lib/python/cs/fstags.5.md
--rw-r--r--   0 cameron    (501) cameron    (502)    72299 2024-03-16 06:48:19.000000 cs.fstags-20240316/lib/python/cs/fstags.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:49:13.633953 cs.fstags-20240316/lib/python/cs.fstags.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    21183 2024-03-16 06:49:13.000000 cs.fstags-20240316/lib/python/cs.fstags.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      424 2024-03-16 06:49:13.000000 cs.fstags-20240316/lib/python/cs.fstags.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:49:13.000000 cs.fstags-20240316/lib/python/cs.fstags.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       42 2024-03-16 06:49:13.000000 cs.fstags-20240316/lib/python/cs.fstags.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      249 2024-03-16 06:49:13.000000 cs.fstags-20240316/lib/python/cs.fstags.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:49:13.000000 cs.fstags-20240316/lib/python/cs.fstags.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    21966 2024-03-16 06:49:12.000000 cs.fstags-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:49:13.634812 cs.fstags-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.348170 cs.fstags-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)      148 2024-04-12 05:44:16.000000 cs.fstags-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    37873 2024-04-12 05:44:48.347893 cs.fstags-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    37084 2024-04-12 05:44:26.000000 cs.fstags-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.341050 cs.fstags-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.341279 cs.fstags-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.345249 cs.fstags-20240412/lib/python/cs/
+-rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-04-12 05:44:16.000000 cs.fstags-20240412/lib/python/cs/fstags.1
+-rw-r--r--   0 cameron    (501) cameron    (502)     7052 2024-04-12 05:44:01.000000 cs.fstags-20240412/lib/python/cs/fstags.1.md
+-rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-04-12 05:44:16.000000 cs.fstags-20240412/lib/python/cs/fstags.5
+-rw-r--r--   0 cameron    (501) cameron    (502)    17938 2024-04-12 05:44:01.000000 cs.fstags-20240412/lib/python/cs/fstags.5.md
+-rw-r--r--   0 cameron    (501) cameron    (502)    72286 2024-04-12 05:44:01.000000 cs.fstags-20240412/lib/python/cs/fstags.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.347503 cs.fstags-20240412/lib/python/cs.fstags.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    37873 2024-04-12 05:44:47.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      424 2024-04-12 05:44:48.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:44:47.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       42 2024-04-12 05:44:47.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      247 2024-04-12 05:44:48.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:44:48.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    38674 2024-04-12 05:44:46.000000 cs.fstags-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:44:48.348254 cs.fstags-20240412/setup.cfg
```

### Comparing `cs.fstags-20240316/README.md` & `cs.fstags-20240412/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Simple filesystem based file tagging
 and the associated `fstags` command line script.
 
-*Latest release 20240316*:
-* TaggedPath.infer_tags: add _dt, _date, _f conversions, skip conversions which raise TypeError or ValueError.
-* rpaths: fix to yield relative paths.
+*Latest release 20240412*:
+Changes to accomodate dropping BaseCommandOptions.runstate.
 
 Many basic tasks can be performed with the `fstags` command line utility,
 documented under the `FSTagsCommand` class below.
 
 Why `fstags`?
 By storing the tags in a separate file we:
 * can store tags without modifying a file
@@ -79,15 +78,15 @@
 for the first cascade `value` found in `tagset`,
 or `None` if there is no match.
 
 ## `DEFAULT_FSTAGS = FSTags('.fstags')`
 
 A class to examine filesystem tags.
 
-## Class `FSTags(cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `FSTags(cs.resources.MultiOpenMixin)`
 
 A class to examine filesystem tags.
 
 *Method `FSTags.__init__(self, tagsfile_basename=None, ontology_filepath=None, physical=None, update_mapping: Optional[Mapping] = None, update_prefix: Optional[str] = 'cs.fstags', update_uuid_tag_name: Optional[str] = 'uuid')`*:
 Initialise the `FSTags` instance.
 
 Parameters:
@@ -392,15 +391,15 @@
           Update extended attributes from tags.
 
 *`FSTagsCommand.Options`*
 
 *Method `FSTagsCommand.apply_opt(self, opt, val)`*:
 Apply command line option.
 
-*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd)`*:
+*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
 Usage: {cmd} paths...
 Tag paths based on rules from the rc file.
 
 *Method `FSTagsCommand.cmd_cp(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX cp(1) equivalent, but also copying tags:
 copy files and their tags into targetdir.
@@ -418,27 +417,27 @@
 Edit the direct tagsets of path, default: '.'
 If path is a directory, provide the tags of its entries.
 Otherwise edit just the tags for path.
 -a    List all names in directory edit mode; normally
       names commencing with a dot are omitted.
 -d    Treat directories like files: edit just its tags.
 
-*Method `FSTagsCommand.cmd_export(self, argv)`*:
+*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
 Usage: {cmd} [-a] [--direct] path {{tag[=value]|-tag}}...
 Export tags for files from paths matching all the constraints.
 -a        Export all paths, not just those with tags.
 --direct  Export the direct tags instead of the computed tags.
 The output is in the same CSV format as that from "sqltags export",
 with the following columns:
 * unixtime: the file's st_mtime from os.stat.
 * id: empty
 * name: the file path
 * tags: the file's direct or indirect tags
 
-*Method `FSTagsCommand.cmd_find(self, argv)`*:
+*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
 Usage: {cmd} [--direct] [--for-rsync] [-o output_format] path {{tag[=value]|-tag}}...
 List files from path matching all the constraints.
 --direct    Use direct tags instead of all tags.
 --for-rsync Instead of listing matching paths, emit a
             sequence of rsync(1) patterns suitable for use with
             --include-from in order to do a selective rsync of the
             matched paths.
@@ -470,15 +469,15 @@
 POSIX ln(1) equivalent, but also copying the tags:
 link files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
 -n  No remove: fail if the destination exists.
 -v  Verbose: show linked files.
 
-*Method `FSTagsCommand.cmd_ls(self, argv)`*:
+*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
 Usage: {cmd} [-d] [--direct] [-o output_format] [paths...]
 List files from paths and their tags.
 -d          Treat directories like files, do not recurse.
 --direct    List direct tags instead of all tags.
 -l          Long format.
 -o output_format
             Use output_format as a Python format string to lay out
@@ -561,15 +560,15 @@
 * `f`: the source CSV file
 * `convert_name`: a callable to convert each input name
   into a file path; the default is to use the input name directly
 
 *Method `FSTagsCommand.run_context(self)`*:
 Push the `FSTags`.
 
-## Class `FSTagsConfig(cs.fs.FSPathBasedSingleton, cs.obj.SingletonMixin, cs.fs.HasFSPath)`
+## Class `FSTagsConfig(cs.fs.FSPathBasedSingleton)`
 
 A configuration for fstags.
 
 *Method `FSTagsConfig.__init__(self, rcfilepath=None, physical=None)`*:
 Initialise the config.
 
 Parameters:
@@ -584,15 +583,15 @@
 
 *Method `FSTagsConfig.load_config(rcfilepath)`*:
 Read an rc file, return a `ConfigParser` instance.
 
 *Property `FSTagsConfig.tagsfile_basename`*:
 The tags filename, default `'.fstags'`.
 
-## Class `FSTagsTagFile(cs.tagset.TagFile, cs.fs.FSPathBasedSingleton, cs.obj.SingletonMixin, cs.fs.HasFSPath, cs.tagset.BaseTagSets, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container, HasFSTagsMixin)`
+## Class `FSTagsTagFile(cs.tagset.TagFile, HasFSTagsMixin)`
 
 A `FSTagsTagFile` indexing `TagSet`s for file paths
 which lives in the file path's directory.
 
 *Method `FSTagsTagFile.TagSetClass(self, name: str) -> cs.fstags.TaggedPath`*:
 factory to create a `TaggedPath` from a `name`.
 
@@ -636,15 +635,15 @@
 for all selected subpaths.
 
 ## Function `rsync_patterns(paths, top_path)`
 
 Return a list of rsync include lines
 suitable for use with the `--include-from` option.
 
-## Class `TaggedPath(cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin, HasFSTagsMixin, cs.fs.HasFSPath, cs.deco.Promotable)`
+## Class `TaggedPath(cs.tagset.TagSet, HasFSTagsMixin, cs.fs.HasFSPath, cs.deco.Promotable)`
 
 Class to manipulate the tags for a specific path.
 
 *Property `TaggedPath.all_tags`*:
 Cached cumulative tags for this path as a `TagSet`
 by merging the tags from the root to the path.
 
@@ -701,15 +700,15 @@
 the following additional names are available:
 * `fspath.basename`: basename of the `TaggedPath.fspath`
 * `fspath.ext`: the file extension of the basename
   of the `TaggedPath.fspath`
 * `fspath.pathname`: the `TaggedPath.fspath`
 * `fspath.encoded`: the JSON encoded fspath
 
-*Method `TaggedPath.from_str(fspath, *, fstags: cs.fstags.FSTags)`*:
+*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x1112f9510>)`*:
 Supports the `@promote` decorator.
 
 *Method `TaggedPath.get_xattr_tagset(self, xattr_name=None)`*:
 Return a new `TagSet`
 from the extended attribute `xattr_name` of `self.fspath`.
 The default `xattr_name` is `XATTR_B` (`None`).
 
@@ -782,14 +781,17 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20240412*:
+Changes to accomodate dropping BaseCommandOptions.runstate.
+
 *Release 20240316*:
 * TaggedPath.infer_tags: add _dt, _date, _f conversions, skip conversions which raise TypeError or ValueError.
 * rpaths: fix to yield relative paths.
 
 *Release 20240211*:
 * TaggedPath: subclass Promotable, add from_str(fspath) class method.
 * FSTags: new mv(srcpath,dstpath) method to move/link/symlink a file bringing its tags.
```

### Comparing `cs.fstags-20240316/lib/python/cs/fstags.1.md` & `cs.fstags-20240412/lib/python/cs/fstags.1.md`

 * *Files identical despite different names*

### Comparing `cs.fstags-20240316/lib/python/cs/fstags.5.md` & `cs.fstags-20240412/lib/python/cs/fstags.5.md`

 * *Files identical despite different names*

### Comparing `cs.fstags-20240316/lib/python/cs/fstags.py` & `cs.fstags-20240412/lib/python/cs/fstags.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,30 +111,30 @@
     cutsuffix,
     get_ini_clause_entryname,
     FormatAsError,
     titleify_lc,
 )
 from cs.logutils import error, warning, ifverbose
 from cs.pfx import Pfx, pfx, pfx_method, pfx_call
-from cs.resources import MultiOpenMixin
+from cs.resources import MultiOpenMixin, RunState, uses_runstate
 from cs.tagset import (
     Tag,
     TagSet,
     TagBasedTest,
     TagsOntology,
     TagFile,
     TagsOntologyCommand,
     TagsCommandMixin,
     RegexpTagRule,
     tag_or_tag_value,
 )
 from cs.threads import locked, locked_property, State
 from cs.upd import Upd, UpdProxy, uses_upd, print  # pylint: disable=redefined-builtin
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -235,21 +235,21 @@
             options,
             fstags=fstags,
             physical=fstags.config.physical,
         ):
           yield
 
   @uses_upd
-  def cmd_autotag(self, argv, *, upd: Upd):
+  @uses_runstate
+  def cmd_autotag(self, argv, *, upd: Upd, runstate: RunState):
     ''' Usage: {cmd} paths...
           Tag paths based on rules from the rc file.
     '''
     options = self.options
     fstags = options.fstags
-    runstate = options.runstate
     if not argv:
       argv = ['.']
     filename_rules = fstags.config.filename_rules
     with state(verbose=True):
       with UpdProxy() as proxy:
         for top_path in argv:
           for isdir, path in rpaths(top_path, yield_dirs=True):
@@ -332,29 +332,29 @@
           # edit the Tags, one per line
           fstags[path].edit(verbose=state.verbose, comments=["", path, ""])
         # edit the tagsets, on per file on a line
         elif not fstags.edit_dirpath(path, all_names=all_names):
           xit = 1
     return xit
 
-  def cmd_export(self, argv):
+  @uses_runstate
+  def cmd_export(self, argv, *, runstate: RunState):
     ''' Usage: {cmd} [-a] [--direct] path {{tag[=value]|-tag}}...
           Export tags for files from paths matching all the constraints.
           -a        Export all paths, not just those with tags.
           --direct  Export the direct tags instead of the computed tags.
           The output is in the same CSV format as that from "sqltags export",
           with the following columns:
           * unixtime: the file's st_mtime from os.stat.
           * id: empty
           * name: the file path
           * tags: the file's direct or indirect tags
     '''
     options = self.options
     fstags = options.fstags
-    runstate = options.runstate
     badopts = False
     all_paths = False
     use_direct_tags = False
     opts, argv = getopt(argv, 'a', longopts=['direct'])
     for opt, _ in opts:
       with Pfx(opt):
         if opt == '-a':
@@ -374,42 +374,41 @@
       badopts = True
     if badopts:
       raise GetoptError("bad arguments")
     xit = 0
     csvw = csv.writer(sys.stdout)
     for fspath in fstags.find(realpath(path), tag_choices,
                               use_direct_tags=use_direct_tags):
-      if runstate.cancelled:
-        return 1
+      runstate.raiseif()
       tagged_path = fstags[fspath]
       # pylint: disable=superfluous-parens
       if (not all_paths
           and not (tagged_path if use_direct_tags else tagged_path.all_tags)):
         continue
       # TODO: this always writes the direct tags only
       csvw.writerow(tagged_path.csvrow)
     return xit
 
   # pylint: disable=too-many-branches
-  def cmd_find(self, argv):
+  @uses_runstate
+  def cmd_find(self, argv, *, runstate: RunState):
     ''' Usage: {cmd} [--direct] [--for-rsync] [-o output_format] path {{tag[=value]|-tag}}...
           List files from path matching all the constraints.
           --direct    Use direct tags instead of all tags.
           --for-rsync Instead of listing matching paths, emit a
                       sequence of rsync(1) patterns suitable for use with
                       --include-from in order to do a selective rsync of the
                       matched paths.
           -o output_format
                       Use output_format as a Python format string to lay out
                       the listing.
                       Default: {FIND_OUTPUT_FORMAT_DEFAULT}
     '''
     options = self.options
     fstags = options.fstags
-    runstate = options.runstate
     badopts = False
     use_direct_tags = False
     as_rsync_includes = False
     output_format = FIND_OUTPUT_FORMAT_DEFAULT
     opts, argv = getopt(argv, 'o:', longopts=['direct', 'for-rsync'])
     for opt, value in opts:
       with Pfx(opt):
@@ -441,16 +440,15 @@
         realpath(path), tag_choices, use_direct_tags=use_direct_tags
     )
     if as_rsync_includes:
       for include in rsync_patterns(filepaths, path):
         print(include)
     else:
       for fspath in filepaths:
-        if runstate.cancelled:
-          return 1
+        runstate.raiseif()
         with Pfx(fspath):
           try:
             output = fstags[fspath].format_as(
                 output_format, error_sep='\n  ', direct=use_direct_tags
             )
           except FormatAsError as e:
             error(str(e))
@@ -581,28 +579,28 @@
           for key, value in data.items():
             tag_name = '.'.join((tag_prefix, key)) if tag_prefix else key
             tagged_path.add(
                 Tag(tag_name, value, ontology=ont), verbose=verbose
             )
     return 0
 
-  def cmd_ls(self, argv):
+  @uses_runstate
+  def cmd_ls(self, argv, *, runstate: RunState):
     ''' Usage: {cmd} [-d] [--direct] [-o output_format] [paths...]
           List files from paths and their tags.
           -d          Treat directories like files, do not recurse.
           --direct    List direct tags instead of all tags.
           -l          Long format.
           -o output_format
                       Use output_format as a Python format string to lay out
                       the listing.
                       Default: {LS_OUTPUT_FORMAT_DEFAULT}
     '''
     options = self.options
     fstags = options.fstags
-    runstate = options.runstate
     directories_like_files = False
     use_direct_tags = False
     long_format = False
     output_format = LS_OUTPUT_FORMAT_DEFAULT
     opts, argv = getopt(argv, 'dlo:', longopts=['direct'])
     for opt, value in opts:
       with Pfx(opt):
@@ -618,16 +616,15 @@
           raise RuntimeError("unsupported option")
     xit = 0
     paths = argv or ['.']
     for path in paths:
       fullpath = realpath(path)
       for fspath in ((fullpath,)
                      if directories_like_files else rfilepaths(fullpath)):
-        if runstate.cancelled:
-          return 1
+        runstate.raiseif()
         with Pfx(fspath):
           tags = fstags[fspath]
           if long_format:
             print(fspath)
             for tag in tags.as_tags(all_tags=not use_direct_tags):
               print(" ", tag)
           else:
```


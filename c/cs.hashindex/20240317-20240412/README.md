# Comparing `tmp/cs.hashindex-20240317.tar.gz` & `tmp/cs.hashindex-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.hashindex-20240317.tar", last modified: Sun Mar 17 01:40:36 2024, max compression
+gzip compressed data, was "cs.hashindex-20240412.tar", last modified: Fri Apr 12 05:46:36 2024, max compression
```

## Comparing `cs.hashindex-20240317.tar` & `cs.hashindex-20240412.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 01:40:36.038702 cs.hashindex-20240317/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-17 01:40:27.000000 cs.hashindex-20240317/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    13493 2024-03-17 01:40:36.038309 cs.hashindex-20240317/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    14828 2024-03-17 01:40:29.000000 cs.hashindex-20240317/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 01:40:36.033497 cs.hashindex-20240317/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 01:40:36.033800 cs.hashindex-20240317/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 01:40:36.035211 cs.hashindex-20240317/lib/python/cs/
--rwxr-xr-x   0 cameron    (501) cameron    (502)    32963 2024-03-17 01:38:53.000000 cs.hashindex-20240317/lib/python/cs/hashindex.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 01:40:36.037827 cs.hashindex-20240317/lib/python/cs.hashindex.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    13493 2024-03-17 01:40:35.000000 cs.hashindex-20240317/lib/python/cs.hashindex.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      347 2024-03-17 01:40:35.000000 cs.hashindex-20240317/lib/python/cs.hashindex.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-17 01:40:35.000000 cs.hashindex-20240317/lib/python/cs.hashindex.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       48 2024-03-17 01:40:35.000000 cs.hashindex-20240317/lib/python/cs.hashindex.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      257 2024-03-17 01:40:35.000000 cs.hashindex-20240317/lib/python/cs.hashindex.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-17 01:40:35.000000 cs.hashindex-20240317/lib/python/cs.hashindex.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    14219 2024-03-17 01:40:34.000000 cs.hashindex-20240317/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-17 01:40:36.038807 cs.hashindex-20240317/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:46:36.213867 cs.hashindex-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:46:28.000000 cs.hashindex-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    16367 2024-04-12 05:46:36.213478 cs.hashindex-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15522 2024-04-12 05:46:30.000000 cs.hashindex-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:46:36.208346 cs.hashindex-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:46:36.208666 cs.hashindex-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:46:36.210220 cs.hashindex-20240412/lib/python/cs/
+-rwxr-xr-x   0 cameron    (501) cameron    (502)    33128 2024-04-12 05:46:15.000000 cs.hashindex-20240412/lib/python/cs/hashindex.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:46:36.212911 cs.hashindex-20240412/lib/python/cs.hashindex.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    16367 2024-04-12 05:46:35.000000 cs.hashindex-20240412/lib/python/cs.hashindex.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      347 2024-04-12 05:46:36.000000 cs.hashindex-20240412/lib/python/cs.hashindex.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:46:35.000000 cs.hashindex-20240412/lib/python/cs.hashindex.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       48 2024-04-12 05:46:35.000000 cs.hashindex-20240412/lib/python/cs.hashindex.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      257 2024-04-12 05:46:36.000000 cs.hashindex-20240412/lib/python/cs.hashindex.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:46:36.000000 cs.hashindex-20240412/lib/python/cs.hashindex.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17096 2024-04-12 05:46:34.000000 cs.hashindex-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:46:36.213973 cs.hashindex-20240412/setup.cfg
```

### Comparing `cs.hashindex-20240317/PKG-INFO` & `cs.hashindex-20240412/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,14 @@
-Metadata-Version: 2.1
-Name: cs.hashindex
-Version: 20240317
-Summary: A command and utility functions for making listings of file content hashcodes and manipulating directory trees based on such a hash index.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 A command and utility functions for making listings of file content hashcodes
 and manipulating directory trees based on such a hash index.
 
-*Latest release 20240317*:
-* HashIndexCommand.cmd_ls: default to listing the current directory.
-* HashIndexCommand: new -o output_format to allow outputting only hashcodes or fspaths.
-* HashIndexCommand.cmd_comm: new -r (relative) option.
+*Latest release 20240412*:
+* file_checksum: skip any nonregular file, only use run_task when checksumming more than 1MiB.
+* HashIndexCommand.cmd_rearrange: run the refdir index in relative mode.
+* Small fixes.
 
 This largely exists to solve my "what has changed remotely?" or
 "what has been filed where?" problems by comparing file trees
 using the files' content hashcodes.
 
 This does require reading every file once to compute its hashcode,
 but the hashcodes (and file sizes and mtimes when read) are
@@ -67,34 +49,35 @@
 from the source to the new tree.
 
 If network bandwith is limited or quotaed, you can use the
 comparison function to prepare a list of files missing from the
 remote location and copy them to a transfer drive for carrying
 to the remote site when opportune. Example:
 
-    hashindex comm -1 -o '{fspath}' src rhost:dst         | rsync -a --files-from=- src/ xferdir/
+    hashindex comm -1 -o '{fspath}' src rhost:dst \
+    | rsync -a --files-from=- src/ xferdir/
 
 I've got a script [`pref-xfer`](https://hg.sr.ht/~cameron-simpson/css/browse/bin-cs/prep-xfer)
 which does this with some conveniences and sanity checks.
 
-## Function `dir_filepaths(dirpath: str, *, fstags: cs.fstags.FSTags)`
+## Function `dir_filepaths(dirpath: str, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Generator yielding the filesystem paths of the files in `dirpath`.
 
 ## Function `dir_remap(srcdirpath: str, fspaths_by_hashcode: Mapping[cs.hashutils.BaseHashCode, List[str]], *, hashname: str)`
 
 Generator yielding `(srcpath,[remapped_paths])` 2-tuples
 based on the hashcodes keying `rfspaths_by_hashcode`.
 
-## Function `file_checksum(fspath: str, hashname: str = 'sha256', *, fstags: cs.fstags.FSTags) -> Optional[cs.hashutils.BaseHashCode]`
+## Function `file_checksum(fspath: str, hashname: str = 'sha256', *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>) -> Optional[cs.hashutils.BaseHashCode]`
 
 Return the hashcode for the contents of the file at `fspath`.
 Warn and return `None` on `OSError`.
 
-## Function `get_fstags_hashcode(fspath: str, hashname: str, fstags: cs.fstags.FSTags) -> Tuple[Optional[cs.hashutils.BaseHashCode], Optional[os.stat_result]]`
+## Function `get_fstags_hashcode(fspath: str, hashname: str, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>) -> Tuple[Optional[cs.hashutils.BaseHashCode], Optional[os.stat_result]]`
 
 Obtain the hashcode cached in the fstags if still valid.
 Return a 2-tuple of `(hashcode,stat_result)`
 where `hashcode` is a `BaseHashCode` subclass instance is valid
 or `None` if missing or no longer valid
 and `stat_result` is the current `os.stat` result for `fspath`.
 
@@ -161,28 +144,78 @@
                         which may be local or remote.
             dstdir      Optional destination directory for the rearranged files.
                         Default is the targetdir.
                         It is taken to be on the same host as targetdir.
         shell
           Run a command prompt via cmd.Cmd using this command's subcommands.
 
+*`HashIndexCommand.Options`*
+
+*Method `HashIndexCommand.cmd_comm(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`*:
+Usage: {cmd} {{-1|-2|-3}} {{path1|-}} {{path2|-}}
+Compare the filepaths in path1 and path2 by content.
+-1            List hashes and paths only present in path1.
+-2            List hashes and paths only present in path2.
+-3            List hashes and paths present in path1 and path2.
+-e ssh_exe    Specify the ssh executable.
+-h hashname   Specify the file content hash algorithm name.
+-H hashindex_exe
+              Specify the remote hashindex executable.
+-o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+-r            Emit relative paths in the listing.
+
+*Method `HashIndexCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`*:
+Usage: {cmd} [options...] [[host:]path...]
+Walk filesystem paths and emit a listing.
+The default path is the current directory.
+Options:
+-e ssh_exe    Specify the ssh executable.
+-h hashname   Specify the file content hash algorithm name.
+-H hashindex_exe
+              Specify the remote hashindex executable.
+-o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+-r            Emit relative paths in the listing.
+              This requires each path to be a directory.
+
+*Method `HashIndexCommand.cmd_rearrange(self, argv)`*:
+Usage: {cmd} [options...] {{[[user@]host:]refdir|-}} [[user@]rhost:]targetdir [dstdir]
+Rearrange files from targetdir into dstdir based on their positions in refdir.
+Options:
+  -e ssh_exe  Specify the ssh executable.
+  -h hashname Specify the file content hash algorithm name.
+  -H hashindex_exe
+              Specify the remote hashindex executable.
+  --mv        Move mode.
+  -n          No action, dry run.
+  -o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+  -s          Symlink mode.
+Other arguments:
+  refdir      The reference directory, which may be local or remote
+              or "-" indicating that a hash index will be read from
+              standard input.
+  targetdir   The directory containing the files to be rearranged,
+              which may be local or remote.
+  dstdir      Optional destination directory for the rearranged files.
+              Default is the targetdir.
+              It is taken to be on the same host as targetdir.
+
 ## Function `localpath(fspath: str) -> str`
 
 Return a filesystem path modified so that it connot be
 misinterpreted as a remote path such as `user@host:path`.
 
 If `fspath` contains no colon (`:`) or is an absolute path
 or starts with `./` then it is returned unchanged.
 Otherwise a leading `./` is prepended.
 
 ## Function `main(argv=None)`
 
 Commandline implementation.
 
-## Function `merge(srcpath: str, dstpath: str, *, opname=None, hashname: str, move_mode: bool = False, symlink_mode=False, doit=False, quiet=False, fstags: cs.fstags.FSTags)`
+## Function `merge(srcpath: str, dstpath: str, *, opname=None, hashname: str, move_mode: bool = False, symlink_mode=False, doit=False, quiet=False, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Merge `srcpath` to `dstpath`.
 
 If `dstpath` does not exist, move/link/symlink `srcpath` to `dstpath`.
 Otherwise checksum their contents and raise `FileExistsError` if they differ.
 
 ## Function `paths_remap(srcpaths: Iterable[str], fspaths_by_hashcode: Mapping[cs.hashutils.BaseHashCode, List[str]], *, hashname: str)`
@@ -210,15 +243,15 @@
 * `hashindex_exe`: the remote `hashindex` executable,
   default `HASHINDEX_EXE_DEFAULT`: `'hashindex'`
 * `relative`: optional flag, default `False`;
   if true pass `'-r'` to the remote `hashindex ls` command
 * `check`: whether to check that the remote command has a `0` return code,
   default `True`
 
-## Function `rearrange(srcdirpath: str, rfspaths_by_hashcode, dstdirpath=None, *, hashname: str, move_mode: bool = False, symlink_mode=False, doit: bool, quiet: bool = False, fstags: cs.fstags.FSTags, runstate: cs.resources.RunState)`
+## Function `rearrange(srcdirpath: str, rfspaths_by_hashcode, dstdirpath=None, *, hashname: str, move_mode: bool = False, symlink_mode=False, doit: bool, quiet: bool = False, fstags: cs.fstags.FSTags, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`
 
 Rearrange the files in `dirpath` according to the
 hashcode->[relpaths] `fspaths_by_hashcode`.
 
 Parameters:
 * `srcdirpath`: the directory whose files are to be rearranged
 * `rfspaths_by_hashcode`: a mapping of hashcode to relative
@@ -227,15 +260,15 @@
   defaults to `srcdirpath`, rearranging the files in place
 * `hashname`: the file content hash algorithm name
 * `move_move`: move files instead of linking them
 * `symlink_mode`: symlink files instead of linking them
 * `doit`: if true do the link/move/symlink, otherwise just print
 * `quiet`: default `False`; if true do not print
 
-## Function `run_remote_hashindex(rhost: str, argv, *, ssh_exe=None, hashindex_exe=None, check: bool = True, doit: bool = None, quiet: Optional[bool] = None, options: cs.cmdutils.BaseCommandOptions, **subp_options)`
+## Function `run_remote_hashindex(rhost: str, argv, *, ssh_exe=None, hashindex_exe=None, check: bool = True, doit: bool = None, quiet: Optional[bool] = None, options: Optional[cs.cmdutils.BaseCommandOptions] = <function uses_cmd_options.<locals>.<lambda> at 0x101c29bd0>, **subp_options)`
 
 Run a remote `hashindex` command.
 Return the `CompletedProcess` result or `None` if `doit` is false.
 Note that as with `cs.psutils.run`, the arguments are resolved
 via `cs.psutils.prep_argv`.
 
 Parameters:
@@ -247,22 +280,27 @@
 * `hashindex_exe`: the remote `hashindex` executable,
   default `HASHINDEX_EXE_DEFAULT`: `'hashindex'`
 * `check`: whether to check that the remote command has a `0` return code,
   default `True`
 * `doit`: whether to actually run the command, default `True`
 Other keyword parameters are passed therough to `cs.psutils.run`.
 
-## Function `set_fstags_hashcode(fspath: str, hashcode, S: os.stat_result, fstags: cs.fstags.FSTags)`
+## Function `set_fstags_hashcode(fspath: str, hashcode, S: os.stat_result, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Record `hashcode` against `fspath`.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* file_checksum: skip any nonregular file, only use run_task when checksumming more than 1MiB.
+* HashIndexCommand.cmd_rearrange: run the refdir index in relative mode.
+* Small fixes.
+
 *Release 20240317*:
 * HashIndexCommand.cmd_ls: default to listing the current directory.
 * HashIndexCommand: new -o output_format to allow outputting only hashcodes or fspaths.
 * HashIndexCommand.cmd_comm: new -r (relative) option.
 
 *Release 20240316*:
 Fixed release upload artifacts.
@@ -281,8 +319,7 @@
 * dir_filepaths: skip dot files, the fstags .fstags file and nonregular files.
 
 *Release 20240211.1*:
 Better module docstring.
 
 *Release 20240211*:
 Initial PyPI release: "hashindex" command and utility functions for listing file hashcodes and rearranging trees based on a hash index.
-
```

### Comparing `cs.hashindex-20240317/README.md` & `cs.hashindex-20240412/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,32 @@
+Metadata-Version: 2.1
+Name: cs.hashindex
+Version: 20240412
+Summary: A command and utility functions for making listings of file content hashcodes and manipulating directory trees based on such a hash index.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 A command and utility functions for making listings of file content hashcodes
 and manipulating directory trees based on such a hash index.
 
-*Latest release 20240317*:
-* HashIndexCommand.cmd_ls: default to listing the current directory.
-* HashIndexCommand: new -o output_format to allow outputting only hashcodes or fspaths.
-* HashIndexCommand.cmd_comm: new -r (relative) option.
+*Latest release 20240412*:
+* file_checksum: skip any nonregular file, only use run_task when checksumming more than 1MiB.
+* HashIndexCommand.cmd_rearrange: run the refdir index in relative mode.
+* Small fixes.
 
 This largely exists to solve my "what has changed remotely?" or
 "what has been filed where?" problems by comparing file trees
 using the files' content hashcodes.
 
 This does require reading every file once to compute its hashcode,
 but the hashcodes (and file sizes and mtimes when read) are
@@ -49,34 +67,35 @@
 from the source to the new tree.
 
 If network bandwith is limited or quotaed, you can use the
 comparison function to prepare a list of files missing from the
 remote location and copy them to a transfer drive for carrying
 to the remote site when opportune. Example:
 
-    hashindex comm -1 -o '{fspath}' src rhost:dst         | rsync -a --files-from=- src/ xferdir/
+    hashindex comm -1 -o '{fspath}' src rhost:dst \
+    | rsync -a --files-from=- src/ xferdir/
 
 I've got a script [`pref-xfer`](https://hg.sr.ht/~cameron-simpson/css/browse/bin-cs/prep-xfer)
 which does this with some conveniences and sanity checks.
 
-## Function `dir_filepaths(dirpath: str, *, fstags: cs.fstags.FSTags)`
+## Function `dir_filepaths(dirpath: str, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Generator yielding the filesystem paths of the files in `dirpath`.
 
 ## Function `dir_remap(srcdirpath: str, fspaths_by_hashcode: Mapping[cs.hashutils.BaseHashCode, List[str]], *, hashname: str)`
 
 Generator yielding `(srcpath,[remapped_paths])` 2-tuples
 based on the hashcodes keying `rfspaths_by_hashcode`.
 
-## Function `file_checksum(fspath: str, hashname: str = 'sha256', *, fstags: cs.fstags.FSTags) -> Optional[cs.hashutils.BaseHashCode]`
+## Function `file_checksum(fspath: str, hashname: str = 'sha256', *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>) -> Optional[cs.hashutils.BaseHashCode]`
 
 Return the hashcode for the contents of the file at `fspath`.
 Warn and return `None` on `OSError`.
 
-## Function `get_fstags_hashcode(fspath: str, hashname: str, fstags: cs.fstags.FSTags) -> Tuple[Optional[cs.hashutils.BaseHashCode], Optional[os.stat_result]]`
+## Function `get_fstags_hashcode(fspath: str, hashname: str, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>) -> Tuple[Optional[cs.hashutils.BaseHashCode], Optional[os.stat_result]]`
 
 Obtain the hashcode cached in the fstags if still valid.
 Return a 2-tuple of `(hashcode,stat_result)`
 where `hashcode` is a `BaseHashCode` subclass instance is valid
 or `None` if missing or no longer valid
 and `stat_result` is the current `os.stat` result for `fspath`.
 
@@ -145,28 +164,28 @@
                         Default is the targetdir.
                         It is taken to be on the same host as targetdir.
         shell
           Run a command prompt via cmd.Cmd using this command's subcommands.
 
 *`HashIndexCommand.Options`*
 
-*Method `HashIndexCommand.cmd_comm(self, argv)`*:
+*Method `HashIndexCommand.cmd_comm(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`*:
 Usage: {cmd} {{-1|-2|-3}} {{path1|-}} {{path2|-}}
 Compare the filepaths in path1 and path2 by content.
 -1            List hashes and paths only present in path1.
 -2            List hashes and paths only present in path2.
 -3            List hashes and paths present in path1 and path2.
 -e ssh_exe    Specify the ssh executable.
 -h hashname   Specify the file content hash algorithm name.
 -H hashindex_exe
               Specify the remote hashindex executable.
 -o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
 -r            Emit relative paths in the listing.
 
-*Method `HashIndexCommand.cmd_ls(self, argv)`*:
+*Method `HashIndexCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`*:
 Usage: {cmd} [options...] [[host:]path...]
 Walk filesystem paths and emit a listing.
 The default path is the current directory.
 Options:
 -e ssh_exe    Specify the ssh executable.
 -h hashname   Specify the file content hash algorithm name.
 -H hashindex_exe
@@ -206,15 +225,15 @@
 or starts with `./` then it is returned unchanged.
 Otherwise a leading `./` is prepended.
 
 ## Function `main(argv=None)`
 
 Commandline implementation.
 
-## Function `merge(srcpath: str, dstpath: str, *, opname=None, hashname: str, move_mode: bool = False, symlink_mode=False, doit=False, quiet=False, fstags: cs.fstags.FSTags)`
+## Function `merge(srcpath: str, dstpath: str, *, opname=None, hashname: str, move_mode: bool = False, symlink_mode=False, doit=False, quiet=False, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Merge `srcpath` to `dstpath`.
 
 If `dstpath` does not exist, move/link/symlink `srcpath` to `dstpath`.
 Otherwise checksum their contents and raise `FileExistsError` if they differ.
 
 ## Function `paths_remap(srcpaths: Iterable[str], fspaths_by_hashcode: Mapping[cs.hashutils.BaseHashCode, List[str]], *, hashname: str)`
@@ -242,15 +261,15 @@
 * `hashindex_exe`: the remote `hashindex` executable,
   default `HASHINDEX_EXE_DEFAULT`: `'hashindex'`
 * `relative`: optional flag, default `False`;
   if true pass `'-r'` to the remote `hashindex ls` command
 * `check`: whether to check that the remote command has a `0` return code,
   default `True`
 
-## Function `rearrange(srcdirpath: str, rfspaths_by_hashcode, dstdirpath=None, *, hashname: str, move_mode: bool = False, symlink_mode=False, doit: bool, quiet: bool = False, fstags: cs.fstags.FSTags, runstate: cs.resources.RunState)`
+## Function `rearrange(srcdirpath: str, rfspaths_by_hashcode, dstdirpath=None, *, hashname: str, move_mode: bool = False, symlink_mode=False, doit: bool, quiet: bool = False, fstags: cs.fstags.FSTags, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`
 
 Rearrange the files in `dirpath` according to the
 hashcode->[relpaths] `fspaths_by_hashcode`.
 
 Parameters:
 * `srcdirpath`: the directory whose files are to be rearranged
 * `rfspaths_by_hashcode`: a mapping of hashcode to relative
@@ -259,15 +278,15 @@
   defaults to `srcdirpath`, rearranging the files in place
 * `hashname`: the file content hash algorithm name
 * `move_move`: move files instead of linking them
 * `symlink_mode`: symlink files instead of linking them
 * `doit`: if true do the link/move/symlink, otherwise just print
 * `quiet`: default `False`; if true do not print
 
-## Function `run_remote_hashindex(rhost: str, argv, *, ssh_exe=None, hashindex_exe=None, check: bool = True, doit: bool = None, quiet: Optional[bool] = None, options: cs.cmdutils.BaseCommandOptions, **subp_options)`
+## Function `run_remote_hashindex(rhost: str, argv, *, ssh_exe=None, hashindex_exe=None, check: bool = True, doit: bool = None, quiet: Optional[bool] = None, options: Optional[cs.cmdutils.BaseCommandOptions] = <function uses_cmd_options.<locals>.<lambda> at 0x101c29bd0>, **subp_options)`
 
 Run a remote `hashindex` command.
 Return the `CompletedProcess` result or `None` if `doit` is false.
 Note that as with `cs.psutils.run`, the arguments are resolved
 via `cs.psutils.prep_argv`.
 
 Parameters:
@@ -279,22 +298,27 @@
 * `hashindex_exe`: the remote `hashindex` executable,
   default `HASHINDEX_EXE_DEFAULT`: `'hashindex'`
 * `check`: whether to check that the remote command has a `0` return code,
   default `True`
 * `doit`: whether to actually run the command, default `True`
 Other keyword parameters are passed therough to `cs.psutils.run`.
 
-## Function `set_fstags_hashcode(fspath: str, hashcode, S: os.stat_result, fstags: cs.fstags.FSTags)`
+## Function `set_fstags_hashcode(fspath: str, hashcode, S: os.stat_result, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Record `hashcode` against `fspath`.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* file_checksum: skip any nonregular file, only use run_task when checksumming more than 1MiB.
+* HashIndexCommand.cmd_rearrange: run the refdir index in relative mode.
+* Small fixes.
+
 *Release 20240317*:
 * HashIndexCommand.cmd_ls: default to listing the current directory.
 * HashIndexCommand: new -o output_format to allow outputting only hashcodes or fspaths.
 * HashIndexCommand.cmd_comm: new -r (relative) option.
 
 *Release 20240316*:
 Fixed release upload artifacts.
@@ -313,7 +337,8 @@
 * dir_filepaths: skip dot files, the fstags .fstags file and nonregular files.
 
 *Release 20240211.1*:
 Better module docstring.
 
 *Release 20240211*:
 Initial PyPI release: "hashindex" command and utility functions for listing file hashcodes and rearranging trees based on a hash index.
+
```

### Comparing `cs.hashindex-20240317/lib/python/cs/hashindex.py` & `cs.hashindex-20240412/lib/python/cs/hashindex.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     from the source to the new tree.
 
     If network bandwith is limited or quotaed, you can use the
     comparison function to prepare a list of files missing from the
     remote location and copy them to a transfer drive for carrying
     to the remote site when opportune. Example:
 
-        hashindex comm -1 -o '{fspath}' src rhost:dst \
+        hashindex comm -1 -o '{fspath}' src rhost:dst \\
         | rsync -a --files-from=- src/ xferdir/
 
     I've got a script [`pref-xfer`](https://hg.sr.ht/~cameron-simpson/css/browse/bin-cs/prep-xfer)
     which does this with some conveniences and sanity checks.
 '''
 
 from collections import defaultdict
@@ -96,15 +96,15 @@
 from cs.lex import r, split_remote_path
 from cs.logutils import warning
 from cs.pfx import Pfx, pfx, pfx_call
 from cs.psutils import prep_argv, pipefrom, run
 from cs.resources import RunState, uses_runstate
 from cs.upd import print, run_task, without  # pylint: disable=redefined-builtin
 
-__version__ = '20240317'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -171,15 +171,15 @@
     hashindex_exe: str = HASHINDEX_EXE_DEFAULT
     symlink_mode: bool = False
     relative: Optional[bool] = None
     output_format: str = OUTPUT_FORMAT_DEFAULT
 
     # pylint: disable=use-dict-literal
     COMMON_OPT_SPECS = dict(
-        e='ssh_exe',
+        e_='ssh_exe',
         h_='hashname',
         H_='hashindex_exe',
         o_='output_format',
         **BaseCommand.Options.COMMON_OPT_SPECS,
     )
 
   # pylint: disable=arguments-differ
@@ -187,15 +187,16 @@
   @uses_fstags
   def run_context(self, *, fstags: FSTags, **kw):
     with fstags:
       with super().run_context(**kw):
         yield
 
   #pylint: disable=too-many-locals
-  def cmd_comm(self, argv):
+  @uses_runstate
+  def cmd_comm(self, argv, *, runstate: RunState):
     ''' Usage: {cmd} {{-1|-2|-3}} {{path1|-}} {{path2|-}}
           Compare the filepaths in path1 and path2 by content.
           -1            List hashes and paths only present in path1.
           -2            List hashes and paths only present in path2.
           -3            List hashes and paths present in path1 and path2.
           -e ssh_exe    Specify the ssh executable.
           -h hashname   Specify the file content hash algorithm name.
@@ -217,15 +218,14 @@
         _3='path12',
         r='relative',
     )
     hashindex_exe = options.hashindex_exe
     hashname = options.hashname
     output_format = options.output_format
     relative = options.relative
-    runstate = options.runstate
     ssh_exe = options.ssh_exe
     path1_only = options.path1_only
     path2_only = options.path2_only
     path12 = options.path12
     mode_count = len(list(filter(None, (path1_only, path2_only, path12))))
     if not mode_count:
       warning("one of -1, -2 or -3 must be provided")
@@ -313,15 +313,16 @@
       assert path12
       for hashcode in fspaths2_by_hashcode.keys() & fspaths1_by_hashcode.keys(
       ):
         runstate.raiseif()
         for fspath in fspaths1_by_hashcode[hashcode]:
           print(output_format.format(hashcode=hashcode, fspath=fspath))
 
-  def cmd_ls(self, argv):
+  @uses_runstate
+  def cmd_ls(self, argv, *, runstate: RunState):
     ''' Usage: {cmd} [options...] [[host:]path...]
           Walk filesystem paths and emit a listing.
           The default path is the current directory.
           Options:
           -e ssh_exe    Specify the ssh executable.
           -h hashname   Specify the file content hash algorithm name.
           -H hashindex_exe
@@ -336,15 +337,14 @@
         argv,
         r='relative',
     )
     hashindex_exe = options.hashindex_exe
     hashname = options.hashname
     output_format = options.output_format
     relative = options.relative
-    runstate = options.runstate
     ssh_exe = options.ssh_exe
     if not argv:
       argv = ['.']
     xit = 0
     for path in argv:
       runstate.raiseif()
       with Pfx(path):
@@ -402,14 +402,15 @@
     move_mode = options.move_mode
     quiet = options.quiet
     ssh_exe = options.ssh_exe
     symlink_mode = options.symlink_mode
     if not argv:
       warning("missing refdir")
       badopts = True
+      refdir = None
     else:
       refspec = argv.pop(0)
       with Pfx("refdir %r", refspec):
         refhost, refdir = split_remote_path(refspec)
         if refhost is None:
           if refdir != '-':
             if not isdirpath(refdir):
@@ -417,14 +418,15 @@
               badopts = True
         elif refdir == '-':
           warning("remote \"-\" not supported")
           badopts = True
     if not argv:
       warning("missing targetdir")
       badopts = True
+      targetdir = None
     else:
       targetspec = argv.pop(0)
       with Pfx("targetdir %r", targetspec):
         targethost, targetdir = split_remote_path(targetspec)
         if targethost is None:
           if not isdirpath(targetdir):
             warning("not a directory")
@@ -447,14 +449,15 @@
     xit = 0
     with run_task(f'hashindex {refspec}'):
       for hashcode, fspath in hashindex(
           (refhost, refdir),
           hashname=hashname,
           ssh_exe=ssh_exe,
           hashindex_exe=hashindex_exe,
+          relative=True,
       ):
         if hashcode is not None:
           fspaths_by_hashcode[hashcode].append(fspath)
     # rearrange the target directory.
     with (nullcontext()
           if refhost or targethost else run_task(f'rearrange {targetspec}')):
       if targethost is None:
@@ -498,32 +501,36 @@
             input=input_s,
             text=True,
             doit=True,  # we pass -n to the remote hashindex
             quiet=False,
         ).returncode
     return xit
 
-@uses_fstags
 @pfx
+@uses_fstags
 def file_checksum(
     fspath: str,
     hashname: str = HASHNAME_DEFAULT,
     *,
     fstags: FSTags,
 ) -> Union[BaseHashCode, None]:
   ''' Return the hashcode for the contents of the file at `fspath`.
       Warn and return `None` on `OSError`.
   '''
   hashcode, S = get_fstags_hashcode(fspath, hashname)
-  if S_ISLNK(S.st_mode):
-    # ignore symlinks
+  if not S_ISREG(S.st_mode):
+    # ignore nonregular files
     return None
   if hashcode is None:
     hashclass = BaseHashCode.hashclass(hashname)
-    with run_task(f'checksum {shortpath(fspath)}'):
+    with contextif(
+        S.st_size > 1024 * 1024,
+        run_task,
+        f'checksum {shortpath(fspath)}',
+    ):
       try:
         hashcode = hashclass.from_fspath(fspath)
       except OSError as e:
         warning("%s.from_fspath(%r): %s", hashclass.__name__, fspath, e)
         return None
     set_fstags_hashcode(fspath, hashcode, S, fstags=fstags)
   return hashcode
```

### Comparing `cs.hashindex-20240317/lib/python/cs.hashindex.egg-info/PKG-INFO` & `cs.hashindex-20240412/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,64 @@
-Metadata-Version: 2.1
-Name: cs.hashindex
-Version: 20240317
-Summary: A command and utility functions for making listings of file content hashcodes and manipulating directory trees based on such a hash index.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
+[project]
+name = "cs.hashindex"
+description = "A command and utility functions for making listings of file content hashcodes and manipulating directory trees based on such a hash index."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python3",
+]
+dependencies = [
+    "cs.cmdutils>=20240211",
+    "cs.context>=20240412",
+    "cs.deco>=20240412",
+    "cs.fs>=20240412",
+    "cs.fstags>=20240412",
+    "cs.hashutils>=20240412",
+    "cs.lex>=20240316",
+    "cs.logutils>=20230212",
+    "cs.pfx>=20240412",
+    "cs.psutils>=20240316",
+    "cs.resources>=20240412",
+    "cs.upd>=20240412",
+    "icontract",
+    "typeguard",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20240412"
+
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
 
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.scripts]
+hashindex = "cs.hashindex:main"
+
+[project.readme]
+text = """
 A command and utility functions for making listings of file content hashcodes
 and manipulating directory trees based on such a hash index.
 
-*Latest release 20240317*:
-* HashIndexCommand.cmd_ls: default to listing the current directory.
-* HashIndexCommand: new -o output_format to allow outputting only hashcodes or fspaths.
-* HashIndexCommand.cmd_comm: new -r (relative) option.
+*Latest release 20240412*:
+* file_checksum: skip any nonregular file, only use run_task when checksumming more than 1MiB.
+* HashIndexCommand.cmd_rearrange: run the refdir index in relative mode.
+* Small fixes.
 
-This largely exists to solve my "what has changed remotely?" or
-"what has been filed where?" problems by comparing file trees
+This largely exists to solve my \"what has changed remotely?\" or
+\"what has been filed where?\" problems by comparing file trees
 using the files' content hashcodes.
 
 This does require reading every file once to compute its hashcode,
 but the hashcodes (and file sizes and mtimes when read) are
 stored beside the file in `.fstags` files (see the `cs.fstags`
 module), so that a file does not need to be reread on subsequent
 comparisons.
@@ -51,15 +80,15 @@
 the destination can be equivalently rearranged without copying
 the files, for example:
 
     hashindex rearrange sourcehost:sourcetree localtree
 
 If `fstags mv` was used to do the original rearrangement then
 the hashcodes will be copied to the new locations, saving a
-rescan of the source file. I keep a shell alias `mv="fstags mv"`
+rescan of the source file. I keep a shell alias `mv=\"fstags mv\"`
 so this is routine for me.
 
 I have a backup script [`histbackup`](https://hg.sr.ht/~cameron-simpson/css/browse/bin/histbackup)
 which works by making a hard link tree of the previous backup
 and `rsync`ing into it.  It has long been subject to huge
 transfers if the source tree gets rearranged. Now it has a
 `--hashindex` option to get it to run a `hashindex rearrange`
@@ -67,34 +96,35 @@
 from the source to the new tree.
 
 If network bandwith is limited or quotaed, you can use the
 comparison function to prepare a list of files missing from the
 remote location and copy them to a transfer drive for carrying
 to the remote site when opportune. Example:
 
-    hashindex comm -1 -o '{fspath}' src rhost:dst         | rsync -a --files-from=- src/ xferdir/
+    hashindex comm -1 -o '{fspath}' src rhost:dst \\
+    | rsync -a --files-from=- src/ xferdir/
 
 I've got a script [`pref-xfer`](https://hg.sr.ht/~cameron-simpson/css/browse/bin-cs/prep-xfer)
 which does this with some conveniences and sanity checks.
 
-## Function `dir_filepaths(dirpath: str, *, fstags: cs.fstags.FSTags)`
+## Function `dir_filepaths(dirpath: str, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Generator yielding the filesystem paths of the files in `dirpath`.
 
 ## Function `dir_remap(srcdirpath: str, fspaths_by_hashcode: Mapping[cs.hashutils.BaseHashCode, List[str]], *, hashname: str)`
 
 Generator yielding `(srcpath,[remapped_paths])` 2-tuples
 based on the hashcodes keying `rfspaths_by_hashcode`.
 
-## Function `file_checksum(fspath: str, hashname: str = 'sha256', *, fstags: cs.fstags.FSTags) -> Optional[cs.hashutils.BaseHashCode]`
+## Function `file_checksum(fspath: str, hashname: str = 'sha256', *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>) -> Optional[cs.hashutils.BaseHashCode]`
 
 Return the hashcode for the contents of the file at `fspath`.
 Warn and return `None` on `OSError`.
 
-## Function `get_fstags_hashcode(fspath: str, hashname: str, fstags: cs.fstags.FSTags) -> Tuple[Optional[cs.hashutils.BaseHashCode], Optional[os.stat_result]]`
+## Function `get_fstags_hashcode(fspath: str, hashname: str, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>) -> Tuple[Optional[cs.hashutils.BaseHashCode], Optional[os.stat_result]]`
 
 Obtain the hashcode cached in the fstags if still valid.
 Return a 2-tuple of `(hashcode,stat_result)`
 where `hashcode` is a `BaseHashCode` subclass instance is valid
 or `None` if missing or no longer valid
 and `stat_result` is the current `os.stat` result for `fspath`.
 
@@ -151,38 +181,88 @@
                         Specify the remote hashindex executable.
             --mv        Move mode.
             -n          No action, dry run.
             -o output_format Default: '{hashcode} {fspath}'.
             -s          Symlink mode.
           Other arguments:
             refdir      The reference directory, which may be local or remote
-                        or "-" indicating that a hash index will be read from
+                        or \"-\" indicating that a hash index will be read from
                         standard input.
             targetdir   The directory containing the files to be rearranged,
                         which may be local or remote.
             dstdir      Optional destination directory for the rearranged files.
                         Default is the targetdir.
                         It is taken to be on the same host as targetdir.
         shell
           Run a command prompt via cmd.Cmd using this command's subcommands.
 
+*`HashIndexCommand.Options`*
+
+*Method `HashIndexCommand.cmd_comm(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`*:
+Usage: {cmd} {{-1|-2|-3}} {{path1|-}} {{path2|-}}
+Compare the filepaths in path1 and path2 by content.
+-1            List hashes and paths only present in path1.
+-2            List hashes and paths only present in path2.
+-3            List hashes and paths present in path1 and path2.
+-e ssh_exe    Specify the ssh executable.
+-h hashname   Specify the file content hash algorithm name.
+-H hashindex_exe
+              Specify the remote hashindex executable.
+-o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+-r            Emit relative paths in the listing.
+
+*Method `HashIndexCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`*:
+Usage: {cmd} [options...] [[host:]path...]
+Walk filesystem paths and emit a listing.
+The default path is the current directory.
+Options:
+-e ssh_exe    Specify the ssh executable.
+-h hashname   Specify the file content hash algorithm name.
+-H hashindex_exe
+              Specify the remote hashindex executable.
+-o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+-r            Emit relative paths in the listing.
+              This requires each path to be a directory.
+
+*Method `HashIndexCommand.cmd_rearrange(self, argv)`*:
+Usage: {cmd} [options...] {{[[user@]host:]refdir|-}} [[user@]rhost:]targetdir [dstdir]
+Rearrange files from targetdir into dstdir based on their positions in refdir.
+Options:
+  -e ssh_exe  Specify the ssh executable.
+  -h hashname Specify the file content hash algorithm name.
+  -H hashindex_exe
+              Specify the remote hashindex executable.
+  --mv        Move mode.
+  -n          No action, dry run.
+  -o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+  -s          Symlink mode.
+Other arguments:
+  refdir      The reference directory, which may be local or remote
+              or \"-\" indicating that a hash index will be read from
+              standard input.
+  targetdir   The directory containing the files to be rearranged,
+              which may be local or remote.
+  dstdir      Optional destination directory for the rearranged files.
+              Default is the targetdir.
+              It is taken to be on the same host as targetdir.
+
 ## Function `localpath(fspath: str) -> str`
 
 Return a filesystem path modified so that it connot be
 misinterpreted as a remote path such as `user@host:path`.
 
 If `fspath` contains no colon (`:`) or is an absolute path
 or starts with `./` then it is returned unchanged.
 Otherwise a leading `./` is prepended.
 
 ## Function `main(argv=None)`
 
 Commandline implementation.
 
-## Function `merge(srcpath: str, dstpath: str, *, opname=None, hashname: str, move_mode: bool = False, symlink_mode=False, doit=False, quiet=False, fstags: cs.fstags.FSTags)`
+## Function `merge(srcpath: str, dstpath: str, *, opname=None, hashname: str, move_mode: bool = False, symlink_mode=False, doit=False, quiet=False, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Merge `srcpath` to `dstpath`.
 
 If `dstpath` does not exist, move/link/symlink `srcpath` to `dstpath`.
 Otherwise checksum their contents and raise `FileExistsError` if they differ.
 
 ## Function `paths_remap(srcpaths: Iterable[str], fspaths_by_hashcode: Mapping[cs.hashutils.BaseHashCode, List[str]], *, hashname: str)`
@@ -210,15 +290,15 @@
 * `hashindex_exe`: the remote `hashindex` executable,
   default `HASHINDEX_EXE_DEFAULT`: `'hashindex'`
 * `relative`: optional flag, default `False`;
   if true pass `'-r'` to the remote `hashindex ls` command
 * `check`: whether to check that the remote command has a `0` return code,
   default `True`
 
-## Function `rearrange(srcdirpath: str, rfspaths_by_hashcode, dstdirpath=None, *, hashname: str, move_mode: bool = False, symlink_mode=False, doit: bool, quiet: bool = False, fstags: cs.fstags.FSTags, runstate: cs.resources.RunState)`
+## Function `rearrange(srcdirpath: str, rfspaths_by_hashcode, dstdirpath=None, *, hashname: str, move_mode: bool = False, symlink_mode=False, doit: bool, quiet: bool = False, fstags: cs.fstags.FSTags, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`
 
 Rearrange the files in `dirpath` according to the
 hashcode->[relpaths] `fspaths_by_hashcode`.
 
 Parameters:
 * `srcdirpath`: the directory whose files are to be rearranged
 * `rfspaths_by_hashcode`: a mapping of hashcode to relative
@@ -227,15 +307,15 @@
   defaults to `srcdirpath`, rearranging the files in place
 * `hashname`: the file content hash algorithm name
 * `move_move`: move files instead of linking them
 * `symlink_mode`: symlink files instead of linking them
 * `doit`: if true do the link/move/symlink, otherwise just print
 * `quiet`: default `False`; if true do not print
 
-## Function `run_remote_hashindex(rhost: str, argv, *, ssh_exe=None, hashindex_exe=None, check: bool = True, doit: bool = None, quiet: Optional[bool] = None, options: cs.cmdutils.BaseCommandOptions, **subp_options)`
+## Function `run_remote_hashindex(rhost: str, argv, *, ssh_exe=None, hashindex_exe=None, check: bool = True, doit: bool = None, quiet: Optional[bool] = None, options: Optional[cs.cmdutils.BaseCommandOptions] = <function uses_cmd_options.<locals>.<lambda> at 0x101c29bd0>, **subp_options)`
 
 Run a remote `hashindex` command.
 Return the `CompletedProcess` result or `None` if `doit` is false.
 Note that as with `cs.psutils.run`, the arguments are resolved
 via `cs.psutils.prep_argv`.
 
 Parameters:
@@ -247,22 +327,27 @@
 * `hashindex_exe`: the remote `hashindex` executable,
   default `HASHINDEX_EXE_DEFAULT`: `'hashindex'`
 * `check`: whether to check that the remote command has a `0` return code,
   default `True`
 * `doit`: whether to actually run the command, default `True`
 Other keyword parameters are passed therough to `cs.psutils.run`.
 
-## Function `set_fstags_hashcode(fspath: str, hashcode, S: os.stat_result, fstags: cs.fstags.FSTags)`
+## Function `set_fstags_hashcode(fspath: str, hashcode, S: os.stat_result, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Record `hashcode` against `fspath`.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* file_checksum: skip any nonregular file, only use run_task when checksumming more than 1MiB.
+* HashIndexCommand.cmd_rearrange: run the refdir index in relative mode.
+* Small fixes.
+
 *Release 20240317*:
 * HashIndexCommand.cmd_ls: default to listing the current directory.
 * HashIndexCommand: new -o output_format to allow outputting only hashcodes or fspaths.
 * HashIndexCommand.cmd_comm: new -r (relative) option.
 
 *Release 20240316*:
 Fixed release upload artifacts.
@@ -280,9 +365,25 @@
 * New run_remote_hashindex() and read_remote_hashindex() functions.
 * dir_filepaths: skip dot files, the fstags .fstags file and nonregular files.
 
 *Release 20240211.1*:
 Better module docstring.
 
 *Release 20240211*:
-Initial PyPI release: "hashindex" command and utility functions for listing file hashcodes and rearranging trees based on a hash index.
+Initial PyPI release: \"hashindex\" command and utility functions for listing file hashcodes and rearranging trees based on a hash index."""
+content-type = "text/markdown"
+
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+
+[tool.setuptools]
+py-modules = [
+    "cs.hashindex",
+]
 
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

### Comparing `cs.hashindex-20240317/pyproject.toml` & `cs.hashindex-20240412/lib/python/cs.hashindex.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,35 @@
-[project]
-name = "cs.hashindex"
-description = "A command and utility functions for making listings of file content hashcodes and manipulating directory trees based on such a hash index."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python3",
-]
-dependencies = [
-    "cs.cmdutils>=20240211",
-    "cs.context>=20240316",
-    "cs.deco>=20240316",
-    "cs.fs>=20240316",
-    "cs.fstags>=20240316",
-    "cs.hashutils>=20240316",
-    "cs.lex>=20240316",
-    "cs.logutils>=20230212",
-    "cs.pfx>=20230604",
-    "cs.psutils>=20240316",
-    "cs.resources>=20240316",
-    "cs.upd>=20240316",
-    "icontract",
-    "typeguard",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20240317"
-
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
+Metadata-Version: 2.1
+Name: cs.hashindex
+Version: 20240412
+Summary: A command and utility functions for making listings of file content hashcodes and manipulating directory trees based on such a hash index.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.scripts]
-hashindex = "cs.hashindex:main"
-
-[project.readme]
-text = """
 A command and utility functions for making listings of file content hashcodes
 and manipulating directory trees based on such a hash index.
 
-*Latest release 20240317*:
-* HashIndexCommand.cmd_ls: default to listing the current directory.
-* HashIndexCommand: new -o output_format to allow outputting only hashcodes or fspaths.
-* HashIndexCommand.cmd_comm: new -r (relative) option.
+*Latest release 20240412*:
+* file_checksum: skip any nonregular file, only use run_task when checksumming more than 1MiB.
+* HashIndexCommand.cmd_rearrange: run the refdir index in relative mode.
+* Small fixes.
 
-This largely exists to solve my \"what has changed remotely?\" or
-\"what has been filed where?\" problems by comparing file trees
+This largely exists to solve my "what has changed remotely?" or
+"what has been filed where?" problems by comparing file trees
 using the files' content hashcodes.
 
 This does require reading every file once to compute its hashcode,
 but the hashcodes (and file sizes and mtimes when read) are
 stored beside the file in `.fstags` files (see the `cs.fstags`
 module), so that a file does not need to be reread on subsequent
 comparisons.
@@ -80,15 +51,15 @@
 the destination can be equivalently rearranged without copying
 the files, for example:
 
     hashindex rearrange sourcehost:sourcetree localtree
 
 If `fstags mv` was used to do the original rearrangement then
 the hashcodes will be copied to the new locations, saving a
-rescan of the source file. I keep a shell alias `mv=\"fstags mv\"`
+rescan of the source file. I keep a shell alias `mv="fstags mv"`
 so this is routine for me.
 
 I have a backup script [`histbackup`](https://hg.sr.ht/~cameron-simpson/css/browse/bin/histbackup)
 which works by making a hard link tree of the previous backup
 and `rsync`ing into it.  It has long been subject to huge
 transfers if the source tree gets rearranged. Now it has a
 `--hashindex` option to get it to run a `hashindex rearrange`
@@ -96,34 +67,35 @@
 from the source to the new tree.
 
 If network bandwith is limited or quotaed, you can use the
 comparison function to prepare a list of files missing from the
 remote location and copy them to a transfer drive for carrying
 to the remote site when opportune. Example:
 
-    hashindex comm -1 -o '{fspath}' src rhost:dst         | rsync -a --files-from=- src/ xferdir/
+    hashindex comm -1 -o '{fspath}' src rhost:dst \
+    | rsync -a --files-from=- src/ xferdir/
 
 I've got a script [`pref-xfer`](https://hg.sr.ht/~cameron-simpson/css/browse/bin-cs/prep-xfer)
 which does this with some conveniences and sanity checks.
 
-## Function `dir_filepaths(dirpath: str, *, fstags: cs.fstags.FSTags)`
+## Function `dir_filepaths(dirpath: str, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Generator yielding the filesystem paths of the files in `dirpath`.
 
 ## Function `dir_remap(srcdirpath: str, fspaths_by_hashcode: Mapping[cs.hashutils.BaseHashCode, List[str]], *, hashname: str)`
 
 Generator yielding `(srcpath,[remapped_paths])` 2-tuples
 based on the hashcodes keying `rfspaths_by_hashcode`.
 
-## Function `file_checksum(fspath: str, hashname: str = 'sha256', *, fstags: cs.fstags.FSTags) -> Optional[cs.hashutils.BaseHashCode]`
+## Function `file_checksum(fspath: str, hashname: str = 'sha256', *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>) -> Optional[cs.hashutils.BaseHashCode]`
 
 Return the hashcode for the contents of the file at `fspath`.
 Warn and return `None` on `OSError`.
 
-## Function `get_fstags_hashcode(fspath: str, hashname: str, fstags: cs.fstags.FSTags) -> Tuple[Optional[cs.hashutils.BaseHashCode], Optional[os.stat_result]]`
+## Function `get_fstags_hashcode(fspath: str, hashname: str, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>) -> Tuple[Optional[cs.hashutils.BaseHashCode], Optional[os.stat_result]]`
 
 Obtain the hashcode cached in the fstags if still valid.
 Return a 2-tuple of `(hashcode,stat_result)`
 where `hashcode` is a `BaseHashCode` subclass instance is valid
 or `None` if missing or no longer valid
 and `stat_result` is the current `os.stat` result for `fspath`.
 
@@ -180,38 +152,88 @@
                         Specify the remote hashindex executable.
             --mv        Move mode.
             -n          No action, dry run.
             -o output_format Default: '{hashcode} {fspath}'.
             -s          Symlink mode.
           Other arguments:
             refdir      The reference directory, which may be local or remote
-                        or \"-\" indicating that a hash index will be read from
+                        or "-" indicating that a hash index will be read from
                         standard input.
             targetdir   The directory containing the files to be rearranged,
                         which may be local or remote.
             dstdir      Optional destination directory for the rearranged files.
                         Default is the targetdir.
                         It is taken to be on the same host as targetdir.
         shell
           Run a command prompt via cmd.Cmd using this command's subcommands.
 
+*`HashIndexCommand.Options`*
+
+*Method `HashIndexCommand.cmd_comm(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`*:
+Usage: {cmd} {{-1|-2|-3}} {{path1|-}} {{path2|-}}
+Compare the filepaths in path1 and path2 by content.
+-1            List hashes and paths only present in path1.
+-2            List hashes and paths only present in path2.
+-3            List hashes and paths present in path1 and path2.
+-e ssh_exe    Specify the ssh executable.
+-h hashname   Specify the file content hash algorithm name.
+-H hashindex_exe
+              Specify the remote hashindex executable.
+-o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+-r            Emit relative paths in the listing.
+
+*Method `HashIndexCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`*:
+Usage: {cmd} [options...] [[host:]path...]
+Walk filesystem paths and emit a listing.
+The default path is the current directory.
+Options:
+-e ssh_exe    Specify the ssh executable.
+-h hashname   Specify the file content hash algorithm name.
+-H hashindex_exe
+              Specify the remote hashindex executable.
+-o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+-r            Emit relative paths in the listing.
+              This requires each path to be a directory.
+
+*Method `HashIndexCommand.cmd_rearrange(self, argv)`*:
+Usage: {cmd} [options...] {{[[user@]host:]refdir|-}} [[user@]rhost:]targetdir [dstdir]
+Rearrange files from targetdir into dstdir based on their positions in refdir.
+Options:
+  -e ssh_exe  Specify the ssh executable.
+  -h hashname Specify the file content hash algorithm name.
+  -H hashindex_exe
+              Specify the remote hashindex executable.
+  --mv        Move mode.
+  -n          No action, dry run.
+  -o output_format Default: {OUTPUT_FORMAT_DEFAULT!r}.
+  -s          Symlink mode.
+Other arguments:
+  refdir      The reference directory, which may be local or remote
+              or "-" indicating that a hash index will be read from
+              standard input.
+  targetdir   The directory containing the files to be rearranged,
+              which may be local or remote.
+  dstdir      Optional destination directory for the rearranged files.
+              Default is the targetdir.
+              It is taken to be on the same host as targetdir.
+
 ## Function `localpath(fspath: str) -> str`
 
 Return a filesystem path modified so that it connot be
 misinterpreted as a remote path such as `user@host:path`.
 
 If `fspath` contains no colon (`:`) or is an absolute path
 or starts with `./` then it is returned unchanged.
 Otherwise a leading `./` is prepended.
 
 ## Function `main(argv=None)`
 
 Commandline implementation.
 
-## Function `merge(srcpath: str, dstpath: str, *, opname=None, hashname: str, move_mode: bool = False, symlink_mode=False, doit=False, quiet=False, fstags: cs.fstags.FSTags)`
+## Function `merge(srcpath: str, dstpath: str, *, opname=None, hashname: str, move_mode: bool = False, symlink_mode=False, doit=False, quiet=False, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Merge `srcpath` to `dstpath`.
 
 If `dstpath` does not exist, move/link/symlink `srcpath` to `dstpath`.
 Otherwise checksum their contents and raise `FileExistsError` if they differ.
 
 ## Function `paths_remap(srcpaths: Iterable[str], fspaths_by_hashcode: Mapping[cs.hashutils.BaseHashCode, List[str]], *, hashname: str)`
@@ -239,15 +261,15 @@
 * `hashindex_exe`: the remote `hashindex` executable,
   default `HASHINDEX_EXE_DEFAULT`: `'hashindex'`
 * `relative`: optional flag, default `False`;
   if true pass `'-r'` to the remote `hashindex ls` command
 * `check`: whether to check that the remote command has a `0` return code,
   default `True`
 
-## Function `rearrange(srcdirpath: str, rfspaths_by_hashcode, dstdirpath=None, *, hashname: str, move_mode: bool = False, symlink_mode=False, doit: bool, quiet: bool = False, fstags: cs.fstags.FSTags, runstate: cs.resources.RunState)`
+## Function `rearrange(srcdirpath: str, rfspaths_by_hashcode, dstdirpath=None, *, hashname: str, move_mode: bool = False, symlink_mode=False, doit: bool, quiet: bool = False, fstags: cs.fstags.FSTags, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x101a85d80>)`
 
 Rearrange the files in `dirpath` according to the
 hashcode->[relpaths] `fspaths_by_hashcode`.
 
 Parameters:
 * `srcdirpath`: the directory whose files are to be rearranged
 * `rfspaths_by_hashcode`: a mapping of hashcode to relative
@@ -256,15 +278,15 @@
   defaults to `srcdirpath`, rearranging the files in place
 * `hashname`: the file content hash algorithm name
 * `move_move`: move files instead of linking them
 * `symlink_mode`: symlink files instead of linking them
 * `doit`: if true do the link/move/symlink, otherwise just print
 * `quiet`: default `False`; if true do not print
 
-## Function `run_remote_hashindex(rhost: str, argv, *, ssh_exe=None, hashindex_exe=None, check: bool = True, doit: bool = None, quiet: Optional[bool] = None, options: cs.cmdutils.BaseCommandOptions, **subp_options)`
+## Function `run_remote_hashindex(rhost: str, argv, *, ssh_exe=None, hashindex_exe=None, check: bool = True, doit: bool = None, quiet: Optional[bool] = None, options: Optional[cs.cmdutils.BaseCommandOptions] = <function uses_cmd_options.<locals>.<lambda> at 0x101c29bd0>, **subp_options)`
 
 Run a remote `hashindex` command.
 Return the `CompletedProcess` result or `None` if `doit` is false.
 Note that as with `cs.psutils.run`, the arguments are resolved
 via `cs.psutils.prep_argv`.
 
 Parameters:
@@ -276,22 +298,27 @@
 * `hashindex_exe`: the remote `hashindex` executable,
   default `HASHINDEX_EXE_DEFAULT`: `'hashindex'`
 * `check`: whether to check that the remote command has a `0` return code,
   default `True`
 * `doit`: whether to actually run the command, default `True`
 Other keyword parameters are passed therough to `cs.psutils.run`.
 
-## Function `set_fstags_hashcode(fspath: str, hashcode, S: os.stat_result, fstags: cs.fstags.FSTags)`
+## Function `set_fstags_hashcode(fspath: str, hashcode, S: os.stat_result, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x101bcd510>)`
 
 Record `hashcode` against `fspath`.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* file_checksum: skip any nonregular file, only use run_task when checksumming more than 1MiB.
+* HashIndexCommand.cmd_rearrange: run the refdir index in relative mode.
+* Small fixes.
+
 *Release 20240317*:
 * HashIndexCommand.cmd_ls: default to listing the current directory.
 * HashIndexCommand: new -o output_format to allow outputting only hashcodes or fspaths.
 * HashIndexCommand.cmd_comm: new -r (relative) option.
 
 *Release 20240316*:
 Fixed release upload artifacts.
@@ -309,25 +336,9 @@
 * New run_remote_hashindex() and read_remote_hashindex() functions.
 * dir_filepaths: skip dot files, the fstags .fstags file and nonregular files.
 
 *Release 20240211.1*:
 Better module docstring.
 
 *Release 20240211*:
-Initial PyPI release: \"hashindex\" command and utility functions for listing file hashcodes and rearranging trees based on a hash index."""
-content-type = "text/markdown"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-
-[tool.setuptools]
-py-modules = [
-    "cs.hashindex",
-]
+Initial PyPI release: "hashindex" command and utility functions for listing file hashcodes and rearranging trees based on a hash index.
 
-[tool.setuptools.package-dir]
-"" = "lib/python"
```


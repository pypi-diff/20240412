# Comparing `tmp/edwh_bundler_plugin-1.0.3.tar.gz` & `tmp/edwh_bundler_plugin-1.0.4.tar.gz`

## Comparing `edwh_bundler_plugin-1.0.3.tar` & `edwh_bundler_plugin-1.0.4.tar`

### file list

```diff
@@ -1,54 +1,20 @@
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/bundle.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/bundle.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/variables.toml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    14814 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/0.2.0/13622622447153152646
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/0.2.0/4805992839270043881
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/0.2.0/4890930990488170852
--rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/0.2.0/5070498930187809184
--rw-r--r--   0        0        0    14814 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/0.2.0/7752834211199787233
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/0.2.0/7834756439681645559
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/1f9e4a58da8d2c26
--rw-r--r--   0        0        0     7022 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/220b27ae11e39699
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/3dc94e2d1efa3301
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/5027a93bf2669d41
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/6ea63e2814e06e42
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/85d9dd2626db0e16
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/959f9db9cc5f252
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/96aa7be2468fbf55
--rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/a09dd4d952cac3e5
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/b0d43905b9deaf37
--rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/b2099f46af8e2519
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/b2b9ae5402e8649c
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/bf9617f57e2db17f
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/c6577c4b8daee6fc
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/c760163cd51b546a
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/d11b042324a5bc7a
--rw-r--r--   0        0        0    37619 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/d30abc2bed5b27c3
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/d6a66d1ed646ec2d
--rw-r--r--   0        0        0    37075 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/eecca4e4fd0f7365
--rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.ruff_cache/content/f7f39c01752b9dad
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/example_src/example.sass
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/example_src/variables.scss
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/__about__.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/__init__.py
--rw-r--r--   0        0        0    24800 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/bundler_plugin.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/css.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/js.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/lazy.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/shared.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/tests/test_to_scss.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/README.md
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/bundle.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/bundle.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/variables.toml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/example_src/example.sass
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/example_src/variables.scss
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/__about__.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/__init__.py
+-rw-r--r--   0        0        0    24872 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/bundler_plugin.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/css.py
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/js.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/lazy.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/shared.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/tests/test_to_scss.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/README.md
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 edwh_bundler_plugin-1.0.4/PKG-INFO
```

### Comparing `edwh_bundler_plugin-1.0.3/CHANGELOG.md` & `edwh_bundler_plugin-1.0.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.4 (2024-04-12)
+
+### Fix
+
+* Require_sudo before chmod ([`c50193a`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/c50193a8b5112e514a46b72d98cdaccedb1ad881))
+
 ## v1.0.3 (2024-02-02)
 ### Fix
 * **pyproject:** Pyproject.toml can now be used via -c option (instead of as fallback only) ([`cfc0cf0`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/cfc0cf046409c63e74ae9394ccd5d8fc7f2c2f45))
 
 ## v1.0.2 (2024-01-16)
 ### Fix
 * Database-based build now works via pathlib + auto creates tmp folders (incl. parents) ([`2eb06fa`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/2eb06fa4b74ca1cb67b816f33f6cbcc025877bcf))
```

### Comparing `edwh_bundler_plugin-1.0.3/bundle.yaml` & `edwh_bundler_plugin-1.0.4/bundle.yaml`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-1.0.3/.ruff_cache/content/b2b9ae5402e8649c` & `edwh_bundler_plugin-1.0.4/tests/test_to_scss.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,145 +1,126 @@
-00000000: 0100 0000 0000 0000 1200 0000 0000 0000  ................
-00000010: 7465 7374 732e 7465 7374 5f74 6f5f 7363  tests.test_to_sc
-00000020: 7373 0300 0000 0000 0000 0800 0000 0000  ss..............
-00000030: 0000 7465 7874 7772 6170 0000 0000 0f00  ..textwrap......
-00000040: 0000 0400 0000 0000 0000 7361 7373 1100  ..........sass..
-00000050: 0000 1c00 0000 3500 0000 0000 0000 7372  ......5.......sr
-00000060: 632e 6564 7768 5f62 756e 646c 6572 5f70  c.edwh_bundler_p
-00000070: 6c75 6769 6e2e 6373 732e 636f 6e76 6572  lugin.css.conver
-00000080: 745f 746f 5f73 6173 735f 7661 7269 6162  t_to_sass_variab
-00000090: 6c65 7346 0000 005f 0000 0001 0000 0000  lesF..._........
-000000a0: 0000 0005 0000 0000 0000 0050 7269 6e74  ...........Print
-000000b0: 0d00 0000 0000 0000 6070 7269 6e74 6020  ........`print` 
-000000c0: 666f 756e 6400 2707 0000 2c07 0000 0000  found.'...,.....
-000000d0: 0000 0000 0000 0027 0700 0001 0000 0000  .......'........
-000000e0: 0000 003d 0000 0000 0000 002f 686f 6d65  ...=......./home
-000000f0: 2f72 6f62 696e 2f77 6572 6b2f 4557 2f65  /robin/werk/EW/e
-00000100: 6477 682d 6275 6e64 6c65 722d 706c 7567  dwh-bundler-plug
-00000110: 696e 2f74 6573 7473 2f74 6573 745f 746f  in/tests/test_to
-00000120: 5f73 6373 732e 7079 d307 0000 0000 0000  _scss.py........
-00000130: 696d 706f 7274 2074 6578 7477 7261 700a  import textwrap.
-00000140: 0a69 6d70 6f72 7420 7361 7373 0a0a 6672  .import sass..fr
-00000150: 6f6d 2073 7263 2e65 6477 685f 6275 6e64  om src.edwh_bund
-00000160: 6c65 725f 706c 7567 696e 2e63 7373 2069  ler_plugin.css i
-00000170: 6d70 6f72 7420 636f 6e76 6572 745f 746f  mport convert_to
-00000180: 5f73 6173 735f 7661 7269 6162 6c65 730a  _sass_variables.
-00000190: 0a0a 6465 6620 7465 7374 5f63 6f6e 7665  ..def test_conve
-000001a0: 7274 6572 2829 3a0a 2020 2020 7363 7373  rter():.    scss
-000001b0: 5f63 6f64 6520 3d20 636f 6e76 6572 745f  _code = convert_
-000001c0: 746f 5f73 6173 735f 7661 7269 6162 6c65  to_sass_variable
-000001d0: 7328 0a20 2020 2020 2020 2066 6f6e 743d  s(.        font=
-000001e0: 5b22 4172 6961 6c22 2c20 2273 616e 732d  ["Arial", "sans-
-000001f0: 7365 7269 6622 5d2c 0a20 2020 2020 2020  serif"],.       
-00000200: 2063 6f6c 6f72 3d22 2338 3530 3462 6422   color="#8504bd"
-00000210: 2c0a 2020 2020 2020 2020 666f 6e74 5f73  ,.        font_s
-00000220: 697a 653d 3136 2c0a 2020 2020 2020 2020  ize=16,.        
-00000230: 6e6f 7468 696e 673d 4e6f 6e65 2c0a 2020  nothing=None,.  
-00000240: 2020 2020 2020 6d61 7962 653d 4661 6c73        maybe=Fals
-00000250: 652c 0a20 2020 2020 2020 206d 6170 7069  e,.        mappi
-00000260: 6e67 3d7b 0a20 2020 2020 2020 2020 2020  ng={.           
-00000270: 2022 7072 696d 6172 792d 636f 6c6f 7222   "primary-color"
-00000280: 3a20 2272 6762 6128 3235 352c 2030 2c20  : "rgba(255, 0, 
-00000290: 302c 2030 2e35 2922 2c0a 2020 2020 2020  0, 0.5)",.      
-000002a0: 2020 2020 2020 2273 6563 6f6e 6461 7279        "secondary
-000002b0: 2d63 6f6c 6f72 223a 2022 6873 6c28 3132  -color": "hsl(12
-000002c0: 312c 2031 3030 252c 2035 3025 2922 2c0a  1, 100%, 50%)",.
-000002d0: 2020 2020 2020 2020 7d2c 0a20 2020 2029          },.    )
-000002e0: 0a0a 2020 2020 7361 7373 5f63 6f64 6520  ..    sass_code 
-000002f0: 3d20 636f 6e76 6572 745f 746f 5f73 6173  = convert_to_sas
-00000300: 735f 7661 7269 6162 6c65 7328 0a20 2020  s_variables(.   
-00000310: 2020 2020 2066 6f6e 743d 5b22 4172 6961       font=["Aria
-00000320: 6c22 2c20 2273 616e 732d 7365 7269 6622  l", "sans-serif"
-00000330: 5d2c 0a20 2020 2020 2020 2063 6f6c 6f72  ],.        color
-00000340: 3d22 2338 3530 3462 6422 2c0a 2020 2020  ="#8504bd",.    
-00000350: 2020 2020 666f 6e74 5f73 697a 653d 3136      font_size=16
-00000360: 2c0a 2020 2020 2020 2020 6e6f 7468 696e  ,.        nothin
-00000370: 673d 4e6f 6e65 2c0a 2020 2020 2020 2020  g=None,.        
-00000380: 6d61 7962 653d 4661 6c73 652c 0a20 2020  maybe=False,.   
-00000390: 2020 2020 206d 6170 7069 6e67 3d7b 0a20       mapping={. 
-000003a0: 2020 2020 2020 2020 2020 2022 7072 696d             "prim
-000003b0: 6172 792d 636f 6c6f 7222 3a20 2272 6762  ary-color": "rgb
-000003c0: 6128 3235 352c 2030 2c20 302c 2030 2e35  a(255, 0, 0, 0.5
-000003d0: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
-000003e0: 2273 6563 6f6e 6461 7279 2d63 6f6c 6f72  "secondary-color
-000003f0: 223a 2022 6873 6c28 3132 312c 2031 3030  ": "hsl(121, 100
-00000400: 252c 2035 3025 2922 2c0a 2020 2020 2020  %, 50%)",.      
-00000410: 2020 7d2c 0a20 2020 2020 2020 205f 6c61    },.        _la
-00000420: 6e67 7561 6765 3d22 7361 7373 222c 0a20  nguage="sass",. 
-00000430: 2020 2029 0a0a 2020 2020 7363 7373 5f63     )..    scss_c
-00000440: 6f64 6520 2b3d 2022 2222 0a20 2020 2020  ode += """.     
-00000450: 2020 2020 2020 2068 3120 7b0a 2020 2020         h1 {.    
-00000460: 2020 2020 2020 2020 2020 666f 6e74 2d66            font-f
-00000470: 616d 696c 793a 2024 666f 6e74 3b0a 2020  amily: $font;.  
-00000480: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00000490: 723a 2024 636f 6c6f 723b 0a20 2020 2020  r: $color;.     
-000004a0: 2020 2020 2020 2020 2066 6f6e 742d 7369           font-si
-000004b0: 7a65 3a20 2466 6f6e 742d 7369 7a65 3b0a  ze: $font-size;.
-000004c0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-000004d0: 7267 696e 3a20 246e 6f74 6869 6e67 3b0a  rgin: $nothing;.
-000004e0: 0a20 2020 2020 2020 2020 2020 2020 2040  .              @
-000004f0: 6966 2024 6d61 7962 6520 7b0a 2020 2020  if $maybe {.    
-00000500: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-00000510: 6c61 793a 206e 6f6e 653b 0a20 2020 2020  lay: none;.     
-00000520: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-00000530: 2020 2020 2020 2020 2020 2f2f 206d 6170            // map
-00000540: 0a20 2020 2020 2020 2020 2020 2020 2040  .              @
-00000550: 6561 6368 2024 6b65 792c 2024 7661 6c75  each $key, $valu
-00000560: 6520 696e 2024 6d61 7070 696e 6720 7b20  e in $mapping { 
-00000570: 2f2f 2043 6f72 7265 6374 6564 2076 6172  // Corrected var
-00000580: 6961 626c 6520 6e61 6d65 2074 6f20 246d  iable name to $m
-00000590: 6170 7069 6e67 0a20 2020 2020 2020 2020  apping.         
-000005a0: 2020 2020 2020 2026 2e23 7b24 6b65 797d         &.#{$key}
-000005b0: 2d63 6f6e 7461 696e 6572 207b 0a20 2020  -container {.   
-000005c0: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-000005d0: 237b 246b 6579 7d20 7b0a 2020 2020 2020  #{$key} {.      
-000005e0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-000005f0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
-00000600: 2476 616c 7565 3b0a 2020 2020 2020 2020  $value;.        
-00000610: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000620: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000630: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000640: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000650: 2020 2020 2222 220a 0a20 2020 2073 6173      """..    sas
-00000660: 735f 636f 6465 202b 3d20 7465 7874 7772  s_code += textwr
-00000670: 6170 2e64 6564 656e 7428 0a20 2020 2020  ap.dedent(.     
-00000680: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
-00000690: 2020 2068 310a 2020 2020 2020 2020 2020     h1.          
-000006a0: 2020 2020 666f 6e74 2d66 616d 696c 793a      font-family:
-000006b0: 2024 666f 6e74 0a20 2020 2020 2020 2020   $font.         
-000006c0: 2020 2020 2063 6f6c 6f72 3a20 2463 6f6c       color: $col
-000006d0: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-000006e0: 2066 6f6e 742d 7369 7a65 3a20 2466 6f6e   font-size: $fon
-000006f0: 742d 7369 7a65 0a20 2020 2020 2020 2020  t-size.         
-00000700: 2020 2020 206d 6172 6769 6e3a 2024 6e6f       margin: $no
-00000710: 7468 696e 670a 0a20 2020 2020 2020 2020  thing..         
-00000720: 2020 2020 2040 6966 2024 6d61 7962 650a       @if $maybe.
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 6469 7370 6c61 793a 206e 6f6e 650a 0a20  display: none.. 
-00000750: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
-00000760: 6d61 700a 2020 2020 2020 2020 2020 2020  map.            
-00000770: 2020 4065 6163 6820 246b 6579 2c20 2476    @each $key, $v
-00000780: 616c 7565 2069 6e20 246d 6170 7069 6e67  alue in $mapping
-00000790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007a0: 2026 2e23 7b24 6b65 797d 2d63 6f6e 7461   &.#{$key}-conta
-000007b0: 696e 6572 0a20 2020 2020 2020 2020 2020  iner.           
-000007c0: 2020 2020 2020 202e 237b 246b 6579 7d0a         .#{$key}.
-000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007e0: 2020 2020 6261 636b 6772 6f75 6e64 2d63      background-c
-000007f0: 6f6c 6f72 3a20 2476 616c 7565 0a20 2020  olor: $value.   
-00000800: 2020 2020 2022 2222 0a20 2020 2029 0a0a       """.    )..
-00000810: 2020 2020 6373 7320 3d20 7361 7373 2e63      css = sass.c
-00000820: 6f6d 7069 6c65 2873 7472 696e 673d 7363  ompile(string=sc
-00000830: 7373 5f63 6f64 652c 206f 7574 7075 745f  ss_code, output_
-00000840: 7374 796c 653d 2265 7870 616e 6465 6422  style="expanded"
-00000850: 290a 0a20 2020 2070 7269 6e74 2863 7373  )..    print(css
-00000860: 290a 0a20 2020 2061 7373 6572 7420 6373  )..    assert cs
-00000870: 730a 2020 2020 6173 7365 7274 2022 6469  s.    assert "di
-00000880: 7370 6c61 793a 206e 6f6e 6522 206e 6f74  splay: none" not
-00000890: 2069 6e20 6373 730a 0a20 2020 2063 7373   in css..    css
-000008a0: 3220 3d20 7361 7373 2e63 6f6d 7069 6c65  2 = sass.compile
-000008b0: 2873 7472 696e 673d 7361 7373 5f63 6f64  (string=sass_cod
-000008c0: 652c 206f 7574 7075 745f 7374 796c 653d  e, output_style=
-000008d0: 2265 7870 616e 6465 6422 2c20 696e 6465  "expanded", inde
-000008e0: 6e74 6564 3d54 7275 6529 0a0a 2020 2020  nted=True)..    
-000008f0: 6173 7365 7274 2063 7373 203d 3d20 6373  assert css == cs
-00000900: 7332 0a                                  s2.
+00000000: 696d 706f 7274 2074 6578 7477 7261 700a  import textwrap.
+00000010: 0a69 6d70 6f72 7420 7361 7373 0a0a 6672  .import sass..fr
+00000020: 6f6d 2073 7263 2e65 6477 685f 6275 6e64  om src.edwh_bund
+00000030: 6c65 725f 706c 7567 696e 2e63 7373 2069  ler_plugin.css i
+00000040: 6d70 6f72 7420 636f 6e76 6572 745f 746f  mport convert_to
+00000050: 5f73 6173 735f 7661 7269 6162 6c65 730a  _sass_variables.
+00000060: 0a0a 6465 6620 7465 7374 5f63 6f6e 7665  ..def test_conve
+00000070: 7274 6572 2829 3a0a 2020 2020 7363 7373  rter():.    scss
+00000080: 5f63 6f64 6520 3d20 636f 6e76 6572 745f  _code = convert_
+00000090: 746f 5f73 6173 735f 7661 7269 6162 6c65  to_sass_variable
+000000a0: 7328 0a20 2020 2020 2020 2066 6f6e 743d  s(.        font=
+000000b0: 5b22 4172 6961 6c22 2c20 2273 616e 732d  ["Arial", "sans-
+000000c0: 7365 7269 6622 5d2c 0a20 2020 2020 2020  serif"],.       
+000000d0: 2063 6f6c 6f72 3d22 2338 3530 3462 6422   color="#8504bd"
+000000e0: 2c0a 2020 2020 2020 2020 666f 6e74 5f73  ,.        font_s
+000000f0: 697a 653d 3136 2c0a 2020 2020 2020 2020  ize=16,.        
+00000100: 6e6f 7468 696e 673d 4e6f 6e65 2c0a 2020  nothing=None,.  
+00000110: 2020 2020 2020 6d61 7962 653d 4661 6c73        maybe=Fals
+00000120: 652c 0a20 2020 2020 2020 206d 6170 7069  e,.        mappi
+00000130: 6e67 3d7b 0a20 2020 2020 2020 2020 2020  ng={.           
+00000140: 2022 7072 696d 6172 792d 636f 6c6f 7222   "primary-color"
+00000150: 3a20 2272 6762 6128 3235 352c 2030 2c20  : "rgba(255, 0, 
+00000160: 302c 2030 2e35 2922 2c0a 2020 2020 2020  0, 0.5)",.      
+00000170: 2020 2020 2020 2273 6563 6f6e 6461 7279        "secondary
+00000180: 2d63 6f6c 6f72 223a 2022 6873 6c28 3132  -color": "hsl(12
+00000190: 312c 2031 3030 252c 2035 3025 2922 2c0a  1, 100%, 50%)",.
+000001a0: 2020 2020 2020 2020 7d2c 0a20 2020 2029          },.    )
+000001b0: 0a0a 2020 2020 7361 7373 5f63 6f64 6520  ..    sass_code 
+000001c0: 3d20 636f 6e76 6572 745f 746f 5f73 6173  = convert_to_sas
+000001d0: 735f 7661 7269 6162 6c65 7328 0a20 2020  s_variables(.   
+000001e0: 2020 2020 2066 6f6e 743d 5b22 4172 6961       font=["Aria
+000001f0: 6c22 2c20 2273 616e 732d 7365 7269 6622  l", "sans-serif"
+00000200: 5d2c 0a20 2020 2020 2020 2063 6f6c 6f72  ],.        color
+00000210: 3d22 2338 3530 3462 6422 2c0a 2020 2020  ="#8504bd",.    
+00000220: 2020 2020 666f 6e74 5f73 697a 653d 3136      font_size=16
+00000230: 2c0a 2020 2020 2020 2020 6e6f 7468 696e  ,.        nothin
+00000240: 673d 4e6f 6e65 2c0a 2020 2020 2020 2020  g=None,.        
+00000250: 6d61 7962 653d 4661 6c73 652c 0a20 2020  maybe=False,.   
+00000260: 2020 2020 206d 6170 7069 6e67 3d7b 0a20       mapping={. 
+00000270: 2020 2020 2020 2020 2020 2022 7072 696d             "prim
+00000280: 6172 792d 636f 6c6f 7222 3a20 2272 6762  ary-color": "rgb
+00000290: 6128 3235 352c 2030 2c20 302c 2030 2e35  a(255, 0, 0, 0.5
+000002a0: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
+000002b0: 2273 6563 6f6e 6461 7279 2d63 6f6c 6f72  "secondary-color
+000002c0: 223a 2022 6873 6c28 3132 312c 2031 3030  ": "hsl(121, 100
+000002d0: 252c 2035 3025 2922 2c0a 2020 2020 2020  %, 50%)",.      
+000002e0: 2020 7d2c 0a20 2020 2020 2020 205f 6c61    },.        _la
+000002f0: 6e67 7561 6765 3d22 7361 7373 222c 0a20  nguage="sass",. 
+00000300: 2020 2029 0a0a 2020 2020 7363 7373 5f63     )..    scss_c
+00000310: 6f64 6520 2b3d 2022 2222 0a20 2020 2020  ode += """.     
+00000320: 2020 2020 2020 2068 3120 7b0a 2020 2020         h1 {.    
+00000330: 2020 2020 2020 2020 2020 666f 6e74 2d66            font-f
+00000340: 616d 696c 793a 2024 666f 6e74 3b0a 2020  amily: $font;.  
+00000350: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+00000360: 723a 2024 636f 6c6f 723b 0a20 2020 2020  r: $color;.     
+00000370: 2020 2020 2020 2020 2066 6f6e 742d 7369           font-si
+00000380: 7a65 3a20 2466 6f6e 742d 7369 7a65 3b0a  ze: $font-size;.
+00000390: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+000003a0: 7267 696e 3a20 246e 6f74 6869 6e67 3b0a  rgin: $nothing;.
+000003b0: 0a20 2020 2020 2020 2020 2020 2020 2040  .              @
+000003c0: 6966 2024 6d61 7962 6520 7b0a 2020 2020  if $maybe {.    
+000003d0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+000003e0: 6c61 793a 206e 6f6e 653b 0a20 2020 2020  lay: none;.     
+000003f0: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
+00000400: 2020 2020 2020 2020 2020 2f2f 206d 6170            // map
+00000410: 0a20 2020 2020 2020 2020 2020 2020 2040  .              @
+00000420: 6561 6368 2024 6b65 792c 2024 7661 6c75  each $key, $valu
+00000430: 6520 696e 2024 6d61 7070 696e 6720 7b20  e in $mapping { 
+00000440: 2f2f 2043 6f72 7265 6374 6564 2076 6172  // Corrected var
+00000450: 6961 626c 6520 6e61 6d65 2074 6f20 246d  iable name to $m
+00000460: 6170 7069 6e67 0a20 2020 2020 2020 2020  apping.         
+00000470: 2020 2020 2020 2026 2e23 7b24 6b65 797d         &.#{$key}
+00000480: 2d63 6f6e 7461 696e 6572 207b 0a20 2020  -container {.   
+00000490: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+000004a0: 237b 246b 6579 7d20 7b0a 2020 2020 2020  #{$key} {.      
+000004b0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+000004c0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
+000004d0: 2476 616c 7565 3b0a 2020 2020 2020 2020  $value;.        
+000004e0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000004f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00000500: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00000510: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000520: 2020 2020 2222 220a 0a20 2020 2073 6173      """..    sas
+00000530: 735f 636f 6465 202b 3d20 7465 7874 7772  s_code += textwr
+00000540: 6170 2e64 6564 656e 7428 0a20 2020 2020  ap.dedent(.     
+00000550: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
+00000560: 2020 2068 310a 2020 2020 2020 2020 2020     h1.          
+00000570: 2020 2020 666f 6e74 2d66 616d 696c 793a      font-family:
+00000580: 2024 666f 6e74 0a20 2020 2020 2020 2020   $font.         
+00000590: 2020 2020 2063 6f6c 6f72 3a20 2463 6f6c       color: $col
+000005a0: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+000005b0: 2066 6f6e 742d 7369 7a65 3a20 2466 6f6e   font-size: $fon
+000005c0: 742d 7369 7a65 0a20 2020 2020 2020 2020  t-size.         
+000005d0: 2020 2020 206d 6172 6769 6e3a 2024 6e6f       margin: $no
+000005e0: 7468 696e 670a 0a20 2020 2020 2020 2020  thing..         
+000005f0: 2020 2020 2040 6966 2024 6d61 7962 650a       @if $maybe.
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 6469 7370 6c61 793a 206e 6f6e 650a 0a20  display: none.. 
+00000620: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
+00000630: 6d61 700a 2020 2020 2020 2020 2020 2020  map.            
+00000640: 2020 4065 6163 6820 246b 6579 2c20 2476    @each $key, $v
+00000650: 616c 7565 2069 6e20 246d 6170 7069 6e67  alue in $mapping
+00000660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000670: 2026 2e23 7b24 6b65 797d 2d63 6f6e 7461   &.#{$key}-conta
+00000680: 696e 6572 0a20 2020 2020 2020 2020 2020  iner.           
+00000690: 2020 2020 2020 202e 237b 246b 6579 7d0a         .#{$key}.
+000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006b0: 2020 2020 6261 636b 6772 6f75 6e64 2d63      background-c
+000006c0: 6f6c 6f72 3a20 2476 616c 7565 0a20 2020  olor: $value.   
+000006d0: 2020 2020 2022 2222 0a20 2020 2029 0a0a       """.    )..
+000006e0: 2020 2020 6373 7320 3d20 7361 7373 2e63      css = sass.c
+000006f0: 6f6d 7069 6c65 2873 7472 696e 673d 7363  ompile(string=sc
+00000700: 7373 5f63 6f64 652c 206f 7574 7075 745f  ss_code, output_
+00000710: 7374 796c 653d 2265 7870 616e 6465 6422  style="expanded"
+00000720: 290a 0a20 2020 2070 7269 6e74 2863 7373  )..    print(css
+00000730: 290a 0a20 2020 2061 7373 6572 7420 6373  )..    assert cs
+00000740: 730a 2020 2020 6173 7365 7274 2022 6469  s.    assert "di
+00000750: 7370 6c61 793a 206e 6f6e 6522 206e 6f74  splay: none" not
+00000760: 2069 6e20 6373 730a 0a20 2020 2063 7373   in css..    css
+00000770: 3220 3d20 7361 7373 2e63 6f6d 7069 6c65  2 = sass.compile
+00000780: 2873 7472 696e 673d 7361 7373 5f63 6f64  (string=sass_cod
+00000790: 652c 206f 7574 7075 745f 7374 796c 653d  e, output_style=
+000007a0: 2265 7870 616e 6465 6422 2c20 696e 6465  "expanded", inde
+000007b0: 6e74 6564 3d54 7275 6529 0a0a 2020 2020  nted=True)..    
+000007c0: 6173 7365 7274 2063 7373 203d 3d20 6373  assert css == cs
+000007d0: 7332 0a                                  s2.
```

### Comparing `edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/bundler_plugin.py` & `edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/bundler_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import warnings
 from contextlib import contextmanager
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from shutil import rmtree
 
+import edwh
 import invoke
 import tomlkit
 import yaml
 from dotenv import load_dotenv
 from invoke import Context, task
 
 from .css import extract_contents_for_css
@@ -546,14 +547,16 @@
     """
     Return a dict of {column name: value} for an sqlite row.
     """
     return {col[0]: row[idx] for idx, col in enumerate(cursor.description)}
 
 
 def assert_chmod_777(c: Context, filepath: str | list[str]):
+    edwh.tasks.require_sudo(c)  # can't chmod without sudo
+
     filepaths: list[str] = [filepath] if isinstance(filepath, str) else filepath
 
     for fp in filepaths:
         resp = c.run(f'stat --format "%a  %n" {fp}', hide=True)
         chmod = resp.stdout.split(" ")[0]
         if chmod != 777:
             c.sudo(f"chmod 777 {fp}")
```

### Comparing `edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/css.py` & `edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/css.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/js.py` & `edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/js.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/lazy.py` & `edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/lazy.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-1.0.3/src/edwh_bundler_plugin/shared.py` & `edwh_bundler_plugin-1.0.4/src/edwh_bundler_plugin/shared.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-1.0.3/LICENSE.txt` & `edwh_bundler_plugin-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-1.0.3/README.md` & `edwh_bundler_plugin-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-1.0.3/pyproject.toml` & `edwh_bundler_plugin-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    'invoke',
+    'edwh',
+    'tomlkit',
     'python-dotenv',
     'libsass',
     'rjsmin',
     'requests',
     'pyyaml',
     'configuraptor',
     ]
```

### Comparing `edwh_bundler_plugin-1.0.3/PKG-INFO` & `edwh_bundler_plugin-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: edwh-bundler-plugin
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python-only static file (js, css) bundler for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-bundler-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-bundler-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-bundler-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -13,20 +13,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: configuraptor
-Requires-Dist: invoke
+Requires-Dist: edwh
 Requires-Dist: libsass
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: rjsmin
+Requires-Dist: tomlkit
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # edwh-bundler-plugin
```


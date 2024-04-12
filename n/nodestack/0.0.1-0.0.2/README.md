# Comparing `tmp/nodestack-0.0.1.tar.gz` & `tmp/nodestack-0.0.2.tar.gz`

## Comparing `nodestack-0.0.1.tar` & `nodestack-0.0.2.tar`

### file list

```diff
@@ -1,78 +1,75 @@
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 nodestack-0.0.1/.pyproject.toml.swp
--rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 nodestack-0.0.1/nodestack.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 nodestack-0.0.1/nohup.out
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/make.bat
--rw-r--r--   0        0        0    46266 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/doctrees/api.doctree
--rw-r--r--   0        0        0   100049 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/doctrees/usage.doctree
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/doctrees/generated/pynodes.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/.buildinfo
--rw-r--r--   0        0        0    23389 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/api.html
--rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/genindex.html
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/index.html
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/objects.inv
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/search.html
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/searchindex.js
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/usage.html
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_modules/index.html
--rw-r--r--   0        0        0    38270 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_modules/nodestack.html
--rw-r--r--   0        0        0    38232 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_modules/pynodes.html
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_sources/api.rst.txt
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_sources/usage.rst.txt
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_sources/generated/pynodes.rst.txt
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/alabaster.css
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/classic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/forkme_right_darkblue_121621.png
--rw-r--r--   0        0        0   288550 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/sidebar.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    68398 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/underscore.js
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/build/html/generated/pynodes.html
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/source/.conf.py.swp
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/source/.index.rst.swp
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/source/api.rst
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 nodestack-0.0.1/docs/source/index.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 nodestack-0.0.1/tests/test_nodes.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nodestack-0.0.1/tests/tests.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nodestack-0.0.1/LICENSE
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nodestack-0.0.1/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 nodestack-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 nodestack-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 nodestack-0.0.2/nodestack.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 nodestack-0.0.2/nohup.out
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0    46266 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/doctrees/api.doctree
+-rw-r--r--   0        0        0   100307 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/doctrees/usage.doctree
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/doctrees/generated/pynodes.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    23389 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/api.html
+-rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/index.html
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/search.html
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/usage.html
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_modules/index.html
+-rw-r--r--   0        0        0    38270 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_modules/nodestack.html
+-rw-r--r--   0        0        0    38232 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_modules/pynodes.html
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_sources/api.rst.txt
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_sources/usage.rst.txt
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_sources/generated/pynodes.rst.txt
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/classic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/forkme_right_darkblue_121621.png
+-rw-r--r--   0        0        0   288550 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/sidebar.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    68398 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/underscore.js
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/build/html/generated/pynodes.html
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/source/api.rst
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nodestack-0.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 nodestack-0.0.2/tests/test_nodes.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nodestack-0.0.2/tests/tests.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nodestack-0.0.2/LICENSE
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 nodestack-0.0.2/README.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 nodestack-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 nodestack-0.0.2/PKG-INFO
```

### Comparing `nodestack-0.0.1/nodestack.py` & `nodestack-0.0.2/nodestack.py`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/nohup.out` & `nodestack-0.0.2/nohup.out`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/Makefile` & `nodestack-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/make.bat` & `nodestack-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/doctrees/api.doctree` & `nodestack-0.0.2/docs/build/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/doctrees/index.doctree` & `nodestack-0.0.2/docs/build/doctrees/index.doctree`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9536 1900 0000 0000 008c 0f73 7068  ...6.........sph
+00000000: 8005 9564 1800 0000 0000 008c 0f73 7068  ...d.........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
 00000070: 6805 8cce 6e6f 6465 7374 6163 6b20 646f  h...nodestack do
@@ -130,276 +130,262 @@
 00000810: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
 00000820: 9468 1f5d 9468 215d 9468 2368 248c 0566  .h.].h!].h#h$..f
 00000830: 6f72 6365 9489 8c08 6c61 6e67 7561 6765  orce....language
 00000840: 948c 0763 6f6e 736f 6c65 948c 0e68 6967  ...console...hig
 00000850: 686c 6967 6874 5f61 7267 7394 7d94 7568  hlight_args.}.uh
 00000860: 2568 ab68 2768 2868 294b 1768 1668 9a68  %h.h'h(h)K.h.h.h
 00000870: 2668 0375 6268 4629 8194 7d94 2868 058c  &h.ubhF)..}.(h..
-00000880: 5d53 6f75 7263 6520 636f 6465 2069 7320  ]Source code is 
-00000890: 686f 7374 6564 206f 6e20 6d79 206f 776e  hosted on my own
-000008a0: 2069 6e73 7461 6e63 6520 6f66 2060 6769   instance of `gi
-000008b0: 7465 6120 3c68 7474 7073 3a2f 2f67 6974  tea <https://git
-000008c0: 6561 2e6c 7574 6978 2e6f 7267 2f66 7467  ea.lutix.org/ftg
-000008d0: 2f6e 6f64 6573 7461 636b 3e60 5f2e 9468  /nodestack>`_..h
-000008e0: 075d 9428 6811 8c2c 536f 7572 6365 2063  .].(h..,Source c
-000008f0: 6f64 6520 6973 2068 6f73 7465 6420 6f6e  ode is hosted on
-00000900: 206d 7920 6f77 6e20 696e 7374 616e 6365   my own instance
-00000910: 206f 6620 9485 9481 947d 9428 6816 68c0   of .....}.(h.h.
-00000920: 6826 6803 6827 4e68 294e 7562 6809 8c09  h&h.h'Nh)Nubh...
-00000930: 7265 6665 7265 6e63 6594 9394 2981 947d  reference...)..}
-00000940: 9428 6805 8c30 6067 6974 6561 203c 6874  .(h..0`gitea <ht
-00000950: 7470 733a 2f2f 6769 7465 612e 6c75 7469  tps://gitea.luti
-00000960: 782e 6f72 672f 6674 672f 6e6f 6465 7374  x.org/ftg/nodest
-00000970: 6163 6b3e 605f 9468 075d 9468 118c 0567  ack>`_.h.].h...g
-00000980: 6974 6561 9485 9481 947d 9428 6816 68ca  itea.....}.(h.h.
-00000990: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
-000009a0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-000009b0: 5d94 6821 5d94 8c04 6e61 6d65 948c 0567  ].h!]...name...g
-000009c0: 6974 6561 948c 0672 6566 7572 6994 8c25  itea...refuri..%
-000009d0: 6874 7470 733a 2f2f 6769 7465 612e 6c75  https://gitea.lu
-000009e0: 7469 782e 6f72 672f 6674 672f 6e6f 6465  tix.org/ftg/node
-000009f0: 7374 6163 6b94 7568 2568 c868 1668 c075  stack.uh%h.h.h.u
-00000a00: 6268 098c 0674 6172 6765 7494 9394 2981  bh...target...).
-00000a10: 947d 9428 6805 8c28 203c 6874 7470 733a  .}.(h..( <https:
-00000a20: 2f2f 6769 7465 612e 6c75 7469 782e 6f72  //gitea.lutix.or
-00000a30: 672f 6674 672f 6e6f 6465 7374 6163 6b3e  g/ftg/nodestack>
-00000a40: 9468 075d 9468 177d 9428 6819 5d94 8c05  .h.].h.}.(h.]...
-00000a50: 6769 7465 6194 6168 1b5d 9468 1d5d 948c  gitea.ah.].h.]..
-00000a60: 0567 6974 6561 9461 681f 5d94 6821 5d94  .gitea.ah.].h!].
-00000a70: 8c06 7265 6675 7269 9468 db75 6825 68dc  ..refuri.h.uh%h.
-00000a80: 8c0a 7265 6665 7265 6e63 6564 944b 0168  ..referenced.K.h
-00000a90: 1668 c075 6268 118c 012e 9485 9481 947d  .h.ubh.........}
-00000aa0: 9428 6816 68c0 6826 6803 6827 4e68 294e  .(h.h.h&h.h'Nh)N
-00000ab0: 7562 6568 177d 9428 6819 5d94 681b 5d94  ubeh.}.(h.].h.].
-00000ac0: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-00000ad0: 4568 2768 2868 294b 1b68 1668 9a68 2668  Eh'h(h)K.h.h.h&h
-00000ae0: 0375 6265 6817 7d94 2868 195d 948c 0c69  .ubeh.}.(h.]...i
-00000af0: 6e73 7461 6c6c 6174 696f 6e94 6168 1b5d  nstallation.ah.]
-00000b00: 9468 1d5d 948c 0d69 6e73 7461 6c6c 6174  .h.]...installat
-00000b10: 696f 6e3a 9461 681f 5d94 6821 5d94 7568  ion:.ah.].h!].uh
-00000b20: 2568 2a68 1668 2c68 2668 0368 2768 2868  %h*h.h,h&h.h'h(h
-00000b30: 294b 1675 6268 2b29 8194 7d94 2868 0568  )K.ubh+)..}.(h.h
-00000b40: 0668 075d 9428 6830 2981 947d 9428 6805  .h.].(h0)..}.(h.
-00000b50: 8c0c 4261 7369 6320 5573 6167 653a 9468  ..Basic Usage:.h
-00000b60: 075d 9468 118c 0c42 6173 6963 2055 7361  .].h...Basic Usa
-00000b70: 6765 3a94 8594 8194 7d94 2868 166a 0101  ge:.....}.(h.j..
-00000b80: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
-00000b90: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-00000ba0: 681f 5d94 6821 5d94 7568 2568 2f68 1668  h.].h!].uh%h/h.h
-00000bb0: fe68 2668 0368 2768 2868 294b 1e75 6268  .h&h.h'h(h)K.ubh
-00000bc0: ac29 8194 7d94 2868 0558 2901 0000 696d  .)..}.(h.X)...im
-00000bd0: 706f 7274 206e 6f64 6573 7461 636b 0a0a  port nodestack..
-00000be0: 636c 6173 7320 5065 7273 6f6e 286e 6f64  class Person(nod
-00000bf0: 6573 7461 636b 2e4e 6f64 6529 3a0a 2020  estack.Node):.  
-00000c00: 2020 7061 7373 0a0a 626f 6220 3d20 5065    pass..bob = Pe
-00000c10: 7273 6f6e 2827 426f 6227 290a 6576 6520  rson('Bob').eve 
-00000c20: 3d20 5065 7273 6f6e 2827 4576 6527 290a  = Person('Eve').
-00000c30: 616c 6963 6520 3d20 5065 7273 6f6e 2827  alice = Person('
-00000c40: 416c 6963 6527 290a 616c 6963 655f 6167  Alice').alice_ag
-00000c50: 6169 6e20 3d20 5065 7273 6f6e 2827 416c  ain = Person('Al
-00000c60: 6963 6527 2920 2320 7769 6c6c 2072 6169  ice') # will rai
-00000c70: 7365 2061 6e20 6572 726f 720a 0a0a 2320  se an error...# 
-00000c80: 416c 6963 6520 6973 2070 6172 656e 7420  Alice is parent 
-00000c90: 6f66 2062 6f62 2061 6e64 2065 7665 0a61  of bob and eve.a
-00000ca0: 6c69 6365 2e61 6464 5f63 6869 6c64 2862  lice.add_child(b
-00000cb0: 6f62 290a 616c 6963 652e 6164 645f 6368  ob).alice.add_ch
-00000cc0: 696c 6428 6576 6529 0a0a 616c 6963 652e  ild(eve)..alice.
-00000cd0: 7072 6574 7479 5f70 7269 6e74 2829 0a0a  pretty_print()..
-00000ce0: 416c 6963 650a 2020 2d2d 2042 6f62 0a20  Alice.  -- Bob. 
-00000cf0: 202d 2d20 4576 6594 6807 5d94 6811 5829   -- Eve.h.].h.X)
-00000d00: 0100 0069 6d70 6f72 7420 6e6f 6465 7374  ...import nodest
-00000d10: 6163 6b0a 0a63 6c61 7373 2050 6572 736f  ack..class Perso
-00000d20: 6e28 6e6f 6465 7374 6163 6b2e 4e6f 6465  n(nodestack.Node
-00000d30: 293a 0a20 2020 2070 6173 730a 0a62 6f62  ):.    pass..bob
-00000d40: 203d 2050 6572 736f 6e28 2742 6f62 2729   = Person('Bob')
-00000d50: 0a65 7665 203d 2050 6572 736f 6e28 2745  .eve = Person('E
-00000d60: 7665 2729 0a61 6c69 6365 203d 2050 6572  ve').alice = Per
-00000d70: 736f 6e28 2741 6c69 6365 2729 0a61 6c69  son('Alice').ali
-00000d80: 6365 5f61 6761 696e 203d 2050 6572 736f  ce_again = Perso
-00000d90: 6e28 2741 6c69 6365 2729 2023 2077 696c  n('Alice') # wil
-00000da0: 6c20 7261 6973 6520 616e 2065 7272 6f72  l raise an error
-00000db0: 0a0a 0a23 2041 6c69 6365 2069 7320 7061  ...# Alice is pa
-00000dc0: 7265 6e74 206f 6620 626f 6220 616e 6420  rent of bob and 
-00000dd0: 6576 650a 616c 6963 652e 6164 645f 6368  eve.alice.add_ch
-00000de0: 696c 6428 626f 6229 0a61 6c69 6365 2e61  ild(bob).alice.a
-00000df0: 6464 5f63 6869 6c64 2865 7665 290a 0a61  dd_child(eve)..a
-00000e00: 6c69 6365 2e70 7265 7474 795f 7072 696e  lice.pretty_prin
-00000e10: 7428 290a 0a41 6c69 6365 0a20 202d 2d20  t()..Alice.  -- 
-00000e20: 426f 620a 2020 2d2d 2045 7665 9485 9481  Bob.  -- Eve....
-00000e30: 947d 9468 166a 0f01 0000 7362 6168 177d  .}.h.j....sbah.}
-00000e40: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00000e50: 5d94 6821 5d94 6823 6824 68bb 8968 bc8c  ].h!].h#h$h..h..
-00000e60: 0670 7974 686f 6e94 68be 7d94 7568 2568  .python.h.}.uh%h
-00000e70: ab68 2768 2868 294b 2068 1668 fe68 2668  .h'h(h)K h.h.h&h
-00000e80: 0375 6265 6817 7d94 2868 195d 948c 0b62  .ubeh.}.(h.]...b
-00000e90: 6173 6963 2d75 7361 6765 9461 681b 5d94  asic-usage.ah.].
-00000ea0: 681d 5d94 8c0c 6261 7369 6320 7573 6167  h.]...basic usag
-00000eb0: 653a 9461 681f 5d94 6821 5d94 7568 2568  e:.ah.].h!].uh%h
-00000ec0: 2a68 1668 2c68 2668 0368 2768 2868 294b  *h.h,h&h.h'h(h)K
-00000ed0: 1e75 6265 6817 7d94 2868 195d 948c 2477  .ubeh.}.(h.]..$w
-00000ee0: 656c 636f 6d65 2d74 6f2d 6e6f 6465 7374  elcome-to-nodest
-00000ef0: 6163 6b2d 732d 646f 6375 6d65 6e74 6174  ack-s-documentat
-00000f00: 696f 6e94 6168 1b5d 9468 1d5d 948c 2577  ion.ah.].h.]..%w
-00000f10: 656c 636f 6d65 2074 6f20 6e6f 6465 7374  elcome to nodest
-00000f20: 6163 6b27 7320 646f 6375 6d65 6e74 6174  ack's documentat
-00000f30: 696f 6e21 9461 681f 5d94 6821 5d94 7568  ion!.ah.].h!].uh
-00000f40: 2568 2a68 1668 0368 2668 0368 2768 2868  %h*h.h.h&h.h'h(h
-00000f50: 294b 0775 6265 6817 7d94 2868 195d 9468  )K.ubeh.}.(h.].h
-00000f60: 1b5d 9468 1d5d 9468 1f5d 9468 215d 948c  .].h.].h.].h!]..
-00000f70: 0673 6f75 7263 6594 6828 8c14 7472 616e  .source.h(..tran
-00000f80: 736c 6174 696f 6e5f 7072 6f67 7265 7373  slation_progress
-00000f90: 947d 9428 8c05 746f 7461 6c94 4b00 8c0a  .}.(..total.K...
-00000fa0: 7472 616e 736c 6174 6564 944b 0075 7568  translated.K.uuh
-00000fb0: 2568 018c 0e63 7572 7265 6e74 5f73 6f75  %h...current_sou
-00000fc0: 7263 6594 4e8c 0c63 7572 7265 6e74 5f6c  rce.N..current_l
-00000fd0: 696e 6594 4e8c 0873 6574 7469 6e67 7394  ine.N..settings.
-00000fe0: 8c11 646f 6375 7469 6c73 2e66 726f 6e74  ..docutils.front
-00000ff0: 656e 6494 8c06 5661 6c75 6573 9493 9429  end...Values...)
-00001000: 8194 7d94 288c 066f 7574 7075 7494 4e68  ..}.(..output.Nh
-00001010: 2f4e 8c09 6765 6e65 7261 746f 7294 4e8c  /N..generator.N.
-00001020: 0964 6174 6573 7461 6d70 944e 8c0b 736f  .datestamp.N..so
-00001030: 7572 6365 5f6c 696e 6b94 4e8c 0a73 6f75  urce_link.N..sou
-00001040: 7263 655f 7572 6c94 4e8c 0d74 6f63 5f62  rce_url.N..toc_b
-00001050: 6163 6b6c 696e 6b73 948c 0565 6e74 7279  acklinks...entry
-00001060: 948c 1266 6f6f 746e 6f74 655f 6261 636b  ...footnote_back
-00001070: 6c69 6e6b 7394 4b01 8c0d 7365 6374 6e75  links.K...sectnu
-00001080: 6d5f 7866 6f72 6d94 4b01 8c0e 7374 7269  m_xform.K...stri
-00001090: 705f 636f 6d6d 656e 7473 944e 8c1b 7374  p_comments.N..st
-000010a0: 7269 705f 656c 656d 656e 7473 5f77 6974  rip_elements_wit
-000010b0: 685f 636c 6173 7365 7394 4e8c 0d73 7472  h_classes.N..str
-000010c0: 6970 5f63 6c61 7373 6573 944e 8c0c 7265  ip_classes.N..re
-000010d0: 706f 7274 5f6c 6576 656c 944b 028c 0a68  port_level.K...h
-000010e0: 616c 745f 6c65 7665 6c94 4b05 8c11 6578  alt_level.K...ex
-000010f0: 6974 5f73 7461 7475 735f 6c65 7665 6c94  it_status_level.
-00001100: 4b05 8c05 6465 6275 6794 4e8c 0e77 6172  K...debug.N..war
-00001110: 6e69 6e67 5f73 7472 6561 6d94 4e8c 0974  ning_stream.N..t
-00001120: 7261 6365 6261 636b 9488 8c0e 696e 7075  raceback....inpu
-00001130: 745f 656e 636f 6469 6e67 948c 0975 7466  t_encoding...utf
-00001140: 2d38 2d73 6967 948c 1c69 6e70 7574 5f65  -8-sig...input_e
-00001150: 6e63 6f64 696e 675f 6572 726f 725f 6861  ncoding_error_ha
-00001160: 6e64 6c65 7294 8c06 7374 7269 6374 948c  ndler...strict..
-00001170: 0f6f 7574 7075 745f 656e 636f 6469 6e67  .output_encoding
-00001180: 948c 0575 7466 2d38 948c 1d6f 7574 7075  ...utf-8...outpu
-00001190: 745f 656e 636f 6469 6e67 5f65 7272 6f72  t_encoding_error
-000011a0: 5f68 616e 646c 6572 946a 5701 0000 8c0e  _handler.jW.....
-000011b0: 6572 726f 725f 656e 636f 6469 6e67 948c  error_encoding..
-000011c0: 0575 7466 2d38 948c 1c65 7272 6f72 5f65  .utf-8...error_e
-000011d0: 6e63 6f64 696e 675f 6572 726f 725f 6861  ncoding_error_ha
-000011e0: 6e64 6c65 7294 8c10 6261 636b 736c 6173  ndler...backslas
-000011f0: 6872 6570 6c61 6365 948c 0d6c 616e 6775  hreplace...langu
-00001200: 6167 655f 636f 6465 948c 0265 6e94 8c13  age_code...en...
-00001210: 7265 636f 7264 5f64 6570 656e 6465 6e63  record_dependenc
-00001220: 6965 7394 4e8c 0663 6f6e 6669 6794 4e8c  ies.N..config.N.
-00001230: 0969 645f 7072 6566 6978 9468 068c 0e61  .id_prefix.h...a
-00001240: 7574 6f5f 6964 5f70 7265 6669 7894 8c02  uto_id_prefix...
-00001250: 6964 948c 0d64 756d 705f 7365 7474 696e  id...dump_settin
-00001260: 6773 944e 8c0e 6475 6d70 5f69 6e74 6572  gs.N..dump_inter
-00001270: 6e61 6c73 944e 8c0f 6475 6d70 5f74 7261  nals.N..dump_tra
-00001280: 6e73 666f 726d 7394 4e8c 0f64 756d 705f  nsforms.N..dump_
-00001290: 7073 6575 646f 5f78 6d6c 944e 8c10 6578  pseudo_xml.N..ex
-000012a0: 706f 7365 5f69 6e74 6572 6e61 6c73 944e  pose_internals.N
-000012b0: 8c0e 7374 7269 6374 5f76 6973 6974 6f72  ..strict_visitor
-000012c0: 944e 8c0f 5f64 6973 6162 6c65 5f63 6f6e  .N.._disable_con
-000012d0: 6669 6794 4e8c 075f 736f 7572 6365 9468  fig.N.._source.h
-000012e0: 288c 0c5f 6465 7374 696e 6174 696f 6e94  (.._destination.
-000012f0: 4e8c 0d5f 636f 6e66 6967 5f66 696c 6573  N.._config_files
-00001300: 945d 948c 1666 696c 655f 696e 7365 7274  .]...file_insert
-00001310: 696f 6e5f 656e 6162 6c65 6494 888c 0b72  ion_enabled....r
-00001320: 6177 5f65 6e61 626c 6564 944b 018c 116c  aw_enabled.K...l
-00001330: 696e 655f 6c65 6e67 7468 5f6c 696d 6974  ine_length_limit
-00001340: 944d 1027 8c0e 7065 705f 7265 6665 7265  .M.'..pep_refere
-00001350: 6e63 6573 944e 8c0c 7065 705f 6261 7365  nces.N..pep_base
-00001360: 5f75 726c 948c 1868 7474 7073 3a2f 2f70  _url...https://p
-00001370: 6570 732e 7079 7468 6f6e 2e6f 7267 2f94  eps.python.org/.
-00001380: 8c15 7065 705f 6669 6c65 5f75 726c 5f74  ..pep_file_url_t
-00001390: 656d 706c 6174 6594 8c08 7065 702d 2530  emplate...pep-%0
-000013a0: 3464 948c 0e72 6663 5f72 6566 6572 656e  4d...rfc_referen
-000013b0: 6365 7394 4e8c 0c72 6663 5f62 6173 655f  ces.N..rfc_base_
-000013c0: 7572 6c94 8c26 6874 7470 733a 2f2f 6461  url..&https://da
-000013d0: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
-000013e0: 7267 2f64 6f63 2f68 746d 6c2f 948c 0974  rg/doc/html/...t
-000013f0: 6162 5f77 6964 7468 944b 088c 1d74 7269  ab_width.K...tri
-00001400: 6d5f 666f 6f74 6e6f 7465 5f72 6566 6572  m_footnote_refer
-00001410: 656e 6365 5f73 7061 6365 9489 8c10 7379  ence_space....sy
-00001420: 6e74 6178 5f68 6967 686c 6967 6874 948c  ntax_highlight..
-00001430: 046c 6f6e 6794 8c0c 736d 6172 745f 7175  .long...smart_qu
-00001440: 6f74 6573 9488 8c13 736d 6172 7471 756f  otes....smartquo
-00001450: 7465 735f 6c6f 6361 6c65 7394 5d94 8c1d  tes_locales.]...
-00001460: 6368 6172 6163 7465 725f 6c65 7665 6c5f  character_level_
-00001470: 696e 6c69 6e65 5f6d 6172 6b75 7094 898c  inline_markup...
-00001480: 0e64 6f63 7469 746c 655f 7866 6f72 6d94  .doctitle_xform.
-00001490: 898c 0d64 6f63 696e 666f 5f78 666f 726d  ...docinfo_xform
-000014a0: 944b 018c 1273 6563 7473 7562 7469 746c  .K...sectsubtitl
-000014b0: 655f 7866 6f72 6d94 898c 0d69 6d61 6765  e_xform....image
-000014c0: 5f6c 6f61 6469 6e67 948c 046c 696e 6b94  _loading...link.
-000014d0: 8c10 656d 6265 645f 7374 796c 6573 6865  ..embed_styleshe
-000014e0: 6574 9489 8c15 636c 6f61 6b5f 656d 6169  et....cloak_emai
-000014f0: 6c5f 6164 6472 6573 7365 7394 888c 1173  l_addresses....s
-00001500: 6563 7469 6f6e 5f73 656c 665f 6c69 6e6b  ection_self_link
-00001510: 9489 8c03 656e 7694 4e75 628c 0872 6570  ....env.Nub..rep
-00001520: 6f72 7465 7294 4e8c 1069 6e64 6972 6563  orter.N..indirec
-00001530: 745f 7461 7267 6574 7394 5d94 8c11 7375  t_targets.]...su
-00001540: 6273 7469 7475 7469 6f6e 5f64 6566 7394  bstitution_defs.
-00001550: 7d94 8c12 7375 6273 7469 7475 7469 6f6e  }...substitution
-00001560: 5f6e 616d 6573 947d 948c 0872 6566 6e61  _names.}...refna
-00001570: 6d65 7394 7d94 8c06 7265 6669 6473 947d  mes.}...refids.}
-00001580: 948c 076e 616d 6569 6473 947d 9428 6a2c  ...nameids.}.(j,
-00001590: 0100 006a 2901 0000 6897 6894 68fb 68f8  ...j)...h.h.h.h.
-000015a0: 68e7 68e4 6a24 0100 006a 2101 0000 758c  h.h.j$...j!...u.
-000015b0: 096e 616d 6574 7970 6573 947d 9428 6a2c  .nametypes.}.(j,
-000015c0: 0100 0089 6897 8968 fb89 68e7 886a 2401  ....h..h..h..j$.
-000015d0: 0000 8975 6819 7d94 286a 2901 0000 682c  ...uh.}.(j)...h,
-000015e0: 6894 685a 68f8 689a 68e4 68de 6a21 0100  h.hZh.h.h.h.j!..
-000015f0: 0068 fe75 8c0d 666f 6f74 6e6f 7465 5f72  .h.u..footnote_r
-00001600: 6566 7394 7d94 8c0d 6369 7461 7469 6f6e  efs.}...citation
-00001610: 5f72 6566 7394 7d94 8c0d 6175 746f 666f  _refs.}...autofo
-00001620: 6f74 6e6f 7465 7394 5d94 8c11 6175 746f  otnotes.]...auto
-00001630: 666f 6f74 6e6f 7465 5f72 6566 7394 5d94  footnote_refs.].
-00001640: 8c10 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-00001650: 6573 945d 948c 1473 796d 626f 6c5f 666f  es.]...symbol_fo
-00001660: 6f74 6e6f 7465 5f72 6566 7394 5d94 8c09  otnote_refs.]...
-00001670: 666f 6f74 6e6f 7465 7394 5d94 8c09 6369  footnotes.]...ci
-00001680: 7461 7469 6f6e 7394 5d94 8c12 6175 746f  tations.]...auto
-00001690: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
-000016a0: 018c 1573 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
-000016b0: 7465 5f73 7461 7274 944b 008c 0a69 645f  te_start.K...id_
-000016c0: 636f 756e 7465 7294 8c0b 636f 6c6c 6563  counter...collec
-000016d0: 7469 6f6e 7394 8c07 436f 756e 7465 7294  tions...Counter.
-000016e0: 9394 7d94 8594 5294 8c0e 7061 7273 655f  ..}...R...parse_
-000016f0: 6d65 7373 6167 6573 945d 9468 098c 0e73  messages.].h...s
-00001700: 7973 7465 6d5f 6d65 7373 6167 6594 9394  ystem_message...
-00001710: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-00001720: 4629 8194 7d94 2868 058c 1a54 6974 6c65  F)..}.(h...Title
-00001730: 2075 6e64 6572 6c69 6e65 2074 6f6f 2073   underline too s
-00001740: 686f 7274 2e94 6807 5d94 6811 8c1a 5469  hort..h.].h...Ti
-00001750: 746c 6520 756e 6465 726c 696e 6520 746f  tle underline to
-00001760: 6f20 7368 6f72 742e 9485 9481 947d 9428  o short......}.(
-00001770: 6816 6abd 0100 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
-00001780: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
-00001790: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
-000017a0: 6845 6816 6aba 0100 0075 6268 ac29 8194  hEh.j....ubh.)..
-000017b0: 7d94 2868 058c 4957 656c 636f 6d65 2074  }.(h..IWelcome t
-000017c0: 6f20 6e6f 6465 7374 6163 6b27 7320 646f  o nodestack's do
-000017d0: 6375 6d65 6e74 6174 696f 6e21 0a3d 3d3d  cumentation!.===
-000017e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000017f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001800: 9468 075d 9468 118c 4957 656c 636f 6d65  .h.].h..IWelcome
-00001810: 2074 6f20 6e6f 6465 7374 6163 6b27 7320   to nodestack's 
-00001820: 646f 6375 6d65 6e74 6174 696f 6e21 0a3d  documentation!.=
-00001830: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001850: 3d3d 9485 9481 947d 9468 166a cb01 0000  ==.....}.h.j....
-00001860: 7362 6168 177d 9428 6819 5d94 681b 5d94  sbah.}.(h.].h.].
-00001870: 681d 5d94 681f 5d94 6821 5d94 6823 6824  h.].h.].h!].h#h$
-00001880: 7568 2568 ab68 166a ba01 0000 6827 6828  uh%h.h.j....h'h(
-00001890: 7562 6568 177d 9428 6819 5d94 681b 5d94  ubeh.}.(h.].h.].
-000018a0: 681d 5d94 681f 5d94 6821 5d94 8c05 6c65  h.].h.].h!]...le
-000018b0: 7665 6c94 4b02 8c04 7479 7065 948c 0757  vel.K...type...W
-000018c0: 4152 4e49 4e47 948c 046c 696e 6594 4b07  ARNING...line.K.
-000018d0: 8c06 736f 7572 6365 9468 2875 6825 6ab8  ..source.h(uh%j.
-000018e0: 0100 0068 1668 2c68 2668 0368 2768 2868  ...h.h,h&h.h'h(h
-000018f0: 294b 0775 6261 8c12 7472 616e 7366 6f72  )K.uba..transfor
-00001900: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
-00001910: 7261 6e73 666f 726d 6572 944e 8c0b 696e  ransformer.N..in
-00001920: 636c 7564 655f 6c6f 6794 5d94 8c0a 6465  clude_log.]...de
-00001930: 636f 7261 7469 6f6e 944e 6826 6803 7562  coration.Nh&h.ub
-00001940: 2e                                       .
+00000880: 026f 7294 6807 5d94 6811 8c02 6f72 9485  .or.h.].h...or..
+00000890: 9481 947d 9428 6816 68c0 6826 6803 6827  ...}.(h.h.h&h.h'
+000008a0: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
+000008b0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+000008c0: 7568 2568 4568 2768 2868 294b 1b68 1668  uh%hEh'h(h)K.h.h
+000008d0: 9a68 2668 0375 6268 ac29 8194 7d94 2868  .h&h.ubh.)..}.(h
+000008e0: 058c 1e28 7665 6e76 2920 2420 7069 7020  ...(venv) $ pip 
+000008f0: 696e 7374 616c 6c20 6e6f 6465 7374 6163  install nodestac
+00000900: 6b94 6807 5d94 6811 8c1e 2876 656e 7629  k.h.].h...(venv)
+00000910: 2024 2070 6970 2069 6e73 7461 6c6c 206e   $ pip install n
+00000920: 6f64 6573 7461 636b 9485 9481 947d 9468  odestack.....}.h
+00000930: 1668 ce73 6261 6817 7d94 2868 195d 9468  .h.sbah.}.(h.].h
+00000940: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9468  .].h.].h.].h!].h
+00000950: 2368 2468 bb89 68bc 8c07 636f 6e73 6f6c  #h$h..h...consol
+00000960: 6594 68be 7d94 7568 2568 ab68 2768 2868  e.h.}.uh%h.h'h(h
+00000970: 294b 1d68 1668 9a68 2668 0375 6268 4629  )K.h.h.h&h.ubhF)
+00000980: 8194 7d94 2868 058c 5d53 6f75 7263 6520  ..}.(h..]Source 
+00000990: 636f 6465 2069 7320 686f 7374 6564 206f  code is hosted o
+000009a0: 6e20 6d79 206f 776e 2069 6e73 7461 6e63  n my own instanc
+000009b0: 6520 6f66 2060 6769 7465 6120 3c68 7474  e of `gitea <htt
+000009c0: 7073 3a2f 2f67 6974 6561 2e6c 7574 6978  ps://gitea.lutix
+000009d0: 2e6f 7267 2f66 7467 2f6e 6f64 6573 7461  .org/ftg/nodesta
+000009e0: 636b 3e60 5f2e 9468 075d 9428 6811 8c2c  ck>`_..h.].(h..,
+000009f0: 536f 7572 6365 2063 6f64 6520 6973 2068  Source code is h
+00000a00: 6f73 7465 6420 6f6e 206d 7920 6f77 6e20  osted on my own 
+00000a10: 696e 7374 616e 6365 206f 6620 9485 9481  instance of ....
+00000a20: 947d 9428 6816 68de 6826 6803 6827 4e68  .}.(h.h.h&h.h'Nh
+00000a30: 294e 7562 6809 8c09 7265 6665 7265 6e63  )Nubh...referenc
+00000a40: 6594 9394 2981 947d 9428 6805 8c30 6067  e...)..}.(h..0`g
+00000a50: 6974 6561 203c 6874 7470 733a 2f2f 6769  itea <https://gi
+00000a60: 7465 612e 6c75 7469 782e 6f72 672f 6674  tea.lutix.org/ft
+00000a70: 672f 6e6f 6465 7374 6163 6b3e 605f 9468  g/nodestack>`_.h
+00000a80: 075d 9468 118c 0567 6974 6561 9485 9481  .].h...gitea....
+00000a90: 947d 9428 6816 68e8 6826 6803 6827 4e68  .}.(h.h.h&h.h'Nh
+00000aa0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+00000ab0: 5d94 681d 5d94 681f 5d94 6821 5d94 8c04  ].h.].h.].h!]...
+00000ac0: 6e61 6d65 948c 0567 6974 6561 948c 0672  name...gitea...r
+00000ad0: 6566 7572 6994 8c25 6874 7470 733a 2f2f  efuri..%https://
+00000ae0: 6769 7465 612e 6c75 7469 782e 6f72 672f  gitea.lutix.org/
+00000af0: 6674 672f 6e6f 6465 7374 6163 6b94 7568  ftg/nodestack.uh
+00000b00: 2568 e668 1668 de75 6268 098c 0674 6172  %h.h.h.ubh...tar
+00000b10: 6765 7494 9394 2981 947d 9428 6805 8c28  get...)..}.(h..(
+00000b20: 203c 6874 7470 733a 2f2f 6769 7465 612e   <https://gitea.
+00000b30: 6c75 7469 782e 6f72 672f 6674 672f 6e6f  lutix.org/ftg/no
+00000b40: 6465 7374 6163 6b3e 9468 075d 9468 177d  destack>.h.].h.}
+00000b50: 9428 6819 5d94 8c05 6769 7465 6194 6168  .(h.]...gitea.ah
+00000b60: 1b5d 9468 1d5d 948c 0567 6974 6561 9461  .].h.]...gitea.a
+00000b70: 681f 5d94 6821 5d94 8c06 7265 6675 7269  h.].h!]...refuri
+00000b80: 9468 f975 6825 68fa 8c0a 7265 6665 7265  .h.uh%h...refere
+00000b90: 6e63 6564 944b 0168 1668 de75 6268 118c  nced.K.h.h.ubh..
+00000ba0: 012e 9485 9481 947d 9428 6816 68de 6826  .......}.(h.h.h&
+00000bb0: 6803 6827 4e68 294e 7562 6568 177d 9428  h.h'Nh)Nubeh.}.(
+00000bc0: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00000bd0: 6821 5d94 7568 2568 4568 2768 2868 294b  h!].uh%hEh'h(h)K
+00000be0: 2168 1668 9a68 2668 0375 6265 6817 7d94  !h.h.h&h.ubeh.}.
+00000bf0: 2868 195d 948c 0c69 6e73 7461 6c6c 6174  (h.]...installat
+00000c00: 696f 6e94 6168 1b5d 9468 1d5d 948c 0d69  ion.ah.].h.]...i
+00000c10: 6e73 7461 6c6c 6174 696f 6e3a 9461 681f  nstallation:.ah.
+00000c20: 5d94 6821 5d94 7568 2568 2a68 1668 2c68  ].h!].uh%h*h.h,h
+00000c30: 2668 0368 2768 2868 294b 1675 6268 2b29  &h.h'h(h)K.ubh+)
+00000c40: 8194 7d94 2868 0568 0668 075d 9428 6830  ..}.(h.h.h.].(h0
+00000c50: 2981 947d 9428 6805 8c0c 4261 7369 6320  )..}.(h...Basic 
+00000c60: 5573 6167 653a 9468 075d 9468 118c 0c42  Usage:.h.].h...B
+00000c70: 6173 6963 2055 7361 6765 3a94 8594 8194  asic Usage:.....
+00000c80: 7d94 2868 166a 1f01 0000 6826 6803 6827  }.(h.j....h&h.h'
+00000c90: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
+00000ca0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+00000cb0: 7568 2568 2f68 166a 1c01 0000 6826 6803  uh%h/h.j....h&h.
+00000cc0: 6827 6828 6829 4b24 7562 68ac 2981 947d  h'h(h)K$ubh.)..}
+00000cd0: 9428 6805 5829 0100 0069 6d70 6f72 7420  .(h.X)...import 
+00000ce0: 6e6f 6465 7374 6163 6b0a 0a63 6c61 7373  nodestack..class
+00000cf0: 2050 6572 736f 6e28 6e6f 6465 7374 6163   Person(nodestac
+00000d00: 6b2e 4e6f 6465 293a 0a20 2020 2070 6173  k.Node):.    pas
+00000d10: 730a 0a62 6f62 203d 2050 6572 736f 6e28  s..bob = Person(
+00000d20: 2742 6f62 2729 0a65 7665 203d 2050 6572  'Bob').eve = Per
+00000d30: 736f 6e28 2745 7665 2729 0a61 6c69 6365  son('Eve').alice
+00000d40: 203d 2050 6572 736f 6e28 2741 6c69 6365   = Person('Alice
+00000d50: 2729 0a61 6c69 6365 5f61 6761 696e 203d  ').alice_again =
+00000d60: 2050 6572 736f 6e28 2741 6c69 6365 2729   Person('Alice')
+00000d70: 2023 2077 696c 6c20 7261 6973 6520 616e   # will raise an
+00000d80: 2065 7272 6f72 0a0a 0a23 2041 6c69 6365   error...# Alice
+00000d90: 2069 7320 7061 7265 6e74 206f 6620 626f   is parent of bo
+00000da0: 6220 616e 6420 6576 650a 616c 6963 652e  b and eve.alice.
+00000db0: 6164 645f 6368 696c 6428 626f 6229 0a61  add_child(bob).a
+00000dc0: 6c69 6365 2e61 6464 5f63 6869 6c64 2865  lice.add_child(e
+00000dd0: 7665 290a 0a61 6c69 6365 2e70 7265 7474  ve)..alice.prett
+00000de0: 795f 7072 696e 7428 290a 0a41 6c69 6365  y_print()..Alice
+00000df0: 0a20 202d 2d20 426f 620a 2020 2d2d 2045  .  -- Bob.  -- E
+00000e00: 7665 9468 075d 9468 1158 2901 0000 696d  ve.h.].h.X)...im
+00000e10: 706f 7274 206e 6f64 6573 7461 636b 0a0a  port nodestack..
+00000e20: 636c 6173 7320 5065 7273 6f6e 286e 6f64  class Person(nod
+00000e30: 6573 7461 636b 2e4e 6f64 6529 3a0a 2020  estack.Node):.  
+00000e40: 2020 7061 7373 0a0a 626f 6220 3d20 5065    pass..bob = Pe
+00000e50: 7273 6f6e 2827 426f 6227 290a 6576 6520  rson('Bob').eve 
+00000e60: 3d20 5065 7273 6f6e 2827 4576 6527 290a  = Person('Eve').
+00000e70: 616c 6963 6520 3d20 5065 7273 6f6e 2827  alice = Person('
+00000e80: 416c 6963 6527 290a 616c 6963 655f 6167  Alice').alice_ag
+00000e90: 6169 6e20 3d20 5065 7273 6f6e 2827 416c  ain = Person('Al
+00000ea0: 6963 6527 2920 2320 7769 6c6c 2072 6169  ice') # will rai
+00000eb0: 7365 2061 6e20 6572 726f 720a 0a0a 2320  se an error...# 
+00000ec0: 416c 6963 6520 6973 2070 6172 656e 7420  Alice is parent 
+00000ed0: 6f66 2062 6f62 2061 6e64 2065 7665 0a61  of bob and eve.a
+00000ee0: 6c69 6365 2e61 6464 5f63 6869 6c64 2862  lice.add_child(b
+00000ef0: 6f62 290a 616c 6963 652e 6164 645f 6368  ob).alice.add_ch
+00000f00: 696c 6428 6576 6529 0a0a 616c 6963 652e  ild(eve)..alice.
+00000f10: 7072 6574 7479 5f70 7269 6e74 2829 0a0a  pretty_print()..
+00000f20: 416c 6963 650a 2020 2d2d 2042 6f62 0a20  Alice.  -- Bob. 
+00000f30: 202d 2d20 4576 6594 8594 8194 7d94 6816   -- Eve.....}.h.
+00000f40: 6a2d 0100 0073 6261 6817 7d94 2868 195d  j-...sbah.}.(h.]
+00000f50: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00000f60: 9468 2368 2468 bb89 68bc 8c06 7079 7468  .h#h$h..h...pyth
+00000f70: 6f6e 9468 be7d 9475 6825 68ab 6827 6828  on.h.}.uh%h.h'h(
+00000f80: 6829 4b26 6816 6a1c 0100 0068 2668 0375  h)K&h.j....h&h.u
+00000f90: 6265 6817 7d94 2868 195d 948c 0b62 6173  beh.}.(h.]...bas
+00000fa0: 6963 2d75 7361 6765 9461 681b 5d94 681d  ic-usage.ah.].h.
+00000fb0: 5d94 8c0c 6261 7369 6320 7573 6167 653a  ]...basic usage:
+00000fc0: 9461 681f 5d94 6821 5d94 7568 2568 2a68  .ah.].h!].uh%h*h
+00000fd0: 1668 2c68 2668 0368 2768 2868 294b 2475  .h,h&h.h'h(h)K$u
+00000fe0: 6265 6817 7d94 2868 195d 948c 2477 656c  beh.}.(h.]..$wel
+00000ff0: 636f 6d65 2d74 6f2d 6e6f 6465 7374 6163  come-to-nodestac
+00001000: 6b2d 732d 646f 6375 6d65 6e74 6174 696f  k-s-documentatio
+00001010: 6e94 6168 1b5d 9468 1d5d 948c 2577 656c  n.ah.].h.]..%wel
+00001020: 636f 6d65 2074 6f20 6e6f 6465 7374 6163  come to nodestac
+00001030: 6b27 7320 646f 6375 6d65 6e74 6174 696f  k's documentatio
+00001040: 6e21 9461 681f 5d94 6821 5d94 7568 2568  n!.ah.].h!].uh%h
+00001050: 2a68 1668 0368 2668 0368 2768 2868 294b  *h.h.h&h.h'h(h)K
+00001060: 0775 6265 6817 7d94 2868 195d 9468 1b5d  .ubeh.}.(h.].h.]
+00001070: 9468 1d5d 9468 1f5d 9468 215d 948c 0673  .h.].h.].h!]...s
+00001080: 6f75 7263 6594 6828 8c14 7472 616e 736c  ource.h(..transl
+00001090: 6174 696f 6e5f 7072 6f67 7265 7373 947d  ation_progress.}
+000010a0: 9428 8c05 746f 7461 6c94 4b00 8c0a 7472  .(..total.K...tr
+000010b0: 616e 736c 6174 6564 944b 0075 7568 2568  anslated.K.uuh%h
+000010c0: 018c 0e63 7572 7265 6e74 5f73 6f75 7263  ...current_sourc
+000010d0: 6594 4e8c 0c63 7572 7265 6e74 5f6c 696e  e.N..current_lin
+000010e0: 6594 4e8c 0873 6574 7469 6e67 7394 8c11  e.N..settings...
+000010f0: 646f 6375 7469 6c73 2e66 726f 6e74 656e  docutils.fronten
+00001100: 6494 8c06 5661 6c75 6573 9493 9429 8194  d...Values...)..
+00001110: 7d94 288c 066f 7574 7075 7494 4e68 2f4e  }.(..output.Nh/N
+00001120: 8c09 6765 6e65 7261 746f 7294 4e8c 0964  ..generator.N..d
+00001130: 6174 6573 7461 6d70 944e 8c0b 736f 7572  atestamp.N..sour
+00001140: 6365 5f6c 696e 6b94 4e8c 0a73 6f75 7263  ce_link.N..sourc
+00001150: 655f 7572 6c94 4e8c 0d74 6f63 5f62 6163  e_url.N..toc_bac
+00001160: 6b6c 696e 6b73 948c 0565 6e74 7279 948c  klinks...entry..
+00001170: 1266 6f6f 746e 6f74 655f 6261 636b 6c69  .footnote_backli
+00001180: 6e6b 7394 4b01 8c0d 7365 6374 6e75 6d5f  nks.K...sectnum_
+00001190: 7866 6f72 6d94 4b01 8c0e 7374 7269 705f  xform.K...strip_
+000011a0: 636f 6d6d 656e 7473 944e 8c1b 7374 7269  comments.N..stri
+000011b0: 705f 656c 656d 656e 7473 5f77 6974 685f  p_elements_with_
+000011c0: 636c 6173 7365 7394 4e8c 0d73 7472 6970  classes.N..strip
+000011d0: 5f63 6c61 7373 6573 944e 8c0c 7265 706f  _classes.N..repo
+000011e0: 7274 5f6c 6576 656c 944b 028c 0a68 616c  rt_level.K...hal
+000011f0: 745f 6c65 7665 6c94 4b05 8c11 6578 6974  t_level.K...exit
+00001200: 5f73 7461 7475 735f 6c65 7665 6c94 4b05  _status_level.K.
+00001210: 8c05 6465 6275 6794 4e8c 0e77 6172 6e69  ..debug.N..warni
+00001220: 6e67 5f73 7472 6561 6d94 4e8c 0974 7261  ng_stream.N..tra
+00001230: 6365 6261 636b 9488 8c0e 696e 7075 745f  ceback....input_
+00001240: 656e 636f 6469 6e67 948c 0975 7466 2d38  encoding...utf-8
+00001250: 2d73 6967 948c 1c69 6e70 7574 5f65 6e63  -sig...input_enc
+00001260: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
+00001270: 6c65 7294 8c06 7374 7269 6374 948c 0f6f  ler...strict...o
+00001280: 7574 7075 745f 656e 636f 6469 6e67 948c  utput_encoding..
+00001290: 0575 7466 2d38 948c 1d6f 7574 7075 745f  .utf-8...output_
+000012a0: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
+000012b0: 616e 646c 6572 946a 7501 0000 8c0e 6572  andler.ju.....er
+000012c0: 726f 725f 656e 636f 6469 6e67 948c 0575  ror_encoding...u
+000012d0: 7466 2d38 948c 1c65 7272 6f72 5f65 6e63  tf-8...error_enc
+000012e0: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
+000012f0: 6c65 7294 8c10 6261 636b 736c 6173 6872  ler...backslashr
+00001300: 6570 6c61 6365 948c 0d6c 616e 6775 6167  eplace...languag
+00001310: 655f 636f 6465 948c 0265 6e94 8c13 7265  e_code...en...re
+00001320: 636f 7264 5f64 6570 656e 6465 6e63 6965  cord_dependencie
+00001330: 7394 4e8c 0663 6f6e 6669 6794 4e8c 0969  s.N..config.N..i
+00001340: 645f 7072 6566 6978 9468 068c 0e61 7574  d_prefix.h...aut
+00001350: 6f5f 6964 5f70 7265 6669 7894 8c02 6964  o_id_prefix...id
+00001360: 948c 0d64 756d 705f 7365 7474 696e 6773  ...dump_settings
+00001370: 944e 8c0e 6475 6d70 5f69 6e74 6572 6e61  .N..dump_interna
+00001380: 6c73 944e 8c0f 6475 6d70 5f74 7261 6e73  ls.N..dump_trans
+00001390: 666f 726d 7394 4e8c 0f64 756d 705f 7073  forms.N..dump_ps
+000013a0: 6575 646f 5f78 6d6c 944e 8c10 6578 706f  eudo_xml.N..expo
+000013b0: 7365 5f69 6e74 6572 6e61 6c73 944e 8c0e  se_internals.N..
+000013c0: 7374 7269 6374 5f76 6973 6974 6f72 944e  strict_visitor.N
+000013d0: 8c0f 5f64 6973 6162 6c65 5f63 6f6e 6669  .._disable_confi
+000013e0: 6794 4e8c 075f 736f 7572 6365 9468 288c  g.N.._source.h(.
+000013f0: 0c5f 6465 7374 696e 6174 696f 6e94 4e8c  ._destination.N.
+00001400: 0d5f 636f 6e66 6967 5f66 696c 6573 945d  ._config_files.]
+00001410: 948c 1666 696c 655f 696e 7365 7274 696f  ...file_insertio
+00001420: 6e5f 656e 6162 6c65 6494 888c 0b72 6177  n_enabled....raw
+00001430: 5f65 6e61 626c 6564 944b 018c 116c 696e  _enabled.K...lin
+00001440: 655f 6c65 6e67 7468 5f6c 696d 6974 944d  e_length_limit.M
+00001450: 1027 8c0e 7065 705f 7265 6665 7265 6e63  .'..pep_referenc
+00001460: 6573 944e 8c0c 7065 705f 6261 7365 5f75  es.N..pep_base_u
+00001470: 726c 948c 1868 7474 7073 3a2f 2f70 6570  rl...https://pep
+00001480: 732e 7079 7468 6f6e 2e6f 7267 2f94 8c15  s.python.org/...
+00001490: 7065 705f 6669 6c65 5f75 726c 5f74 656d  pep_file_url_tem
+000014a0: 706c 6174 6594 8c08 7065 702d 2530 3464  plate...pep-%04d
+000014b0: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
+000014c0: 7394 4e8c 0c72 6663 5f62 6173 655f 7572  s.N..rfc_base_ur
+000014d0: 6c94 8c26 6874 7470 733a 2f2f 6461 7461  l..&https://data
+000014e0: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
+000014f0: 2f64 6f63 2f68 746d 6c2f 948c 0974 6162  /doc/html/...tab
+00001500: 5f77 6964 7468 944b 088c 1d74 7269 6d5f  _width.K...trim_
+00001510: 666f 6f74 6e6f 7465 5f72 6566 6572 656e  footnote_referen
+00001520: 6365 5f73 7061 6365 9489 8c10 7379 6e74  ce_space....synt
+00001530: 6178 5f68 6967 686c 6967 6874 948c 046c  ax_highlight...l
+00001540: 6f6e 6794 8c0c 736d 6172 745f 7175 6f74  ong...smart_quot
+00001550: 6573 9488 8c13 736d 6172 7471 756f 7465  es....smartquote
+00001560: 735f 6c6f 6361 6c65 7394 5d94 8c1d 6368  s_locales.]...ch
+00001570: 6172 6163 7465 725f 6c65 7665 6c5f 696e  aracter_level_in
+00001580: 6c69 6e65 5f6d 6172 6b75 7094 898c 0e64  line_markup....d
+00001590: 6f63 7469 746c 655f 7866 6f72 6d94 898c  octitle_xform...
+000015a0: 0d64 6f63 696e 666f 5f78 666f 726d 944b  .docinfo_xform.K
+000015b0: 018c 1273 6563 7473 7562 7469 746c 655f  ...sectsubtitle_
+000015c0: 7866 6f72 6d94 898c 0d69 6d61 6765 5f6c  xform....image_l
+000015d0: 6f61 6469 6e67 948c 046c 696e 6b94 8c10  oading...link...
+000015e0: 656d 6265 645f 7374 796c 6573 6865 6574  embed_stylesheet
+000015f0: 9489 8c15 636c 6f61 6b5f 656d 6169 6c5f  ....cloak_email_
+00001600: 6164 6472 6573 7365 7394 888c 1173 6563  addresses....sec
+00001610: 7469 6f6e 5f73 656c 665f 6c69 6e6b 9489  tion_self_link..
+00001620: 8c03 656e 7694 4e75 628c 0872 6570 6f72  ..env.Nub..repor
+00001630: 7465 7294 4e8c 1069 6e64 6972 6563 745f  ter.N..indirect_
+00001640: 7461 7267 6574 7394 5d94 8c11 7375 6273  targets.]...subs
+00001650: 7469 7475 7469 6f6e 5f64 6566 7394 7d94  titution_defs.}.
+00001660: 8c12 7375 6273 7469 7475 7469 6f6e 5f6e  ..substitution_n
+00001670: 616d 6573 947d 948c 0872 6566 6e61 6d65  ames.}...refname
+00001680: 7394 7d94 8c06 7265 6669 6473 947d 948c  s.}...refids.}..
+00001690: 076e 616d 6569 6473 947d 9428 6a4a 0100  .nameids.}.(jJ..
+000016a0: 006a 4701 0000 6897 6894 6a19 0100 006a  .jG...h.h.j....j
+000016b0: 1601 0000 6a05 0100 006a 0201 0000 6a42  ....j....j....jB
+000016c0: 0100 006a 3f01 0000 758c 096e 616d 6574  ...j?...u..namet
+000016d0: 7970 6573 947d 9428 6a4a 0100 0089 6897  ypes.}.(jJ....h.
+000016e0: 896a 1901 0000 896a 0501 0000 886a 4201  .j.....j.....jB.
+000016f0: 0000 8975 6819 7d94 286a 4701 0000 682c  ...uh.}.(jG...h,
+00001700: 6894 685a 6a16 0100 0068 9a6a 0201 0000  h.hZj....h.j....
+00001710: 68fc 6a3f 0100 006a 1c01 0000 758c 0d66  h.j?...j....u..f
+00001720: 6f6f 746e 6f74 655f 7265 6673 947d 948c  ootnote_refs.}..
+00001730: 0d63 6974 6174 696f 6e5f 7265 6673 947d  .citation_refs.}
+00001740: 948c 0d61 7574 6f66 6f6f 746e 6f74 6573  ...autofootnotes
+00001750: 945d 948c 1161 7574 6f66 6f6f 746e 6f74  .]...autofootnot
+00001760: 655f 7265 6673 945d 948c 1073 796d 626f  e_refs.]...symbo
+00001770: 6c5f 666f 6f74 6e6f 7465 7394 5d94 8c14  l_footnotes.]...
+00001780: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
+00001790: 7265 6673 945d 948c 0966 6f6f 746e 6f74  refs.]...footnot
+000017a0: 6573 945d 948c 0963 6974 6174 696f 6e73  es.]...citations
+000017b0: 945d 948c 1261 7574 6f66 6f6f 746e 6f74  .]...autofootnot
+000017c0: 655f 7374 6172 7494 4b01 8c15 7379 6d62  e_start.K...symb
+000017d0: 6f6c 5f66 6f6f 746e 6f74 655f 7374 6172  ol_footnote_star
+000017e0: 7494 4b00 8c0a 6964 5f63 6f75 6e74 6572  t.K...id_counter
+000017f0: 948c 0b63 6f6c 6c65 6374 696f 6e73 948c  ...collections..
+00001800: 0743 6f75 6e74 6572 9493 947d 9485 9452  .Counter...}...R
+00001810: 948c 0e70 6172 7365 5f6d 6573 7361 6765  ...parse_message
+00001820: 7394 5d94 8c12 7472 616e 7366 6f72 6d5f  s.]...transform_
+00001830: 6d65 7373 6167 6573 945d 948c 0b74 7261  messages.]...tra
+00001840: 6e73 666f 726d 6572 944e 8c0b 696e 636c  nsformer.N..incl
+00001850: 7564 655f 6c6f 6794 5d94 8c0a 6465 636f  ude_log.]...deco
+00001860: 7261 7469 6f6e 944e 6826 6803 7562 2e    ration.Nh&h.ub.
```

### Comparing `nodestack-0.0.1/docs/build/doctrees/usage.doctree` & `nodestack-0.0.2/docs/build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/doctrees/generated/pynodes.doctree` & `nodestack-0.0.2/docs/build/doctrees/generated/pynodes.doctree`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/api.html` & `nodestack-0.0.2/docs/build/html/api.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/genindex.html` & `nodestack-0.0.2/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/index.html` & `nodestack-0.0.2/docs/build/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,18 @@
 </div>
 </section>
 <section id="installation">
 <h2>Installation:<a class="headerlink" href="#installation" title="Link to this heading">¶</a></h2>
 <div class="highlight-console notranslate"><div class="highlight"><pre><span></span><span class="gp gp-VirtualEnv">(venv)</span> <span class="gp">$ </span>git<span class="w"> </span>clone<span class="w"> </span>https://gitea.lutix.org/ftg/nodestack.git
 </pre></div>
 </div>
+<p>or</p>
+<div class="highlight-console notranslate"><div class="highlight"><pre><span></span><span class="gp gp-VirtualEnv">(venv)</span> <span class="gp">$ </span>pip<span class="w"> </span>install<span class="w"> </span>nodestack
+</pre></div>
+</div>
 <p>Source code is hosted on my own instance of <a class="reference external" href="https://gitea.lutix.org/ftg/nodestack">gitea</a>.</p>
 </section>
 <section id="basic-usage">
 <h2>Basic Usage:<a class="headerlink" href="#basic-usage" title="Link to this heading">¶</a></h2>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">nodestack</span>
 
 <span class="k">class</span> <span class="nc">Person</span><span class="p">(</span><span class="n">nodestack</span><span class="o">.</span><span class="n">Node</span><span class="p">):</span>
```

#### html2text {}

```diff
@@ -9,14 +9,16 @@
 Note
 This project is under active development.
 ********** CCoonntteenntt::_?¶ **********
     * _A_P_I
           o _N_o_d_e
 ********** IInnssttaallllaattiioonn::_?¶ **********
 (venv) $ git clone https://gitea.lutix.org/ftg/nodestack.git
+or
+(venv) $ pip install nodestack
 Source code is hosted on my own instance of _g_i_t_e_a.
 ********** BBaassiicc UUssaaggee::_?¶ **********
 import nodestack
 
 class Person(nodestack.Node):
     pass
```

### Comparing `nodestack-0.0.1/docs/build/html/py-modindex.html` & `nodestack-0.0.2/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/search.html` & `nodestack-0.0.2/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/usage.html` & `nodestack-0.0.2/docs/build/html/usage.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_modules/index.html` & `nodestack-0.0.2/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_modules/nodestack.html` & `nodestack-0.0.2/docs/build/html/_modules/nodestack.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_modules/pynodes.html` & `nodestack-0.0.2/docs/build/html/_modules/pynodes.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_sources/index.rst.txt` & `nodestack-0.0.2/docs/build/html/_sources/index.rst.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. nodestack documentation master file, created by
    sphinx-quickstart on Sat Mar 30 18:38:12 2024.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to nodestack's documentation!
-===================================
+=====================================
 
 .. note::
 
    This project is under active development.
 
 Content:
 --------
@@ -20,14 +20,20 @@
 
 Installation:
 -------------
 .. code-block:: console
 
    (venv) $ git clone https://gitea.lutix.org/ftg/nodestack.git
 
+or
+
+.. code-block:: console
+
+   (venv) $ pip install nodestack
+
 Source code is hosted on my own instance of `gitea <https://gitea.lutix.org/ftg/nodestack>`_.
 
 Basic Usage:
 ------------
 
 .. code-block:: python
```

### Comparing `nodestack-0.0.1/docs/build/html/_static/alabaster.css` & `nodestack-0.0.2/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/basic.css` & `nodestack-0.0.2/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/classic.css` & `nodestack-0.0.2/docs/build/html/_static/classic.css`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/doctools.js` & `nodestack-0.0.2/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/forkme_right_darkblue_121621.png` & `nodestack-0.0.2/docs/build/html/_static/forkme_right_darkblue_121621.png`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/jquery.js` & `nodestack-0.0.2/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/language_data.js` & `nodestack-0.0.2/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/pygments.css` & `nodestack-0.0.2/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/searchtools.js` & `nodestack-0.0.2/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/sidebar.js` & `nodestack-0.0.2/docs/build/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/sphinx_highlight.js` & `nodestack-0.0.2/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/underscore.js` & `nodestack-0.0.2/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/badge_only.css` & `nodestack-0.0.2/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/theme.css` & `nodestack-0.0.2/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-bold.woff` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-bold.woff2` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-normal.woff` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/css/fonts/lato-normal.woff2` & `nodestack-0.0.2/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/js/badge_only.js` & `nodestack-0.0.2/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `nodestack-0.0.2/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/js/html5shiv.min.js` & `nodestack-0.0.2/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/_static/js/theme.js` & `nodestack-0.0.2/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/build/html/generated/pynodes.html` & `nodestack-0.0.2/docs/build/html/generated/pynodes.html`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/source/conf.py` & `nodestack-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/docs/source/index.rst` & `nodestack-0.0.2/docs/source/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. nodestack documentation master file, created by
    sphinx-quickstart on Sat Mar 30 18:38:12 2024.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to nodestack's documentation!
-===================================
+=====================================
 
 .. note::
 
    This project is under active development.
 
 Content:
 --------
@@ -20,14 +20,20 @@
 
 Installation:
 -------------
 .. code-block:: console
 
    (venv) $ git clone https://gitea.lutix.org/ftg/nodestack.git
 
+or
+
+.. code-block:: console
+
+   (venv) $ pip install nodestack
+
 Source code is hosted on my own instance of `gitea <https://gitea.lutix.org/ftg/nodestack>`_.
 
 Basic Usage:
 ------------
 
 .. code-block:: python
```

### Comparing `nodestack-0.0.1/LICENSE` & `nodestack-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestack-0.0.1/pyproject.toml` & `nodestack-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 exclude = ["venv"]
 
 [project]
 name = "nodestack"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="fabthegreat", email="nodestack@lutix.org" },
 ]
 description = "A simple tree objects library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nodestack-0.0.1/PKG-INFO` & `nodestack-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.3
 Name: nodestack
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple tree objects library
 Project-URL: Homepage, https://gitea.lutix.org/ftg/nodestack
 Project-URL: Issues, https://gitea.lutix.org/ftg/nodestack/issues
 Author-email: fabthegreat <nodestack@lutix.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# Reserved slot
+# Nodestack
 
-Slot reserved for future package.
+Nodestack is a library that allows user to build structured trees of datas.
+
+Project is under active development. Have a look at the repository for usage. Feel free to push patches.
```


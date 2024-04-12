# Comparing `tmp/autodoc_pydantic-2.0.1.tar.gz` & `tmp/autodoc_pydantic-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodoc_pydantic-2.0.1.tar", max compression
+gzip compressed data, was "autodoc_pydantic-2.1.0.tar", max compression
```

## Comparing `autodoc_pydantic-2.0.1.tar` & `autodoc_pydantic-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-08-01 21:53:05.924861 autodoc_pydantic-2.0.1/LICENSE
--rw-r--r--   0        0        0    19092 2023-08-01 21:53:05.924861 autodoc_pydantic-2.0.1/README.md
--rw-r--r--   0        0        0     1944 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/__init__.py
--rw-r--r--   0        0        0     6075 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/__init__.py
--rw-r--r--   0        0        0      181 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/css/autodoc_pydantic.css
--rw-r--r--   0        0        0        0 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/__init__.py
--rw-r--r--   0        0        0    30118 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py
--rw-r--r--   0        0        0     8884 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/directives.py
--rw-r--r--   0        0        0        0 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/__init__.py
--rw-r--r--   0        0        0     9253 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/composites.py
--rw-r--r--   0        0        0     3484 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/definition.py
--rw-r--r--   0        0        0      452 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/enums.py
--rw-r--r--   0        0        0     1814 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/validators.py
--rw-r--r--   0        0        0      838 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/templates.py
--rw-r--r--   0        0        0     1977 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/utility.py
--rw-r--r--   0        0        0      946 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/events.py
--rw-r--r--   0        0        0    15925 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/inspection.py
--rw-r--r--   0        0        0     1736 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/utility.py
--rw-r--r--   0        0        0    20976 1970-01-01 00:00:00.000000 autodoc_pydantic-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-18 08:16:20.825350 autodoc_pydantic-2.1.0/LICENSE
+-rw-r--r--   0        0        0    23098 2024-03-18 08:16:20.825350 autodoc_pydantic-2.1.0/README.md
+-rw-r--r--   0        0        0     2005 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5961 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/__init__.py
+-rw-r--r--   0        0        0      181 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/css/autodoc_pydantic.css
+-rw-r--r--   0        0        0        0 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/__init__.py
+-rw-r--r--   0        0        0    33760 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py
+-rw-r--r--   0        0        0     8884 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/directives.py
+-rw-r--r--   0        0        0        0 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/options/__init__.py
+-rw-r--r--   0        0        0     9948 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/options/composites.py
+-rw-r--r--   0        0        0     3484 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/options/definition.py
+-rw-r--r--   0        0        0      452 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/options/enums.py
+-rw-r--r--   0        0        0     1814 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/options/validators.py
+-rw-r--r--   0        0        0      838 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/templates.py
+-rw-r--r--   0        0        0     1977 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/utility.py
+-rw-r--r--   0        0        0      946 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/events.py
+-rw-r--r--   0        0        0    15925 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/inspection.py
+-rw-r--r--   0        0        0     1736 2024-03-18 08:16:20.837350 autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/utility.py
+-rw-r--r--   0        0        0    25104 1970-01-01 00:00:00.000000 autodoc_pydantic-2.1.0/PKG-INFO
```

### Comparing `autodoc_pydantic-2.0.1/LICENSE` & `autodoc_pydantic-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/README.md` & `autodoc_pydantic-2.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ![Autodoc Pydantic](https://raw.githubusercontent.com/mansenfranzen/autodoc_pydantic/main/docs/source/material/logo_black.svg)
 
 [![PyPI version](https://img.shields.io/pypi/v/autodoc_pydantic?style=for-the-badge)](https://pypi.org/project/autodoc-pydantic/)
-![Python](https://img.shields.io/badge/python-3.7+-blue.svg?style=for-the-badge)
+![Python](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge)
 
 [![Master](https://img.shields.io/github/actions/workflow/status/mansenfranzen/autodoc_pydantic/tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/autodoc_pydantic/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic)
 
 [![Downloads](https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-badge)](https://pypistats.org/packages/autodoc-pydantic)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-37-orange.svg?style=for-the-badge)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-47-orange.svg?style=for-the-badge)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 You love [pydantic](https://pydantic-docs.helpmanual.io/) ❤ and you want to
 document your models and configuration settings with [sphinx](https://www.sphinx-doc.org/en/master/)?
 
 Perfect, let's go. But wait, sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html)
@@ -25,15 +25,16 @@
 - 🔗 adds hyperlinks between validators and corresponding fields
 - 📃 includes collapsable model json schema
 - 🏄 natively integrates with autodoc and autosummary extensions
 - 📎 defines explicit pydantic prefixes for models, settings, fields, validators and model config
 - 📋 shows summary section for model configuration, fields and validators
 - 👀 hides overloaded and redundant model class signature
 - 🔱 visualizes entity-relationship-diagrams for class hierarchies
-- 🍀 Supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0`
+- 🔨 allows complete configurability on global and per-model level
+- 🍀 supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0`
 
 ## Documentation
 
 For more details, please visit the official [documentation](https://autodoc-pydantic.readthedocs.io/en/stable/):
 
 - [Installation](https://autodoc-pydantic.readthedocs.io/en/stable/users/installation.html)
 - [Configuration](https://autodoc-pydantic.readthedocs.io/en/stable/users/configuration.html)
@@ -103,14 +104,26 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/PriOliveira"><img src="https://avatars.githubusercontent.com/u/13801839?v=4?s=100" width="100px;" alt="Priscila Oliveira"/><br /><sub><b>Priscila Oliveira</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3APriOliveira" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-PriOliveira" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/awoimbee"><img src="https://avatars.githubusercontent.com/u/22431493?v=4?s=100" width="100px;" alt="Arthur Woimbée"/><br /><sub><b>Arthur Woimbée</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3Aawoimbee" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-awoimbee" title="User Testing">📓</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/effigies"><img src="https://avatars.githubusercontent.com/u/83442?v=4?s=100" width="100px;" alt="Chris Markiewicz"/><br /><sub><b>Chris Markiewicz</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Aeffigies" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nagledb"><img src="https://avatars.githubusercontent.com/u/727435?v=4?s=100" width="100px;" alt="David B. Nagle"/><br /><sub><b>David B. Nagle</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Anagledb" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jerryjiahaha"><img src="https://avatars.githubusercontent.com/u/3163720?v=4?s=100" width="100px;" alt="JerryJia"/><br /><sub><b>JerryJia</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=jerryjiahaha" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/devmonkey22"><img src="https://avatars.githubusercontent.com/u/5084545?v=4?s=100" width="100px;" alt="Mike D"/><br /><sub><b>Mike D</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=devmonkey22" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Adevmonkey22" title="Bug reports">🐛</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=devmonkey22" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/daquinteroflex"><img src="https://avatars.githubusercontent.com/u/149674618?v=4?s=100" width="100px;" alt="Dario Quintero (Flexcompute)"/><br /><sub><b>Dario Quintero (Flexcompute)</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3Adaquinteroflex" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rafa-guedes"><img src="https://avatars.githubusercontent.com/u/7799184?v=4?s=100" width="100px;" alt="Rafael Guedes"/><br /><sub><b>Rafael Guedes</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=rafa-guedes" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/caerulescens"><img src="https://avatars.githubusercontent.com/u/29284192?v=4?s=100" width="100px;" alt="Andrew Linzie"/><br /><sub><b>Andrew Linzie</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=caerulescens" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tasansal"><img src="https://avatars.githubusercontent.com/u/13684161?v=4?s=100" width="100px;" alt="Altay Sansal"/><br /><sub><b>Altay Sansal</b></sub></a><br /><a href="#ideas-tasansal" title="Ideas, Planning, & Feedback">🤔</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.git-pull.com"><img src="https://avatars.githubusercontent.com/u/26336?v=4?s=100" width="100px;" alt="Tony Narlock"/><br /><sub><b>Tony Narlock</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=tony" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=tony" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://huxuan.org/"><img src="https://avatars.githubusercontent.com/u/726061?v=4?s=100" width="100px;" alt="Xuan (Sean) Hu"/><br /><sub><b>Xuan (Sean) Hu</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Ahuxuan" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Cielquan"><img src="https://avatars.githubusercontent.com/u/43916661?v=4?s=100" width="100px;" alt="Christian Riedel"/><br /><sub><b>Christian Riedel</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3ACielquan" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/morcef"><img src="https://avatars.githubusercontent.com/u/15701746?v=4?s=100" width="100px;" alt="morcef"/><br /><sub><b>morcef</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Amorcef" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alejandro-yousef"><img src="https://avatars.githubusercontent.com/u/93203189?v=4?s=100" width="100px;" alt="alejandro-yousef"/><br /><sub><b>alejandro-yousef</b></sub></a><br /><a href="#ideas-alejandro-yousef" title="Ideas, Planning, & Feedback">🤔</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
 ![Autodoc Pydantic](https://raw.githubusercontent.com/mansenfranzen/
 autodoc_pydantic/main/docs/source/material/logo_black.svg) [![PyPI version]
 (https://img.shields.io/pypi/v/autodoc_pydantic?style=for-the-badge)](https://
 pypi.org/project/autodoc-pydantic/) ![Python](https://img.shields.io/badge/
-python-3.7+-blue.svg?style=for-the-badge) [![Master](https://img.shields.io/
+python-3.8+-blue.svg?style=for-the-badge) [![Master](https://img.shields.io/
 github/actions/workflow/status/mansenfranzen/autodoc_pydantic/
 tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/
 autodoc_pydantic/actions/workflows/tests.yml) [![Coverage](https://
 img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-
 badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic) [![Downloads]
 (https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-
 badge)](https://pypistats.org/packages/autodoc-pydantic) [![All Contributors]
-(https://img.shields.io/badge/all_contributors-37-orange.svg?style=for-the-
+(https://img.shields.io/badge/all_contributors-47-orange.svg?style=for-the-
 badge)](#contributors) You love [pydantic](https://pydantic-docs.helpmanual.io/
 ) â¤ and you want to document your models and configuration settings with
 [sphinx](https://www.sphinx-doc.org/en/master/)? Perfect, let's go. But wait,
 sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/
 autodoc.html) does not integrate too well with pydantic models ð. Don't
 worry - just `pip install autodoc_pydantic` âº. ## Features - ð¬ provides
 default values, alias and constraints for model fields - ð adds hyperlinks
 between validators and corresponding fields - ð includes collapsable model
 json schema - ð natively integrates with autodoc and autosummary extensions
 - ð defines explicit pydantic prefixes for models, settings, fields,
 validators and model config - ð shows summary section for model
 configuration, fields and validators - ð hides overloaded and redundant
 model class signature - ð± visualizes entity-relationship-diagrams for class
-hierarchies - ð Supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0` ##
+hierarchies - ð¨ allows complete configurability on global and per-model
+level - ð supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0` ##
 Documentation For more details, please visit the official [documentation]
 (https://autodoc-pydantic.readthedocs.io/en/stable/): - [Installation](https://
 autodoc-pydantic.readthedocs.io/en/stable/users/installation.html) -
 [Configuration](https://autodoc-pydantic.readthedocs.io/en/stable/users/
 configuration.html) - [Usage](https://autodoc-pydantic.readthedocs.io/en/
 stable/users/usage.html) - [Examples](https://autodoc-pydantic.readthedocs.io/
 en/stable/users/examples.html) - [Developer Guide](https://autodoc-
@@ -40,48 +41,53 @@
 those features in action, jump over to the [example documentation](https://
 autodoc-pydantic.readthedocs.io/en/stable/users/examples.html#default-
 configuration) to compare the appearance of standard sphinx autodoc with
 *autodoc_pydantic*. ## Acknowledgements Thanks to great open source projects
 [sphinx](https://www.sphinx-doc.org/en/master/), [pydantic](https://pydantic-
 docs.helpmanual.io/) and [poetry](https://python-poetry.org/) (and so many
 more) â¤ in addition to the following contributors:
-  _[_F_r_a_n_z       _[_Y_v_e_s   _[_T_h_e_B_e_a_r_d_e_d_B_e_r_s_e_r_k_r_]     _[_J_a_n     _[_a_n_t_v_i_g_]   _[_H_u_g_o_ _O     _[_y_u_r_a
- _W_Ã_¶_l_l_e_r_t_]    _R_e_n_i_e_r_]   _TT_hh_ee_BB_ee_aa_rr_dd_ee_dd_BB_ee_rr_ss_ee_rr_kk_rr  _V_l_Ä__i_n_s_k_Ã_½_]   _aa_nn_tt_vv_ii_gg    _R_i_v_e_r_a_]  _b_o_n_d_a_r_e_n_k_o_]
-   _FF_rr_aa_nn_zz        _YY_vv_ee_ss           _ð__¤_             _JJ_aa_nn      _ð___ _ð___  _HH_uu_gg_oo_ _OO      _yy_uu_rr_aa
- _WW_?Ã_?¶_ll_ll_ee_rr_tt      _RR_ee_nn_ii_ee_rr                        _VV_ll_?Ä_?_ii_nn_ss_kk_?Ã_?½             _RR_ii_vv_ee_rr_aa   _bb_oo_nn_dd_aa_rr_ee_nn_kk_oo
- _ð___§ _ð___      _ð___                          _ð___¡_ï_¸_                _ð__¤_     _ð___ _ð___
+  _[_F_r_a_n_z       _[_Y_v_e_s   _[_T_h_e_B_e_a_r_d_e_d_B_e_r_s_e_r_k_r_]      _[_J_a_n       _[_a_n_t_v_i_g_]    _[_H_u_g_o_ _O     _[_y_u_r_a
+ _W_Ã_¶_l_l_e_r_t_]    _R_e_n_i_e_r_]   _TT_hh_ee_BB_ee_aa_rr_dd_ee_dd_BB_ee_rr_ss_ee_rr_kk_rr   _V_l_Ä__i_n_s_k_Ã_½_]     _aa_nn_tt_vv_ii_gg     _R_i_v_e_r_a_]  _b_o_n_d_a_r_e_n_k_o_]
+   _FF_rr_aa_nn_zz        _YY_vv_ee_ss           _ð__¤_         _JJ_aa_nn_ _VV_ll_?Ä_?_ii_nn_ss_kk_?Ã_?½  _ð___ _ð___   _HH_uu_gg_oo_ _OO      _yy_uu_rr_aa
+ _WW_?Ã_?¶_ll_ll_ee_rr_tt      _RR_ee_nn_ii_ee_rr                          _ð___¡_ï_¸_                  _RR_ii_vv_ee_rr_aa   _bb_oo_nn_dd_aa_rr_ee_nn_kk_oo
+ _ð___§ _ð___      _ð___                                                     _ð__¤_     _ð___ _ð___
 _â__ _ï_¸_ _ð___    _â__ _ï_¸_
                 _ð___
-  _[_T_r_e_v_o_r    _[_t_h_o_m_a_s_-        _[_M_a_t_ _U_t_t_e_r_]      _[_D_a_v_i_d_ _C   _[_J_o_s_h_ _A_.  _[_R_o_d_e_r_i_c_k _[_L_i_l_y_ _W_a_n_g_]
-  _H_o_w_a_r_d_]     _p_e_d_o_t_]          _MM_aa_tt_ _UU_tt_tt_ee_rr        _H_a_l_l_]     _M_i_t_c_h_e_l_l_]    _G_o_]     _LL_ii_ll_yy_ _WW_aa_nn_gg
-  _TT_rr_ee_vv_oo_rr     _tt_hh_oo_mm_aa_ss_--          _ð___ _ð___     _DD_aa_vv_ii_dd_ _CC_ _HH_aa_ll_ll  _JJ_oo_ss_hh_ _AA_..  _RR_oo_dd_ee_rr_ii_cc_kk   _ð___ _ð___
-  _HH_oo_ww_aa_rr_dd      _pp_ee_dd_oo_tt                          _ð__¤_ _ð___   _MM_ii_tt_cc_hh_ee_ll_ll     _GG_oo
- _ð___ _ð___  _ð___ _ð___                                      _ð__¤_     _â__ _ï_¸_
-                                                          _â__ _ï_¸_
-_[_j_-_c_a_r_s_o_n_]    _[_J_a_k_o_b      _[_J_u_a_n_ _L_u_i_s_ _C_a_n_o     _[_M_i_k_a_l_a_i     _[_S_t_i_g     _[_I_l_i_a    _[_G_r_z_e_g_o_r_z
- _jj_--_cc_aa_rr_ss_oo_nn     _L_y_k_k_e         _R_o_d_r_Ã_­_g_u_e_z_]        _C_h_a_l_y_]    _K_o_r_s_n_e_s_]  _K_u_r_e_n_k_o_v_]   _B_o_k_o_t_a_]
- _ð___ _ð___»  _A_n_d_e_r_s_e_n_]      _JJ_uu_aa_nn_ _LL_uu_ii_ss_ _CC_aa_nn_oo     _MM_ii_kk_aa_ll_aa_ii      _SS_tt_ii_gg      _II_ll_ii_aa     _GG_rr_zz_ee_gg_oo_rr_zz
-  _â__ _ï_¸_      _JJ_aa_kk_oo_bb          _RR_oo_dd_rr_?Ã_?­_gg_uu_ee_zz        _CC_hh_aa_ll_yy      _KK_oo_rr_ss_nn_ee_ss  _KK_uu_rr_ee_nn_kk_oo_vv    _BB_oo_kk_oo_tt_aa
-              _LL_yy_kk_kk_ee             _ð___        _ð___ _â__ _ï_¸_  _ð___ _ð__¤_   _ð___       _ð___
+  _[_T_r_e_v_o_r    _[_t_h_o_m_a_s_-        _[_M_a_t_ _U_t_t_e_r_]    _[_D_a_v_i_d_ _C_ _H_a_l_l_]  _[_J_o_s_h_ _A_.   _[_R_o_d_e_r_i_c_k _[_L_i_l_y_ _W_a_n_g_]
+  _H_o_w_a_r_d_]     _p_e_d_o_t_]          _MM_aa_tt_ _UU_tt_tt_ee_rr      _DD_aa_vv_ii_dd_ _CC_ _HH_aa_ll_ll   _M_i_t_c_h_e_l_l_]     _G_o_]     _LL_ii_ll_yy_ _WW_aa_nn_gg
+  _TT_rr_ee_vv_oo_rr     _tt_hh_oo_mm_aa_ss_--          _ð___ _ð___       _ð__¤_ _ð___      _JJ_oo_ss_hh_ _AA_..   _RR_oo_dd_ee_rr_ii_cc_kk   _ð___ _ð___
+  _HH_oo_ww_aa_rr_dd      _pp_ee_dd_oo_tt                                         _MM_ii_tt_cc_hh_ee_ll_ll      _GG_oo
+ _ð___ _ð___  _ð___ _ð___                                      _ð__¤_ _â__ _ï_¸_  _â__ _ï_¸_
+_[_j_-_c_a_r_s_o_n_]    _[_J_a_k_o_b      _[_J_u_a_n_ _L_u_i_s_ _C_a_n_o      _[_M_i_k_a_l_a_i       _[_S_t_i_g      _[_I_l_i_a    _[_G_r_z_e_g_o_r_z
+ _jj_--_cc_aa_rr_ss_oo_nn     _L_y_k_k_e         _R_o_d_r_Ã_­_g_u_e_z_]         _C_h_a_l_y_]      _K_o_r_s_n_e_s_]   _K_u_r_e_n_k_o_v_]   _B_o_k_o_t_a_]
+ _ð___ _ð___»  _A_n_d_e_r_s_e_n_]      _JJ_uu_aa_nn_ _LL_uu_ii_ss_ _CC_aa_nn_oo   _MM_ii_kk_aa_ll_aa_ii_ _CC_hh_aa_ll_yy     _SS_tt_ii_gg       _II_ll_ii_aa     _GG_rr_zz_ee_gg_oo_rr_zz
+  _â__ _ï_¸_      _JJ_aa_kk_oo_bb          _RR_oo_dd_rr_?Ã_?­_gg_uu_ee_zz      _ð___ _â__ _ï_¸_     _KK_oo_rr_ss_nn_ee_ss   _KK_uu_rr_ee_nn_kk_oo_vv    _BB_oo_kk_oo_tt_aa
+              _LL_yy_kk_kk_ee             _ð___                        _ð___ _ð__¤_    _ð___       _ð___
              _AA_nn_dd_ee_rr_ss_ee_nn
                _ð___»
-_[_j_g_u_n_s_t_o_n_e_] _[_i_w_y_r_k_o_r_e_] _[_s_p_a_c_e_m_a_n_s_p_i_f_f_2_0_0_7_]  _[_L_u_k_e_ _H_s_i_a_o_]  _[_D_a_n_i_e_l  _[_E_v_g_e_n_i_y     _[_J_a_n_-
- _jj_gg_uu_nn_ss_tt_oo_nn_ee   _ii_ww_yy_rr_kk_oo_rr_ee   _ss_pp_aa_cc_ee_mm_aa_nn_ss_pp_ii_ff_ff_22_00_00_77    _LL_uu_kk_ee_ _HH_ss_ii_aa_oo   _W_a_l_k_e_r_]  _L_u_p_a_s_h_i_n_]   _H_e_n_d_r_i_k
-   _ð___        _ð___»         _ð___ _ð__¤_           _ð___      _DD_aa_nn_ii_ee_ll    _EE_vv_gg_ee_nn_ii_yy    _E_w_e_r_s_]
-                                                          _WW_aa_ll_kk_ee_rr   _LL_uu_pp_aa_ss_hh_ii_nn  _JJ_aa_nn_--_HH_ee_nn_dd_rr_ii_kk
-                                                           _ð___      _ð___       _EE_ww_ee_rr_ss
-                                                                                _ð___
-  _[_J_o_n_n_y     _[_C_h_a_r_l_e_s  _[_T_h_o_m_a_s_ _K_a_r_a_o_u_z_e_n_e_]  _[_c_a_s_e_y_z_a_k_2_4_] _[_P_r_i_s_c_i_l_a  _[_A_r_t_h_u_r    _[_C_h_r_i_s
- _S_a_u_n_d_e_r_s_]  _M_a_c_h_a_l_o_w_]   _TT_hh_oo_mm_aa_ss_ _KK_aa_rr_aa_oo_uu_zz_ee_nn_ee    _cc_aa_ss_ee_yy_zz_aa_kk_22_44  _O_l_i_v_e_i_r_a_] _W_o_i_m_b_Ã_©_e_] _M_a_r_k_i_e_w_i_c_z_]
-   _JJ_oo_nn_nn_yy     _CC_hh_aa_rr_ll_ee_ss           _ð___             _ð___     _PP_rr_ii_ss_cc_ii_ll_aa   _AA_rr_tt_hh_uu_rr      _CC_hh_rr_ii_ss
- _SS_aa_uu_nn_dd_ee_rr_ss    _MM_aa_cc_hh_aa_ll_oo_ww                                    _OO_ll_ii_vv_ee_ii_rr_aa  _WW_oo_ii_mm_bb_?Ã_?©_ee  _MM_aa_rr_kk_ii_ee_ww_ii_cc_zz
-   _ð___        _ð___¬                                      _ð___ _ð___ _ð___ _ð___    _ð___
-                                                                     _ð___»
-                                                                    _â__ _ï_¸_
- _[_D_a_v_i_d_ _B_.  _[_J_e_r_r_y_J_i_a_]
-  _N_a_g_l_e_]     _JJ_ee_rr_rr_yy_JJ_ii_aa
- _DD_aa_vv_ii_dd_ _BB_..      _ð___»
-   _NN_aa_gg_ll_ee
-   _ð___
+_[_j_g_u_n_s_t_o_n_e_] _[_i_w_y_r_k_o_r_e_] _[_s_p_a_c_e_m_a_n_s_p_i_f_f_2_0_0_7_]   _[_L_u_k_e_ _H_s_i_a_o_]     _[_D_a_n_i_e_l  _[_E_v_g_e_n_i_y     _[_J_a_n_-
+ _jj_gg_uu_nn_ss_tt_oo_nn_ee   _ii_ww_yy_rr_kk_oo_rr_ee   _ss_pp_aa_cc_ee_mm_aa_nn_ss_pp_ii_ff_ff_22_00_00_77     _LL_uu_kk_ee_ _HH_ss_ii_aa_oo      _W_a_l_k_e_r_]  _L_u_p_a_s_h_i_n_]   _H_e_n_d_r_i_k
+   _ð___        _ð___»         _ð___ _ð__¤_            _ð___         _DD_aa_nn_ii_ee_ll    _EE_vv_gg_ee_nn_ii_yy    _E_w_e_r_s_]
+                                                              _WW_aa_ll_kk_ee_rr   _LL_uu_pp_aa_ss_hh_ii_nn  _JJ_aa_nn_--_HH_ee_nn_dd_rr_ii_kk
+                                                               _ð___      _ð___       _EE_ww_ee_rr_ss
+                                                                                    _ð___
+  _[_J_o_n_n_y     _[_C_h_a_r_l_e_s  _[_T_h_o_m_a_s_ _K_a_r_a_o_u_z_e_n_e_]   _[_c_a_s_e_y_z_a_k_2_4_]   _[_P_r_i_s_c_i_l_a   _[_A_r_t_h_u_r    _[_C_h_r_i_s
+ _S_a_u_n_d_e_r_s_]  _M_a_c_h_a_l_o_w_]   _TT_hh_oo_mm_aa_ss_ _KK_aa_rr_aa_oo_uu_zz_ee_nn_ee     _cc_aa_ss_ee_yy_zz_aa_kk_22_44    _O_l_i_v_e_i_r_a_]  _W_o_i_m_b_Ã_©_e_] _M_a_r_k_i_e_w_i_c_z_]
+   _JJ_oo_nn_nn_yy     _CC_hh_aa_rr_ll_ee_ss           _ð___              _ð___       _PP_rr_ii_ss_cc_ii_ll_aa    _AA_rr_tt_hh_uu_rr      _CC_hh_rr_ii_ss
+ _SS_aa_uu_nn_dd_ee_rr_ss    _MM_aa_cc_hh_aa_ll_oo_ww                                       _OO_ll_ii_vv_ee_ii_rr_aa   _WW_oo_ii_mm_bb_?Ã_?©_ee  _MM_aa_rr_kk_ii_ee_ww_ii_cc_zz
+   _ð___        _ð___¬                                         _ð___ _ð___  _ð___ _ð___    _ð___
+                                                                         _ð___»
+                                                                        _â__ _ï_¸_
+ _[_D_a_v_i_d_ _B_.  _[_J_e_r_r_y_J_i_a_]        _[_M_i_k_e_ _D_]          _[_D_a_r_i_o        _[_R_a_f_a_e_l   _[_A_n_d_r_e_w     _[_A_l_t_a_y
+  _N_a_g_l_e_]     _JJ_ee_rr_rr_yy_JJ_ii_aa          _MM_ii_kk_ee_ _DD         _Q_u_i_n_t_e_r_o_        _G_u_e_d_e_s_]   _L_i_n_z_i_e_]     _S_a_n_s_a_l_]
+ _DD_aa_vv_ii_dd_ _BB_..      _ð___»       _ð___» _ð___ _â__ _ï_¸_  _(_F_l_e_x_c_o_m_p_u_t_e_)_]    _RR_aa_ff_aa_ee_ll    _AA_nn_dd_rr_ee_ww       _AA_ll_tt_aa_yy
+   _NN_aa_gg_ll_ee                                    _DD_aa_rr_ii_oo_ _QQ_uu_ii_nn_tt_ee_rr_oo    _GG_uu_ee_dd_ee_ss    _LL_ii_nn_zz_ii_ee      _SS_aa_nn_ss_aa_ll
+   _ð___                                     _((_FF_ll_ee_xx_cc_oo_mm_pp_uu_tt_ee_))      _ð___»      _ð___»        _ð__¤_
+                                                 _ð___
+   _[_T_o_n_y      _[_X_u_a_n_     _[_C_h_r_i_s_t_i_a_n_ _R_i_e_d_e_l_]      _[_m_o_r_c_e_f_]   _[_a_l_e_j_a_n_d_r_o_-
+ _N_a_r_l_o_c_k_]   _(_S_e_a_n_)_ _H_u_]   _CC_hh_rr_ii_ss_tt_ii_aa_nn_ _RR_ii_ee_dd_ee_ll        _mm_oo_rr_cc_ee_ff      _y_o_u_s_e_f_]
+   _TT_oo_nn_yy       _XX_uu_aa_nn_             _ð___               _ð___     _aa_ll_ee_jj_aa_nn_dd_rr_oo_--
+  _NN_aa_rr_ll_oo_cc_kk   _((_SS_ee_aa_nn_))_ _HH_uu                                        _yy_oo_uu_ss_ee_ff
+ _ð___» _ð___     _ð___                                           _ð__¤_
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `autodoc_pydantic-2.0.1/pyproject.toml` & `autodoc_pydantic-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [tool.poetry]
 name = "autodoc_pydantic"
-version = "2.0.1"
+version = "2.1.0"
 description = "Seamlessly integrate pydantic models in your Sphinx documentation."
 authors = ["mansenfranzen <franz.woellert@gmail.com>"]
 packages = [{ include = "sphinxcontrib" }]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mansenfranzen/autodoc_pydantic"
 repository = "https://github.com/mansenfranzen/autodoc_pydantic"
 documentation = "https://github.com/mansenfranzen/autodoc_pydantic"
 keywords = ["sphinx", "pydantic", "autodoc", "documentation", "extension"]
 classifiers = [
+    "Framework :: Pydantic",
+    "Framework :: Pydantic :: 2",
     "Framework :: Sphinx :: Extension",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Software Development :: Documentation"
 ]
 include = ["sphinxcontrib/autodoc_pydantic/css/autodoc_pydantic.css"]
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<4.0.0"
+python = ">=3.8,<4.0.0"
 Sphinx = ">=4.0"
 pydantic = ">=2.0,<3.0.0"
 pydantic-settings = ">=2.0,<3.0.0"
 
 importlib-metadata = { version = ">1", markers = "python_version <= '3.8'" }
 
 sphinx-rtd-theme = { version = "^1.0", optional = true }
```

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/__init__.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,17 +73,14 @@
     """
 
     stem = "autodoc_pydantic_"
     add = app.add_config_value
     json_strategy = OptionsJsonErrorStrategy.WARN
     summary_list_order = OptionsSummaryListOrder.ALPHABETICAL
 
-    add(f'{stem}config_signature_prefix', "model", True, str)
-    add(f'{stem}config_members', True, True, bool)
-
     add(f'{stem}settings_show_json', True, True, bool)
     add(f'{stem}settings_show_json_error_strategy', json_strategy, True, str)
     add(f'{stem}settings_show_config_summary', True, True, bool)
     add(f'{stem}settings_show_validator_members', True, True, bool)
     add(f'{stem}settings_show_validator_summary', True, True, bool)
     add(f'{stem}settings_show_field_summary', True, True, bool)
     add(f'{stem}settings_summary_list_order', summary_list_order, True, str)
```

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,21 @@
     ClassDocumenter,
     AttributeDocumenter,
     Documenter
 )
 from sphinx.util.docstrings import prepare_docstring
 
 from sphinx.util.inspect import object_description
-from sphinx.util.typing import get_type_hints, stringify
+from sphinx.util.typing import get_type_hints
+
+try:
+    from sphinx.util.typing import stringify_annotation
+except ImportError:
+    # fall back to older name for older versions of Sphinx
+    from sphinx.util.typing import stringify as stringify_annotation
 
 from sphinxcontrib.autodoc_pydantic.directives.options.enums import (
     OptionsJsonErrorStrategy,
     OptionsFieldDocPolicy,
     OptionsSummaryListOrder
 )
 from sphinxcontrib.autodoc_pydantic.directives.options.definition import (
@@ -30,15 +36,15 @@
     OPTIONS_SETTINGS,
     OPTIONS_FIELD,
     OPTIONS_VALIDATOR,
     OPTIONS_MERGED
 )
 from sphinxcontrib.autodoc_pydantic.directives.templates import to_collapsable
 from sphinxcontrib.autodoc_pydantic.inspection import ModelInspector, \
-    ValidatorFieldMap
+    ValidatorFieldMap, ASTERISK_FIELD_NAME
 from sphinxcontrib.autodoc_pydantic.directives.options.composites import (
     AutoDocOptions
 )
 from sphinxcontrib.autodoc_pydantic.directives.utility import NONE, \
     intercept_type_annotations_py_gt_39
 
 try:
@@ -124,49 +130,51 @@
         """
 
         if self.options.is_true("field-swap-name-and-alias"):
             return self.inspect.fields.get_alias_or_name(field_name)
         else:
             return field_name
 
-    def get_filtered_member_names(self) -> Set[str]:
+    def get_non_inherited_members(self) -> Set[str]:
         """Return all member names of autodocumented object which are
         prefiltered to exclude inherited members.
 
         """
+        object_members = self._documenter.get_object_members(True)[1]
+        return {x.__name__ for x in object_members}
 
-        return {x[0] for x in self._documenter.get_object_members(True)[1]}
+    def get_base_class_names(self) -> List[str]:
+        return [x.__name__ for x in self.model.__mro__]
 
     def resolve_inherited_validator_reference(self, ref: str) -> str:
         """Provide correct validator reference in case validator is inherited
         and explicitly shown in docs via directive option
         `inherited-members`.
 
         More concretely, inherited validators are not shown from parent class
         unless directive option `inherited-members` is used. The validator
         references may either point to the parent class or the child class.
         This logic is implemented here.
 
         """
-
         ref_parts = ref.split(".")
         class_name = ref_parts[-2]
 
         # early exit if ref class name equals model name -> no inheritance
         if class_name == self.model.__name__:
             return ref
 
         validator_name = ref_parts[-1]
-        base_class_names = (x.__name__ for x in self.model.__mro__)
+        base_class_names = self.get_base_class_names()
 
         is_base_class = class_name in base_class_names
-        is_inherited_enabled = "inherited-members" in self._documenter.options
+        is_inherited = self.options.exists("inherited-members")
         is_member = validator_name in self.inspect.validators.names
 
-        if is_member and is_base_class and is_inherited_enabled:
+        if is_member and is_base_class and is_inherited:
             ref_parts[-2] = self.model.__name__
             return ".".join(ref_parts)
         else:
             return ref
 
 
 class PydanticModelDocumenter(ClassDocumenter):
@@ -207,44 +215,47 @@
         return is_val and is_model
 
     def __init__(self, *args: Any) -> None:
         super().__init__(*args)
         exclude_members = self.options.setdefault("exclude-members", set())
         exclude_members.add("model_fields")
         exclude_members.add("model_config")
+        exclude_members.add("model_computed_fields")
         self.pydantic = PydanticAutoDoc(self, is_child=False)
 
     def document_members(self, *args, **kwargs):
         """Modify member options before starting to document members.
 
         """
 
         self.pydantic.options.set_members_all()
         if self.options.get("undoc-members") is False:
             self.options.pop("undoc-members")
 
-        if self.pydantic.options.is_false("show-config-member", True):
-            self.hide_config_member()
-
         if self.pydantic.options.is_false("show-validator-members", True):
             self.hide_validator_members()
 
         if self.pydantic.options.is_true("hide-reused-validator", True):
             self.hide_reused_validators()
 
-        super().document_members(*args, **kwargs)
+        if self.pydantic.options.exists("inherited-members"):
+            self.hide_inherited_members()
 
-    def hide_config_member(self):
-        """Add `Config` to `exclude_members` option.
+        super().document_members(*args, **kwargs)
 
-        """
+    def hide_inherited_members(self):
+        """If inherited-members is set, make sure that these are excluded from
+        the class documenter, too"""
 
         exclude_members = self.options["exclude-members"]
-        exclude_members.add("Config")  # deprecated since pydantic v2
-        exclude_members.add("model_config")
+        squash_set = self.pydantic._documenter.options['inherited-members']
+        for cl in self.pydantic.model.__mro__:
+            if cl.__name__ in squash_set:
+                for item in dir(cl):
+                    exclude_members.add(item)
 
     def hide_validator_members(self):
         """Add validator names to `exclude_members`.
 
         """
         validators = self.pydantic.inspect.validators.names
         exclude_members = self.options["exclude-members"]
@@ -382,25 +393,26 @@
         `OptionsSummaryListOrder`.
 
         """
 
         sorted_members = self._sort_summary_list(members)
         return {name: idx for idx, name in enumerate(sorted_members)}
 
-    def _get_reference_sort_func(self) -> Callable:
+    def _get_reference_sort_func(self, references: List[ValidatorFieldMap]) -> Callable:  # noqa: E501
         """Helper function to create sorting function for instances of
         `ValidatorFieldMap` which first sorts by validator name and second by
         field name while respecting `OptionsSummaryListOrder`.
 
         This is used for validator summary section.
 
         """
 
-        all_validators = self.pydantic.inspect.validators.names
-        all_fields = self.pydantic.inspect.fields.names
+        all_fields = [ref.field_name for ref in references]
+        all_validators = [ref.validator_name for ref in references]
+
         idx_validators = self._get_idx_mappings(all_validators)
         idx_fields = self._get_idx_mappings(all_fields)
 
         def sort_func(reference: ValidatorFieldMap):
             return (
                 idx_validators.get(reference.validator_name, -1),
                 idx_fields.get(reference.field_name, -1)
@@ -410,16 +422,19 @@
 
     def _get_validator_summary_references(self) -> List[ValidatorFieldMap]:
         """Filter and sort validator-field mappings for validator summary
         section.
 
         """
 
-        references = self.pydantic.inspect.references.mappings
-        sort_func = self._get_reference_sort_func()
+        base_class_validators = self._get_base_model_validators()
+        inherited_validators = self._get_inherited_validators()
+        references = base_class_validators + inherited_validators
+
+        sort_func = self._get_reference_sort_func(references)
         sorted_references = sorted(references, key=sort_func)
 
         return sorted_references
 
     def _build_validator_summary_rest_line(
             self, reference: ValidatorFieldMap) -> str:
         """Generates reST line for validator-field mapping with references for
@@ -443,69 +458,137 @@
         """Adds summary section describing all validators with corresponding
         fields.
 
         """
 
         if not self.pydantic.inspect.validators:
             return
+
         sorted_references = self._get_validator_summary_references()
 
         source_name = self.get_sourcename()
         self.add_line(":Validators:", source_name)
         for ref in sorted_references:
             line = self._build_validator_summary_rest_line(ref)
             self.add_line(line, source_name)
 
         self.add_line("", source_name)
 
+    def _get_base_model_validators(self) -> List[str]:
+        """Return the validators on the model being documented"""
+
+        result = []
+
+        base_model_fields = set(self._get_base_model_fields())
+        base_object = self.object_name
+        references = self.pydantic.inspect.references.mappings
+
+        # The validator is considered part of the base_object if
+        # the field that is being validated is on the object being
+        # documented, if the method that is doing the validating
+        # is on that object (even if that method is validating
+        # an inherited field)
+        for ref in references:
+            if ref.field_name in base_model_fields:
+                result.append(ref)
+            else:
+                validator_class = ref.validator_ref.split(".")[-2]
+                if validator_class == base_object:
+                    result.append(ref)
+        return result
+
+    def _get_inherited_validators(self) -> List[str]:
+        """Return the validators on inherited fields to be documented,
+        if any"""
+
+        if not self.pydantic.options.exists("inherited-members"):
+            return []
+
+        squash_set = self.options['inherited-members']
+        references = self.pydantic.inspect.references.mappings
+        base_object = self.object_name
+        already_documented = self._get_base_model_validators()
+
+        result = []
+        for ref in references:
+            if ref in already_documented:
+                continue
+
+            validator_class = ref.validator_ref.split(".")[-2]
+            foreign_validator = validator_class != base_object
+            not_ignored = validator_class not in squash_set
+
+            if foreign_validator and not_ignored:
+                result.append(ref)
+
+        return result
+
     def add_field_summary(self):
         """Adds summary section describing all fields.
 
         """
-
         if not self.pydantic.inspect.fields:
             return
 
-        valid_fields = self._get_valid_fields()
+        base_class_fields = self._get_base_model_fields()
+        inherited_fields = self._get_inherited_fields()
+        valid_fields = base_class_fields + inherited_fields
+
         sorted_fields = self._sort_summary_list(valid_fields)
 
         source_name = self.get_sourcename()
         self.add_line(":Fields:", source_name)
         for field_name in sorted_fields:
             line = self._get_field_summary_line(field_name)
             self.add_line(line, source_name)
 
         self.add_line("", source_name)
 
-    def _get_valid_fields(self) -> List[str]:
+    def _get_base_model_fields(self) -> List[str]:
         """Returns all field names that are valid members of pydantic model.
 
         """
 
         fields = self.pydantic.inspect.fields.names
-        valid_members = self.pydantic.get_filtered_member_names()
+        valid_members = self.pydantic.get_non_inherited_members()
         return [field for field in fields if field in valid_members]
 
+    def _get_inherited_fields(self) -> List[str]:
+        """Return the inherited fields if inheritance is enabled"""
+
+        if not self.pydantic.options.exists("inherited-members"):
+            return []
+
+        fields = self.pydantic.inspect.fields.names
+        base_class_fields = self.pydantic.get_non_inherited_members()
+        return [field for field in fields if field not in base_class_fields]
+
     def _sort_summary_list(self, names: Iterable[str]) -> List[str]:
         """Sort member names according to given sort order
         `OptionsSummaryListOrder`.
 
         """
-
         sort_order = self.pydantic.options.get_value(name="summary-list-order",
                                                      prefix=True,
                                                      force_availability=True)
 
         if sort_order == OptionsSummaryListOrder.ALPHABETICAL:
             def sort_func(name: str):
                 return name
         elif sort_order == OptionsSummaryListOrder.BYSOURCE:
             def sort_func(name: str):
-                name_with_class = f"{self.object_name}.{name}"
-                return self.analyzer.tagorder.get(name_with_class)
+                if name in self.analyzer.tagorder:
+                    return self.analyzer.tagorder.get(name)
+                for base in self.pydantic.get_base_class_names():
+                    name_with_class = f"{base}.{name}"
+                    if name_with_class in self.analyzer.tagorder:
+                        return self.analyzer.tagorder.get(name_with_class)
+                # a pseudo-field name used by root validators
+                if name == ASTERISK_FIELD_NAME:
+                    return -1
         else:
             raise ValueError(
                 f"Invalid value `{sort_order}` provided for "
                 f"`summary_list_order`. Valid options are: "
                 f"{OptionsSummaryListOrder.values()}")
 
         return sorted(names, key=sort_func)
@@ -525,15 +608,15 @@
         """Get proper string representation of type for given `member_nane`
         relying on sphinx functionality.
 
         """
 
         type_aliases = self.config.autodoc_type_aliases
         annotations = get_type_hints(self.object, None, type_aliases)
-        return stringify(annotations.get(field_name, ""))
+        return stringify_annotation(annotations.get(field_name, ""))
 
     @staticmethod
     def _convert_json_schema_to_rest(schema: Dict) -> List[str]:
         """Convert model's schema dict into reST.
 
         """
         schema = json.dumps(schema, default=str, indent=3)
@@ -566,14 +649,18 @@
     pyautodoc_set_default_option = (
         "member-order",
         "undoc-members"
     )
 
     pyautodoc_prefix = "settings"
 
+    def __init__(self, *args: Any) -> None:
+        super().__init__(*args)
+        self.options["exclude-members"].add("settings_customise_sources")
+
     @classmethod
     def can_document_member(cls,
                             member: Any,
                             membername: str,
                             isattr: bool,
                             parent: Any) -> bool:
         """Filter only pydantic models.
```

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/directives.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/directives.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/composites.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/options/composites.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,17 +108,19 @@
         if prefix:
             name = f"{self.parent.pyautodoc_prefix}-{name}"
 
         if name in self.parent.options:
             return self.parent.options[name]
         elif force_availability or self.is_available(name):
             return self.get_app_cfg_by_name(name)
+        else:
+            return NONE
 
     def is_false(self, name: str, prefix: bool = False) -> bool:
-        """Get option value for given `name`. First, looks for explicit
+        """Check if option with `name` is False. First, looks for explicit
         directive option values (e.g. :member-order:) which have highest
         priority. Second, if no directive option is given, get the default
         option value provided via the app environment configuration.
 
         Enforces result to be either True or False.
 
         Parameters
@@ -129,15 +131,15 @@
             If True, add `pyautodoc_prefix` to name.
 
         """
 
         return self.get_value(name=name, prefix=prefix) is False
 
     def is_true(self, name: str, prefix: bool = False) -> bool:
-        """Get option value for given `name`. First, looks for explicit
+        """Check if option with `name` is True. First, looks for explicit
         directive option values (e.g. :member-order:) which have highest
         priority. Second, if no directive option is given, get the default
         option value provided via the app environment configuration.
 
         Enforces result to be either True or False.
 
         Parameters
@@ -147,14 +149,33 @@
         prefix: bool
             If True, add `pyautodoc_prefix` to name.
 
         """
 
         return self.get_value(name=name, prefix=prefix) is True
 
+    def exists(self, name: str, prefix: bool = False) -> bool:
+        """Check if option with `name` is set. First, looks for explicit
+        directive option values (e.g. :member-order:) which have highest
+        priority. Second, if no directive option is given, get the default
+        option value provided via the app environment configuration.
+
+        Enforces result to be either True or False.
+
+        Parameters
+        ----------
+        name: str
+            Name of the option.
+        prefix: bool
+            If True, add `pyautodoc_prefix` to name.
+
+        """
+
+        return self.get_value(name=name, prefix=prefix) is not NONE
+
     def set_default_option(self, name: str):
         """Set default option value for given `name` from app environment
         configuration if an explicit directive option was not provided.
 
         Parameters
         ----------
         name: str
```

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/definition.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/options/definition.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/validators.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/options/validators.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/templates.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/templates.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/utility.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/directives/utility.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/events.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/events.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/inspection.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/inspection.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/utility.py` & `autodoc_pydantic-2.1.0/sphinxcontrib/autodoc_pydantic/utility.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.1/PKG-INFO` & `autodoc_pydantic-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
-Name: autodoc-pydantic
-Version: 2.0.1
+Name: autodoc_pydantic
+Version: 2.1.0
 Summary: Seamlessly integrate pydantic models in your Sphinx documentation.
 Home-page: https://github.com/mansenfranzen/autodoc_pydantic
 License: MIT
 Keywords: sphinx,pydantic,autodoc,documentation,extension
 Author: mansenfranzen
 Author-email: franz.woellert@gmail.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0.0
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 2
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: erdantic
 Provides-Extra: test
 Requires-Dist: Sphinx (>=4.0)
@@ -37,21 +40,21 @@
 Project-URL: Documentation, https://github.com/mansenfranzen/autodoc_pydantic
 Project-URL: Repository, https://github.com/mansenfranzen/autodoc_pydantic
 Description-Content-Type: text/markdown
 
 ![Autodoc Pydantic](https://raw.githubusercontent.com/mansenfranzen/autodoc_pydantic/main/docs/source/material/logo_black.svg)
 
 [![PyPI version](https://img.shields.io/pypi/v/autodoc_pydantic?style=for-the-badge)](https://pypi.org/project/autodoc-pydantic/)
-![Python](https://img.shields.io/badge/python-3.7+-blue.svg?style=for-the-badge)
+![Python](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge)
 
 [![Master](https://img.shields.io/github/actions/workflow/status/mansenfranzen/autodoc_pydantic/tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/autodoc_pydantic/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic)
 
 [![Downloads](https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-badge)](https://pypistats.org/packages/autodoc-pydantic)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-37-orange.svg?style=for-the-badge)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-47-orange.svg?style=for-the-badge)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 You love [pydantic](https://pydantic-docs.helpmanual.io/) ❤ and you want to
 document your models and configuration settings with [sphinx](https://www.sphinx-doc.org/en/master/)?
 
 Perfect, let's go. But wait, sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html)
@@ -65,15 +68,16 @@
 - 🔗 adds hyperlinks between validators and corresponding fields
 - 📃 includes collapsable model json schema
 - 🏄 natively integrates with autodoc and autosummary extensions
 - 📎 defines explicit pydantic prefixes for models, settings, fields, validators and model config
 - 📋 shows summary section for model configuration, fields and validators
 - 👀 hides overloaded and redundant model class signature
 - 🔱 visualizes entity-relationship-diagrams for class hierarchies
-- 🍀 Supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0`
+- 🔨 allows complete configurability on global and per-model level
+- 🍀 supports `pydantic >= 1.5.0` and `sphinx >= 4.0.0`
 
 ## Documentation
 
 For more details, please visit the official [documentation](https://autodoc-pydantic.readthedocs.io/en/stable/):
 
 - [Installation](https://autodoc-pydantic.readthedocs.io/en/stable/users/installation.html)
 - [Configuration](https://autodoc-pydantic.readthedocs.io/en/stable/users/configuration.html)
@@ -143,14 +147,26 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/PriOliveira"><img src="https://avatars.githubusercontent.com/u/13801839?v=4?s=100" width="100px;" alt="Priscila Oliveira"/><br /><sub><b>Priscila Oliveira</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3APriOliveira" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-PriOliveira" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/awoimbee"><img src="https://avatars.githubusercontent.com/u/22431493?v=4?s=100" width="100px;" alt="Arthur Woimbée"/><br /><sub><b>Arthur Woimbée</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3Aawoimbee" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-awoimbee" title="User Testing">📓</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/effigies"><img src="https://avatars.githubusercontent.com/u/83442?v=4?s=100" width="100px;" alt="Chris Markiewicz"/><br /><sub><b>Chris Markiewicz</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Aeffigies" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nagledb"><img src="https://avatars.githubusercontent.com/u/727435?v=4?s=100" width="100px;" alt="David B. Nagle"/><br /><sub><b>David B. Nagle</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Anagledb" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jerryjiahaha"><img src="https://avatars.githubusercontent.com/u/3163720?v=4?s=100" width="100px;" alt="JerryJia"/><br /><sub><b>JerryJia</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=jerryjiahaha" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/devmonkey22"><img src="https://avatars.githubusercontent.com/u/5084545?v=4?s=100" width="100px;" alt="Mike D"/><br /><sub><b>Mike D</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=devmonkey22" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Adevmonkey22" title="Bug reports">🐛</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=devmonkey22" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/daquinteroflex"><img src="https://avatars.githubusercontent.com/u/149674618?v=4?s=100" width="100px;" alt="Dario Quintero (Flexcompute)"/><br /><sub><b>Dario Quintero (Flexcompute)</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3Adaquinteroflex" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rafa-guedes"><img src="https://avatars.githubusercontent.com/u/7799184?v=4?s=100" width="100px;" alt="Rafael Guedes"/><br /><sub><b>Rafael Guedes</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=rafa-guedes" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/caerulescens"><img src="https://avatars.githubusercontent.com/u/29284192?v=4?s=100" width="100px;" alt="Andrew Linzie"/><br /><sub><b>Andrew Linzie</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=caerulescens" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tasansal"><img src="https://avatars.githubusercontent.com/u/13684161?v=4?s=100" width="100px;" alt="Altay Sansal"/><br /><sub><b>Altay Sansal</b></sub></a><br /><a href="#ideas-tasansal" title="Ideas, Planning, & Feedback">🤔</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.git-pull.com"><img src="https://avatars.githubusercontent.com/u/26336?v=4?s=100" width="100px;" alt="Tony Narlock"/><br /><sub><b>Tony Narlock</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=tony" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=tony" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://huxuan.org/"><img src="https://avatars.githubusercontent.com/u/726061?v=4?s=100" width="100px;" alt="Xuan (Sean) Hu"/><br /><sub><b>Xuan (Sean) Hu</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Ahuxuan" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Cielquan"><img src="https://avatars.githubusercontent.com/u/43916661?v=4?s=100" width="100px;" alt="Christian Riedel"/><br /><sub><b>Christian Riedel</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3ACielquan" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/morcef"><img src="https://avatars.githubusercontent.com/u/15701746?v=4?s=100" width="100px;" alt="morcef"/><br /><sub><b>morcef</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Amorcef" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alejandro-yousef"><img src="https://avatars.githubusercontent.com/u/93203189?v=4?s=100" width="100px;" alt="alejandro-yousef"/><br /><sub><b>alejandro-yousef</b></sub></a><br /><a href="#ideas-alejandro-yousef" title="Ideas, Planning, & Feedback">🤔</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```


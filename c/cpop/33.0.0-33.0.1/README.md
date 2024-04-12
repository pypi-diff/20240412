# Comparing `tmp/cpop-33.0.0.tar.gz` & `tmp/cpop-33.0.1.tar.gz`

## Comparing `cpop-33.0.0.tar` & `cpop-33.0.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-33.0.0/.coveragerc
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 cpop-33.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/Makefile
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/make.bat
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/outline.rst
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/index.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/releases/32.rst
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/app_merging.rst
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/conf.rst
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/conf_integrate.rst
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/contracts.rst
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/dyne_name.rst
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/func_alias.rst
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/glossary.rst
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/hub_overview.rst
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/ideas_that_were_not_used.rst
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/learning.rst
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/pop.rst
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/pre_contract_returns.rst
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/story.rst
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/sub_patterns.rst
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/subs_overview.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/topics/virtual.rst
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-33.0.0/docs/source/tutorial/quickstart.rst
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/data.pyx
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/dirs.pyx
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/exc.pyx
--rw-r--r--   0        0        0    24958 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/hub.pyx
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/loader.pyx
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/ref.pyx
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/scanner.pyx
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 cpop-33.0.0/src/cpop/verify.pyx
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/config.yaml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/log/basic.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/log/init.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/log/timed_rolling.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/log/contracts/init.py
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/mods/config.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/mods/task.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-33.0.0/src/pop/mods/test.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/contracts/test.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/coro/contracts/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/__init__.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_cli.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_config.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_cpop.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_dyne.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_fail.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_hub.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_log.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_ref.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/proc.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/vtrue.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-33.0.0/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-33.0.0/.gitignore
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 cpop-33.0.0/README.rst
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 cpop-33.0.0/pyproject.toml
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 cpop-33.0.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-33.0.1/.coveragerc
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 cpop-33.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/Makefile
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/make.bat
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/outline.rst
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/releases/32.rst
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/app_merging.rst
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/conf.rst
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/conf_integrate.rst
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/contracts.rst
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/dyne_name.rst
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/func_alias.rst
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/glossary.rst
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/hub_overview.rst
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/ideas_that_were_not_used.rst
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/learning.rst
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/pop.rst
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/pre_contract_returns.rst
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/story.rst
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/sub_patterns.rst
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/subs_overview.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/topics/virtual.rst
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-33.0.1/docs/source/tutorial/quickstart.rst
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/data.pyx
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/dirs.pyx
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/exc.pyx
+-rw-r--r--   0        0        0    25026 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/hub.pyx
+-rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/loader.pyx
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/ref.pyx
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/scanner.pyx
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 cpop-33.0.1/src/cpop/verify.pyx
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/config.yaml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/log/basic.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/log/init.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/log/timed_rolling.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/log/contracts/init.py
+-rw-r--r--   0        0        0     9631 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/mods/config.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-33.0.1/src/pop/mods/test.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/contracts/test.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/__init__.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_cli.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_config.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_cpop.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_dyne.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_hub.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_log.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_ref.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/proc.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-33.0.1/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-33.0.1/.gitignore
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 cpop-33.0.1/README.rst
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 cpop-33.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 cpop-33.0.1/PKG-INFO
```

### Comparing `cpop-33.0.0/.pre-commit-config.yaml` & `cpop-33.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/Makefile` & `cpop-33.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/make.bat` & `cpop-33.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/outline.rst` & `cpop-33.0.1/docs/outline.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/conf.py` & `cpop-33.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/index.rst` & `cpop-33.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/app_merging.rst` & `cpop-33.0.1/docs/source/topics/app_merging.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/conf.rst` & `cpop-33.0.1/docs/source/topics/conf.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/conf_integrate.rst` & `cpop-33.0.1/docs/source/topics/conf_integrate.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/contracts.rst` & `cpop-33.0.1/docs/source/topics/contracts.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/dyne_name.rst` & `cpop-33.0.1/docs/source/topics/dyne_name.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/func_alias.rst` & `cpop-33.0.1/docs/source/topics/func_alias.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/glossary.rst` & `cpop-33.0.1/docs/source/topics/glossary.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/hub_overview.rst` & `cpop-33.0.1/docs/source/topics/hub_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/ideas_that_were_not_used.rst` & `cpop-33.0.1/docs/source/topics/ideas_that_were_not_used.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/learning.rst` & `cpop-33.0.1/docs/source/topics/learning.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/pop.rst` & `cpop-33.0.1/docs/source/topics/pop.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/pre_contract_returns.rst` & `cpop-33.0.1/docs/source/topics/pre_contract_returns.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/story.rst` & `cpop-33.0.1/docs/source/topics/story.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/sub_patterns.rst` & `cpop-33.0.1/docs/source/topics/sub_patterns.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/subs_overview.rst` & `cpop-33.0.1/docs/source/topics/subs_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/topics/virtual.rst` & `cpop-33.0.1/docs/source/topics/virtual.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/docs/source/tutorial/quickstart.rst` & `cpop-33.0.1/docs/source/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/cpop/contract.pyx` & `cpop-33.0.1/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/cpop/data.pyx` & `cpop-33.0.1/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/cpop/dirs.pyx` & `cpop-33.0.1/src/cpop/dirs.pyx`

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,119 @@
 """
 Find directories
 """
 
 import importlib.resources
 import os
-import pathlib
+import aiopath
 import sys
 from collections import defaultdict
 from collections.abc import Iterable
 from typing import Any
 
 import cpop.data
 import yaml
 
 
-def dir_list(pypath: list[str] = None, static: list[str] = None) -> list[pathlib.Path]:
+async def dir_list(pypath: list[str] = None, static: list[str] = None) -> list[aiopath.Path]:
     """
     Return the directories to look for modules in, pypath specifies files
     relative to an installed python package, static is for static dirs
     :param pypath: One or many python paths which will be imported
     :param static: Directories that can be explicitly passed
     """
     ret = set()
     if pypath:
         for path in pypath:
             mod = importlib.import_module(path)
             for m_path in mod.__path__:
                 # If we are inside of an executable the path will be different
-                ret.add(pathlib.Path(m_path))
+                ret.add(aiopath.Path(m_path))
     if static:
-        ret.update(pathlib.Path(dir_) for dir_ in static)
+        ret.update(aiopath.Path(dir_) for dir_ in static)
     return sorted(ret)
 
 
-def inline_dirs(dirs: Iterable[str], subdir: str) -> list[pathlib.Path]:
+async def inline_dirs(dirs: Iterable[str], subdir: str) -> list[aiopath.Path]:
     """
     Look for the named subdir in the list of dirs
     :param dirs: The names of configured dynamic dirs
     :param subdir: The name of the subdir to check for in the list of dynamic dirs
     :return An extended list of dirs that includes the found subdirs
     """
     ret = set()
     for dir_ in dirs:
-        check = pathlib.Path(dir_) / subdir
-        if check.is_dir():
+        check = aiopath.Path(dir_) / subdir
+        if await check.is_dir():
             ret.add(check)
     return sorted(ret)
 
 
-def dynamic_dirs():
+async def dynamic_dirs():
     """
     Iterate over the available python package imports and look for configured
     dynamic dirs in pyproject.toml
     """
     dirs = set()
     for dir_ in sys.path:
         if not dir_:
             continue
-        path = pathlib.Path(dir_)
-        if not path.is_dir():
+        path = aiopath.Path(dir_)
+        if not await path.is_dir():
             continue
-        for sub in os.listdir(dir_):
+        async for sub in path.iterdir():
             full = path / sub
-            if sub.endswith(".egg-link"):
-                with open(full) as rfh:
-                    dirs.add(pathlib.Path(rfh.read().strip()))
-            elif full.is_dir():
+            if str(sub).endswith(".egg-link"):
+                async with full.open() as rfh:
+                    dirs.add(aiopath.Path(await rfh.read().strip()))
+            elif await full.is_dir():
                 dirs.add(full)
 
     # Set up the _dynamic return
     ret = cpop.data.NamespaceDict(
         dyne=cpop.data.NamespaceDict(),
         config=cpop.data.NamespaceDict(),
         imports=cpop.data.NamespaceDict(),
     )
 
     # Iterate over namespaces in sys.path
     for dir_ in dirs:
         config_file = dir_ / "config.yaml"
         try:
-            if not config_file.is_file():
+            if not await config_file.is_file():
                 continue
         except Exception:
             continue
-        dynes, configs, imports = parse_config(config_file)
+        dynes, configs, imports = await parse_config(config_file)
         if dynes:
             cpop.data.update(ret.dyne, dynes, merge_lists=True)
         if configs:
             cpop.data.update(ret.config, configs, merge_lists=True)
         if imports:
             cpop.data.update(ret.imports, imports)
 
     return ret
 
 
-def parse_config(
+async def parse_config(
     config_file
 ) -> tuple[dict[str, object], dict[str, object], set[str]]:
     dyne = defaultdict(lambda: cpop.data.NamespaceDict(paths=set()))
     config = cpop.data.NamespaceDict(
         config=cpop.data.NamespaceDict(),
         cli_config=cpop.data.NamespaceDict(),
         subcommands=cpop.data.NamespaceDict(),
     )
     imports = cpop.data.NamespaceDict()
 
-    config_file = pathlib.Path(config_file)
-    if not config_file.is_file():
+    config_file = aiopath.Path(config_file)
+    if not await config_file.is_file():
         return dyne, config, imports
-    with open(config_file) as f:
-        pop_config = yaml.safe_load(f) or {}
+    async with config_file.open('rb') as f:
+        pop_config = yaml.safe_load(await f.read()) or {}
 
     # Gather dynamic namespace paths for this import
     for name, paths in pop_config.get("dyne", {}).items():
         for path in paths:
             ref = config_file.parent / path.replace(".", os.sep)
             dyne[name]["paths"].add(ref)
```

### Comparing `cpop-33.0.0/src/cpop/exc.pyx` & `cpop-33.0.1/src/cpop/exc.pyx`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/cpop/hub.pyx` & `cpop-33.0.1/src/cpop/hub.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
             await self._subs["pop"]._load_all()
 
         self._load_all_dynes = load_all_dynes
         self._load_all_subdirs = load_all_subdirs
         self._recurse_subdirs = recurse_subdirs
         if self._load_all_dynes:
-            self._scan_dynamic()
+            await self._scan_dynamic()
             await self._load_all()
 
             if load_config:
                 # Overwrite opt with config data
                 self._opt = await self.pop.config.load(cli=cli, **self._dynamic.config)
 
         # Set up a logger
@@ -199,15 +199,15 @@
         Start a task that will be automatically awaited
 
         coro: An unscheduled coroutine object to run
         cb_coro: An unscheduled coroutine to run when the main coroutine completes
         """
         hub._task_count += 1
 
-        task = hub.lib.asyncio.create_task(coro)
+        task = asyncio.create_task(coro)
 
         def _callback(task):
             hub._tasks.put_nowait({"task": task, "cb": cb_coro})
 
         task.add_done_callback(_callback)
         return task
 
@@ -229,15 +229,15 @@
             OPT=cpop.data.unfreeze(self._opt),
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
             attrs=attrs,
         )
         return state
 
     def __reduce__(self):
-        return Hub, (), self.__getstate__()
+        return AsyncHub, (), self.__getstate__()
 
     def __setstate__(self, state: dict):
         subs = state["subs"]
         opt = state["OPT"]
         aliases = state["aliases"]
 
         for subname, modname in state["imports"].items():
@@ -256,20 +256,20 @@
                 sub = self._subs[name]
             else:
                 sub = Sub(hub=self, root=self, **data["init_kwargs"])
                 self._subs[name] = sub
 
             sub.__setstate__(data)
 
-    def _scan_dynamic(self):
+    async def _scan_dynamic(self):
         """
         Refresh the dynamic roots data used for loading app merge module roots
         """
         self._clear()
-        self._dynamic = cpop.dirs.dynamic_dirs()
+        self._dynamic = await cpop.dirs.dynamic_dirs()
         self._dscan = True
 
     def __getattr__(self, item: str):
         if item.startswith("_"):
             return self.__getattribute__(item)
         try:
             return self[item]
@@ -378,32 +378,32 @@
         self._is_contract = is_contract
         self._process_init = init
 
     async def __ainit__(self, *args, **kwargs):
         await self._prepare()
 
     async def _prepare(self):
-        self._dirs = cpop.dirs.dir_list(
+        self._dirs = await cpop.dirs.dir_list(
             self._pypath,
             self._static,
         )
 
         if self._dyne_name:
-            self._load_dyne()
-        self._contract_dirs = cpop.dirs.dir_list(
+            await self._load_dyne()
+        self._contract_dirs = await cpop.dirs.dir_list(
             self._contracts_pypath,
             self._contracts_static,
         )
-        self._contract_dirs.extend(cpop.dirs.inline_dirs(self._dirs, "contracts"))
-        self._recursive_contract_dirs = cpop.dirs.dir_list(
+        self._contract_dirs.extend(await cpop.dirs.inline_dirs(self._dirs, "contracts"))
+        self._recursive_contract_dirs = await cpop.dirs.dir_list(
             [],
             self._recursive_contracts_static,
         )
         self._recursive_contract_dirs.extend(
-            cpop.dirs.inline_dirs(self._dirs, "recursive_contracts")
+            await cpop.dirs.inline_dirs(self._dirs, "recursive_contracts")
         )
 
         self._contract_subs = []
         for i in range(len(self._contract_dirs)):
             sub = await AsyncSub(
                 hub=self._hub,
                 subname=f"{self._subname}._contract_subs[{i}]",
@@ -439,20 +439,20 @@
             self._recursive_contract_subs = getattr(
                 self._root, "_recursive_contract_subs", []
             )
 
         self._name_root = self._load_name_root()
         self._scan = cpop.scanner.scan(self._dirs)
 
-    def _load_dyne(self):
+    async def _load_dyne(self):
         """
         Load up the dynamic dirs for this sub
         """
         if not self._hub._dscan:
-            self._hub._scan_dynamic()
+            await self._hub._scan_dynamic()
         for path in self._hub._dynamic.dyne.get(self._dyne_name, {}).get("paths", []):
             if path not in self._dirs:
                 self._dirs.append(path)
 
         self._clear()
 
     def _load_name_root(self):
@@ -486,15 +486,15 @@
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
             aliases=self._sub_alias,
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
             attrs=attrs,
         )
 
     def __reduce__(self):
-        return Sub, (), self.__getstate__()
+        return AsyncSub, (), self.__getstate__()
 
     def __setstate__(self, state: dict):
         """
         Only a hub can truly restore a sub because of their interdependency
         """
         subs = state["subs"]
         aliases = state["aliases"]
```

### Comparing `cpop-33.0.0/src/cpop/loader.pyx` & `cpop-33.0.1/src/cpop/loader.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -262,20 +262,22 @@
 
     def __getitem__(self, item: str):
         return self._attrs[item]
 
     def __setattr__(self, item: str, value):
         if item.startswith("_"):
             object.__setattr__(self, item, value)
+            return
         elif isinstance(value, types.FunctionType):
             self._funcs[item] = value
         elif isinstance(value, type):
             self._classes[item] = value
         else:
             self._vars[item] = value
+        self._attrs._clear()
 
     def __getstate__(self):
         return {
             "vars": {k: v for k, v in self._vars.items() if isinstance(v, BASE_TYPES)}
         }
 
     def __setstate__(self, state: dict[str, any]):
```

### Comparing `cpop-33.0.0/src/cpop/ref.pyx` & `cpop-33.0.1/src/cpop/ref.pyx`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/cpop/scanner.pyx` & `cpop-33.0.1/src/cpop/scanner.pyx`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/cpop/verify.pyx` & `cpop-33.0.1/src/cpop/verify.pyx`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/pop/config.yaml` & `cpop-33.0.1/src/pop/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -68,22 +68,22 @@
 dyne:
   log:
     - log
 
 # python imports to put on the hub for this plugin
 import:
   - aiologger.handlers.files
+  - aiopath
   - argparse
   - asyncio
   - collections
   - importlib
   - importlib.resources
   - logging
   - os
-  - pathlib
   - cpop.exc
   - cpop.contract
   - cpop.data
   - cpop.hub
   - signal
   - sys
   - yaml
```

### Comparing `cpop-33.0.0/src/pop/log/basic.py` & `cpop-33.0.1/src/pop/log/basic.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/pop/log/init.py` & `cpop-33.0.1/src/pop/log/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         levels = hub.lib.logging.getLevelNamesMapping()
         levels["TRACE"] = 5
         hub.lib.logging.addLevelName(5, "TRACE")
         hub.log.INT_LEVEL = levels[log_level.upper()]
 
     if log_plugin != "init":
         if log_file:
-            path = hub.lib.pathlib.Path(log_file).expanduser()
-            if not path.exists():
-                path.mkdir(parents=True, exist_ok=True)
+            path = await hub.lib.aiopath.Path(log_file).expanduser()
+            if not await path.exists():
+                await path.mkdir(parents=True, exist_ok=True)
             log_file = str(path)
         await hub.log[log_plugin].setup(log_file=log_file, **kwargs)
 
 
 async def trace(hub, msg: str, *args, **kwargs):
     ref, lineno = await hub.log.init.get_caller()
     logger = await hub.log.init.get_logger(ref)
```

### Comparing `cpop-33.0.0/src/pop/log/timed_rolling.py` & `cpop-33.0.1/src/pop/log/timed_rolling.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/pop/mods/config.py` & `cpop-33.0.1/src/pop/mods/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -241,33 +241,36 @@
 async def manage_paths(hub, cli: str, OPT: dict, root_dir: str):
     """
     If a root_dir has been specified, then we support rewriting roots, find all of the options
     for _dir, _path, and _file and update them
     """
     reroot = True if root_dir else False
     if not root_dir:
-        root_dir = hub.lib.pathlib.Path(hub.lib.os.sep)
+        root_dir = hub.lib.aiopath.Path(hub.lib.os.sep)
     if root_dir == hub.lib.os.sep:
         if hasattr(hub.lib.os, "geteuid") and hub.lib.os.geteuid() != 0 and reroot:
-            # Using pathlib.Path on all paths makes testing on multiple OSes much easier.
-            # Since we can just patch pathlib.Path to be pathlib.PureWindowsPath or pathlib.PurePosixPath
-            root_dir = hub.lib.pathlib.Path(hub.lib.os.path.expanduser("~")) / f".{cli}"
+            # Using aiopath.Path on all paths makes testing on multiple OSes much easier.
+            # Since we can just patch aiopath.Path to be aiopath.PureWindowsPath or aiopath.PurePosixPath
+            root_dir = (await hub.lib.aiopath.Path("~").expanduser()) / f".{cli}"
         else:
-            root_dir = hub.lib.pathlib.Path(root_dir)
+            root_dir = hub.lib.aiopath.Path(root_dir)
     else:
         return
 
     for namespace, args in OPT.items():
         for key, val in args.items():
             if key == "root_dir":
-                OPT[namespace][key] = root_dir
+                OPT[namespace][key] = str(root_dir)
                 continue
             try:
-                path = hub.lib.pathlib.Path(val)
-                if key.endswith(("_dir", "_path", "_file")) and path.is_absolute():
+                path = hub.lib.aiopath.Path(val)
+                if (
+                    key.endswith(("_dir", "_path", "_file"))
+                    and await path.is_absolute()
+                ):
                     # only update absolute paths for keys
                     #  ending in _dir, _path or _file
-                    if path.is_absolute():
+                    if await path.is_absolute():
                         # remove the root from the path, then join it to the main root
                         OPT[namespace][key] = root_dir.joinpath(*path.parts[1:])
             except TypeError:
                 continue
```

### Comparing `cpop-33.0.0/src/pop/mods/contract.py` & `cpop-33.0.1/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/pop/mods/sub.py` & `cpop-33.0.1/src/pop/mods/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/pop/mods/task.py` & `cpop-33.0.1/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/src/pop/mods/test.py` & `cpop-33.0.1/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/conftest.py` & `cpop-33.0.1/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import pathlib
 import sys
 import unittest.mock as mock
 
+import aiopath
 import cpop.hub
 import pytest
 
 
 @pytest.fixture()
 async def hub():
     yield await cpop.hub.AsyncHub(
@@ -15,20 +15,20 @@
         recurse_subdirs=False,
         logs=False,
         load_config=False,
     )
 
 
 @pytest.fixture(autouse=True, scope="session")
-def tpath():
-    code_dir = pathlib.Path(__file__).parent.parent.absolute()
-    assert code_dir.exists()
+async def tpath():
+    code_dir = await aiopath.Path(__file__).parent.parent.absolute()
+    assert await code_dir.exists()
 
     tpath_dir = code_dir / "tests" / "tpath"
-    assert tpath_dir.exists()
+    assert await tpath_dir.exists()
 
     NEW_PATH = [str(code_dir), str(tpath_dir)]
 
     for p in sys.path:
         if p not in NEW_PATH:
             NEW_PATH.append(p)
```

### Comparing `cpop-33.0.0/tests/contracts/ctx.py` & `cpop-33.0.1/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/contracts/many.py` & `cpop-33.0.1/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/contracts/test.py` & `cpop-33.0.1/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_basic.py` & `cpop-33.0.1/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_config.py` & `cpop-33.0.1/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_contract_ctx.py` & `cpop-33.0.1/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_fail.py` & `cpop-33.0.1/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_log.py` & `cpop-33.0.1/tests/func/test_log.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_no_raise_on_pre_failure.py` & `cpop-33.0.1/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_raise_on_pre_failure.py` & `cpop-33.0.1/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_ref.py` & `cpop-33.0.1/tests/func/test_ref.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/func/test_serial.py` & `cpop-33.0.1/tests/func/test_serial.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-33.0.1/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-33.0.1/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-33.0.1/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-33.0.1/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-33.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-33.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-33.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-33.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-33.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-33.0.1/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/mods/proc.py` & `cpop-33.0.1/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/mods/test.py` & `cpop-33.0.1/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/regression/contract_masking/test_contract_masking.py` & `cpop-33.0.1/tests/regression/contract_masking/test_contract_masking.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pathlib import Path
+from aiopath import Path
 
 current_dir = Path(globals()["__file__"]).parent
 
 
 async def test_masked_contracts(hub):
     await hub.pop.sub.add(
         pypath=["tests.regression.contract_masking.sub"],
```

### Comparing `cpop-33.0.0/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-33.0.1/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pathlib import Path
+from aiopath import Path
 
 
 current_dir = Path(globals()["__file__"]).parent
 
 
 async def test_repeated_recursive_contracts(hub):
     # A scenario similar to this could occur when recursive contracts
```

### Comparing `cpop-33.0.0/tests/tpath/cn/contract/test.py` & `cpop-33.0.1/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/unit/test_contract.py` & `cpop-33.0.1/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/tests/unit/test_sigs.py` & `cpop-33.0.1/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/.gitignore` & `cpop-33.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/README.rst` & `cpop-33.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-33.0.0/pyproject.toml` & `cpop-33.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "33.0.0"
+version = "33.0.1"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
@@ -17,14 +17,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
 dependencies = [
+    "aiopath",
     "aiofiles",
     "aiologger",
     "argparse",
     "PyYaml",
 ]
 
 [project.optional-dependencies]
@@ -78,11 +79,7 @@
 )
 '''
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 addopts = "--tb native --full-trace --color=yes -vv"
 asyncio_mode = "auto"
-
-
-[tool.cython]
-nthreads = 8
```

### Comparing `cpop-33.0.0/PKG-INFO` & `cpop-33.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 33.0.0
+Version: 33.0.1
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: aiofiles
 Requires-Dist: aiologger
+Requires-Dist: aiopath
 Requires-Dist: argparse
 Requires-Dist: pyyaml
 Provides-Extra: build
 Requires-Dist: cython; extra == 'build'
 Requires-Dist: hatch-cython; extra == 'build'
 Provides-Extra: cli
 Requires-Dist: pop-cli; extra == 'cli'
```


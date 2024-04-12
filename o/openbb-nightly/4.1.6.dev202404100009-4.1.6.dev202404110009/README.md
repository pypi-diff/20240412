# Comparing `tmp/openbb_nightly-4.1.6.dev202404100009.tar.gz` & `tmp/openbb_nightly-4.1.6.dev202404110009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-4.1.6.dev202404100009.tar", max compression
+gzip compressed data, was "openbb_nightly-4.1.6.dev202404110009.tar", max compression
```

## Comparing `openbb_nightly-4.1.6.dev202404100009.tar` & `openbb_nightly-4.1.6.dev202404110009.tar`

### file list

```diff
@@ -1,769 +1,773 @@
--rw-r--r--   0        0        0     6818 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/README.md
--rw-r--r--   0        0        0       19 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/__init__.py
--rw-r--r--   0        0        0      977 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1972 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0       34 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4206 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0       30 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7196 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/user.py
--rw-r--r--   0        0        0       30 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    17483 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2563 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5938 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2705 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2964 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8326 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2238 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      966 2024-04-10 00:09:21.398669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2247 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0       29 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0       38 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      302 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       99 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      551 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      252 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      458 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0     1035 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      398 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3875 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      856 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/custom_parameter.py
--rw-r--r--   0        0        0      502 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2233 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1912 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/fast_api_settings.py
--rw-r--r--   0        0        0     2032 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/features_keys.py
--rw-r--r--   0        0        0      694 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      542 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     4806 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9866 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1418 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      536 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0       37 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0      130 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     3898 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    17912 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/query.py
--rw-r--r--   0        0        0    24789 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/router.py
--rw-r--r--   0        0        0     2627 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10256 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3484 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3064 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0       30 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7759 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     2058 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1582 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1685 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    62954 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3077 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     2224 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5986 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1809 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/version.py
--rw-r--r--   0        0        0     2396 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0      465 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/annotated_result.py
--rw-r--r--   0        0        0     3494 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8881 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1368 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2581 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     9401 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0      630 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-04-10 00:09:21.402669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1288 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     1591 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      423 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2377 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1750 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      888 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1445 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      768 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      902 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2321 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
--rw-r--r--   0        0        0     2390 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
--rw-r--r--   0        0        0     2715 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6200 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-04-10 00:09:21.406669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1819 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3083 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3474 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     5013 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9293 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.410669 openbb_nightly-4.1.6.dev202404100009/core/openbb_core/py.typed
--rw-r--r--   0        0        0       34 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/commodity/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/commodity/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0       31 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0       34 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.414669 openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/py.typed
--rw-r--r--   0        0        0       32 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3848 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/py.typed
--rw-r--r--   0        0        0       15 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      372 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0       39 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/devtools/openbb_devtools/__init__.py
--rw-r--r--   0        0        0       37 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28152 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4117 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/utils.py
--rw-r--r--   0        0        0       32 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/__init__.py
--rw-r--r--   0        0        0     9797 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1754 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.418669 openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/py.typed
--rw-r--r--   0        0        0       19 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2336 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5816 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3493 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     3832 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3787 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0       28 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6060 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/py.typed
--rw-r--r--   0        0        0       32 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-10 00:09:21.422669 openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0       23 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/__init__.py
--rw-r--r--   0        0        0     4097 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/py.typed
--rw-r--r--   0        0        0       29 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/news/openbb_news/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/news/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/news/openbb_news/py.typed
--rw-r--r--   0        0        0       59 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8654 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10131 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14268 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1378 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10942 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0       35 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1889 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0       35 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0       43 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16765 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.426669 openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/py.typed
--rw-r--r--   0        0        0    57458 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/technical_router.py
--rw-r--r--   0        0        0     9791 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/builder.py
--rw-r--r--   0        0        0    16542 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/charting_router.py
--rw-r--r--   0        0        0       28 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-04-10 00:09:21.430669 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17442 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0       42 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     7188 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2554 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58384 2024-04-10 00:09:21.446668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228603 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0       30 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7185 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12351 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0     8398 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    18829 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3299 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5696 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6876 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3546 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    22283 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1437 2024-04-10 00:09:21.470668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   717892 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2246 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0     3666 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/query_params.py
--rw-r--r--   0        0        0     3204 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0    23603 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0      600 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0     1440 2024-04-10 00:09:21.474668 openbb_nightly-4.1.6.dev202404100009/openbb/__init__.py
--rw-r--r--   0        0        0  1186310 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/assets/reference.json
--rw-r--r--   0        0        0     2794 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/__extensions__.py
--rw-r--r--   0        0        0       50 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/__init__.py
--rw-r--r--   0        0        0     3340 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/crypto.py
--rw-r--r--   0        0        0     6589 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    11777 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/currency.py
--rw-r--r--   0        0        0     6481 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12160 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    53423 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/economy.py
--rw-r--r--   0        0        0    12674 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27673 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity.py
--rw-r--r--   0        0        0    18754 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2869 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    26106 2024-04-10 00:09:21.478668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    39105 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   169108 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30667 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26819 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3567 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    75052 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/etf.py
--rw-r--r--   0        0        0     4649 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    20027 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7155 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26900 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    11204 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11919 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/index.py
--rw-r--r--   0        0        0    15535 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/regulators.py
--rw-r--r--   0        0        0    16562 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/package/regulators_sec.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/openbb/py.typed
--rw-r--r--   0        0        0     1106 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0       28 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12452 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0       31 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      877 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0       32 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    14934 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-04-10 00:09:21.482668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9745 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/py.typed
--rw-r--r--   0        0        0       31 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      779 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0       30 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0       20 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0     1779 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2218 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-04-10 00:09:21.486668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6467 2024-04-10 00:09:21.490668 openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      895 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/__init__.py
--rw-r--r--   0        0        0       27 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0       24 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-04-10 00:09:21.494668 openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      716 2024-04-10 00:09:21.542667 openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-04-10 00:09:21.542667 openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-04-10 00:09:21.542667 openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3510 2024-04-10 00:09:21.542667 openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      538 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5553 2024-04-10 00:09:21.550667 openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0     1005 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/__init__.py
--rw-r--r--   0        0        0       30 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9573 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/py.typed
--rw-r--r--   0        0        0       29 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.606666 openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0     8255 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6022 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5202 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6763 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2774 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3607 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5050 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2064 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10603 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3903 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     5922 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3131 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3270 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/py.typed
--rw-r--r--   0        0        0       17 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4246 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.610666 openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0     3126 2024-04-10 00:09:21.630666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-04-10 00:09:21.630666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-04-10 00:09:21.630666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6656 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-04-10 00:09:21.634666 openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      988 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5269 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0       34 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0     5393 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22983 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-04-10 00:09:21.638666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     3273 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     8675 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2376 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7321 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8417 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     9694 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     5090 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3357 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8829 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6513 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     2550 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4006 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-04-10 00:09:21.642666 openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0     1840 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0       35 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3987 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6262 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     6111 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2274 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5090 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0       29 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-04-10 00:09:21.654666 openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      981 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8810 2024-04-10 00:09:21.658666 openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0     2100 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/__init__.py
--rw-r--r--   0        0        0       43 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6130 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6054 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     7020 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     5973 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3618 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/py.typed
--rw-r--r--   0        0        0       28 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3708 2024-04-10 00:09:21.662666 openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0     1562 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/__init__.py
--rw-r--r--   0        0        0       27 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0     8328 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     2615 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2720 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    32406 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2754 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2079 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2790 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3009 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1714 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/py.typed
--rw-r--r--   0        0        0       17 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    13896 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7434 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.678665 openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      512 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      677 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/stockgrid/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0     1120 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-10 00:09:21.770664 openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0     3319 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/__init__.py
--rw-r--r--   0        0        0       27 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5162 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4647 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8843 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5455 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12451 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4479 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3098 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10325 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6105 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5986 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/py.typed
--rw-r--r--   0        0        0       26 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38670 2024-04-10 00:09:21.782664 openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0     1241 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/__init__.py
--rw-r--r--   0        0        0       31 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6568 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9162 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10264 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/py.typed
--rw-r--r--   0        0        0       30 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-04-10 00:09:21.882663 openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      440 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     4606 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4616 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3719 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0     1044 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-04-10 00:09:21.886663 openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0     4232 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     1978 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5722 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10040 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4230 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6639 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-04-10 00:09:21.890663 openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0     6884 2024-04-10 00:09:31.614510 openbb_nightly-4.1.6.dev202404100009/pyproject.toml
--rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.6.dev202404100009/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/README.md
+-rw-r--r--   0        0        0       19 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4206 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7196 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    18495 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-04-11 00:09:31.763667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8326 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1035 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3875 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      856 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/custom_parameter.py
+-rw-r--r--   0        0        0      502 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2233 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1912 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/fast_api_settings.py
+-rw-r--r--   0        0        0     2032 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/hub/features_keys.py
+-rw-r--r--   0        0        0      694 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      542 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     4806 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9866 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1418 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0       37 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     3898 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    18892 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/query.py
+-rw-r--r--   0        0        0    24789 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10256 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3484 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3064 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7759 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2058 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1685 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    62954 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3077 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2224 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1368 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2581 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     9401 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0      630 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-04-11 00:09:31.767667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1288 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     1591 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      423 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2377 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1750 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      888 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1445 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      768 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      902 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2321 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     2390 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-04-11 00:09:31.771667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3083 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3474 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9681 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.775667 openbb_nightly-4.1.6.dev202404110009/core/openbb_core/py.typed
+-rw-r--r--   0        0        0       34 2024-04-11 00:09:31.779667 openbb_nightly-4.1.6.dev202404110009/extensions/commodity/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-11 00:09:31.779667 openbb_nightly-4.1.6.dev202404110009/extensions/commodity/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0       31 2024-04-11 00:09:31.779667 openbb_nightly-4.1.6.dev202404110009/extensions/crypto/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-11 00:09:31.779667 openbb_nightly-4.1.6.dev202404110009/extensions/crypto/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-04-11 00:09:31.779667 openbb_nightly-4.1.6.dev202404110009/extensions/crypto/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-11 00:09:31.779667 openbb_nightly-4.1.6.dev202404110009/extensions/crypto/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.779667 openbb_nightly-4.1.6.dev202404110009/extensions/crypto/openbb_crypto/py.typed
+-rw-r--r--   0        0        0       32 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/currency/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3848 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/currency/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/currency/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/currency/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/currency/openbb_currency/py.typed
+-rw-r--r--   0        0        0       15 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/derivatives/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/derivatives/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/derivatives/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/derivatives/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/derivatives/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0       39 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/devtools/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/econometrics/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/econometrics/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/econometrics/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/econometrics/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0       32 2024-04-11 00:09:31.783667 openbb_nightly-4.1.6.dev202404110009/extensions/economy/openbb_economy/__init__.py
+-rw-r--r--   0        0        0     9797 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/economy/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/economy/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/economy/openbb_economy/py.typed
+-rw-r--r--   0        0        0       19 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     3832 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0       28 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/etf/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/etf/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/etf/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6060 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/etf/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/etf/openbb_etf/py.typed
+-rw-r--r--   0        0        0       32 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-11 00:09:31.787667 openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0       23 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/index/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/index/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/index/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/index/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/index/openbb_index/py.typed
+-rw-r--r--   0        0        0       29 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/news/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/news/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/news/openbb_news/py.typed
+-rw-r--r--   0        0        0       59 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0       35 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/regulators/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/regulators/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/regulators/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/regulators/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/regulators/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0       43 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/technical/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16765 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/technical/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.791667 openbb_nightly-4.1.6.dev202404110009/extensions/technical/openbb_technical/py.typed
+-rw-r--r--   0        0        0    57462 2024-04-11 00:09:31.795667 openbb_nightly-4.1.6.dev202404110009/extensions/technical/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0    19791 2024-04-11 00:09:31.795667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-04-11 00:09:31.795667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/builder.py
+-rw-r--r--   0        0        0    37724 2024-04-11 00:09:31.795667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0       28 2024-04-11 00:09:31.795667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-04-11 00:09:31.795667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-04-11 00:09:31.811667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17442 2024-04-11 00:09:31.811667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-04-11 00:09:31.811667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0       42 2024-04-11 00:09:31.811667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     8068 2024-04-11 00:09:31.811667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2554 2024-04-11 00:09:31.811667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58496 2024-04-11 00:09:31.811667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228603 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0       30 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7185 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12381 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0       25 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
+-rw-r--r--   0        0        0     8555 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    19572 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3300 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5697 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6877 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3547 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    24971 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1437 2024-04-11 00:09:31.835667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   717892 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2246 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0    25617 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/query_params.py
+-rw-r--r--   0        0        0       32 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/styles/__init__.py
+-rw-r--r--   0        0        0      603 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/styles/colors.py
+-rw-r--r--   0        0        0     3462 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0     3339 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0    20197 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
+-rw-r--r--   0        0        0     2493 2024-04-11 00:09:31.839667 openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0     1440 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/__init__.py
+-rw-r--r--   0        0        0  1186310 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2794 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0       50 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6589 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    11777 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/currency.py
+-rw-r--r--   0        0        0     6481 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12160 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    53423 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/economy.py
+-rw-r--r--   0        0        0    12674 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27673 2024-04-11 00:09:31.843667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity.py
+-rw-r--r--   0        0        0    18754 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2869 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    26106 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    39105 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   169108 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30667 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26819 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3567 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    75052 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/etf.py
+-rw-r--r--   0        0        0     4649 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    20027 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7155 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26900 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    11204 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11919 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/index.py
+-rw-r--r--   0        0        0    15535 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/regulators.py
+-rw-r--r--   0        0        0    16562 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/package/regulators_sec.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/openbb/py.typed
+-rw-r--r--   0        0        0     1106 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12452 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5288 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      877 2024-04-11 00:09:31.847667 openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    14934 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6173 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9745 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/biztoc/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/biztoc/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/biztoc/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/biztoc/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/biztoc/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0     1779 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8338 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9657 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-04-11 00:09:31.851667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8336 2024-04-11 00:09:31.855667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-04-11 00:09:31.855667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4725 2024-04-11 00:09:31.855667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     5698 2024-04-11 00:09:31.855667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.855667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-04-11 00:09:31.855667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-04-11 00:09:31.855667 openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      895 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0       24 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-04-11 00:09:31.859667 openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      716 2024-04-11 00:09:31.907667 openbb_nightly-4.1.6.dev202404110009/providers/federal_reserve/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-04-11 00:09:31.907667 openbb_nightly-4.1.6.dev202404110009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-04-11 00:09:31.907667 openbb_nightly-4.1.6.dev202404110009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3510 2024-04-11 00:09:31.907667 openbb_nightly-4.1.6.dev202404110009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      538 2024-04-11 00:09:31.915667 openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-04-11 00:09:31.915667 openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-04-11 00:09:31.915667 openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-04-11 00:09:31.915667 openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-04-11 00:09:31.915667 openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0     1005 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9573 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8241 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    10989 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4379 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3878 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.971667 openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0     8255 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2955 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5909 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5904 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     2272 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6022 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5918 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6102 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5202 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6493 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3446 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3144 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6763 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2774 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3607 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4286 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5050 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5826 2024-04-11 00:09:31.975668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2064 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10603 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3903 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     5922 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3131 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4220 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3270 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:31.979668 openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0     3126 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2980 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6338 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6656 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2720 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-04-11 00:09:31.999668 openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      988 2024-04-11 00:09:32.003667 openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-11 00:09:32.003667 openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-11 00:09:32.003667 openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5269 2024-04-11 00:09:32.003667 openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-04-11 00:09:32.003667 openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-11 00:09:32.003667 openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0     5393 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22983 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     3273 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2211 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     8675 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2376 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4974 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7321 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29027 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8337 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8417 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     9694 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5090 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3676 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12539 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3357 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8829 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6513 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     2550 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-04-11 00:09:32.007668 openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0     1840 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6262 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5105 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5090 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-04-11 00:09:32.019667 openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      981 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0     2100 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     6961 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4600 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6130 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6054 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     6125 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     7020 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     5973 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3618 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-04-11 00:09:32.027668 openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0     1562 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0     8328 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     2615 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2720 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    32406 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2754 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2079 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2790 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3009 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1714 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    13896 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7434 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.043668 openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      512 2024-04-11 00:09:32.135668 openbb_nightly-4.1.6.dev202404110009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-11 00:09:32.135668 openbb_nightly-4.1.6.dev202404110009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-04-11 00:09:32.135668 openbb_nightly-4.1.6.dev202404110009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.135668 openbb_nightly-4.1.6.dev202404110009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-04-11 00:09:32.135668 openbb_nightly-4.1.6.dev202404110009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-11 00:09:32.135668 openbb_nightly-4.1.6.dev202404110009/providers/stockgrid/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-11 00:09:32.135668 openbb_nightly-4.1.6.dev202404110009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0     1120 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3651 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5295 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4662 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5323 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-11 00:09:32.139668 openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0     3319 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6302 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5162 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4647 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8843 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5455 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12451 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3638 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5085 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8409 2024-04-11 00:09:32.147668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9651 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10325 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5986 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5133 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-04-11 00:09:32.151668 openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0     1241 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6568 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9162 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10264 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-04-11 00:09:32.247668 openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      440 2024-04-11 00:09:32.251668 openbb_nightly-4.1.6.dev202404110009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     4606 2024-04-11 00:09:32.251668 openbb_nightly-4.1.6.dev202404110009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-04-11 00:09:32.251668 openbb_nightly-4.1.6.dev202404110009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3719 2024-04-11 00:09:32.251668 openbb_nightly-4.1.6.dev202404110009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0     1044 2024-04-11 00:09:32.251668 openbb_nightly-4.1.6.dev202404110009/providers/wsj/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-04-11 00:09:32.251668 openbb_nightly-4.1.6.dev202404110009/providers/wsj/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-04-11 00:09:32.251668 openbb_nightly-4.1.6.dev202404110009/providers/wsj/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-04-11 00:09:32.251668 openbb_nightly-4.1.6.dev202404110009/providers/wsj/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0     4232 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     1978 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2863 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3450 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3361 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6671 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5858 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3890 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10040 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4711 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4063 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10144 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4646 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4230 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6017 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6639 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-04-11 00:09:32.255668 openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0     6884 2024-04-11 00:09:43.727688 openbb_nightly-4.1.6.dev202404110009/pyproject.toml
+-rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.6.dev202404110009/PKG-INFO
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/README.md` & `openbb_nightly-4.1.6.dev202404110009/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/app_loader.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/app_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/auth/user.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/coverage.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/dependency/system.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/rest_api.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/commands.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/coverage.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/api/router/user.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/command_runner.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/command_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Command runner module."""
 
+# pylint: disable=R0903
+
 from copy import deepcopy
 from dataclasses import asdict, is_dataclass
 from datetime import datetime
 from inspect import Parameter, signature
 from sys import exc_info
 from time import perf_counter_ns
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type
@@ -189,14 +191,16 @@
             model.model_fields.get("extra_params", None), "annotation", None
         )
         if is_dataclass(annotation) and any(
             t is ExtraParams for t in getattr(annotation, "__bases__", [])
         ):
             valid = asdict(annotation())  # type: ignore
             for p in extra_params:
+                if "chart_params" in p:
+                    continue
                 if p not in valid:
                     warn(
                         message=f"Parameter '{p}' not found.",
                         category=OpenBBWarning,
                     )
 
     @staticmethod
@@ -221,23 +225,24 @@
                 Any if p.annotation is Parameter.empty else p.annotation,
                 ... if p.default is Parameter.empty else p.default,
             )
             for n, p in sig.parameters.items()
         }
         # We allow extra fields to return with model with 'cc: CommandContext'
         config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
-        ValidationModel = create_model(func.__name__, __config__=config, **fields)  # type: ignore
+        ValidationModel = create_model(func.__name__, __config__=config, **fields)  # type: ignore  # pylint: disable=C0103
         # Validate and coerce
         model = ValidationModel(**kwargs)
         ParametersBuilder._warn_kwargs(
             ParametersBuilder._as_dict(kwargs.get("extra_params", {})),
             ValidationModel,
         )
         return dict(model)
 
+    # pylint: disable=R0913
     @classmethod
     def build(
         cls,
         args: Tuple[Any, ...],
         execution_context: ExecutionContext,
         func: Callable,
         route: str,
@@ -270,22 +275,24 @@
         kwargs = cls.validate_kwargs(
             func=func,
             kwargs=kwargs,
         )
         return kwargs
 
 
+# pylint: disable=too-few-public-methods
 class StaticCommandRunner:
     """Static Command Runner."""
 
     @classmethod
     async def _command(
         cls,
         func: Callable,
         kwargs: Dict[str, Any],
+        show_warnings: bool = True,  # pylint: disable=unused-argument   # type: ignore
     ) -> OBBject:
         """Run a command and return the output."""
         obbject = await maybe_coroutine(func, **kwargs)
         obbject.provider = getattr(
             kwargs.get("provider_choices", None), "provider", None
         )
         return obbject
@@ -297,16 +304,34 @@
         **kwargs,
     ) -> None:
         """Create a chart from the command output."""
         if "charting" not in obbject.accessors:
             raise OpenBBError(
                 "Charting is not installed. Please install `openbb-charting`."
             )
-        obbject.charting.show(render=False, **kwargs)  # type: ignore
+        chart_params = {}
+        extra_params = kwargs.get("extra_params", {})
+
+        if hasattr(extra_params, "__dict__") and hasattr(extra_params, "chart_params"):
+            chart_params = kwargs["extra_params"].__dict__.get("chart_params", {})
+        elif isinstance(extra_params, dict) and "chart_params" in extra_params:
+            chart_params = kwargs["extra_params"].get("chart_params", {})
+
+        if "chart_params" in kwargs:
+            chart_params.update(kwargs.pop("chart_params", {}))
+
+        if "kwargs" in kwargs:
+            chart_params.update(kwargs.pop("kwargs", {}).get("chart_params", {}))
+
+        if chart_params:
+            kwargs.update(chart_params)
+
+        obbject.charting.show(render=False, **kwargs)
 
+    # pylint: disable=R0913, R0914
     @classmethod
     async def _execute_func(
         cls,
         route: str,
         args: Tuple[Any, ...],
         execution_context: ExecutionContext,
         func: Callable,
@@ -378,14 +403,15 @@
                         filename=w.filename,
                         lineno=w.lineno,
                         file=w.file,
                         line=w.line,
                     )
         return obbject
 
+    # pylint: disable=W0718
     @classmethod
     async def run(
         cls,
         execution_context: ExecutionContext,
         /,
         *args,
         **kwargs,
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/deprecation.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/deprecation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/extension_loader.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/handlers_manager.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/handlers_manager.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/logging_service.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/logging_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/models/logging_settings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/models/logging_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/utils/expired_files.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/utils/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/logs/utils/utils.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/logs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/abstract/singleton.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/abstract/singleton.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/charts/chart.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/charts/chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/charts/charting_settings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/credentials.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/credentials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/custom_parameter.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/custom_parameter.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/example.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/extension.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/fast_api_settings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/fast_api_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/features_keys.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/hub/features_keys.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/hub_session.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/hub/hub_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/hub/hub_user_settings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/hub/hub_user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/metadata.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/metadata.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/obbject.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/obbject.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/preferences.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/preferences.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/profile.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/system_settings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/system_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/model/user_settings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/provider_interface.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/provider_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,24 +160,44 @@
     def _merge_fields(
         current: DataclassField, incoming: DataclassField, query: bool = False
     ) -> DataclassField:
         """Merge 2 dataclass fields."""
         curr_name = current.name
         curr_type: Optional[Type] = current.annotation
         curr_desc = getattr(current.default, "description", "")
+        curr_json_schema_extra = getattr(current.default, "json_schema_extra", {})
 
         inc_type: Optional[Type] = incoming.annotation
         inc_desc = getattr(incoming.default, "description", "")
+        inc_json_schema_extra = getattr(incoming.default, "json_schema_extra", {})
 
         def split_desc(desc: str) -> str:
             """Split field description."""
             item = desc.split(" (provider: ")
             detail = item[0] if item else ""
             return detail
 
+        def merge_json_schema_extra(curr: dict, inc: dict) -> dict:
+            """Merge json schema extra."""
+            for key in curr.keys() & inc.keys():
+                # Merge keys that are in both dictionaries if both are lists
+                curr_value = curr[key]
+                inc_value = inc[key]
+                if isinstance(curr_value, list) and isinstance(inc_value, list):
+                    curr[key] = list(set(curr.get(key, []) + inc.get(key, [])))
+                    inc.pop(key)
+
+            # Add any remaining keys from inc to curr
+            curr.update(inc)
+            return curr
+
+        json_schema_extra: dict = merge_json_schema_extra(
+            curr=curr_json_schema_extra or {}, inc=inc_json_schema_extra or {}
+        )
+
         curr_detail = split_desc(curr_desc)
         inc_detail = split_desc(inc_desc)
 
         curr_title = getattr(current.default, "title", "")
         inc_title = getattr(incoming.default, "title", "")
         providers = ",".join([curr_title, inc_title])
         formatted_prov = providers.replace(",", ", ")
@@ -188,14 +208,15 @@
             new_desc = f"{curr_desc};\n    {inc_desc}"
 
         QF: Callable = Query if query else FieldInfo  # type: ignore[assignment]
         merged_default = QF(
             default=getattr(current.default, "default", None),
             title=providers,
             description=new_desc,
+            json_schema_extra=json_schema_extra,
         )
 
         merged_type: Optional[Type] = (
             Union[curr_type, inc_type]  # type: ignore[assignment]
             if curr_type != inc_type
             else curr_type
         )
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/query.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/router.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/auth_service.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/hub_service.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/service/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/system_service.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/service/system_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/service/user_service.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/service/user_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/account.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/account.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/app_factory.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/app_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/container.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/container.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/coverage.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/package_builder.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/package_builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/reference_loader.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/decorators.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/filters.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/utils/filters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/static/utils/linters.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/utils.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/app/version.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/env.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/env.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/data.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/fetcher.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/fetcher.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/provider.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/abstract/query_params.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/abstract/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/query_executor.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/registry.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/registry.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/registry_map.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/registry_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/analyst_search.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/available_indices.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_prices.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_reference.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/bond_trades.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cik_map.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_filings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_news.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/company_overview.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/compare_groups.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cot.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cot_search.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cp.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/cpi.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/crypto_search.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_info.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_peers.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_performance.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_screener.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_search.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_score.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/esg_sector.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/estr_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_historical.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_info.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_performance.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_search.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fed_projections.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ffrmc.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/forward_sales_estimates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fred_search.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/fred_series.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/futures_historical.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/gdp_real.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_employees.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/historical_splits.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/hqm.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/income_statement.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_historical.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_info.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_search.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_sectors.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/industry_pe.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/key_executives.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_indices.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_movers.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/money_measures.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/moody.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/options_chains.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/options_unusual.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/price_target.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/recent_performance.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/reported_financials.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/risk_premium.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/search_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sector_pe.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/short_volume.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/spot.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/tbffr.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/tmc.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/top_retail.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/unemployment.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/standard_models/world_news.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/standard_models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/client.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/utils/client.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/descriptions.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/core/openbb_core/provider/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/core/openbb_core/provider/utils/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Provider helpers."""
 
 import asyncio
+import os
 import re
-from datetime import date, datetime
+from datetime import date, datetime, timedelta, timezone
 from difflib import SequenceMatcher
 from functools import partial
 from inspect import iscoroutinefunction
 from typing import (
     Awaitable,
     Callable,
     List,
@@ -309,7 +310,14 @@
                 return dt >= start_date
             if end_date:
                 return dt <= end_date
             return True
         return False
 
     return list(filter(_filter, data))
+
+
+def safe_fromtimestamp(timestamp: float, tz: Optional[timezone] = None) -> datetime:
+    """datetime.fromtimestamp alternative which supports negative timestamps on Windows platform."""
+    if os.name == "nt" and timestamp < 0:
+        return datetime(1970, 1, 1, tzinfo=tz) + timedelta(seconds=timestamp)
+    return datetime.fromtimestamp(timestamp, tz)
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/commodity/openbb_commodity/commodity_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/commodity/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/crypto_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/crypto/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/crypto/openbb_crypto/price/price_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/crypto/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/currency_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/currency/openbb_currency/currency_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/currency/openbb_currency/price/price_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/currency/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/futures/futures_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/derivatives/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/derivatives/openbb_derivatives/options/options_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/derivatives/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/econometrics_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/econometrics/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/econometrics/openbb_econometrics/utils.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/econometrics/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/economy_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/economy/openbb_economy/economy_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/economy/openbb_economy/gdp/gdp_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/economy/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/calendar/calendar_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/compare/compare_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/compare/compare_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/darkpool/darkpool_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/discovery/discovery_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/equity_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/estimates/estimates_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/fundamental/fundamental_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/ownership/ownership_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/price/price_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/equity/openbb_equity/shorts/shorts_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/equity/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/discovery/discovery_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/etf/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/etf/openbb_etf/etf_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/etf/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/government/government_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/index_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/index/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/index/openbb_index/price/price_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/index/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/news/openbb_news/news_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/news/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/models.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/performance/performance_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/performance/performance_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/quantitative_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/statistics.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/quantitative/openbb_quantitative/stats/stats_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/quantitative/openbb_quantitative/stats/stats_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/cftc/cftc_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/regulators/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/regulators/openbb_regulators/sec/sec_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/regulators/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/technical/openbb_technical/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/extensions/technical/openbb_technical/technical_router.py` & `openbb_nightly-4.1.6.dev202404110009/extensions/technical/openbb_technical/technical_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,15 +485,15 @@
         APIEx(parameters={"length": 2, "data": APIEx.mock_data("timeseries")}),
     ],
 )
 def aroon(
     data: List[Data],
     index: str = "date",
     length: int = 25,
-    scalar: int = 100,
+    scalar: float = 100,
 ) -> OBBject[List[Data]]:
     """Calculate the Aroon Indicator.
 
     The word aroon is Sanskrit for "dawn's early light." The Aroon
     indicator attempts to show when a new trend is dawning. The indicator consists
     of two lines (Up and Down) that measure how long it has been since the highest
     high/lowest low has occurred within an n period range.
@@ -509,15 +509,15 @@
     ----------
     data : List[Data]
         List of data to be used for the calculation.
     index: str, optional
         Index column name to use with `data`, by default "date".
     length : int, optional
         Number of periods to be used for the calculation, by default 25.
-    scalar : int, optional
+    scalar : float, optional
         Scalar to be used for the calculation, by default 100.
 
     Returns
     -------
     OBBject[List[Data]]
         The calculated data.
     """
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/builder.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/backend.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/chart_style.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 PLT_STYLE_TEMPLATE = "plotly_dark"
 PLT_STYLE_INCREASING = "#00ACFF"
 PLT_STYLE_DECREASING = "#e4003a"
 PLT_CANDLESTICKS = dict(
     increasing=dict(line_color=PLT_STYLE_INCREASING, fillcolor=PLT_STYLE_INCREASING),
     decreasing=dict(line_color=PLT_STYLE_DECREASING, fillcolor=PLT_STYLE_DECREASING),
 )
-PLT_STYLE_INCREASING_GREEN = "#009600"
-PLT_STYLE_DECREASING_RED = "#c80000"
-PLT_FONT = dict(family="Fira Code", size=16)
-PLOTLY_FONT = dict(family="Fira Code", size=18)
+PLT_STYLE_INCREASING_GREEN = "#00ACFF"
+PLT_STYLE_DECREASING_RED = "#e4003a"
+PLT_FONT = dict(family="Arial", size=16)
+PLOTLY_FONT = dict(family="Arial", size=16)
 
 PLT_COLORWAY = [
     "#ffed00",
     "#ef7d00",
     "#e4003a",
     "#c13246",
     "#822661",
@@ -196,66 +196,99 @@
             side="right",
             zeroline=True,
             fixedrange=False,
             title_standoff=20,
             nticks=15,
             showline=True,
             showgrid=True,
+            ticklen=0,
         ),
         yaxis2=dict(
+            side="left",
             zeroline=False,
             fixedrange=False,
             anchor="x",
             layer="above traces",
             overlaying="y2",
             nticks=6,
             tick0=0.5,
             title_standoff=10,
-            tickfont=dict(size=15),
-            showline=True,
+            tickfont=dict(size=12),
+            showline=False,
+            ticklen=0,
         ),
         yaxis3=dict(
             zeroline=False,
             fixedrange=False,
             anchor="x",
             layer="above traces",
             overlaying="y3",
             nticks=6,
             tick0=0.5,
             title_standoff=10,
-            tickfont=dict(size=15),
+            tickfont=dict(size=12),
             showline=True,
+            ticklen=0,
         ),
         yaxis4=dict(
             zeroline=False,
             fixedrange=False,
             anchor="x",
             layer="above traces",
             overlaying="y4",
             nticks=6,
             tick0=0.5,
             title_standoff=10,
-            tickfont=dict(size=15),
+            tickfont=dict(size=12),
             showline=True,
+            ticklen=0,
         ),
         xaxis=dict(
             showgrid=True,
-            zeroline=True,
+            zeroline=False,
             showline=True,
             rangeslider=dict(visible=False),
             tickfont=dict(size=16),
             title_standoff=20,
+            ticklen=0,
+        ),
+        xaxis2=dict(
+            showgrid=True,
+            zeroline=False,
+            showline=True,
+            rangeslider=dict(visible=False),
+            tickfont=dict(size=12),
+            title_standoff=20,
+            ticklen=0,
+        ),
+        xaxis3=dict(
+            showgrid=True,
+            zeroline=False,
+            showline=True,
+            rangeslider=dict(visible=False),
+            tickfont=dict(size=12),
+            title_standoff=20,
+            ticklen=0,
+        ),
+        xaxis4=dict(
+            showgrid=True,
+            zeroline=False,
+            showline=True,
+            rangeslider=dict(visible=False),
+            tickfont=dict(size=12),
+            title_standoff=20,
+            ticklen=0,
         ),
         legend=dict(
-            yanchor="top",
-            y=0.99,
-            xanchor="left",
-            font_size=15,
-            bgcolor="rgba(0, 0, 0, 0)",
-            x=0.01,
+            orientation="h",
+            yanchor="bottom",
+            y=1.02,
+            xanchor="right",
+            x=0.95,
+            font=dict(size=12),
         ),
         dragmode="pan",
         hovermode="x",
         hoverlabel=dict(align="left"),
     ),
     data=dict(
         candlestick=[
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,23 +739,26 @@
             x=df_stock.index,
             y=df_stock[volume_col],
             name="Volume",
             marker_color=colors,
             yaxis="y2",
             row=row,
             col=col,
-            opacity=0.7,
+            opacity=0.5,
             secondary_y=True,
+            showlegend=False,
+            hovertemplate="%{y}<extra></extra>",
         )
         ticksize = 13 - (self.subplots_kwargs["rows"] // 2)
         self.update_layout(
             yaxis2=dict(
-                fixedrange=True,
+                fixedrange=False,
                 side="left",
-                nticks=10,
+                nticks=8,
+                autorange=False,
                 range=vol_scale["range"],
                 tickvals=vol_scale["ticks"],
                 showgrid=False,
                 showline=False,
                 zeroline=False,
                 tickfont=dict(size=ticksize),
                 overlaying="y",
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly.html` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly.html`

 * *Files 0% similar despite different names*

```diff
@@ -296281,20 +296281,20 @@
 00485580: 6561 6465 723a 207b 2066 696c 6c3a 207b  eader: { fill: {
 00485590: 2063 6f6c 6f72 3a20 2223 4338 4434 4533   color: "#C8D4E3
 004855a0: 2220 7d2c 206c 696e 653a 207b 2063 6f6c  " }, line: { col
 004855b0: 6f72 3a20 2277 6869 7465 2220 7d20 7d2c  or: "white" } },
 004855c0: 2074 7970 653a 2022 7461 626c 6522 207d   type: "table" }
 004855d0: 5d2c 2063 616e 646c 6573 7469 636b 3a20  ], candlestick: 
 004855e0: 5b7b 2064 6563 7265 6173 696e 673a 207b  [{ decreasing: {
-004855f0: 2066 696c 6c63 6f6c 6f72 3a20 2223 6338   fillcolor: "#c8
-00485600: 3030 3030 222c 206c 696e 653a 207b 2063  0000", line: { c
+004855f0: 2066 696c 6c63 6f6c 6f72 3a20 2223 6534   fillcolor: "#e4
+00485600: 3030 3361 222c 206c 696e 653a 207b 2063  003a", line: { c
 00485610: 6f6c 6f72 3a20 2223 3939 3030 3030 2220  olor: "#990000" 
 00485620: 7d20 7d2c 2069 6e63 7265 6173 696e 673a  } }, increasing:
 00485630: 207b 2066 696c 6c63 6f6c 6f72 3a20 2223   { fillcolor: "#
-00485640: 3030 3936 3030 222c 206c 696e 653a 207b  009600", line: {
+00485640: 3030 4143 4646 222c 206c 696e 653a 207b  00ACFF", line: {
 00485650: 2063 6f6c 6f72 3a20 2223 3030 3735 3030   color: "#007500
 00485660: 2220 7d20 7d2c 2074 7970 653a 2022 6361  " } }, type: "ca
 00485670: 6e64 6c65 7374 6963 6b22 207d 5d20 7d2c  ndlestick" }] },
 00485680: 206c 6179 6f75 743a 207b 2061 6e6e 6f74   layout: { annot
 00485690: 6174 696f 6e64 6566 6175 6c74 733a 207b  ationdefaults: {
 004856a0: 2061 7272 6f77 636f 6c6f 723a 2022 2332   arrowcolor: "#2
 004856b0: 6133 6635 6622 2c20 6172 726f 7768 6561  a3f5f", arrowhea
@@ -300741,21 +300741,21 @@
 00496c40: 746f 7228 275b 6461 7461 2d74 6974 6c65  tor('[data-title
 00496c50: 3d22 4368 616e 6765 2054 6865 6d65 225d  ="Change Theme"]
 00496c60: 2729 2e67 6574 456c 656d 656e 7473 4279  ').getElementsBy
 00496c70: 5461 674e 616d 6528 2273 7667 2229 5b30  TagName("svg")[0
 00496c80: 5d2e 7365 7441 7474 7269 6275 7465 2822  ].setAttribute("
 00496c90: 7669 6577 426f 7822 2c20 6265 2e76 6965  viewBox", be.vie
 00496ca0: 7742 6f78 293b 2063 6f6e 7374 204e 6520  wBox); const Ne 
-00496cb0: 3d20 6165 203f 207b 2022 2330 3039 3630  = ae ? { "#00960
-00496cc0: 3022 3a20 2223 3030 4143 4646 222c 2022  0": "#00ACFF", "
+00496cb0: 3d20 6165 203f 207b 2022 2330 3041 4346  = ae ? { "#00ACF
+00496cc0: 4622 3a20 2223 3030 4143 4646 222c 2022  F": "#00ACFF", "
 00496cd0: 2363 3830 3030 3022 3a20 2223 6534 3030  #c80000": "#e400
 00496ce0: 3361 2220 7d20 3a20 7b20 2223 6534 3030  3a" } : { "#e400
 00496cf0: 3361 223a 2022 2363 3830 3030 3022 2c20  3a": "#c80000", 
-00496d00: 2223 3030 4143 4646 223a 2022 2330 3039  "#00ACFF": "#009
-00496d10: 3630 3022 207d 3b20 6665 2e66 6f72 4561  600" }; fe.forEa
+00496d00: 2223 3030 4143 4646 223a 2022 2330 3041  "#00ACFF": "#00A
+00496d10: 4346 4622 207d 3b20 6665 2e66 6f72 4561  CFF" }; fe.forEa
 00496d20: 6368 2871 6520 3d3e 207b 2071 652e 7479  ch(qe => { qe.ty
 00496d30: 7065 203d 3d3d 2022 6261 7222 2026 2620  pe === "bar" && 
 00496d40: 4172 7261 792e 6973 4172 7261 7928 7165  Array.isArray(qe
 00496d50: 2e6d 6172 6b65 722e 636f 6c6f 7229 2026  .marker.color) &
 00496d60: 2620 2871 652e 6d61 726b 6572 2e63 6f6c  & (qe.marker.col
 00496d70: 6f72 203d 2071 652e 6d61 726b 6572 2e63  or = qe.marker.c
 00496d80: 6f6c 6f72 2e6d 6170 2876 6520 3d3e 204e  olor.map(ve => N
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import warnings
 from dataclasses import dataclass
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 import pandas as pd
 import pandas_ta as ta
 
-from .ta_helpers import check_columns
+from openbb_charting.core.plotly_ta.ta_helpers import check_columns
 
 # pylint: disable=E1123
 datacls_kwargs = {"slots": True} if sys.version_info >= (3, 10) else {}
 
 
 def columns_regex(df_ta: pd.DataFrame, name: str) -> List[str]:
     """Return columns that match regex name."""
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Custom technical indicators."""
 
 import warnings
 from datetime import datetime, timedelta
 
 import numpy as np
 import pandas as pd
+
 from openbb_charting.core.config.openbb_styles import PLT_FIB_COLORWAY
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import PltTA, indicator
 
 
 class Custom(PltTA):
     """Volatility technical indicators."""
 
     @indicator()
     def plot_srlines(self, fig: OpenBBFigure, df_ta: pd.DataFrame):
         """Add support and resistance lines to plotly figure."""
-        window = self.params["srlines"].get_argument_values("window")
+        window = self.params["srlines"].get_argument_values("window")  # type: ignore
         window = window[0] if isinstance(window, list) and len(window) > 0 else 200
 
         def is_far_from_level(value, levels, df_stock):
             ave = np.mean(df_stock["high"] - df_stock["low"])
             return np.sum([abs(value - level) < ave for _, level in levels]) == 0
 
         def is_support(df, i):
@@ -46,15 +47,15 @@
         if df_ta2.index[-2].date() != df_ta2.index[-1].date():
             interval = 1440
         else:
             interval = (df_ta2.index[1] - df_ta2.index[0]).seconds / 60
 
         if interval <= 15:
             cut_days = 1 if interval < 15 else 2
-            dt_unique_days = df_ta2.index.normalize().unique()
+            dt_unique_days = df_ta2.index.normalize().unique()  # type: ignore
             df_ta2 = df_ta2.loc[
                 (df_ta2.index >= pd.to_datetime(dt_unique_days[-cut_days], unit="ns"))
                 & (df_ta2.index < today)
             ].copy()
 
         levels: list = []
         x_range = df_ta2.index[-1].replace(hour=15, minute=59)
@@ -72,15 +73,15 @@
             if is_support(df_ta2, i):
                 lv = df_ta2["low"][i]
                 if is_far_from_level(lv, levels, df_ta2):
                     levels.append((i, lv))
                     fig.add_scatter(
                         x=[df_ta.index[0], x_range],
                         y=[lv, lv],
-                        opacity=1,
+                        opacity=0.8,
                         mode="lines+text",
                         text=["", f"{lv:{self.get_float_precision()}}"],
                         textposition="top center",
                         textfont=dict(
                             family="Arial Black", color="rgb(120, 70, 200)", size=10
                         ),
                         line=dict(
@@ -95,15 +96,15 @@
             elif is_resistance(df_ta2, i):
                 lv = df_ta2["high"][i]
                 if is_far_from_level(lv, levels, df_ta2):
                     levels.append((i, lv))
                     fig.add_scatter(
                         x=[df_ta.index[0], x_range],
                         y=[lv, lv],
-                        opacity=1,
+                        opacity=0.85,
                         mode="lines+text",
                         text=["", f"{lv:{self.get_float_precision()}}"],
                         textposition="top center",
                         textfont=dict(
                             family="Arial Black", color="rgb(120, 70, 200)", size=10
                         ),
                         line=dict(
@@ -128,26 +129,28 @@
         except ImportError:
             warnings.warn(
                 "In order to use the Fibonacci indicator in your plot,"
                 " you need to install the `openbb-technical` package."
             )
             return fig
 
-        limit = self.params["fib"].get_argument_values("limit") or 120
-        start_date = self.params["fib"].get_argument_values("start_date") or None
-        end_date = self.params["fib"].get_argument_values("end_date") or None
-        close = self.params["fib"].get_argument_values("close") or "close"
+        limit = self.params["fib"].get_argument_values("limit") or 120  # type: ignore
+        start_date = self.params["fib"].get_argument_values("start_date") or None  # type: ignore
+        end_date = self.params["fib"].get_argument_values("end_date") or None  # type: ignore
+        close = self.params["fib"].get_argument_values("close") or "close"  # type: ignore
         (
             df_fib,
             min_date,
             max_date,
             min_pr,
             max_pr,
             lvl_text,
-        ) = calculate_fib_levels(df_ta, close, limit, start_date, end_date)
+        ) = calculate_fib_levels(
+            df_ta, close, limit, start_date, end_date  # type: ignore
+        )
         levels = df_fib.Price
         fibs = [
             "<b>0</b>",
             "<b>0.235</b>",
             "<b>0.382</b>",
             "<b>0.5</b>",
             "<b>0.618</b>",
@@ -170,15 +173,15 @@
             col=1,
             secondary_y=False,
         )
         df_ta2 = df_ta.copy()
         interval = 1440
         if df_ta2.index[-2].date() == df_ta2.index[-1].date():
             interval = (df_ta2.index[1] - df_ta2.index[0]).seconds / 60
-            dt_unique_days = df_ta2.index.normalize().unique()
+            dt_unique_days = df_ta2.index.normalize().unique()  # type: ignore
 
             if interval not in [15, 30, 60] and len(dt_unique_days) <= 3:
                 df_ta2 = df_ta2.loc[
                     (df_ta2.index >= dt_unique_days[-1])
                     & (df_ta2.index < datetime.now())
                 ].copy()
                 df_ta2 = df_ta2.between_time("09:30", "20:00").copy()
@@ -195,15 +198,15 @@
             if lvl_text == "right":
                 text = [text[1], text[0]]
 
             fig.add_scatter(
                 name=fibs[i],
                 x=[min_date, df_ta2.index.max()],
                 y=[levels[i], levels[i]],
-                opacity=0.9,
+                opacity=0.85,
                 mode="lines+text",
                 text=text,
                 textposition=text_pos,
                 textfont=dict(PLT_FIB_COLORWAY[7], color=PLT_FIB_COLORWAY[i]),
                 line_color=PLT_FIB_COLORWAY[i],
                 line_width=1.5,
                 showlegend=False,
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Momentum technical indicators."""
 
 import warnings
 
 import numpy as np
 import pandas as pd
 import pandas_ta as ta
+
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
     columns_regex,
@@ -42,60 +43,60 @@
         fig.add_hrect(
             y0=100,
             y1=dmax,
             fillcolor=fig.theme.down_color,
             opacity=0.2,
             layer="below",
             line_width=0,
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hrect(
             y0=-100,
             y1=dmin,
             fillcolor=fig.theme.up_color,
             opacity=0.2,
             layer="below",
             line_width=0,
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hline(
             y=100,
             opacity=1,
             layer="below",
             line=dict(width=2, color=fig.theme.down_color, dash="dash"),
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hline(
             y=-100,
             opacity=1,
             layer="below",
             line=dict(width=2, color=fig.theme.up_color, dash="dash"),
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
 
         fig.add_annotation(
             xref=f"x{subplot_row} domain",
             yref=f"y{subplot_row + 1} domain",
             text="<b>CCI</b>",
             x=0,
             xanchor="right",
             xshift=-6,
             y=0.97,
             font_size=14,
             font_color="#e0b700",
         )
-        fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)
+        fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)  # type: ignore
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_cg(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
         """Add cg to plotly figure."""
         cg_col = columns_regex(df_ta, "CG")[0]
@@ -140,15 +141,15 @@
             xanchor="right",
             xshift=-6,
             y=0.97,
             yshift=-20,
             font_size=14,
             font_color="#ef7d00",
         )
-        fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)
+        fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)  # type: ignore
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_clenow(self, fig: OpenBBFigure, df_ta: pd.DataFrame, inchart_index: int):
         """Add current close price to plotly figure."""
         try:
@@ -158,16 +159,16 @@
         except ImportError:
             warnings.warn(
                 "In order to use the Clenow momentum indicator in your plot,"
                 " you need to install the `openbb-technical` package."
             )
             return fig, inchart_index
 
-        window = self.params["clenow"].get_argument_values("window") or 90
-        _, _, fit_data = clenow_momentum(df_ta[self.close_column], window=window)
+        window = self.params["clenow"].get_argument_values("window") or 90  # type: ignore
+        _, _, fit_data = clenow_momentum(df_ta[self.close_column], window=window)  # type: ignore
 
         fig.add_scatter(
             x=df_ta.index[-window:],  # type: ignore
             y=pow(np.e, fit_data),
             name="CLenow",
             mode="lines",
             line=dict(color=self.inchart_colors[inchart_index], width=2),
@@ -189,15 +190,15 @@
             opacity=1,
         )
         return fig, inchart_index + 1
 
     @indicator()
     def plot_demark(self, fig: OpenBBFigure, df_ta: pd.DataFrame, inchart_index: int):
         """Add demark to plotly figure."""
-        min_val = self.params["demark"].get_argument_values("min_val") or 5
+        min_val = self.params["demark"].get_argument_values("min_val") or 5  # type: ignore
 
         demark = ta.td_seq(df_ta[self.close_column], asint=True)
         demark = demark.set_index(df_ta.index)
 
         # pylint: disable=unsupported-assignment-operation
         demark["up"] = demark.TD_SEQ_UPa.apply(
             lambda x: f"<b>{x}</b>" if x >= min_val else None
@@ -309,50 +310,50 @@
         fig.add_hrect(
             y0=2,
             y1=(dmax + 4),
             fillcolor=fig.theme.down_color,
             opacity=0.2,
             layer="below",
             line_width=0,
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hrect(
             y0=-2,
             y1=(dmin - 4),
             fillcolor=fig.theme.up_color,
             opacity=0.2,
             layer="below",
             line_width=0,
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hline(
             y=2,
             fillcolor=fig.theme.down_color,
             opacity=1,
             layer="below",
             line=dict(width=2, color=fig.theme.down_color, dash="dash"),
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hline(
             y=-2,
             fillcolor=fig.theme.up_color,
             opacity=1,
             layer="below",
             line=dict(width=2, color=fig.theme.up_color, dash="dash"),
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
-        fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)
+        fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)  # type: ignore
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_macd(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
         """Add macd to plotly figure."""
         fig.add_bar(
@@ -406,15 +407,15 @@
             x=0,
             xanchor="right",
             y=0.70,
             font_size=13,
             xshift=-3,
             font_color="rgb(7, 166, 52)",
         )
-        fig["layout"][f"yaxis{subplot_row + 1}"].update(autorange=True, nticks=5)
+        fig["layout"][f"yaxis{subplot_row + 1}"].update(autorange=True, nticks=5)  # type: ignore
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_rsi(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
         """Add rsi to plotly figure."""
         rsi_col = columns_regex(df_ta, "RSI")[0]
@@ -444,50 +445,50 @@
         fig.add_hrect(
             y0=70,
             y1=100,
             fillcolor=fig.theme.down_color,
             opacity=0.2,
             layer="below",
             line_width=0,
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hrect(
             y0=0,
             y1=30,
             fillcolor=fig.theme.up_color,
             opacity=0.2,
             layer="below",
             line_width=0,
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hline(
             y=70,
             fillcolor=fig.theme.down_color,
             opacity=1,
             layer="below",
             line=dict(width=2, color=fig.theme.down_color, dash="dash"),
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
         fig.add_hline(
             y=30,
             fillcolor=fig.theme.up_color,
             opacity=1,
             layer="below",
             line=dict(width=2, color=fig.theme.up_color, dash="dash"),
-            row=subplot_row,
-            col=1,
+            row=subplot_row,  # type: ignore
+            col=1,  # type: ignore
             secondary_y=False,
         )
-        fig["layout"][f"yaxis{subplot_row + 1}"].update(tickvals=[0, 30, 70, 100])
+        fig["layout"][f"yaxis{subplot_row + 1}"].update(tickvals=[0, 30, 70, 100])  # type: ignore
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_stoch(self, fig: OpenBBFigure, df_ta: pd.DataFrame, subplot_row: int):
         """Add stoch to plotly figure."""
         fig.add_scatter(
@@ -520,54 +521,56 @@
             x=0,
             xanchor="right",
             xshift=-6,
             y=0.98,
             font_size=14,
             font_color="#e0b700",
         )
-        fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)
+        fig["layout"][f"yaxis{subplot_row + 1}"].update(nticks=5, autorange=True)  # type: ignore
 
         return fig, subplot_row + 1
 
     @indicator()
     def plot_ichimoku(self, fig: OpenBBFigure, df_ta: pd.DataFrame, inchart_index: int):
         """Calculate Ichimoku indicator."""
         conversion_period = (
-            self.params["ichimoku"].get_argument_values("conversion_period") or 9
+            self.params["ichimoku"].get_argument_values("conversion_period") or 9  # type: ignore
         )
-        base_period = self.params["ichimoku"].get_argument_values("base_period") or 26
+        base_period = self.params["ichimoku"].get_argument_values("base_period") or 26  # type: ignore
         lagging_line_period = (
-            self.params["ichimoku"].get_argument_values("lagging_line_period") or 52
+            self.params["ichimoku"].get_argument_values("lagging_line_period") or 52  # type: ignore
         )
-        displacement = self.params["ichimoku"].get_argument_values("displacement") or 26
+        displacement = self.params["ichimoku"].get_argument_values("displacement") or 26  # type: ignore
 
         # Tenkan-sen (Conversion Line)
         conversion_line = (
-            df_ta["high"].rolling(window=conversion_period).max()
-            + df_ta["low"].rolling(window=conversion_period).min()
+            df_ta["high"].rolling(window=conversion_period).max()  # type: ignore
+            + df_ta["low"].rolling(window=conversion_period).min()  # type: ignore
         ) / 2
 
         # Kijun-sen (Base Line)
         base_line = (
-            df_ta["high"].rolling(window=base_period).max()
-            + df_ta["low"].rolling(window=base_period).min()
+            df_ta["high"].rolling(window=base_period).max()  # type: ignore
+            + df_ta["low"].rolling(window=base_period).min()  # type: ignore
         ) / 2
 
         # Senkou Span A (Leading Span A)
-        leading_span_a = ((conversion_line + base_line) / 2).shift(displacement)
+        leading_span_a = ((conversion_line + base_line) / 2).shift(displacement)  # type: ignore
 
         # Senkou Span B (Leading Span B)
         lagging_line = df_ta[self.close_column].shift(-lagging_line_period)  # type: ignore
         leading_span_b = (
             (
-                lagging_line.rolling(window=base_period).max()
-                + lagging_line.rolling(window=base_period).min()
+                lagging_line.rolling(window=base_period).max()  # type: ignore
+                + lagging_line.rolling(window=base_period).min()  # type: ignore
             )
             / 2
-        ).shift(displacement)
+        ).shift(
+            displacement  # type: ignore
+        )
 
         # Plot Tenkan-sen and Kijun-sen
         fig.add_scatter(
             x=df_ta.index,
             y=conversion_line,
             line=dict(color="orange", width=1),
             name="Tenkan-sen",
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Overlap technical indicators plugin for Plotly TA."""
 
 import warnings
 
 import pandas as pd
+
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
     columns_regex,
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Trend technical indicators."""
 
 import pandas as pd
+
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
     columns_regex,
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Volatility technical indicators plugin for Plotly TA."""
 
 import pandas as pd
+
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
     columns_regex,
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Volume technical indicators."""
 
 import pandas as pd
+
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.base import (
     PltTA,
     indicator,
 )
 from openbb_charting.core.plotly_ta.data_classes import (
     columns_regex,
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Technical Analysis class for Plotly."""
 
-# pylint: disable=R0902
+# pylint: disable=R0902,R0916,R0912  # type: ignore[index, assignment]
+
 import importlib
 import inspect
 import sys
 import warnings
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union
 
 import pandas as pd
 
 from openbb_charting.core.chart_style import ChartStyle
 from openbb_charting.core.openbb_figure import OpenBBFigure
-
-from .base import PltTA
-from .data_classes import ChartIndicators
-from .ta_helpers import check_columns
+from openbb_charting.core.plotly_ta.base import PltTA
+from openbb_charting.core.plotly_ta.data_classes import ChartIndicators
+from openbb_charting.core.plotly_ta.ta_helpers import check_columns
 
 charting_EXTENSION_PATH = Path(__file__).parent.parent.parent
 CHARTING_INSTALL_PATH = charting_EXTENSION_PATH.parent
 PLUGINS_PATH = Path(__file__).parent / "plugins"
 PLOTLY_TA: Optional["PlotlyTA"] = None
 
 if TYPE_CHECKING:
@@ -127,15 +127,15 @@
         """Initialize the class.
 
         Method is overridden to do nothing, except to clear the internal data structures.
         """
         if not args and not kwargs:
             self._clear_data()
         else:
-            self.df_fib = None
+            self.df_fib = None  # type: ignore
             super().__init__(*args, **kwargs)
 
     @staticmethod
     def setup_theme(chart_style, user_styles_directory) -> ChartStyle:
         """Set up theme for charting."""
         return ChartStyle(chart_style, user_styles_directory)
 
@@ -252,15 +252,15 @@
             Plotly figure to plot on, by default None
         volume_ticks_x : int, optional
             Number to multiply volume, by default 7
         """
         if indicators is None and PLOTLY_TA is not None:
             indicators = PLOTLY_TA.indicators
 
-        return PlotlyTA().__plot__(
+        return PlotlyTA().__plot__(  # type: ignore
             df_stock, indicators, symbol, candles, volume, prepost, fig, volume_ticks_x
         )
 
     @staticmethod
     def _locate_plugins(debug: Optional[bool] = False) -> None:
         """Locate all the plugins in the plugins folder."""
         path = (
@@ -293,23 +293,23 @@
                     and issubclass(obj, (PltTA))
                     and obj != PlotlyTA.__class__
                 ) and obj not in PlotlyTA.plugins:
                     PlotlyTA.plugins.append(obj)
 
     def _clear_data(self):
         """Clear and reset all data to default values."""
-        self.df_stock = None
+        self.df_stock = None  # type: ignore
         self.indicators = ChartIndicators.from_dict({})
         self.params = None
         self.intraday = False
         self.show_volume = True
 
     def calculate_indicators(self):
         """Return dataframe with all indicators."""
-        return self.indicators.to_dataframe(self.df_stock.copy(), self.ma_mode)
+        return self.indicators.to_dataframe(self.df_stock.copy(), self.ma_mode)  # type: ignore
 
     def get_subplot(self, subplot: str) -> bool:
         """Return True if subplots will be able to be plotted with current data."""
         if subplot == "volume":
             return self.show_volume
 
         if subplot in ["ad", "adosc", "obv", "vwap"] and not self.has_volume:
@@ -325,20 +325,20 @@
 
         try:
             indicator = self.indicators.get_indicator(subplot)
             if indicator is None:
                 return False
 
             output = self.indicators.get_indicator_data(
-                self.df_stock.copy(),
+                self.df_stock.copy(),  # type: ignore
                 indicator,
                 **self.indicators.get_options_dict(indicator.name) or {},
             )
             if not isinstance(output, bool):
-                output = output.dropna()
+                output = output.dropna()  # type: ignore
 
                 if output is None or output.empty:
                     output = False
 
             return True
 
         except Exception:
@@ -411,38 +411,39 @@
                 x=self.df_stock.index,
                 open=self.df_stock.open,
                 high=self.df_stock.high,
                 low=self.df_stock.low,
                 close=self.df_stock.close,
                 decreasing=dict(line=dict(width=cc_linewidth)),
                 increasing=dict(line=dict(width=cc_linewidth)),
-                name=f"{symbol} OHLC",
+                name=f"{symbol}",
                 showlegend=False,
                 row=1,
                 col=1,
                 secondary_y=False,
+                hoverinfo="x+y",
             )
         else:
             fig.add_scatter(
                 x=self.df_stock.index,
-                y=self.df_stock[self.close_column],
-                name=f"{symbol} Close",
+                y=self.df_stock[self.close_column],  # type: ignore
+                name=f"{symbol}",
                 connectgaps=True,
                 row=1,
                 col=1,
                 secondary_y=False,
             )
             fig.update_layout(yaxis=dict(nticks=15))
             if self.theme:
                 self.inchart_colors = self.theme.get_colors()[1:]
 
         fig.set_title(symbol, x=0.5, y=0.98, xanchor="center", yanchor="top")
         return fig
 
-    def plot_fig(
+    def plot_fig(  # noqa: PLR0912
         self,
         fig: Optional[OpenBBFigure] = None,
         symbol: str = "",
         candles: bool = True,
         volume_ticks_x: int = 7,
     ) -> OpenBBFigure:
         """Plot indicators on plotly figure.
@@ -461,31 +462,35 @@
         Returns
         -------
         fig : OpenBBFigure
             Plotly figure with candlestick/line chart and volume bar chart (if enabled)
         """
         self.df_ta = self.calculate_indicators()
 
-        symbol = (
+        symbol = (  # type: ignore
             self.df_stock.name
             if hasattr(self.df_stock, "name") and not symbol
             else symbol
         )
 
         figure = self.init_plot(symbol, candles) if fig is None else fig
-
         subplot_row, fig_new = 2, {}
         inchart_index, ma_done = 0, False
 
         figure = self.process_fig(figure, volume_ticks_x)
 
-        # Aroon indicator is always plotted first since it has 2 subplot rows
+        # Aroon indicator is always plotted first since it has 2 subplot rows.
+        # ATR messes up the volume layout so we plot it last.
         plot_indicators = sorted(
             self.indicators.get_active_ids(),
-            key=lambda x: 50 if x == "aroon" else 999 if x in self.subplots else 1,
+            key=lambda x: (
+                50
+                if x == "aroon"
+                else 1000 if x == "atr" else 999 if x in self.subplots else 1
+            ),
         )
 
         for indicator in plot_indicators:
             try:
                 if indicator in self.subplots:
                     figure, subplot_row = getattr(self, f"plot_{indicator}")(
                         figure, self.df_ta, subplot_row
@@ -495,14 +500,15 @@
                         if ma_done:
                             continue
                         indicator, ma_done = "ma", True  # noqa
 
                     figure, inchart_index = getattr(self, f"plot_{indicator}")(
                         figure, self.df_ta, inchart_index
                     )
+                    figure.layout.annotations = None
                 elif indicator in ["fib", "srlines", "demark", "clenow", "ichimoku"]:
                     figure = getattr(self, f"plot_{indicator}")(figure, self.df_ta)
                 else:
                     raise ValueError(f"Unknown indicator: {indicator}")
 
                 fig_new.update(figure.to_plotly_json())
 
@@ -521,43 +527,92 @@
                     )
                     break
             except Exception as e:
                 warnings.warn(f"[bold red]Error plotting {indicator}: {e}[/]")
                 continue
 
         figure.update(fig_new)
-        figure.update_yaxes(
-            row=1,
-            col=1,
-            secondary_y=False,
-            nticks=15 if subplot_row < 3 else 10,
-            tickfont=dict(size=16),
-        )
+        for row in range(0, subplot_row + 1):
+            figure.update_yaxes(
+                row=row,
+                col=1,
+                secondary_y=False,
+                nticks=15 if subplot_row < 3 else 6,
+                tickfont=dict(size=12),
+            )
         figure.update_traces(
             selector=dict(type="scatter", mode="lines"), connectgaps=True
         )
-        figure.update_layout(showlegend=False)
         if hasattr(figure, "hide_holidays"):
-            figure.hide_holidays(self.prepost)
+            figure.hide_holidays(self.prepost)  # type: ignore
 
         if not self.show_volume:
             figure.update_layout(margin=dict(l=20))
 
-        # We remove xaxis labels from all but bottom subplot, and we make sure
-        # they all match the bottom one
+        # We remove xaxis labels from all but bottom subplot,
+        # and we make sure they all match the bottom one
         xbottom = f"y{subplot_row+1}"
         xaxes = list(figure.select_xaxes())
         for xa in xaxes:
             if xa == xaxes[-1]:
                 xa.showticklabels = True
             if not xa.showticklabels and xa.anchor != xbottom:
                 xa.showticklabels = False
             if xa.anchor != xbottom:
                 xa.matches = xbottom.replace("y", "x")
 
+        fib_legend_shown = False
+        sr_legend_shown = False
+        for item in figure.data:
+            if item.name:
+                item.name = item.name.replace("_", " ")
+                if "MA " not in item.name:
+                    item.showlegend = False
+                if "<b>" in item.name:
+                    item.name = "Fib"
+                    item.hoverinfo = "none"
+                    item.hoveron = "fills"
+                    item.pop("hovertemplate", None)
+                    item.legendgroup = "Fib"
+                    if not fib_legend_shown:
+                        item.showlegend = True
+                        fib_legend_shown = True
+                if (
+                    "Historical" not in item.name
+                    and "Candlestick" not in item.name
+                    and "Fib" not in item.name
+                    and item.name is not None
+                ):
+                    if (
+                        "MA " in item.name
+                        or "VWAP" in item.name
+                        or "DC" in item.name
+                        or "KC" in item.name
+                        or "-sen" in item.name
+                        or "Senkou" in item.name
+                    ):
+                        item.showlegend = True
+                        item.hoverinfo = "y"
+                        item.hovertemplate = "%{fullData.name}:%{y}<extra></extra>"
+                    else:
+                        item.hovertemplate = "%{y}<extra></extra>"
+            if item.name is None:
+                item.name = "SR Lines"
+                item.hoverinfo = "none"
+                item.hoveron = "fills"
+                item.legendgroup = "SR Lines"
+                item.pop("hovertemplate", None)
+                if not sr_legend_shown:
+                    item.showlegend = True
+                    sr_legend_shown = True
+
+        if "annotations" in figure.layout:
+            for item in figure.layout.annotations:  # type: ignore
+                item["font"]["size"] = 12
+        figure.update_layout(margin=dict(l=50, r=10, b=10, t=20))
         return figure
 
     def process_fig(self, fig: OpenBBFigure, volume_ticks_x: int = 7) -> OpenBBFigure:
         """Process plotly figure before plotting indicators.
 
         Parameters
         ----------
@@ -571,15 +626,14 @@
         fig : OpenBBFigure
             Processed plotly figure
         """
         new_subplot = OpenBBFigure(charting_settings=self.charting_settings)
         new_subplot = fig.create_subplots(
             shared_xaxes=True, **self.get_fig_settings_dict()
         )
-
         subplots: Dict[str, Dict[str, List[Any]]] = {}
         grid_ref = fig._validate_get_grid_ref()  # pylint: disable=protected-access
         for r, plot_row in enumerate(grid_ref):
             for c, plot_refs in enumerate(plot_row):
                 if not plot_refs:
                     continue
                 for subplot_ref in plot_refs:
@@ -605,16 +659,16 @@
                 and "domain" in fig_json[layout]
                 and any(x in layout for x in ["xaxis", "yaxis"])
             ):
                 fig_json[layout]["domain"] = new_subplot.to_plotly_json()["layout"][
                     layout
                 ]["domain"]
 
-            fig.layout.update({layout: fig_json[layout]})
-            new_subplot.layout.update({layout: fig.layout[layout]})
+            fig.layout.update({layout: fig_json[layout]})  # type: ignore
+            new_subplot.layout.update({layout: fig.layout[layout]})  # type: ignore
 
         if self.show_volume:
             new_subplot.add_inchart_volume(
-                self.df_stock, self.close_column, volume_ticks_x=volume_ticks_x
+                self.df_stock, self.close_column, volume_ticks_x=volume_ticks_x  # type: ignore
             )
 
         return new_subplot
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/table.html` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/core/to_chart.py` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/query_params.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/available_indices.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,111 @@
-"""Charting Extension Query Params."""
+"""Cboe Available Indices Model."""
 
-from typing import List, Optional, Union
+from datetime import time
+from typing import Any, Dict, List, Optional
 
-from openbb_core.provider.abstract.data import Data
-from openbb_core.provider.abstract.query_params import QueryParams
+from openbb_cboe.utils.helpers import get_index_directory
+from openbb_core.provider.abstract.fetcher import Fetcher
+from openbb_core.provider.standard_models.available_indices import (
+    AvailableIndicesData,
+    AvailableIndicesQueryParams,
+)
 from pydantic import Field
 
 
-class FredSeriesChartQueryParams(QueryParams):
+class CboeAvailableIndicesQueryParams(AvailableIndicesQueryParams):
+    """Cboe Available Indices Query.
+
+    Source: https://www.cboe.com/
     """
-    FRED Series Chart Query Params.
 
-    kwargs
-    ------
+    use_cache: bool = Field(
+        default=True,
+        description="When True, the Cboe Index directory will be cached for 24 hours."
+        + " Set as False to bypass.",
+    )
+
 
-        data : List[Data], optional
-            Filtered versions of the data contained in the original results.
-            Example use is to reduce the number of columns or the length of data to plot.
-            To supply additional columns, set `allow_unsafe = True`.
-        title : str, optional
-            Title of the chart.
-        y1title : str, optional
-            Right Y-axis title.
-        y2title : str, optional
-            Left Y-axis title.
-        xtitle : str, optional
-            X-axis title.
-        dropnan: bool, optional (default: True)
-            If True, rows containing NaN will be dropped.
-        normalize: bool, optional (default: False)
-            If True, the data will be normalized and placed on the same axis.
-        allow_unsafe: bool, optional (default: False)
-            If True, the method will attempt to pass all supplied data to the chart constructor.
-            This can result in unexpected behavior.
+class CboeAvailableIndicesData(AvailableIndicesData):
+    """Cboe Available Indices Data.
+
+    Source: https://www.cboe.com/
     """
 
-    data: Optional[Union[Data, List[Data]]] = Field(
+    __alias_dict__ = {
+        "symbol": "index_symbol",
+        "data_delay": "mkt_data_delay",
+        "open_time": "calc_start_time",
+        "close_time": "calc_end_time",
+    }
+
+    symbol: Optional[str] = Field(description="Symbol for the index.")
+
+    description: Optional[str] = Field(
         default=None,
-        description="Filtered versions of the data contained in the original `self.results`."
-        + " Columns should be the same as the original data."
-        + " Example use is to reduce the number of columns or the length of data to plot."
-        + " To supply additional columns, set `allow_unsafe = True`.",
+        description="Description for the index. Valid only for US indices.",
     )
-    title: Optional[str] = Field(
-        default=None,
-        description="Title of the chart.",
+
+    data_delay: Optional[int] = Field(
+        default=None, description="Data delay for the index. Valid only for US indices."
     )
-    y1title: Optional[str] = Field(
+
+    open_time: Optional[time] = Field(
         default=None,
-        description="Right Y-axis title.",
+        description="Opening time for the index. Valid only for US indices.",
     )
-    y2title: Optional[str] = Field(
+
+    close_time: Optional[time] = Field(
         default=None,
-        description="Left Y-axis title.",
+        description="Closing time for the index. Valid only for US indices.",
     )
-    xtitle: Optional[str] = Field(
-        default=None,
-        description="X-axis title.",
+
+    time_zone: Optional[str] = Field(
+        default=None, description="Time zone for the index. Valid only for US indices."
     )
-    dropnan: bool = Field(
-        default=True,
-        description="If True, rows containing NaN will be dropped.",
+
+    tick_days: Optional[str] = Field(
+        default=None,
+        description="The trading days for the index. Valid only for US indices.",
     )
-    normalize: bool = Field(
-        default=False,
-        description="If True, the data will be normalized and placed on the same axis.",
+
+    tick_frequency: Optional[str] = Field(
+        default=None,
+        description="The frequency of the index ticks. Valid only for US indices.",
     )
-    allow_unsafe: bool = Field(
-        default=False,
-        description="If True, the method will attempt to pass all supplied data to the chart constructor."
-        + " This can result in unexpected behavior.",
+
+    tick_period: Optional[str] = Field(
+        default=None,
+        description="The period of the index ticks. Valid only for US indices.",
     )
 
 
-class TechnicalConesChartQueryParams(QueryParams):
-    """
-    Technical Cones Chart Query Params.
+class CboeAvailableIndicesFetcher(
+    Fetcher[
+        CboeAvailableIndicesQueryParams,
+        List[CboeAvailableIndicesData],
+    ]
+):
+    """Transform the query, extract and transform the data from the CBOE endpoints."""
 
-    kwargs
-    ------
+    @staticmethod
+    def transform_query(params: Dict[str, Any]) -> CboeAvailableIndicesQueryParams:
+        """Transform the query params."""
+        return CboeAvailableIndicesQueryParams(**params)
 
-        data : List[Data], optional
-            Filtered versions of the data contained in the original results.
-            Example use is to reduce the number of windows to plot.
-        title : str, optional
-            Title of the chart.
-        symbol: str, optional
-            Symbol represented by the data. Used to label the chart.
-    """
+    @staticmethod
+    async def aextract_data(
+        query: CboeAvailableIndicesQueryParams,
+        credentials: Optional[Dict[str, str]],
+        **kwargs: Any,
+    ) -> List[Dict]:
+        """Return the raw data from the CBOE endpoint."""
 
-    data: Optional[Union[Data, List[Data]]] = Field(
-        default=None,
-        description="Filtered versions of the data contained in the original results."
-        + " Columns should be the same as the original data."
-        + " Example use is to reduce the number of columns or the length of data to plot.",
-    )
-    title: Optional[str] = Field(
-        default=None,
-        description="Title of the chart.",
-    )
-    symbol: Optional[str] = Field(
-        default=None,
-        description="Symbol represented by the data. Used to label the chart.",
-    )
+        data = await get_index_directory(use_cache=query.use_cache, **kwargs)
+        return data.to_dict("records")
+
+    @staticmethod
+    def transform_data(
+        query: CboeAvailableIndicesQueryParams, data: List[Dict], **kwargs: Any
+    ) -> List[CboeAvailableIndicesData]:
+        """Transform the data to the standard format."""
+        return [CboeAvailableIndicesData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9912408873805933%*

 * *Differences: {"'layout'": "{'colorway': ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd', '#8c564b', "*

 * *             "'#e377c2', '#bcbd22', '#17becf', '#aec7e8', '#ffbb78', '#ff9896', '#c5b0d5', "*

 * *             "'#f7b6d2', '#dbdb8d', '#9edae5'], 'font': {'family': 'Arial'}, 'legend': {'bgcolor': "*

 * *             "'rgba(0, 0, 0, 0)', 'x': 1, 'xanchor': 'right', 'y': 1.02, 'yanchor': 'bottom', "*

 * *             "'font': {'size': 12}}, 'xaxis': {'title': {'font': OrderedDict([('size', 16)])}}, "*

 * *             "'yaxis': {'tit […]*

```diff
@@ -20,45 +20,49 @@
     },
     "layout": {
         "annotationdefaults": {
             "showarrow": false
         },
         "autotypenumbers": "strict",
         "colorway": [
-            "#ffed00",
-            "#ef7d00",
-            "#e4003a",
-            "#c13246",
-            "#822661",
-            "#48277c",
-            "#005ca9",
-            "#00aaff",
-            "#9b30d9",
-            "#af005f",
-            "#5f00af",
-            "#af87ff"
+            "#1f77b4",
+            "#ff7f0e",
+            "#2ca02c",
+            "#d62728",
+            "#9467bd",
+            "#8c564b",
+            "#e377c2",
+            "#bcbd22",
+            "#17becf",
+            "#aec7e8",
+            "#ffbb78",
+            "#ff9896",
+            "#c5b0d5",
+            "#f7b6d2",
+            "#dbdb8d",
+            "#9edae5"
         ],
         "dragmode": "pan",
         "font": {
-            "family": "Fira Code",
+            "family": "Arial",
             "size": 18
         },
         "hoverlabel": {
             "align": "left"
         },
         "hovermode": "x",
         "legend": {
-            "bgcolor": "rgba(0, 0, 0, 0.5)",
+            "bgcolor": "rgba(0, 0, 0, 0)",
             "font": {
-                "size": 15
+                "size": 12
             },
-            "x": 0.01,
-            "xanchor": "left",
-            "y": 0.99,
-            "yanchor": "top"
+            "x": 1,
+            "xanchor": "right",
+            "y": 1.02,
+            "yanchor": "bottom"
         },
         "legend2": {
             "bgcolor": "rgba(0, 0, 0, 0.5)",
             "font": {
                 "size": 15
             }
         },
@@ -97,31 +101,37 @@
             "showline": true,
             "tick0": 1,
             "tickfont": {
                 "size": 14
             },
             "ticks": "outside",
             "title": {
+                "font": {
+                    "size": 16
+                },
                 "standoff": 20
             },
             "zeroline": false
         },
         "yaxis": {
             "anchor": "x",
             "automargin": true,
             "fixedrange": false,
-            "gridcolor": "#283442",
+            "gridcolor": "rgba(128, 128, 128, 0.25)",
             "linecolor": "#F5EFF3",
             "mirror": true,
             "showgrid": true,
             "showline": true,
             "side": "right",
             "tick0": 0.5,
             "ticks": "outside",
             "title": {
+                "font": {
+                    "size": 16
+                },
                 "standoff": 20
             },
             "zeroline": false
         }
     },
     "line": {
         "color": "#ffed00",
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_nightly-4.1.6.dev202404110009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/assets/reference.json` & `openbb_nightly-4.1.6.dev202404110009/openbb/assets/reference.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/__extensions__.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/crypto.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/crypto.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/crypto_price.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/crypto_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/currency.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/currency.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/currency_price.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/currency_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/derivatives.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/derivatives_options.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/derivatives_options.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/economy.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/economy.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/economy_gdp.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/economy_gdp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_calendar.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_compare.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_compare.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_discovery.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_discovery.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_estimates.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_fundamental.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_fundamental.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_price.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/equity_shorts.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/equity_shorts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/etf.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/etf.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_corporate.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome_corporate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_government.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome_government.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_rate.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/fixedincome_spreads.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/fixedincome_spreads.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/index.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/index.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/news.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/openbb/package/regulators_sec.py` & `openbb_nightly-4.1.6.dev202404110009/openbb/package/regulators_sec.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/analyst_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/company_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/price_target.py` & `openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/benzinga/openbb_benzinga/models/world_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/benzinga/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/biztoc/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/models/world_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/biztoc/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/biztoc/openbb_biztoc/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/biztoc/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/index_search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-"""Cboe Available Indices Model."""
+"""CBOE Index Search Model."""
 
 from datetime import time
 from typing import Any, Dict, List, Optional
 
 from openbb_cboe.utils.helpers import get_index_directory
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.available_indices import (
-    AvailableIndicesData,
-    AvailableIndicesQueryParams,
+from openbb_core.provider.standard_models.index_search import (
+    IndexSearchData,
+    IndexSearchQueryParams,
 )
 from pydantic import Field
 
 
-class CboeAvailableIndicesQueryParams(AvailableIndicesQueryParams):
-    """Cboe Available Indices Query.
+class CboeIndexSearchQueryParams(IndexSearchQueryParams):
+    """CBOE Index Search Query.
 
     Source: https://www.cboe.com/
     """
 
     use_cache: bool = Field(
         default=True,
         description="When True, the Cboe Index directory will be cached for 24 hours."
         + " Set as False to bypass.",
     )
 
 
-class CboeAvailableIndicesData(AvailableIndicesData):
-    """Cboe Available Indices Data.
-
-    Source: https://www.cboe.com/
-    """
+class CboeIndexSearchData(IndexSearchData):
+    """CBOE Index Search Data."""
 
     __alias_dict__ = {
         "symbol": "index_symbol",
         "data_delay": "mkt_data_delay",
         "open_time": "calc_start_time",
         "close_time": "calc_end_time",
     }
 
-    symbol: Optional[str] = Field(description="Symbol for the index.")
-
     description: Optional[str] = Field(
-        default=None,
-        description="Description for the index. Valid only for US indices.",
+        description="Description for the index.", default=None
     )
-
     data_delay: Optional[int] = Field(
-        default=None, description="Data delay for the index. Valid only for US indices."
+        description="Data delay for the index. Valid only for US indices.", default=None
+    )
+    currency: Optional[str] = Field(description="Currency for the index.", default=None)
+    time_zone: Optional[str] = Field(
+        description="Time zone for the index. Valid only for US indices.", default=None
     )
-
     open_time: Optional[time] = Field(
-        default=None,
         description="Opening time for the index. Valid only for US indices.",
+        default=None,
     )
-
     close_time: Optional[time] = Field(
-        default=None,
         description="Closing time for the index. Valid only for US indices.",
+        default=None,
     )
-
-    time_zone: Optional[str] = Field(
-        default=None, description="Time zone for the index. Valid only for US indices."
-    )
-
     tick_days: Optional[str] = Field(
-        default=None,
         description="The trading days for the index. Valid only for US indices.",
+        default=None,
     )
-
     tick_frequency: Optional[str] = Field(
+        description="Tick frequency for the index. Valid only for US indices.",
         default=None,
-        description="The frequency of the index ticks. Valid only for US indices.",
     )
-
     tick_period: Optional[str] = Field(
+        description="Tick period for the index. Valid only for US indices.",
         default=None,
-        description="The period of the index ticks. Valid only for US indices.",
     )
 
 
-class CboeAvailableIndicesFetcher(
+class CboeIndexSearchFetcher(
     Fetcher[
-        CboeAvailableIndicesQueryParams,
-        List[CboeAvailableIndicesData],
+        CboeIndexSearchQueryParams,
+        List[CboeIndexSearchData],
     ]
 ):
     """Transform the query, extract and transform the data from the CBOE endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> CboeAvailableIndicesQueryParams:
-        """Transform the query params."""
-        return CboeAvailableIndicesQueryParams(**params)
+    def transform_query(params: Dict[str, Any]) -> CboeIndexSearchQueryParams:
+        """Transform the query."""
+        return CboeIndexSearchQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: CboeAvailableIndicesQueryParams,
+        query: CboeIndexSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the CBOE endpoint."""
 
-        data = await get_index_directory(use_cache=query.use_cache, **kwargs)
-        return data.to_dict("records")
+        symbols = await get_index_directory(use_cache=query.use_cache, **kwargs)
+        symbols.drop(columns=["source"], inplace=True)
+        if query.is_symbol is True:
+            result = symbols[
+                symbols["index_symbol"].str.contains(query.query, case=False)
+            ]
+        else:
+            result = symbols[
+                symbols["name"].str.contains(query.query, case=False)
+                | symbols["index_symbol"].str.contains(query.query, case=False)
+                | symbols["description"].str.contains(query.query, case=False)
+            ]
+
+        return result.to_dict("records")
 
     @staticmethod
     def transform_data(
-        query: CboeAvailableIndicesQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[CboeAvailableIndicesData]:
+        query: CboeIndexSearchQueryParams, data: dict, **kwargs: Any
+    ) -> List[CboeIndexSearchData]:
         """Transform the data to the standard format."""
-        return [CboeAvailableIndicesData.model_validate(d) for d in data]
+        return [CboeIndexSearchData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/index_constituents.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,116 @@
-"""CBOE Index Search Model."""
+"""FMP Index Constituents Model."""
 
-from datetime import time
-from typing import Any, Dict, List, Optional
+from datetime import (
+    date as dateType,
+    datetime,
+)
+from typing import Any, Dict, List, Literal, Optional, Union
 
-from openbb_cboe.utils.helpers import get_index_directory
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.index_search import (
-    IndexSearchData,
-    IndexSearchQueryParams,
+from openbb_core.provider.standard_models.index_constituents import (
+    IndexConstituentsData,
+    IndexConstituentsQueryParams,
 )
-from pydantic import Field
+from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
+from openbb_fmp.utils.helpers import get_data_many
+from pydantic import Field, field_validator
 
 
-class CboeIndexSearchQueryParams(IndexSearchQueryParams):
-    """CBOE Index Search Query.
+class FMPIndexConstituentsQueryParams(IndexConstituentsQueryParams):
+    """FMP Index Constituents Query.
 
-    Source: https://www.cboe.com/
+    Source: https://site.financialmodelingprep.com/developer/docs/list-of-dow-companies-api/
+            https://site.financialmodelingprep.com/developer/docs/list-of-sp-500-companies-api/
+            https://site.financialmodelingprep.com/developer/docs/list-of-nasdaq-companies-api/
     """
 
-    use_cache: bool = Field(
-        default=True,
-        description="When True, the Cboe Index directory will be cached for 24 hours."
-        + " Set as False to bypass.",
+    symbol: Literal["dowjones", "sp500", "nasdaq"] = Field(
+        default="dowjones",
     )
 
 
-class CboeIndexSearchData(IndexSearchData):
-    """CBOE Index Search Data."""
+class FMPIndexConstituentsData(IndexConstituentsData):
+    """FMP Index Constituents Data."""
 
     __alias_dict__ = {
-        "symbol": "index_symbol",
-        "data_delay": "mkt_data_delay",
-        "open_time": "calc_start_time",
-        "close_time": "calc_end_time",
+        "headquarter": "headQuarter",
+        "date_first_added": "dateFirstAdded",
+        "sub_sector": "subSector",
     }
 
-    description: Optional[str] = Field(
-        description="Description for the index.", default=None
-    )
-    data_delay: Optional[int] = Field(
-        description="Data delay for the index. Valid only for US indices.", default=None
-    )
-    currency: Optional[str] = Field(description="Currency for the index.", default=None)
-    time_zone: Optional[str] = Field(
-        description="Time zone for the index. Valid only for US indices.", default=None
+    sector: str = Field(
+        description="Sector the constituent company in the index belongs to."
     )
-    open_time: Optional[time] = Field(
-        description="Opening time for the index. Valid only for US indices.",
+    sub_sector: Optional[str] = Field(
         default=None,
+        description="Sub-sector the constituent company in the index belongs to.",
     )
-    close_time: Optional[time] = Field(
-        description="Closing time for the index. Valid only for US indices.",
+    headquarter: Optional[str] = Field(
         default=None,
+        description="Location of the headquarter of the constituent company in the index.",
     )
-    tick_days: Optional[str] = Field(
-        description="The trading days for the index. Valid only for US indices.",
-        default=None,
+    date_first_added: Optional[Union[dateType, str]] = Field(
+        default=None, description="Date the constituent company was added to the index."
     )
-    tick_frequency: Optional[str] = Field(
-        description="Tick frequency for the index. Valid only for US indices.",
-        default=None,
+    cik: Optional[int] = Field(
+        description=DATA_DESCRIPTIONS.get("cik", ""), default=None
     )
-    tick_period: Optional[str] = Field(
-        description="Tick period for the index. Valid only for US indices.",
+    founded: Optional[Union[dateType, str]] = Field(
         default=None,
+        description="Founding year of the constituent company in the index.",
     )
 
+    @field_validator("dateFirstAdded", mode="before", check_fields=False)
+    @classmethod
+    def date_first_added_validate(cls, v):  # pylint: disable=E0213
+        """Return the date_first_added date as a datetime object for valid cases."""
+        try:
+            return datetime.strptime(v, "%Y-%m-%d") if v else None
+        except Exception:
+            # For returning string in case of mismatched dates
+            return v
+
+    @field_validator("founded", mode="before", check_fields=False)
+    @classmethod
+    def founded_validate(cls, v):  # pylint: disable=E0213
+        """Return the founded date as a datetime object for valid cases."""
+        try:
+            return datetime.strptime(v, "%Y-%m-%d") if v else None
+        except Exception:
+            # For returning string in case of mismatched dates
+            return v
+
 
-class CboeIndexSearchFetcher(
+class FMPIndexConstituentsFetcher(
     Fetcher[
-        CboeIndexSearchQueryParams,
-        List[CboeIndexSearchData],
+        FMPIndexConstituentsQueryParams,
+        List[FMPIndexConstituentsData],
     ]
 ):
-    """Transform the query, extract and transform the data from the CBOE endpoints."""
+    """Transform the query, extract and transform the data from the FMP endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> CboeIndexSearchQueryParams:
-        """Transform the query."""
-        return CboeIndexSearchQueryParams(**params)
+    def transform_query(params: Dict[str, Any]) -> FMPIndexConstituentsQueryParams:
+        """Transform the query params."""
+        return FMPIndexConstituentsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: CboeIndexSearchQueryParams,
+        query: FMPIndexConstituentsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Return the raw data from the CBOE endpoint."""
+        """Return the raw data from the FMP endpoint."""
+        api_key = credentials.get("fmp_api_key") if credentials else ""
 
-        symbols = await get_index_directory(use_cache=query.use_cache, **kwargs)
-        symbols.drop(columns=["source"], inplace=True)
-        if query.is_symbol is True:
-            result = symbols[
-                symbols["index_symbol"].str.contains(query.query, case=False)
-            ]
-        else:
-            result = symbols[
-                symbols["name"].str.contains(query.query, case=False)
-                | symbols["index_symbol"].str.contains(query.query, case=False)
-                | symbols["description"].str.contains(query.query, case=False)
-            ]
+        base_url = "https://financialmodelingprep.com/api/v3"
+        url = f"{base_url}/{query.symbol}_constituent/?apikey={api_key}"
 
-        return result.to_dict("records")
+        return await get_data_many(url, **kwargs)
 
     @staticmethod
     def transform_data(
-        query: CboeIndexSearchQueryParams, data: dict, **kwargs: Any
-    ) -> List[CboeIndexSearchData]:
-        """Transform the data to the standard format."""
-        return [CboeIndexSearchData.model_validate(d) for d in data]
+        query: FMPIndexConstituentsQueryParams, data: List[Dict], **kwargs: Any
+    ) -> List[FMPIndexConstituentsData]:
+        """Return the raw data from the FMP endpoint."""
+        return [FMPIndexConstituentsData.model_validate(d) for d in data]
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/cboe/openbb_cboe/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/cboe/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/balance_of_payments.py` & `openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/currency_reference_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/models/eu_yield_curve.py` & `openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/bps_series.py` & `openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/ecb_helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/ecb/openbb_ecb/utils/yield_curve_series.py` & `openbb_nightly-4.1.6.dev202404110009/providers/ecb/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/federal_reserve/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py` & `openbb_nightly-4.1.6.dev202404110009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/models/equity_short_interest.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/models/otc_aggregate.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/utils/data_storage.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finra/openbb_finra/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finra/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/compare_groups.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/price_performance.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/models/price_target.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/finviz/openbb_finviz/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404110009/providers/finviz/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/analyst_estimates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/calendar_splits.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/cash_flow_growth.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/company_overview.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/crypto_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/currency_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/discovery_filings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_peers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_screener.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings_date.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/executive_compensation.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_employees.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/historical_splits.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/income_statement_growth.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/key_executives.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_performance.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_target.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/revenue_business_line.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/revenue_geographic.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/risk_premium.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/models/world_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fmp/openbb_fmp/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fmp/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ameribor_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/cp.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/cpi.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/dwpcr_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ecb_interest_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/estr_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/fed_projections.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ffrmc.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/hqm.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/ice_bofa.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/iorb_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/moody.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/regional.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/series.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/sofr_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/sonia_rates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/spot.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/tbffr.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/tmc.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/models/us_yield_curve.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/commercial_paper.csv` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/cpi.csv` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/fred_base.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/fred_helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/harmonized_cpi.csv` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_nightly-4.1.6.dev202404110009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/treasury_auctions.py` & `openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/government_us/openbb_government_us/models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/government_us/openbb_government_us/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/company_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_info.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/financial_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/fred_series.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/historical_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/latest_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/options_unusual.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/reported_financials.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/search_attributes.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/models/world_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/intrinio/openbb_intrinio/utils/references.py` & `openbb_nightly-4.1.6.dev202404110009/providers/intrinio/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/cot.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/cot_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/models/top_retail.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/query_params.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py` & `openbb_nightly-4.1.6.dev202404110009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_forecast.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_nominal.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/gdp_real.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/models/unemployment.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/utils/constants.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/oecd/openbb_oecd/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/oecd/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/company_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/equity_nbbo.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/polygon/openbb_polygon/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/polygon/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/cik_map.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/equity_ftd.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/form_13FHR.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/institutions_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/rss_litigation.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/schema_files.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/sic_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/models/symbol_map.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/sec/openbb_sec/utils/parse_13f.py` & `openbb_nightly-4.1.6.dev202404110009/providers/sec/openbb_sec/utils/parse_13f.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_nightly-4.1.6.dev202404110009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/stockgrid/openbb_stockgrid/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/stockgrid/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/stockgrid/openbb_stockgrid/models/short_volume.py` & `openbb_nightly-4.1.6.dev202404110009/providers/stockgrid/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/company_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/models/world_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tiingo/openbb_tiingo/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tiingo/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/bond_prices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/company_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/gainers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_sectors.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/gql.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tmx/openbb_tmx/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tmx/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradier/openbb_tradier/utils/constants.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradier/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py` & `openbb_nightly-4.1.6.dev202404110009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/wsj/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/active.py` & `openbb_nightly-4.1.6.dev202404110009/providers/wsj/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/gainers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/wsj/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/wsj/openbb_wsj/models/losers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/wsj/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/__init__.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/active.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/company_news.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/equity_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """YFinance Equity Profile Model."""
 
 # pylint: disable=unused-argument
 import asyncio
 import warnings
-from datetime import datetime
+from datetime import (
+    date as dateType,
+    timezone,
+)
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_info import (
     EquityInfoData,
     EquityInfoQueryParams,
 )
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from pydantic import Field, field_validator
 from yfinance import Ticker
 
 _warn = warnings.warn
 
 
 class YFinanceEquityProfileQueryParams(EquityInfoQueryParams):
@@ -93,17 +97,17 @@
     beta: Optional[float] = Field(
         description="The beta of the asset relative to the broad market.",
         default=None,
     )
 
     @field_validator("first_stock_price_date", mode="before", check_fields=False)
     @classmethod
-    def validate_first_trade_date(cls, v):
+    def validate_first_trade_date(cls, v: float) -> Optional[dateType]:
         """Validate first stock price date."""
-        return datetime.utcfromtimestamp(v).date() if v else None
+        return safe_fromtimestamp(v, tz=timezone.utc).date() if v else None
 
 
 class YFinanceEquityProfileFetcher(
     Fetcher[YFinanceEquityProfileQueryParams, List[YFinanceEquityProfileData]]
 ):
     """YFinance Equity Profile fetcher."""
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/etf_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/futures_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/gainers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/key_executives.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/losers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/futures.csv` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/providers/yfinance/openbb_yfinance/utils/references.py` & `openbb_nightly-4.1.6.dev202404110009/providers/yfinance/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404100009/pyproject.toml` & `openbb_nightly-4.1.6.dev202404110009/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openbb-nightly"
-version = "4.1.6.dev202404100009"
+version = "4.1.6.dev202404110009"
 description = "OpenBB"
 authors = [ "OpenBB Team <hello@openbb.co>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "openbb"
 
 [[tool.poetry.packages]]
```

### Comparing `openbb_nightly-4.1.6.dev202404100009/PKG-INFO` & `openbb_nightly-4.1.6.dev202404110009/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 4.1.6.dev202404100009
+Version: 4.1.6.dev202404110009
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


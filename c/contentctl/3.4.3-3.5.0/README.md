# Comparing `tmp/contentctl-3.4.3.tar.gz` & `tmp/contentctl-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentctl-3.4.3.tar", max compression
+gzip compressed data, was "contentctl-3.5.0.tar", max compression
```

## Comparing `contentctl-3.4.3.tar` & `contentctl-3.5.0.tar`

### file list

```diff
@@ -1,175 +1,175 @@
--rw-r--r--   0        0        0    11344 2024-04-12 17:30:51.165243 contentctl-3.4.3/LICENSE.md
--rw-r--r--   0        0        0    17550 2024-04-12 17:30:51.165243 contentctl-3.4.3/README.md
--rw-r--r--   0        0        0       22 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/__init__.py
--rw-r--r--   0        0        0     1418 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/acs_deploy.py
--rw-r--r--   0        0        0     2999 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/apav_deploy.py
--rw-r--r--   0        0        0     6965 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/api_deploy.py
--rw-r--r--   0        0        0      704 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/convert.py
--rw-r--r--   0        0        0     5580 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/DataManipulation.py
--rw-r--r--   0        0        0     7257 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/DetectionTestingManager.py
--rw-r--r--   0        0        0    11155 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/GitService.py
--rw-r--r--   0        0        0     2259 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
--rw-r--r--   0        0        0    53520 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
--rw-r--r--   0        0        0     5327 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
--rw-r--r--   0        0        0      370 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
--rw-r--r--   0        0        0     3244 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/progress_bar.py
--rw-r--r--   0        0        0     6106 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/views/DetectionTestingView.py
--rw-r--r--   0        0        0     2050 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
--rw-r--r--   0        0        0     1386 2024-04-12 17:30:51.165243 contentctl-3.4.3/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
--rw-r--r--   0        0        0     4706 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
--rw-r--r--   0        0        0      857 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/doc_gen.py
--rw-r--r--   0        0        0     5273 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/generate.py
--rw-r--r--   0        0        0     3102 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/initialize.py
--rw-r--r--   0        0        0     9333 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/initialize_old.py
--rw-r--r--   0        0        0      992 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/new_content.py
--rw-r--r--   0        0        0     8637 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/release_notes.py
--rw-r--r--   0        0        0     1102 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/reporting.py
--rw-r--r--   0        0        0     3863 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/test.py
--rw-r--r--   0        0        0     2595 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/actions/validate.py
--rw-r--r--   0        0        0    31622 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/contentctl.py
--rw-r--r--   0        0        0     4392 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/enrichments/attack_enrichment.py
--rw-r--r--   0        0        0     3242 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/enrichments/cve_enrichment.py
--rw-r--r--   0        0        0     3418 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/enrichments/splunk_app_enrichment.py
--rw-r--r--   0        0        0     3032 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/helper/config_handler.py
--rw-r--r--   0        0        0     7238 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/helper/link_validator.py
--rw-r--r--   0        0        0        0 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/helper/logger.py
--rw-r--r--   0        0        0    15577 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/helper/utils.py
--rw-r--r--   0        0        0     5861 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/backend_splunk_ba.py
--rw-r--r--   0        0        0     2472 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/baseline_builder.py
--rw-r--r--   0        0        0     2270 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/basic_builder.py
--rw-r--r--   0        0        0    17905 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/detection_builder.py
--rw-r--r--   0        0        0    12666 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/director.py
--rw-r--r--   0        0        0     1244 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/investigation_builder.py
--rw-r--r--   0        0        0     4979 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/new_content_generator.py
--rw-r--r--   0        0        0     5610 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/new_content_questions.py
--rw-r--r--   0        0        0     2100 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/playbook_builder.py
--rw-r--r--   0        0        0    19074 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/sigma_converter.py
--rw-r--r--   0        0        0     7584 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/ssa_detection_builder.py
--rw-r--r--   0        0        0     4755 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/story_builder.py
--rw-r--r--   0        0        0     1385 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/input/yml_reader.py
--rw-r--r--   0        0        0    12594 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/abstract_security_content_objects/detection_abstract.py
--rw-r--r--   0        0        0     3015 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
--rw-r--r--   0        0        0     7519 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/app.py
--rw-r--r--   0        0        0     1028 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/base_test.py
--rw-r--r--   0        0        0     4752 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/base_test_result.py
--rw-r--r--   0        0        0     1931 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/baseline.py
--rw-r--r--   0        0        0      711 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/baseline_tags.py
--rw-r--r--   0        0        0     6069 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/config.py
--rw-r--r--   0        0        0     3518 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/constants.py
--rw-r--r--   0        0        0    36903 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/correlation_search.py
--rw-r--r--   0        0        0      434 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/data_source.py
--rw-r--r--   0        0        0     1137 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/deployment.py
--rw-r--r--   0        0        0      141 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/deployment_email.py
--rw-r--r--   0        0        0      164 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/deployment_notable.py
--rw-r--r--   0        0        0      201 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/deployment_phantom.py
--rw-r--r--   0        0        0      111 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/deployment_rba.py
--rw-r--r--   0        0        0      193 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/deployment_scheduling.py
--rw-r--r--   0        0        0      129 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/deployment_slack.py
--rw-r--r--   0        0        0     1849 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/detection.py
--rw-r--r--   0        0        0     6338 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/detection_tags.py
--rw-r--r--   0        0        0     2963 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/enums.py
--rw-r--r--   0        0        0     1285 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/integration_test.py
--rw-r--r--   0        0        0      429 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/integration_test_result.py
--rw-r--r--   0        0        0     2151 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/investigation.py
--rw-r--r--   0        0        0      191 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/investigation_tags.py
--rw-r--r--   0        0        0     2397 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/lookup.py
--rw-r--r--   0        0        0     3255 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/macro.py
--rw-r--r--   0        0        0      219 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/mitre_attack_enrichment.py
--rw-r--r--   0        0        0     1605 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/notable_action.py
--rw-r--r--   0        0        0     1288 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/observable.py
--rw-r--r--   0        0        0     1081 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/playbook.py
--rw-r--r--   0        0        0      315 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/playbook_tags.py
--rw-r--r--   0        0        0     6353 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/repo_config.py
--rw-r--r--   0        0        0     4288 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/risk_analysis_action.py
--rw-r--r--   0        0        0      904 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/risk_object.py
--rw-r--r--   0        0        0      325 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/security_content_object.py
--rw-r--r--   0        0        0     5806 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/ssa_detection.py
--rw-r--r--   0        0        0     5668 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/ssa_detection_tags.py
--rw-r--r--   0        0        0     1532 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/story.py
--rw-r--r--   0        0        0     1213 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/story_tags.py
--rw-r--r--   0        0        0    25020 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/test_config.py
--rw-r--r--   0        0        0     2600 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/test_group.py
--rw-r--r--   0        0        0      711 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/threat_object.py
--rw-r--r--   0        0        0     1412 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/unit_test.py
--rw-r--r--   0        0        0      606 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/unit_test_attack_data.py
--rw-r--r--   0        0        0      255 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/unit_test_baseline.py
--rw-r--r--   0        0        0      182 2024-04-12 17:30:51.169243 contentctl-3.4.3/contentctl/objects/unit_test_old.py
--rw-r--r--   0        0        0     2598 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/objects/unit_test_result.py
--rw-r--r--   0        0        0     6174 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/api_json_output.py
--rw-r--r--   0        0        0     1701 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/attack_nav_output.py
--rw-r--r--   0        0        0     2130 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/attack_nav_writer.py
--rw-r--r--   0        0        0     5938 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/ba_yml_output.py
--rw-r--r--   0        0        0    24175 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/conf_output.py
--rw-r--r--   0        0        0     2960 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/conf_writer.py
--rw-r--r--   0        0        0      960 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/detection_writer.py
--rw-r--r--   0        0        0     3238 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/doc_md_output.py
--rw-r--r--   0        0        0     3935 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/finding_report_writer.py
--rw-r--r--   0        0        0     1089 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/jinja_writer.py
--rw-r--r--   0        0        0      209 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/json_writer.py
--rw-r--r--   0        0        0     2254 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/new_content_yml_output.py
--rw-r--r--   0        0        0     3084 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/svg_output.py
--rw-r--r--   0        0        0      745 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/analyticstories_detections.j2
--rw-r--r--   0        0        0      496 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/analyticstories_investigations.j2
--rw-r--r--   0        0        0      592 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/analyticstories_stories.j2
--rw-r--r--   0        0        0      717 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/app.conf.j2
--rw-r--r--   0        0        0     1047 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/app.manifest.j2
--rw-r--r--   0        0        0      181 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/collections.j2
--rw-r--r--   0        0        0       54 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/content-version.j2
--rw-r--r--   0        0        0      670 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/detection_count.j2
--rw-r--r--   0        0        0      671 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/detection_coverage.j2
--rw-r--r--   0        0        0     1002 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/doc_detection_page.j2
--rw-r--r--   0        0        0     6586 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/doc_detections.j2
--rw-r--r--   0        0        0     1471 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/doc_navigation.j2
--rw-r--r--   0        0        0      203 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/doc_navigation_pages.j2
--rw-r--r--   0        0        0     1681 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/doc_playbooks.j2
--rw-r--r--   0        0        0      679 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/doc_playbooks_page.j2
--rw-r--r--   0        0        0     1822 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/doc_stories.j2
--rw-r--r--   0        0        0      874 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/doc_story_page.j2
--rw-r--r--   0        0        0      994 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/es_investigations_investigations.j2
--rw-r--r--   0        0        0      369 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/es_investigations_stories.j2
--rw-r--r--   0        0        0     1753 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/finding_report.j2
--rw-r--r--   0        0        0      177 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/header.j2
--rw-r--r--   0        0        0      424 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/macros.j2
--rw-r--r--   0        0        0      282 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/macros_detections.j2
--rw-r--r--   0        0        0      221 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/panel.j2
--rw-r--r--   0        0        0     1645 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/savedsearches_baselines.j2
--rw-r--r--   0        0        0     6213 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/savedsearches_detections.j2
--rw-r--r--   0        0        0     1180 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/savedsearches_investigations.j2
--rw-r--r--   0        0        0      897 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt
--rw-r--r--   0        0        0     2538 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/README/essoc_summary.txt
--rw-r--r--   0        0        0     2432 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt
--rw-r--r--   0        0        0      467 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/README.md
--rw-r--r--   0        0        0      168 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/analytic_stories.conf
--rw-r--r--   0        0        0      685 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/app.conf
--rw-r--r--   0        0        0      319 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/commands.conf
--rw-r--r--   0        0        0       34 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/content-version.conf
--rw-r--r--   0        0        0      208 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/data/ui/nav/default.xml
--rw-r--r--   0        0        0     8635 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml
--rw-r--r--   0        0        0      696 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml
--rw-r--r--   0        0        0      156 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/distsearch.conf
--rw-r--r--   0        0        0     4257 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/usage_searches.conf
--rw-r--r--   0        0        0      168 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/default/use_case_library.conf
--rw-r--r--   0        0        0      423 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/metadata/default.meta
--rw-r--r--   0        0        0     3658 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/static/appIcon.png
--rw-r--r--   0        0        0     2656 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/static/appIconAlt.png
--rw-r--r--   0        0        0     7442 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png
--rw-r--r--   0        0        0     3657 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/splunk_app/static/appIcon_2x.png
--rw-r--r--   0        0        0     1416 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/transforms.j2
--rw-r--r--   0        0        0      925 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/templates/workflow_actions.j2
--rw-r--r--   0        0        0     2682 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/yml_output.py
--rw-r--r--   0        0        0      240 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/output/yml_writer.py
--rw-r--r--   0        0        0      133 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/README
--rw-r--r--   0        0        0     6390 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/app_default.yml
--rw-r--r--   0        0        0     9381 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/datamodels_cim.conf
--rw-r--r--   0        0        0      480 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/datamodels_custom.conf
--rw-r--r--   0        0        0      426 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/deployments/00_default_anomaly.yml
--rw-r--r--   0        0        0      342 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/deployments/00_default_baseline.yml
--rw-r--r--   0        0        0      528 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/deployments/00_default_correlation.yml
--rw-r--r--   0        0        0      336 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/deployments/00_default_hunting.yml
--rw-r--r--   0        0        0      556 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/deployments/00_default_ttp.yml
--rw-r--r--   0        0        0     3342 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/detections/anomalous_usage_of_7zip.yml
--rw-r--r--   0        0        0      159 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/macros/security_content_ctime.yml
--rw-r--r--   0        0        0      162 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/macros/security_content_summariesonly.yml
--rw-r--r--   0        0        0     3095 2024-04-12 17:30:51.173243 contentctl-3.4.3/contentctl/templates/stories/cobalt_strike.yml
--rw-r--r--   0        0        0      815 2024-04-12 17:30:51.173243 contentctl-3.4.3/pyproject.toml
--rw-r--r--   0        0        0    18805 1970-01-01 00:00:00.000000 contentctl-3.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-12 17:31:40.635777 contentctl-3.5.0/LICENSE.md
+-rw-r--r--   0        0        0    17550 2024-04-12 17:31:40.635777 contentctl-3.5.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/__init__.py
+-rw-r--r--   0        0        0     1418 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/acs_deploy.py
+-rw-r--r--   0        0        0     2999 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/apav_deploy.py
+-rw-r--r--   0        0        0     6965 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/api_deploy.py
+-rw-r--r--   0        0        0      704 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/convert.py
+-rw-r--r--   0        0        0     5580 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/DataManipulation.py
+-rw-r--r--   0        0        0     7257 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/DetectionTestingManager.py
+-rw-r--r--   0        0        0    11155 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/GitService.py
+-rw-r--r--   0        0        0     2259 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
+-rw-r--r--   0        0        0    53389 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
+-rw-r--r--   0        0        0     5327 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
+-rw-r--r--   0        0        0      370 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
+-rw-r--r--   0        0        0     3244 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/progress_bar.py
+-rw-r--r--   0        0        0     7015 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingView.py
+-rw-r--r--   0        0        0     2050 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
+-rw-r--r--   0        0        0     1386 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
+-rw-r--r--   0        0        0     4706 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
+-rw-r--r--   0        0        0      857 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/doc_gen.py
+-rw-r--r--   0        0        0     5273 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/generate.py
+-rw-r--r--   0        0        0     3102 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/initialize.py
+-rw-r--r--   0        0        0     9333 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/initialize_old.py
+-rw-r--r--   0        0        0      992 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/new_content.py
+-rw-r--r--   0        0        0    10193 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/actions/release_notes.py
+-rw-r--r--   0        0        0     1102 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/actions/reporting.py
+-rw-r--r--   0        0        0     3863 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/actions/test.py
+-rw-r--r--   0        0        0     2595 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/actions/validate.py
+-rw-r--r--   0        0        0    31622 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/contentctl.py
+-rw-r--r--   0        0        0     4392 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/enrichments/attack_enrichment.py
+-rw-r--r--   0        0        0     3242 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/enrichments/cve_enrichment.py
+-rw-r--r--   0        0        0     3418 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/enrichments/splunk_app_enrichment.py
+-rw-r--r--   0        0        0     3032 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/helper/config_handler.py
+-rw-r--r--   0        0        0     7238 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/helper/link_validator.py
+-rw-r--r--   0        0        0        0 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/helper/logger.py
+-rw-r--r--   0        0        0    15577 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/helper/utils.py
+-rw-r--r--   0        0        0     5861 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/backend_splunk_ba.py
+-rw-r--r--   0        0        0     2472 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/baseline_builder.py
+-rw-r--r--   0        0        0     2270 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/basic_builder.py
+-rw-r--r--   0        0        0    18813 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/detection_builder.py
+-rw-r--r--   0        0        0    13161 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/director.py
+-rw-r--r--   0        0        0     1244 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/investigation_builder.py
+-rw-r--r--   0        0        0     4979 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/new_content_generator.py
+-rw-r--r--   0        0        0     5610 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/new_content_questions.py
+-rw-r--r--   0        0        0     2100 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/playbook_builder.py
+-rw-r--r--   0        0        0    19512 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/sigma_converter.py
+-rw-r--r--   0        0        0     7584 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/ssa_detection_builder.py
+-rw-r--r--   0        0        0     4755 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/story_builder.py
+-rw-r--r--   0        0        0     1385 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/yml_reader.py
+-rw-r--r--   0        0        0    15069 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/abstract_security_content_objects/detection_abstract.py
+-rw-r--r--   0        0        0     3015 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
+-rw-r--r--   0        0        0     7519 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/app.py
+-rw-r--r--   0        0        0     1028 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/base_test.py
+-rw-r--r--   0        0        0     4752 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/base_test_result.py
+-rw-r--r--   0        0        0     1931 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/baseline.py
+-rw-r--r--   0        0        0      711 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/baseline_tags.py
+-rw-r--r--   0        0        0     6069 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/config.py
+-rw-r--r--   0        0        0     3518 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/constants.py
+-rw-r--r--   0        0        0    36903 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/correlation_search.py
+-rw-r--r--   0        0        0      434 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/data_source.py
+-rw-r--r--   0        0        0     1137 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment.py
+-rw-r--r--   0        0        0      141 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_email.py
+-rw-r--r--   0        0        0      164 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_notable.py
+-rw-r--r--   0        0        0      201 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_phantom.py
+-rw-r--r--   0        0        0      111 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_rba.py
+-rw-r--r--   0        0        0      193 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_scheduling.py
+-rw-r--r--   0        0        0      129 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_slack.py
+-rw-r--r--   0        0        0      644 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/detection.py
+-rw-r--r--   0        0        0     6338 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/detection_tags.py
+-rw-r--r--   0        0        0     2963 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/enums.py
+-rw-r--r--   0        0        0     1285 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/integration_test.py
+-rw-r--r--   0        0        0      429 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/integration_test_result.py
+-rw-r--r--   0        0        0     2151 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/investigation.py
+-rw-r--r--   0        0        0      191 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/investigation_tags.py
+-rw-r--r--   0        0        0     2397 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/lookup.py
+-rw-r--r--   0        0        0     3255 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/macro.py
+-rw-r--r--   0        0        0      219 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/mitre_attack_enrichment.py
+-rw-r--r--   0        0        0     1605 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/notable_action.py
+-rw-r--r--   0        0        0     1288 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/observable.py
+-rw-r--r--   0        0        0     1081 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/playbook.py
+-rw-r--r--   0        0        0      315 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/playbook_tags.py
+-rw-r--r--   0        0        0     6353 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/repo_config.py
+-rw-r--r--   0        0        0     4288 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/risk_analysis_action.py
+-rw-r--r--   0        0        0      904 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/risk_object.py
+-rw-r--r--   0        0        0      325 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/security_content_object.py
+-rw-r--r--   0        0        0     5806 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/ssa_detection.py
+-rw-r--r--   0        0        0     5668 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/ssa_detection_tags.py
+-rw-r--r--   0        0        0     1532 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/story.py
+-rw-r--r--   0        0        0     1213 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/story_tags.py
+-rw-r--r--   0        0        0    25020 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/test_config.py
+-rw-r--r--   0        0        0     2600 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/test_group.py
+-rw-r--r--   0        0        0      711 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/threat_object.py
+-rw-r--r--   0        0        0     1412 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test.py
+-rw-r--r--   0        0        0      606 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test_attack_data.py
+-rw-r--r--   0        0        0      255 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test_baseline.py
+-rw-r--r--   0        0        0      182 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test_old.py
+-rw-r--r--   0        0        0     2874 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test_result.py
+-rw-r--r--   0        0        0     6174 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/api_json_output.py
+-rw-r--r--   0        0        0     1701 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/attack_nav_output.py
+-rw-r--r--   0        0        0     2130 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/attack_nav_writer.py
+-rw-r--r--   0        0        0     5938 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/ba_yml_output.py
+-rw-r--r--   0        0        0    24175 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/conf_output.py
+-rw-r--r--   0        0        0     2960 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/conf_writer.py
+-rw-r--r--   0        0        0      960 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/detection_writer.py
+-rw-r--r--   0        0        0     3238 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/doc_md_output.py
+-rw-r--r--   0        0        0     3935 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/finding_report_writer.py
+-rw-r--r--   0        0        0     1089 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/jinja_writer.py
+-rw-r--r--   0        0        0      209 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/json_writer.py
+-rw-r--r--   0        0        0     2254 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/new_content_yml_output.py
+-rw-r--r--   0        0        0     3084 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/svg_output.py
+-rw-r--r--   0        0        0      745 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/analyticstories_detections.j2
+-rw-r--r--   0        0        0      496 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/analyticstories_investigations.j2
+-rw-r--r--   0        0        0      592 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/analyticstories_stories.j2
+-rw-r--r--   0        0        0      717 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/app.conf.j2
+-rw-r--r--   0        0        0     1047 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/app.manifest.j2
+-rw-r--r--   0        0        0      181 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/collections.j2
+-rw-r--r--   0        0        0       54 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/content-version.j2
+-rw-r--r--   0        0        0      670 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/detection_count.j2
+-rw-r--r--   0        0        0      671 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/detection_coverage.j2
+-rw-r--r--   0        0        0     1002 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_detection_page.j2
+-rw-r--r--   0        0        0     6586 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_detections.j2
+-rw-r--r--   0        0        0     1471 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_navigation.j2
+-rw-r--r--   0        0        0      203 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_navigation_pages.j2
+-rw-r--r--   0        0        0     1681 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_playbooks.j2
+-rw-r--r--   0        0        0      679 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_playbooks_page.j2
+-rw-r--r--   0        0        0     1822 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_stories.j2
+-rw-r--r--   0        0        0      874 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_story_page.j2
+-rw-r--r--   0        0        0      994 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/es_investigations_investigations.j2
+-rw-r--r--   0        0        0      369 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/es_investigations_stories.j2
+-rw-r--r--   0        0        0     1753 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/finding_report.j2
+-rw-r--r--   0        0        0      177 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/header.j2
+-rw-r--r--   0        0        0      424 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/macros.j2
+-rw-r--r--   0        0        0      282 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/macros_detections.j2
+-rw-r--r--   0        0        0      221 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/panel.j2
+-rw-r--r--   0        0        0     1645 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/savedsearches_baselines.j2
+-rw-r--r--   0        0        0     6213 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/savedsearches_detections.j2
+-rw-r--r--   0        0        0     1180 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/savedsearches_investigations.j2
+-rw-r--r--   0        0        0      897 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt
+-rw-r--r--   0        0        0     2538 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_summary.txt
+-rw-r--r--   0        0        0     2432 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt
+-rw-r--r--   0        0        0      467 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/README.md
+-rw-r--r--   0        0        0      168 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/analytic_stories.conf
+-rw-r--r--   0        0        0      685 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/app.conf
+-rw-r--r--   0        0        0      319 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/commands.conf
+-rw-r--r--   0        0        0       34 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/content-version.conf
+-rw-r--r--   0        0        0      208 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/nav/default.xml
+-rw-r--r--   0        0        0     8635 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml
+-rw-r--r--   0        0        0      696 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml
+-rw-r--r--   0        0        0      156 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/distsearch.conf
+-rw-r--r--   0        0        0     4257 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/usage_searches.conf
+-rw-r--r--   0        0        0      168 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/use_case_library.conf
+-rw-r--r--   0        0        0      423 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/metadata/default.meta
+-rw-r--r--   0        0        0     3658 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIcon.png
+-rw-r--r--   0        0        0     2656 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIconAlt.png
+-rw-r--r--   0        0        0     7442 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png
+-rw-r--r--   0        0        0     3657 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png
+-rw-r--r--   0        0        0     1416 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/transforms.j2
+-rw-r--r--   0        0        0      925 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/workflow_actions.j2
+-rw-r--r--   0        0        0     2682 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/yml_output.py
+-rw-r--r--   0        0        0      240 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/yml_writer.py
+-rw-r--r--   0        0        0      133 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/README
+-rw-r--r--   0        0        0     6390 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/app_default.yml
+-rw-r--r--   0        0        0     9381 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/datamodels_cim.conf
+-rw-r--r--   0        0        0      480 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/datamodels_custom.conf
+-rw-r--r--   0        0        0      426 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_anomaly.yml
+-rw-r--r--   0        0        0      342 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_baseline.yml
+-rw-r--r--   0        0        0      528 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_correlation.yml
+-rw-r--r--   0        0        0      336 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_hunting.yml
+-rw-r--r--   0        0        0      556 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_ttp.yml
+-rw-r--r--   0        0        0     3342 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml
+-rw-r--r--   0        0        0      159 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/macros/security_content_ctime.yml
+-rw-r--r--   0        0        0      162 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/macros/security_content_summariesonly.yml
+-rw-r--r--   0        0        0     3095 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/stories/cobalt_strike.yml
+-rw-r--r--   0        0        0      815 2024-04-12 17:31:40.643777 contentctl-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18805 1970-01-01 00:00:00.000000 contentctl-3.5.0/PKG-INFO
```

### Comparing `contentctl-3.4.3/LICENSE.md` & `contentctl-3.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/README.md` & `contentctl-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/acs_deploy.py` & `contentctl-3.5.0/contentctl/actions/acs_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/apav_deploy.py` & `contentctl-3.5.0/contentctl/actions/apav_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/api_deploy.py` & `contentctl-3.5.0/contentctl/actions/api_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/convert.py` & `contentctl-3.5.0/contentctl/actions/convert.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/DataManipulation.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/DataManipulation.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/DetectionTestingManager.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/DetectionTestingManager.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/GitService.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/GitService.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/generate_detection_coverage_badge.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,23 +410,20 @@
     def test_detection(self, detection: Detection) -> None:
         """
         Tests a single detection; iterates over the TestGroups for the detection (one TestGroup per
         unit test, where a TestGroup is a unit test and integration test relying on the same attack
         data)
         :param detection: the Detection to test
         """
-        # TODO: do we want to return a failure here if no test exists for a production detection?
-        # Log and return if no tests exist
-        if detection.tests is None:
-            self.pbar.write(f"No test(s) found for {detection.name}")
-            return
 
         # iterate TestGroups
         for test_group in detection.test_groups:
-            # If all tests in the group have been skipped, report and continue
+            # If all tests in the group have been skipped, report and continue.
+            # Note that the logic for skipping tests for detections tagged manual_test exists in
+            # the detection builder.
             if test_group.all_tests_skipped():
                 self.pbar.write(
                     self.format_pbar_string(
                         TestReportingType.GROUP,
                         test_group.name,
                         FinalTestingStates.SKIP.value,
                         time.time(),
```

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/progress_bar.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/progress_bar.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/views/DetectionTestingView.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingView.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,33 +80,45 @@
         :param test_job_fields: fields to pull from the job content of the test result
         :returns: summary dict
         """
         # Init the list of tested detections, and some metrics aggregate counters
         tested_detections = []
         total_pass = 0
         total_fail = 0
+        total_skipped = 0
 
         # Iterate the detections tested (anything in the output queue was tested)
         for detection in self.sync_obj.outputQueue:
             # Get a summary dict of the testing of the detection
             summary = detection.get_summary(
                 test_job_fields=test_job_fields, test_result_fields=test_result_fields
             )
 
             # Aggregate detection pass/fail metrics
-            if summary["success"] is True:
-                total_pass += 1
-            else:
+            if summary["success"] is False:
                 total_fail += 1
+            else:
+                #Test is marked as a success, but we need to determine if there were skipped unit tests
+                #SKIPPED tests still show a success in this field, but we want to count them differently
+                pass_increment = 1
+                for test in summary.get("tests"):
+                    if test.get("test_type") == "unit" and test.get("status") == "skip":
+                        total_skipped += 1
+                        #Test should not count as a pass, so do not increment the count
+                        pass_increment = 0
+                        break
+                total_pass += pass_increment
+                
 
             # Append to our list
             tested_detections.append(summary)
 
         # Sort s.t. all failures appear first (then by name)
-        tested_detections.sort(key=lambda x: (x["success"], x["name"]))
+        #Second short condition is a hack to get detections with unit skipped tests to appear above pass tests
+        tested_detections.sort(key=lambda x: (x["success"], 0 if x.get("tests",[{}])[0].get("status","status_missing")=="skip" else 1, x["name"]))
 
         # Aggregate summaries for the untested detections (anything still in the input queue was untested)
         total_untested = len(self.sync_obj.inputQueue)
         untested_detections = []
         for detection in self.sync_obj.inputQueue:
             untested_detections.append(detection.get_summary())
 
@@ -124,35 +136,37 @@
         # If any detection failed, the overall success is False
         if (total_fail + len(untested_detections)) == 0:
             overall_success = True
         else:
             overall_success = False
 
         # Compute total detections
-        total_detections = total_fail + total_pass + total_untested
+        total_detections = total_fail + total_pass + total_untested + total_skipped
+
 
         # Compute the percentage of completion for testing, as well as the success rate
         percent_complete = Utils.getPercent(
             len(tested_detections), len(untested_detections), 1
         )
         success_rate = Utils.getPercent(
-            total_pass, total_detections, 1
+            total_pass, total_detections-total_skipped, 1
         )
 
         # TODO (cmcginley): add stats around total test cases and unit/integration test
         #   sucess/failure? maybe configurable reporting? add section to summary called
         #   "testwise_summary" listing per test metrics (e.g. total test, total tests passed, ...);
         #   also list num skipped at both detection and test level
         # Construct and return the larger results dict
         result_dict = {
             "summary": {
                 "success": overall_success,
                 "total_detections": total_detections,
                 "total_pass": total_pass,
                 "total_fail": total_fail,
+                "total_skipped": total_skipped,
                 "total_untested": total_untested,
                 "total_experimental_or_deprecated": len(deprecated_detections+experimental_detections),
                 "success_rate": success_rate,
             },
             "tested_detections": tested_detections,
             "untested_detections": untested_detections,
             "percent_complete": percent_complete,
```

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py` & `contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/doc_gen.py` & `contentctl-3.5.0/contentctl/actions/doc_gen.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/generate.py` & `contentctl-3.5.0/contentctl/actions/generate.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/initialize.py` & `contentctl-3.5.0/contentctl/actions/initialize.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/initialize_old.py` & `contentctl-3.5.0/contentctl/actions/initialize_old.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/new_content.py` & `contentctl-3.5.0/contentctl/actions/new_content.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/release_notes.py` & `contentctl-3.5.0/contentctl/actions/release_notes.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,45 +26,59 @@
                         with open(file_path, 'r') as file:
                             try:
                                 data = yaml.safe_load(file)
                                 # Check and create story link
                                 if 'name' in data and 'stories/' in file_path:
                                     story_link = "https://research.splunk.com/stories/" + data['name']
                                     story_link=story_link.replace(" ","_")
-                                    story_link=story_link.replace("- ","_")
                                     story_link = story_link.lower()
                                     print("- "+"["+f"{data['name']}"+"]"+"("+story_link+")")
-                                # Check and create detection link
-                                if 'name' in data and 'id' in data and 'detections/' in file_path:
-                                    temp_link = "https://research.splunk.com" + file_path.replace(repo_path,"")
-                                    pattern = r'(?<=/)[^/]*$'
-                                    detection_link = re.sub(pattern, data['id'], temp_link)
-                                    detection_link = detection_link.replace("detections","" )
-                                    detection_link = detection_link.replace(".com//",".com/" )
-                                    print("- "+"["+f"{data['name']}"+"]"+"("+detection_link+")")    
+              
                                 if 'name' in data and'playbooks/' in file_path:
                                     playbook_link = "https://research.splunk.com" + file_path.replace(repo_path,"")
                                     playbook_link=playbook_link.replace(".yml","/").lower()
                                     print("- "+"["+f"{data['name']}"+"]"+"("+playbook_link+")")
 
                                 if 'name' in data and'macros/' in file_path:
                                     print("- " + f"{data['name']}")
 
                                 if 'name' in data and'lookups/' in file_path:
                                     print("- " + f"{data['name']}")
 
+                               # Create only SSA link when its production
+                                if 'name' in data and 'id' in data and 'ssa_detections/' in file_path:
+                                    if data['status'] == "production":
+                                        temp_link = "https://research.splunk.com" + file_path.replace(repo_path,"")
+                                        pattern = r'(?<=/)[^/]*$'
+                                        detection_link = re.sub(pattern, data['id'], temp_link)
+                                        detection_link = detection_link.replace("detections","" )
+                                        detection_link = detection_link.replace("ssa_/","" )
+                                        print("- "+"["+f"{data['name']}"+"]"+"("+detection_link+")")   
+
+                                    if data['status'] == "validation":
+                                        print("- "+f"{data['name']}"+" (Validation Mode)")   
+
+                                # Check and create detection link
+                                if 'name' in data and 'id' in data and 'detections/' in file_path and not 'ssa_detections/' in file_path:
+                                    temp_link = "https://research.splunk.com" + file_path.replace(repo_path,"")
+                                    pattern = r'(?<=/)[^/]*$'
+                                    detection_link = re.sub(pattern, data['id'], temp_link)
+                                    detection_link = detection_link.replace("detections","" )
+                                    detection_link = detection_link.replace(".com//",".com/" )
+                                    print("- "+"["+f"{data['name']}"+"]"+"("+detection_link+")") 
+
                             except yaml.YAMLError as exc:
                                 print(f"Error parsing YAML file {file_path}: {exc}")
                 else:
                     print(f"File not found or is not a file: {file_path}")
 
     def release_notes(self, input_dto: DirectorInputDto, old_tag:Union[str,None], new_tag:str, latest_branch:str) -> None:
 
         ### Remove hard coded path
-        directories = ['detections/','stories/','macros/','lookups/','playbooks']
+        directories = ['detections/','stories/','macros/','lookups/','playbooks/','ssa_detections/']
         repo_path = os.path.abspath(input_dto.director_input_dto.input_path)
         repo = Repo(repo_path)
         # Ensure the new tag is in the tags if tags are supplied
       
         if new_tag:    
             if new_tag not in repo.tags:
                 raise ValueError(f"new_tag {new_tag} does not exist in the repository. Make sure your branch nameis ")
@@ -100,55 +114,63 @@
             file_path = diff.a_path
 
             # Check if the file is in the specified directories
             if any(file_path.startswith(directory) for directory in directories):
                 # Check if a file is Modified
                 if diff.change_type == 'M':
                     modified_files.append(file_path)
+
+
                 # Check if a file is Added
                 elif diff.change_type == 'A':
                     added_files.append(file_path)
                     # print(added_files)
-
         detections_added = []
+        ba_detections_added = []
         stories_added = []
         macros_added = []
         lookups_added = []
         playbooks_added = []      
         detections_modified = []
+        ba_detections_modified = []
         stories_modified = []
         macros_modified = []
         lookups_modified = []
         playbooks_modified = []
 
         for file in modified_files:
             file=repo_path +"/"+file
-            if 'detections/' in file:
+            if 'detections/' in file and 'ssa_detections/' not in file:
                 detections_modified.append(file)
             if 'stories/' in file:
                 stories_modified.append(file)
             if 'macros/' in file:
                 macros_modified.append(file)
             if 'lookups/' in file:
                 lookups_modified.append(file)
             if 'playbooks/' in file:
                 playbooks_modified.append(file)
+            if 'ssa_detections/' in file:
+                ba_detections_modified.append(file)
 
         for file in added_files:
             file=repo_path +"/"+file
-            if 'detections/' in file:
+            if 'detections/' in file and 'ssa_detections/' not in file:
                 detections_added.append(file)
             if 'stories/' in file:
                 stories_added.append(file)
             if 'macros/' in file:
                 macros_added.append(file)
             if 'lookups/' in file:
                 lookups_added.append(file)
             if 'playbooks/' in file:
                 playbooks_added.append(file)
+            if 'ssa_detections/' in file:
+                ba_detections_added.append(file)
+
         if new_tag:
 
             print(f"Generating release notes       - \033[92m{latest_tag}\033[0m")
             print(f"Compared against               - \033[92m{previous_tag}\033[0m")
             print("\n## Release notes for ESCU " + latest_tag)
 
         if latest_branch:
@@ -173,10 +195,20 @@
         print("\n### Lookups Updated")    
         self.create_notes(repo_path,lookups_modified)
         print("\n### Playbooks Added")    
         self.create_notes(repo_path,playbooks_added)
         print("\n### Playbooks Updated")    
         self.create_notes(repo_path,playbooks_modified)
 
-        print("\n### Other Updates\n-\n") 
+        print("\n### Other Updates\n-\n")
+
+        print("\n## BA Release Notes")
+
+        print("\n### New BA Analytics")
+        self.create_notes(repo_path,ba_detections_added)
+
+        print("\n### Updated BA Analytics")    
+        self.create_notes(repo_path,ba_detections_modified) 
+
+
         
         print(f"Release notes completed succesfully")
```

### Comparing `contentctl-3.4.3/contentctl/actions/reporting.py` & `contentctl-3.5.0/contentctl/actions/reporting.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/test.py` & `contentctl-3.5.0/contentctl/actions/test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/actions/validate.py` & `contentctl-3.5.0/contentctl/actions/validate.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/contentctl.py` & `contentctl-3.5.0/contentctl/contentctl.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/enrichments/attack_enrichment.py` & `contentctl-3.5.0/contentctl/enrichments/attack_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/enrichments/cve_enrichment.py` & `contentctl-3.5.0/contentctl/enrichments/cve_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/enrichments/splunk_app_enrichment.py` & `contentctl-3.5.0/contentctl/enrichments/splunk_app_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/helper/config_handler.py` & `contentctl-3.5.0/contentctl/helper/config_handler.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/helper/link_validator.py` & `contentctl-3.5.0/contentctl/helper/link_validator.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/helper/utils.py` & `contentctl-3.5.0/contentctl/helper/utils.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/backend_splunk_ba.py` & `contentctl-3.5.0/contentctl/input/backend_splunk_ba.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/baseline_builder.py` & `contentctl-3.5.0/contentctl/input/baseline_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/basic_builder.py` & `contentctl-3.5.0/contentctl/input/basic_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/detection_builder.py` & `contentctl-3.5.0/contentctl/input/detection_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -340,14 +340,31 @@
                 if isinstance(test, IntegrationTest):
                     test.skip("TEST SKIPPED: Skipping all integration tests")
         else:
             raise ValueError(
                 "security_content_obj must be an instance of Detection to skip integration tests, "
                 f"not {type(self.security_content_obj)}"
                 )
+    
+    def skipAllTests(self, manual_test_explanation:str) -> None:
+        """
+        Skip all unit and integration tests if the manual_test flag is defined in the yml
+        """
+        # Sanity check for typing and in setObject wasn't called yet 
+        if self.security_content_obj is not None and isinstance(self.security_content_obj, Detection):
+            for test in self.security_content_obj.tests:
+                #This should skip both unit and integration tests as appropriate
+                test.skip(f"TEST SKIPPED: Detection marked as 'manual_test' with explanation: {manual_test_explanation}")
+                
+        else:
+            raise ValueError(
+                "security_content_obj must be an instance of Detection to skip unit and integration tests due "
+                f"to the presence of the manual_test field, not {type(self.security_content_obj)}"
+                )
+
 
     def reset(self) -> None:
         self.security_content_obj = None
 
 
     def getObject(self) -> SecurityContentObject:
         return self.security_content_obj
```

### Comparing `contentctl-3.4.3/contentctl/input/director.py` & `contentctl-3.5.0/contentctl/input/director.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,21 @@
         if self.input_dto.config.enrichments.splunk_app_enrichment:
             builder.addSplunkApp()
 
         # Skip all integration tests if configured to do so
         # TODO: is there a better way to handle this? The `test` portion of the config is not defined for validate
         if (self.input_dto.config.test is not None) and (not self.input_dto.config.test.enable_integration_testing):
             builder.skipIntegrationTests()
+        
+        if builder.security_content_obj is not None and \
+           builder.security_content_obj.tags is not None and \
+           isinstance(builder.security_content_obj.tags.manual_test,str):
+            # Set all tests, both Unit AND Integration, to manual_test.  Note that integration test messages
+            # will intentionally overwrite the justification in the skipIntegrationTests call above. 
+            builder.skipAllTests(builder.security_content_obj.tags.manual_test)
 
 
     def constructSSADetection(self, builder: DetectionBuilder, file_path: str) -> None:
         builder.reset()
         builder.setObject(file_path)
         builder.addMitreAttackEnrichment(self.attack_enrichment)
         builder.addKillChainPhase()
```

### Comparing `contentctl-3.4.3/contentctl/input/investigation_builder.py` & `contentctl-3.5.0/contentctl/input/investigation_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/new_content_generator.py` & `contentctl-3.5.0/contentctl/input/new_content_generator.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/new_content_questions.py` & `contentctl-3.5.0/contentctl/input/new_content_questions.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/playbook_builder.py` & `contentctl-3.5.0/contentctl/input/playbook_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/sigma_converter.py` & `contentctl-3.5.0/contentctl/input/sigma_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from sigma.collection import SigmaCollection
 from sigma.backends.splunk import SplunkBackend
 from sigma.processing.pipeline import ProcessingItem, ProcessingPipeline
 
 from contentctl.input.yml_reader import YmlReader
 from contentctl.objects.detection import Detection
 from contentctl.objects.data_source import DataSource
+from contentctl.objects.unit_test import UnitTest
 from contentctl.objects.enums import *
 from contentctl.helper.utils import Utils
 from contentctl.input.backend_splunk_ba import SplunkBABackend
 
 
 @dataclass(frozen=True)
 class SigmaConverterInputDto:
@@ -221,14 +222,20 @@
         #it passes validation, then updated the name after the object
         #is constructed.  Because we do not have Pydantic configured
         #to validate each new field assignment, this will not throw
         #an error
         name = yml_dict.get("name","")
         yml_dict["name"] = name[:67]
         detection = Detection.parse_obj(yml_dict)
+        # Remove any Integration Tests.  IntegrationTests are only relevant
+        # for ESCU Content and NOT for BA Content. Instead of filtering OUT
+        # IntegrationTest, we will ONLY include UnitTest. This supports the introduction
+        # of additional ESCU Test Types in the future.
+        detection.tests = list(filter(lambda t: isinstance(t, UnitTest), detection.tests))
+
         detection.name = name
 
         detection.source = os.path.split(os.path.dirname(detection_path))[-1]  
         return detection 
 
 
     def load_data_source(self, input_path: str, data_source_name: str) -> DataSource:
```

### Comparing `contentctl-3.4.3/contentctl/input/ssa_detection_builder.py` & `contentctl-3.5.0/contentctl/input/ssa_detection_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/story_builder.py` & `contentctl-3.5.0/contentctl/input/story_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/input/yml_reader.py` & `contentctl-3.5.0/contentctl/input/yml_reader.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/abstract_security_content_objects/detection_abstract.py` & `contentctl-3.5.0/contentctl/objects/abstract_security_content_objects/detection_abstract.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from contentctl.objects.integration_test import IntegrationTest
 from contentctl.objects.macro import Macro
 from contentctl.objects.lookup import Lookup
 from contentctl.objects.baseline import Baseline
 from contentctl.objects.playbook import Playbook
 from contentctl.helper.link_validator import LinkValidator
 from contentctl.objects.enums import SecurityContentType
-
+from contentctl.objects.test_group import TestGroup
 
 class Detection_Abstract(SecurityContentObject):
     # contentType: SecurityContentType = SecurityContentType.detections
     # NOTE: because `use_enum_values` is configured, this will actually be type str
     type: AnalyticsType = ...
     file_path: str = None
     # status field is REQUIRED (the way to denote this with pydantic is ...)
@@ -56,14 +56,42 @@
     providing_technologies: list = None
     runtime: str = None
     enabled_by_default: bool = False
 
     class Config:
         use_enum_values = True
 
+
+    # A list of groups of tests, relying on the same data
+    test_groups: Union[list[TestGroup], None] = None
+
+    @validator("test_groups", always=True)
+    def validate_test_groups(cls, value, values) -> Union[list[TestGroup], None]:
+        """
+        Validates the `test_groups` field and constructs the model from the list of unit tests
+        if no explicit construct was provided
+        :param value: the value of the field `test_groups`
+        :param values: a dict of the other fields in the Detection model
+        """
+        # if the value was not the None default, do nothing
+        if value is not None:
+            return value
+
+        # iterate over the unit tests and create a TestGroup (and as a result, an IntegrationTest) for each
+        test_groups: list[TestGroup] = []
+        for unit_test in values["tests"]:
+            test_group = TestGroup.derive_from_unit_test(unit_test, values["name"])
+            test_groups.append(test_group)
+
+        # now add each integration test to the list of tests
+        for test_group in test_groups:
+            values["tests"].append(test_group.integration_test)
+        return test_groups
+
+
     def get_content_dependencies(self) -> list[SecurityContentObject]:
         return self.playbooks + self.baselines + self.macros + self.lookups
 
     @staticmethod
     def get_detections_from_filenames(
         detection_filenames: set[str],
         all_detections: list[Detection_Abstract]
@@ -190,24 +218,47 @@
             if len(error_messages) > 0 and values.get("status") == DetectionStatus.production.value:
                 msg = "\n\t".join(error_messages)
                 raise (ValueError(msg))
 
         # Found everything
         return v
 
-    # TODO (cmcginley): Fix detection_abstract.tests_validate so that it surfaces validation errors
-    #   (e.g. a lack of tests) to the final results, instead of just showing a failed detection w/
-    #   no tests (maybe have a message propagated at the detection level? do a separate coverage
-    #   check as part of validation?):
-    @validator("tests")
+    @validator("tests", always=True)
     def tests_validate(cls, v, values):
-        if values.get("status", "") == DetectionStatus.production.value and not v:
-            raise ValueError(
-                "At least one test is REQUIRED for production detection: " + values["name"]
-            )
+        # TODO (cmcginley): Fix detection_abstract.tests_validate so that it surfaces validation errors
+        #   (e.g. a lack of tests) to the final results, instead of just showing a failed detection w/
+        #   no tests (maybe have a message propagated at the detection level? do a separate coverage
+        #   check as part of validation?):
+    
+    
+        #Only production analytics require tests
+        if values.get("status","") != DetectionStatus.production.value:
+            return v
+        
+        # All types EXCEPT Correlation MUST have test(s). Any other type, including newly defined types, requires them.
+        # Accordingly, we do not need to do additional checks if the type is Correlation
+        if values.get("type","") in set([AnalyticsType.Correlation.value]):
+            return v
+        
+            
+        # Ensure that there is at least 1 test        
+        if len(v) == 0:
+            if values.get("tags",None) and values.get("tags").manual_test is not None:
+                # Detections that are manual_test MAY have detections, but it is not required.  If they
+                # do not have one, then create one which will be a placeholder.
+                # Note that this fake UnitTest (and by extension, Integration Test) will NOT be generated
+                # if there ARE test(s) defined for a Detection.
+                placeholder_test = UnitTest(name="PLACEHOLDER FOR DETECTION TAGGED MANUAL_TEST WITH NO TESTS SPECIFIED IN YML FILE", attack_data=[])
+                return [placeholder_test]
+            
+            else:
+                raise ValueError("At least one test is REQUIRED for production detection: " + values.get("name", "NO NAME FOUND"))
+
+
+        #No issues - at least one test provided for production type requiring testing
         return v
 
     @validator("datamodel")
     def datamodel_valid(cls, v, values):
         for datamodel in v:
             if datamodel not in [el.name for el in DataModel]:
                 raise ValueError("not valid data model: " + values["name"])
```

### Comparing `contentctl-3.4.3/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py` & `contentctl-3.5.0/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/app.py` & `contentctl-3.5.0/contentctl/objects/app.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/base_test.py` & `contentctl-3.5.0/contentctl/objects/base_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/base_test_result.py` & `contentctl-3.5.0/contentctl/objects/base_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/baseline.py` & `contentctl-3.5.0/contentctl/objects/baseline.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/baseline_tags.py` & `contentctl-3.5.0/contentctl/objects/baseline_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/config.py` & `contentctl-3.5.0/contentctl/objects/config.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/constants.py` & `contentctl-3.5.0/contentctl/objects/constants.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/correlation_search.py` & `contentctl-3.5.0/contentctl/objects/correlation_search.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/deployment.py` & `contentctl-3.5.0/contentctl/objects/deployment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/detection_tags.py` & `contentctl-3.5.0/contentctl/objects/detection_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/enums.py` & `contentctl-3.5.0/contentctl/objects/enums.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/integration_test.py` & `contentctl-3.5.0/contentctl/objects/integration_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/investigation.py` & `contentctl-3.5.0/contentctl/objects/investigation.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/lookup.py` & `contentctl-3.5.0/contentctl/objects/lookup.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/macro.py` & `contentctl-3.5.0/contentctl/objects/macro.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/notable_action.py` & `contentctl-3.5.0/contentctl/objects/notable_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/observable.py` & `contentctl-3.5.0/contentctl/objects/observable.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/playbook.py` & `contentctl-3.5.0/contentctl/objects/playbook.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/repo_config.py` & `contentctl-3.5.0/contentctl/objects/repo_config.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/risk_analysis_action.py` & `contentctl-3.5.0/contentctl/objects/risk_analysis_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/risk_object.py` & `contentctl-3.5.0/contentctl/objects/risk_object.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/ssa_detection.py` & `contentctl-3.5.0/contentctl/objects/ssa_detection.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/ssa_detection_tags.py` & `contentctl-3.5.0/contentctl/objects/ssa_detection_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/story.py` & `contentctl-3.5.0/contentctl/objects/story.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/story_tags.py` & `contentctl-3.5.0/contentctl/objects/story_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/test_config.py` & `contentctl-3.5.0/contentctl/objects/test_config.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/test_group.py` & `contentctl-3.5.0/contentctl/objects/test_group.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/threat_object.py` & `contentctl-3.5.0/contentctl/objects/threat_object.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/unit_test.py` & `contentctl-3.5.0/contentctl/objects/unit_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/unit_test_attack_data.py` & `contentctl-3.5.0/contentctl/objects/unit_test_attack_data.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/objects/unit_test_result.py` & `contentctl-3.5.0/contentctl/objects/unit_test_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 NO_SID = "Testing Failed, NO Search ID"
 SID_TEMPLATE = "{server}:{web_port}/en-US/app/search/search?sid={sid}"
 
 
 class UnitTestResult(BaseTestResult):
     missing_observables: list[str] = []
-
+    
     def set_job_content(
         self,
         content: Union[Record, None],
         config: Infrastructure,
         status: TestResultStatus,
         exception: Union[Exception, None] = None,
         duration: float = 0,
@@ -33,39 +33,44 @@
             (float, in seconds)
         :returns: bool indicating test success (inclusive of PASS and SKIP)
         """
         # Set duration, exception and status
         self.duration = round(duration, 2)
         self.exception = exception
         self.status = status
-
+        self.job_content = content
+        
         # Set the job content, if given
         if content is not None:
-            self.job_content = content
-
             if self.status == TestResultStatus.PASS:
                 self.message = "TEST PASSED"
             elif self.status == TestResultStatus.FAIL:
                 self.message = "TEST FAILED"
             elif self.status == TestResultStatus.ERROR:
-                self.message == "TEST FAILED (ERROR)"
+                self.message = "TEST ERROR"
             elif self.status == TestResultStatus.SKIP:
+                #A test that was SKIPPED should not have job content since it should not have been run.
                 self.message = "TEST SKIPPED"
 
             if not config.instance_address.startswith("http://"):
                 sid_template = f"http://{SID_TEMPLATE}"
             else:
                 sid_template = SID_TEMPLATE
             self.sid_link = sid_template.format(
                 server=config.instance_address,
                 web_port=config.web_ui_port,
                 sid=content.get("sid", None),
             )
 
+        elif self.status == TestResultStatus.SKIP:
+            self.message = "TEST SKIPPED" 
+            pass
+
         elif content is None:
-            self.job_content = None
             self.status = TestResultStatus.ERROR
             if self.exception is not None:
                 self.message = f"EXCEPTION: {str(self.exception)}"
+            else:
+                self.message = f"ERROR with no more specific message available."
             self.sid_link = NO_SID
 
         return self.success
```

### Comparing `contentctl-3.4.3/contentctl/output/api_json_output.py` & `contentctl-3.5.0/contentctl/output/api_json_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/attack_nav_output.py` & `contentctl-3.5.0/contentctl/output/attack_nav_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/attack_nav_writer.py` & `contentctl-3.5.0/contentctl/output/attack_nav_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/ba_yml_output.py` & `contentctl-3.5.0/contentctl/output/ba_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/conf_output.py` & `contentctl-3.5.0/contentctl/output/conf_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/conf_writer.py` & `contentctl-3.5.0/contentctl/output/conf_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/detection_writer.py` & `contentctl-3.5.0/contentctl/output/detection_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/doc_md_output.py` & `contentctl-3.5.0/contentctl/output/doc_md_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/finding_report_writer.py` & `contentctl-3.5.0/contentctl/output/finding_report_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/jinja_writer.py` & `contentctl-3.5.0/contentctl/output/jinja_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/new_content_yml_output.py` & `contentctl-3.5.0/contentctl/output/new_content_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/svg_output.py` & `contentctl-3.5.0/contentctl/output/svg_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/analyticstories_detections.j2` & `contentctl-3.5.0/contentctl/output/templates/analyticstories_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/analyticstories_stories.j2` & `contentctl-3.5.0/contentctl/output/templates/analyticstories_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/app.conf.j2` & `contentctl-3.5.0/contentctl/output/templates/app.conf.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/app.manifest.j2` & `contentctl-3.5.0/contentctl/output/templates/app.manifest.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/detection_count.j2` & `contentctl-3.5.0/contentctl/output/templates/detection_count.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/detection_coverage.j2` & `contentctl-3.5.0/contentctl/output/templates/detection_coverage.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/doc_detection_page.j2` & `contentctl-3.5.0/contentctl/output/templates/doc_detection_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/doc_detections.j2` & `contentctl-3.5.0/contentctl/output/templates/doc_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/doc_navigation.j2` & `contentctl-3.5.0/contentctl/output/templates/doc_navigation.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/doc_playbooks.j2` & `contentctl-3.5.0/contentctl/output/templates/doc_playbooks.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/doc_playbooks_page.j2` & `contentctl-3.5.0/contentctl/output/templates/doc_playbooks_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/doc_stories.j2` & `contentctl-3.5.0/contentctl/output/templates/doc_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/doc_story_page.j2` & `contentctl-3.5.0/contentctl/output/templates/doc_story_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/es_investigations_investigations.j2` & `contentctl-3.5.0/contentctl/output/templates/es_investigations_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/finding_report.j2` & `contentctl-3.5.0/contentctl/output/templates/finding_report.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/savedsearches_baselines.j2` & `contentctl-3.5.0/contentctl/output/templates/savedsearches_baselines.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/savedsearches_detections.j2` & `contentctl-3.5.0/contentctl/output/templates/savedsearches_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/savedsearches_investigations.j2` & `contentctl-3.5.0/contentctl/output/templates/savedsearches_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/README/essoc_summary.txt` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_summary.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/default/app.conf` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/default/app.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/default/usage_searches.conf` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/default/usage_searches.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/static/appIcon.png` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIcon.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/static/appIconAlt.png` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIconAlt.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/splunk_app/static/appIcon_2x.png` & `contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/transforms.j2` & `contentctl-3.5.0/contentctl/output/templates/transforms.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/templates/workflow_actions.j2` & `contentctl-3.5.0/contentctl/output/templates/workflow_actions.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/output/yml_output.py` & `contentctl-3.5.0/contentctl/output/yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/templates/app_default.yml` & `contentctl-3.5.0/contentctl/templates/app_default.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/templates/datamodels_cim.conf` & `contentctl-3.5.0/contentctl/templates/datamodels_cim.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/templates/deployments/00_default_correlation.yml` & `contentctl-3.5.0/contentctl/templates/deployments/00_default_correlation.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/templates/deployments/00_default_ttp.yml` & `contentctl-3.5.0/contentctl/templates/deployments/00_default_ttp.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/templates/detections/anomalous_usage_of_7zip.yml` & `contentctl-3.5.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/contentctl/templates/stories/cobalt_strike.yml` & `contentctl-3.5.0/contentctl/templates/stories/cobalt_strike.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.4.3/pyproject.toml` & `contentctl-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contentctl"
-version = "3.4.3"
+version = "3.5.0"
 description = "Splunk Content Control Tool"
 authors = ["STRT <research@splunk.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 contentctl = 'contentctl.contentctl:main'
```

### Comparing `contentctl-3.4.3/PKG-INFO` & `contentctl-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contentctl
-Version: 3.4.3
+Version: 3.5.0
 Summary: Splunk Content Control Tool
 License: Apache 2.0
 Author: STRT
 Author-email: research@splunk.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


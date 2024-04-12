# Comparing `tmp/honeyhive-0.1.91-py3-none-any.whl.zip` & `tmp/honeyhive-0.1.92-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,82 +1,158 @@
-Zip file size: 82353 bytes, number of entries: 80
--rw-r--r--  2.0 unx      127 b- defN 24-Mar-15 00:38 honeyhive/__init__.py
--rw-r--r--  2.0 unx    11706 b- defN 24-Mar-15 00:38 honeyhive/configurations.py
--rw-r--r--  2.0 unx    15200 b- defN 24-Mar-15 00:38 honeyhive/datapoints.py
--rw-r--r--  2.0 unx    11897 b- defN 24-Mar-15 00:38 honeyhive/datasets.py
--rw-r--r--  2.0 unx     9081 b- defN 24-Mar-15 00:38 honeyhive/events.py
--rw-r--r--  2.0 unx    11381 b- defN 24-Mar-15 00:38 honeyhive/metrics.py
--rw-r--r--  2.0 unx    12178 b- defN 24-Mar-15 00:38 honeyhive/projects.py
--rw-r--r--  2.0 unx     3560 b- defN 24-Mar-15 00:38 honeyhive/sdk.py
--rw-r--r--  2.0 unx     1239 b- defN 24-Mar-15 00:38 honeyhive/sdkconfiguration.py
--rw-r--r--  2.0 unx    12469 b- defN 24-Mar-15 00:38 honeyhive/session.py
--rw-r--r--  2.0 unx    10453 b- defN 24-Mar-15 00:38 honeyhive/tools.py
--rw-r--r--  2.0 unx      121 b- defN 24-Mar-15 00:38 honeyhive/_hooks/__init__.py
--rw-r--r--  2.0 unx     2392 b- defN 24-Mar-15 00:38 honeyhive/_hooks/sdkhooks.py
--rw-r--r--  2.0 unx     2069 b- defN 24-Mar-15 00:38 honeyhive/_hooks/types.py
--rw-r--r--  2.0 unx       87 b- defN 24-Mar-15 00:38 honeyhive/models/__init__.py
--rw-r--r--  2.0 unx     1971 b- defN 24-Mar-15 00:38 honeyhive/models/components/__init__.py
--rw-r--r--  2.0 unx     4769 b- defN 24-Mar-15 00:38 honeyhive/models/components/configuration.py
--rw-r--r--  2.0 unx     2938 b- defN 24-Mar-15 00:38 honeyhive/models/components/createdatapointrequest.py
--rw-r--r--  2.0 unx     2851 b- defN 24-Mar-15 00:38 honeyhive/models/components/createdatasetrequest.py
--rw-r--r--  2.0 unx     5281 b- defN 24-Mar-15 00:38 honeyhive/models/components/createeventrequest.py
--rw-r--r--  2.0 unx      950 b- defN 24-Mar-15 00:38 honeyhive/models/components/createprojectrequest.py
--rw-r--r--  2.0 unx     3538 b- defN 24-Mar-15 00:38 honeyhive/models/components/datapoint.py
--rw-r--r--  2.0 unx     3030 b- defN 24-Mar-15 00:38 honeyhive/models/components/dataset.py
--rw-r--r--  2.0 unx     2215 b- defN 24-Mar-15 00:38 honeyhive/models/components/datasetupdate.py
--rw-r--r--  2.0 unx     6041 b- defN 24-Mar-15 00:38 honeyhive/models/components/event.py
--rw-r--r--  2.0 unx     4286 b- defN 24-Mar-15 00:38 honeyhive/models/components/metric.py
--rw-r--r--  2.0 unx     4636 b- defN 24-Mar-15 00:38 honeyhive/models/components/metricedit.py
--rw-r--r--  2.0 unx      965 b- defN 24-Mar-15 00:38 honeyhive/models/components/project.py
--rw-r--r--  2.0 unx      330 b- defN 24-Mar-15 00:38 honeyhive/models/components/security.py
--rw-r--r--  2.0 unx     5089 b- defN 24-Mar-15 00:38 honeyhive/models/components/sessionstartrequest.py
--rw-r--r--  2.0 unx     1502 b- defN 24-Mar-15 00:38 honeyhive/models/components/tool.py
--rw-r--r--  2.0 unx     1060 b- defN 24-Mar-15 00:38 honeyhive/models/components/toolupdate.py
--rw-r--r--  2.0 unx     2699 b- defN 24-Mar-15 00:38 honeyhive/models/components/updatedatapointrequest.py
--rw-r--r--  2.0 unx      124 b- defN 24-Mar-15 00:38 honeyhive/models/errors/__init__.py
--rw-r--r--  2.0 unx      700 b- defN 24-Mar-15 00:38 honeyhive/models/errors/sdkerror.py
--rw-r--r--  2.0 unx     2710 b- defN 24-Mar-15 00:38 honeyhive/models/operations/__init__.py
--rw-r--r--  2.0 unx      559 b- defN 24-Mar-15 00:38 honeyhive/models/operations/createconfiguration.py
--rw-r--r--  2.0 unx     1395 b- defN 24-Mar-15 00:38 honeyhive/models/operations/createdatapoint.py
--rw-r--r--  2.0 unx      759 b- defN 24-Mar-15 00:38 honeyhive/models/operations/createproject.py
--rw-r--r--  2.0 unx      760 b- defN 24-Mar-15 00:38 honeyhive/models/operations/createtool.py
--rw-r--r--  2.0 unx      808 b- defN 24-Mar-15 00:38 honeyhive/models/operations/delete_datasets.py
--rw-r--r--  2.0 unx      880 b- defN 24-Mar-15 00:38 honeyhive/models/operations/delete_events_event_id_.py
--rw-r--r--  2.0 unx      742 b- defN 24-Mar-15 00:38 honeyhive/models/operations/delete_metrics.py
--rw-r--r--  2.0 unx      770 b- defN 24-Mar-15 00:38 honeyhive/models/operations/deleteconfiguration.py
--rw-r--r--  2.0 unx      758 b- defN 24-Mar-15 00:38 honeyhive/models/operations/deletedatapoint.py
--rw-r--r--  2.0 unx      732 b- defN 24-Mar-15 00:38 honeyhive/models/operations/deleteproject.py
--rw-r--r--  2.0 unx      746 b- defN 24-Mar-15 00:38 honeyhive/models/operations/deletesession.py
--rw-r--r--  2.0 unx      740 b- defN 24-Mar-15 00:38 honeyhive/models/operations/deletetool.py
--rw-r--r--  2.0 unx     2076 b- defN 24-Mar-15 00:38 honeyhive/models/operations/get_datasets.py
--rw-r--r--  2.0 unx     1002 b- defN 24-Mar-15 00:38 honeyhive/models/operations/get_metrics.py
--rw-r--r--  2.0 unx     1385 b- defN 24-Mar-15 00:38 honeyhive/models/operations/getconfigurations.py
--rw-r--r--  2.0 unx      968 b- defN 24-Mar-15 00:38 honeyhive/models/operations/getdatapoint.py
--rw-r--r--  2.0 unx     2022 b- defN 24-Mar-15 00:38 honeyhive/models/operations/getdatapoints.py
--rw-r--r--  2.0 unx      970 b- defN 24-Mar-15 00:38 honeyhive/models/operations/getprojects.py
--rw-r--r--  2.0 unx      932 b- defN 24-Mar-15 00:38 honeyhive/models/operations/getsession.py
--rw-r--r--  2.0 unx      981 b- defN 24-Mar-15 00:38 honeyhive/models/operations/gettools.py
--rw-r--r--  2.0 unx     1567 b- defN 24-Mar-15 00:38 honeyhive/models/operations/post_datasets.py
--rw-r--r--  2.0 unx     1658 b- defN 24-Mar-15 00:38 honeyhive/models/operations/post_events.py
--rw-r--r--  2.0 unx      551 b- defN 24-Mar-15 00:38 honeyhive/models/operations/post_metrics.py
--rw-r--r--  2.0 unx     1850 b- defN 24-Mar-15 00:38 honeyhive/models/operations/processeventtrace.py
--rw-r--r--  2.0 unx      551 b- defN 24-Mar-15 00:38 honeyhive/models/operations/put_datasets.py
--rw-r--r--  2.0 unx     1810 b- defN 24-Mar-15 00:38 honeyhive/models/operations/put_events.py
--rw-r--r--  2.0 unx      550 b- defN 24-Mar-15 00:38 honeyhive/models/operations/put_metrics.py
--rw-r--r--  2.0 unx     1531 b- defN 24-Mar-15 00:38 honeyhive/models/operations/startsession.py
--rw-r--r--  2.0 unx      983 b- defN 24-Mar-15 00:38 honeyhive/models/operations/updateconfiguration.py
--rw-r--r--  2.0 unx     1049 b- defN 24-Mar-15 00:38 honeyhive/models/operations/updatedatapoint.py
--rw-r--r--  2.0 unx      755 b- defN 24-Mar-15 00:38 honeyhive/models/operations/updateproject.py
--rw-r--r--  2.0 unx      760 b- defN 24-Mar-15 00:38 honeyhive/models/operations/updatetool.py
--rw-r--r--  2.0 unx      120 b- defN 24-Mar-15 00:38 honeyhive/utils/__init__.py
--rw-r--r--  2.0 unx    30292 b- defN 24-Mar-15 00:38 honeyhive/utils/langchain_tracer.py
--rw-r--r--  2.0 unx    14142 b- defN 24-Mar-15 00:38 honeyhive/utils/llamaindex_tracer.py
--rw-r--r--  2.0 unx     3778 b- defN 24-Mar-15 00:38 honeyhive/utils/retries.py
--rw-r--r--  2.0 unx    24467 b- defN 24-Apr-04 19:32 honeyhive/utils/tracer.py
--rw-r--r--  2.0 unx    29904 b- defN 24-Mar-15 00:38 honeyhive/utils/utils.py
--rw-r--r--  2.0 unx     1067 b- defN 24-Apr-04 19:37 honeyhive-0.1.91.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    10104 b- defN 24-Apr-04 19:37 honeyhive-0.1.91.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 19:37 honeyhive-0.1.91.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-04 19:37 honeyhive-0.1.91.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-04 19:37 honeyhive-0.1.91.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7526 b- defN 24-Apr-04 19:37 honeyhive-0.1.91.dist-info/RECORD
-80 files, 316801 bytes uncompressed, 70161 bytes compressed:  77.9%
+Zip file size: 137210 bytes, number of entries: 156
+-rw-r--r--  2.0 unx      127 b- defN 23-Nov-16 16:25 honeyhive/__init__.py
+-rw-r--r--  2.0 unx    11706 b- defN 24-Mar-07 22:14 honeyhive/configurations.py
+-rw-r--r--  2.0 unx    15200 b- defN 24-Mar-07 22:14 honeyhive/datapoints.py
+-rw-r--r--  2.0 unx    11897 b- defN 24-Mar-07 22:14 honeyhive/datasets.py
+-rw-r--r--  2.0 unx     9081 b- defN 24-Mar-07 22:14 honeyhive/events.py
+-rw-r--r--  2.0 unx    11381 b- defN 24-Mar-07 22:14 honeyhive/metrics.py
+-rw-r--r--  2.0 unx    12178 b- defN 24-Mar-07 22:14 honeyhive/projects.py
+-rw-r--r--  2.0 unx     3560 b- defN 24-Mar-13 14:43 honeyhive/sdk.py
+-rw-r--r--  2.0 unx     1239 b- defN 24-Mar-18 19:22 honeyhive/sdkconfiguration.py
+-rw-r--r--  2.0 unx    12469 b- defN 24-Mar-07 22:14 honeyhive/session.py
+-rw-r--r--  2.0 unx    10453 b- defN 24-Mar-07 22:14 honeyhive/tools.py
+-rw-r--r--  2.0 unx      121 b- defN 24-Mar-07 22:14 honeyhive/_hooks/__init__.py
+-rw-r--r--  2.0 unx     2392 b- defN 24-Mar-07 22:14 honeyhive/_hooks/sdkhooks.py
+-rw-r--r--  2.0 unx     2069 b- defN 24-Mar-07 22:14 honeyhive/_hooks/types.py
+-rw-r--r--  2.0 unx       87 b- defN 23-Nov-16 16:25 honeyhive/models/__init__.py
+-rw-r--r--  2.0 unx     1971 b- defN 24-Mar-07 22:14 honeyhive/models/components/__init__.py
+-rw-r--r--  2.0 unx     2285 b- defN 23-Nov-16 16:25 honeyhive/models/components/chatcompletionrequest.py
+-rw-r--r--  2.0 unx     1769 b- defN 23-Nov-16 16:25 honeyhive/models/components/chatcompletionresponse.py
+-rw-r--r--  2.0 unx     4769 b- defN 24-Mar-07 22:14 honeyhive/models/components/configuration.py
+-rw-r--r--  2.0 unx     2938 b- defN 24-Mar-07 22:14 honeyhive/models/components/createdatapointrequest.py
+-rw-r--r--  2.0 unx     2851 b- defN 24-Mar-07 22:14 honeyhive/models/components/createdatasetrequest.py
+-rw-r--r--  2.0 unx     5281 b- defN 24-Mar-07 22:14 honeyhive/models/components/createeventrequest.py
+-rw-r--r--  2.0 unx      950 b- defN 24-Mar-07 22:14 honeyhive/models/components/createprojectrequest.py
+-rw-r--r--  2.0 unx     3538 b- defN 24-Mar-07 22:14 honeyhive/models/components/datapoint.py
+-rw-r--r--  2.0 unx     3030 b- defN 24-Mar-07 22:14 honeyhive/models/components/dataset.py
+-rw-r--r--  2.0 unx     3051 b- defN 23-Nov-16 16:25 honeyhive/models/components/datasetresponse.py
+-rw-r--r--  2.0 unx     2215 b- defN 24-Mar-07 22:14 honeyhive/models/components/datasetupdate.py
+-rw-r--r--  2.0 unx      653 b- defN 23-Nov-16 16:25 honeyhive/models/components/deleteresponse.py
+-rw-r--r--  2.0 unx     4000 b- defN 23-Nov-16 16:25 honeyhive/models/components/evaluation.py
+-rw-r--r--  2.0 unx     3785 b- defN 23-Nov-16 16:25 honeyhive/models/components/evaluationloggingquery.py
+-rw-r--r--  2.0 unx     3492 b- defN 23-Nov-16 16:25 honeyhive/models/components/evaluationupdaterequest.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-Mar-07 22:14 honeyhive/models/components/event.py
+-rw-r--r--  2.0 unx     1277 b- defN 23-Nov-16 16:25 honeyhive/models/components/feedbackquery.py
+-rw-r--r--  2.0 unx     1750 b- defN 23-Nov-16 16:25 honeyhive/models/components/feedbackresponse.py
+-rw-r--r--  2.0 unx     3390 b- defN 23-Nov-16 16:25 honeyhive/models/components/finetunedmodelresponse.py
+-rw-r--r--  2.0 unx     3272 b- defN 23-Nov-16 16:25 honeyhive/models/components/generatequery.py
+-rw-r--r--  2.0 unx     3185 b- defN 23-Nov-16 16:25 honeyhive/models/components/generation.py
+-rw-r--r--  2.0 unx     3802 b- defN 23-Nov-16 16:25 honeyhive/models/components/generationloggingquery.py
+-rw-r--r--  2.0 unx     1258 b- defN 23-Nov-16 16:25 honeyhive/models/components/generationresponse.py
+-rw-r--r--  2.0 unx     4286 b- defN 24-Mar-07 22:14 honeyhive/models/components/metric.py
+-rw-r--r--  2.0 unx      731 b- defN 23-Nov-16 16:25 honeyhive/models/components/metriccomputerequest.py
+-rw-r--r--  2.0 unx      522 b- defN 23-Nov-16 16:25 honeyhive/models/components/metriccomputeresponse.py
+-rw-r--r--  2.0 unx     2570 b- defN 23-Nov-16 16:25 honeyhive/models/components/metriccreaterequest.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Nov-16 16:25 honeyhive/models/components/metriccreateresponse.py
+-rw-r--r--  2.0 unx      522 b- defN 23-Nov-16 16:25 honeyhive/models/components/metricdeleteresponse.py
+-rw-r--r--  2.0 unx     4636 b- defN 24-Mar-07 22:14 honeyhive/models/components/metricedit.py
+-rw-r--r--  2.0 unx     3290 b- defN 23-Nov-16 16:25 honeyhive/models/components/metricresponse.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Nov-16 16:25 honeyhive/models/components/metricupdaterequest.py
+-rw-r--r--  2.0 unx      522 b- defN 23-Nov-16 16:25 honeyhive/models/components/metricupdateresponse.py
+-rw-r--r--  2.0 unx      965 b- defN 24-Mar-07 22:14 honeyhive/models/components/project.py
+-rw-r--r--  2.0 unx     2442 b- defN 23-Nov-16 16:25 honeyhive/models/components/promptcreationquery.py
+-rw-r--r--  2.0 unx     3146 b- defN 23-Nov-16 16:25 honeyhive/models/components/promptresponse.py
+-rw-r--r--  2.0 unx     2042 b- defN 23-Nov-16 16:25 honeyhive/models/components/promptupdatequery.py
+-rw-r--r--  2.0 unx      330 b- defN 23-Nov-16 16:25 honeyhive/models/components/security.py
+-rw-r--r--  2.0 unx      834 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessionendresponse.py
+-rw-r--r--  2.0 unx     4299 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessioneventquery.py
+-rw-r--r--  2.0 unx      856 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessioneventresponse.py
+-rw-r--r--  2.0 unx     2286 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessioneventupdate.py
+-rw-r--r--  2.0 unx      889 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessionfeedback.py
+-rw-r--r--  2.0 unx     1524 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessionstartquery.py
+-rw-r--r--  2.0 unx     5089 b- defN 24-Mar-07 22:14 honeyhive/models/components/sessionstartrequest.py
+-rw-r--r--  2.0 unx      853 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessionstartresponse.py
+-rw-r--r--  2.0 unx      675 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessiontrace.py
+-rw-r--r--  2.0 unx      849 b- defN 23-Nov-16 16:25 honeyhive/models/components/successresponse.py
+-rw-r--r--  2.0 unx      872 b- defN 23-Nov-16 16:25 honeyhive/models/components/successtraceresponse.py
+-rw-r--r--  2.0 unx     2871 b- defN 23-Nov-16 16:25 honeyhive/models/components/taskcreationquery.py
+-rw-r--r--  2.0 unx     3212 b- defN 23-Nov-16 16:25 honeyhive/models/components/taskresponse.py
+-rw-r--r--  2.0 unx     2192 b- defN 23-Nov-16 16:25 honeyhive/models/components/taskupdatequery.py
+-rw-r--r--  2.0 unx     1493 b- defN 23-Nov-16 16:25 honeyhive/models/components/taskupdateresponse.py
+-rw-r--r--  2.0 unx     1502 b- defN 24-Mar-07 22:14 honeyhive/models/components/tool.py
+-rw-r--r--  2.0 unx     1060 b- defN 24-Mar-07 22:14 honeyhive/models/components/toolupdate.py
+-rw-r--r--  2.0 unx     1516 b- defN 23-Nov-16 16:25 honeyhive/models/components/traceevent.py
+-rw-r--r--  2.0 unx     2699 b- defN 24-Mar-07 22:14 honeyhive/models/components/updatedatapointrequest.py
+-rw-r--r--  2.0 unx      681 b- defN 23-Nov-16 16:25 honeyhive/models/components/updateresponse.py
+-rw-r--r--  2.0 unx     1673 b- defN 23-Nov-16 16:25 honeyhive/models/components/uploaddataset.py
+-rw-r--r--  2.0 unx      124 b- defN 23-Nov-16 16:25 honeyhive/models/errors/__init__.py
+-rw-r--r--  2.0 unx      700 b- defN 23-Nov-16 16:25 honeyhive/models/errors/sdkerror.py
+-rw-r--r--  2.0 unx     2710 b- defN 24-Mar-07 22:14 honeyhive/models/operations/__init__.py
+-rw-r--r--  2.0 unx      559 b- defN 24-Mar-07 22:14 honeyhive/models/operations/createconfiguration.py
+-rw-r--r--  2.0 unx     1395 b- defN 24-Mar-07 22:14 honeyhive/models/operations/createdatapoint.py
+-rw-r--r--  2.0 unx      759 b- defN 24-Mar-07 22:14 honeyhive/models/operations/createproject.py
+-rw-r--r--  2.0 unx      760 b- defN 24-Mar-07 22:14 honeyhive/models/operations/createtool.py
+-rw-r--r--  2.0 unx      808 b- defN 24-Mar-07 22:14 honeyhive/models/operations/delete_datasets.py
+-rw-r--r--  2.0 unx      969 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_datasets_name_.py
+-rw-r--r--  2.0 unx      967 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_evaluations_id_.py
+-rw-r--r--  2.0 unx      880 b- defN 24-Mar-07 22:14 honeyhive/models/operations/delete_events_event_id_.py
+-rw-r--r--  2.0 unx      750 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_fine_tuned_models_id_.py
+-rw-r--r--  2.0 unx      742 b- defN 24-Mar-07 22:14 honeyhive/models/operations/delete_metrics.py
+-rw-r--r--  2.0 unx      959 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_prompts_id_.py
+-rw-r--r--  2.0 unx      994 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_session_session_id_.py
+-rw-r--r--  2.0 unx      953 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_tasks.py
+-rw-r--r--  2.0 unx      770 b- defN 24-Mar-07 22:14 honeyhive/models/operations/deleteconfiguration.py
+-rw-r--r--  2.0 unx      758 b- defN 24-Mar-07 22:14 honeyhive/models/operations/deletedatapoint.py
+-rw-r--r--  2.0 unx      732 b- defN 24-Mar-07 22:14 honeyhive/models/operations/deleteproject.py
+-rw-r--r--  2.0 unx      746 b- defN 24-Mar-07 22:14 honeyhive/models/operations/deletesession.py
+-rw-r--r--  2.0 unx      740 b- defN 24-Mar-07 22:14 honeyhive/models/operations/deletetool.py
+-rw-r--r--  2.0 unx     2076 b- defN 24-Mar-07 22:14 honeyhive/models/operations/get_datasets.py
+-rw-r--r--  2.0 unx      767 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_evaluations.py
+-rw-r--r--  2.0 unx      940 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_evaluations_id_.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_fine_tuned_models.py
+-rw-r--r--  2.0 unx     1011 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_fine_tuned_models_id_.py
+-rw-r--r--  2.0 unx     1271 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_generations.py
+-rw-r--r--  2.0 unx     1002 b- defN 24-Mar-07 22:14 honeyhive/models/operations/get_metrics.py
+-rw-r--r--  2.0 unx     1123 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_prompts.py
+-rw-r--r--  2.0 unx     1450 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_session.py
+-rw-r--r--  2.0 unx      999 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_session_session_id_.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_session_session_id_export.py
+-rw-r--r--  2.0 unx      967 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_tasks.py
+-rw-r--r--  2.0 unx     1385 b- defN 24-Mar-07 22:14 honeyhive/models/operations/getconfigurations.py
+-rw-r--r--  2.0 unx      968 b- defN 24-Mar-07 22:14 honeyhive/models/operations/getdatapoint.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-Mar-07 22:14 honeyhive/models/operations/getdatapoints.py
+-rw-r--r--  2.0 unx      970 b- defN 24-Mar-07 22:14 honeyhive/models/operations/getprojects.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Mar-07 22:14 honeyhive/models/operations/getsession.py
+-rw-r--r--  2.0 unx      981 b- defN 24-Mar-07 22:14 honeyhive/models/operations/gettools.py
+-rw-r--r--  2.0 unx      814 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_chat.py
+-rw-r--r--  2.0 unx     1567 b- defN 24-Mar-07 22:14 honeyhive/models/operations/post_datasets.py
+-rw-r--r--  2.0 unx      785 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_evaluations.py
+-rw-r--r--  2.0 unx     1658 b- defN 24-Mar-07 22:14 honeyhive/models/operations/post_events.py
+-rw-r--r--  2.0 unx      787 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_feedback.py
+-rw-r--r--  2.0 unx     1907 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_fine_tuned_models.py
+-rw-r--r--  2.0 unx      800 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_generations.py
+-rw-r--r--  2.0 unx      803 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_generations_log.py
+-rw-r--r--  2.0 unx      551 b- defN 24-Mar-07 22:14 honeyhive/models/operations/post_metrics.py
+-rw-r--r--  2.0 unx      819 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_metrics_compute.py
+-rw-r--r--  2.0 unx      776 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_prompts.py
+-rw-r--r--  2.0 unx     1012 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_session_id_end.py
+-rw-r--r--  2.0 unx     1261 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_session_id_event.py
+-rw-r--r--  2.0 unx     1230 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_session_id_feedback.py
+-rw-r--r--  2.0 unx     1237 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_session_id_traces.py
+-rw-r--r--  2.0 unx      812 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_start.py
+-rw-r--r--  2.0 unx      764 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_tasks.py
+-rw-r--r--  2.0 unx     1850 b- defN 24-Mar-07 22:14 honeyhive/models/operations/processeventtrace.py
+-rw-r--r--  2.0 unx      551 b- defN 24-Mar-07 22:14 honeyhive/models/operations/put_datasets.py
+-rw-r--r--  2.0 unx     1250 b- defN 23-Nov-16 16:25 honeyhive/models/operations/put_evaluations_id_.py
+-rw-r--r--  2.0 unx     1810 b- defN 24-Mar-07 22:14 honeyhive/models/operations/put_events.py
+-rw-r--r--  2.0 unx      550 b- defN 24-Mar-07 22:14 honeyhive/models/operations/put_metrics.py
+-rw-r--r--  2.0 unx     1188 b- defN 23-Nov-16 16:25 honeyhive/models/operations/put_prompts_id_.py
+-rw-r--r--  2.0 unx     1252 b- defN 23-Nov-16 16:25 honeyhive/models/operations/put_session_session_id_.py
+-rw-r--r--  2.0 unx      794 b- defN 23-Nov-16 16:25 honeyhive/models/operations/put_tasks.py
+-rw-r--r--  2.0 unx     1531 b- defN 24-Mar-07 22:14 honeyhive/models/operations/startsession.py
+-rw-r--r--  2.0 unx      983 b- defN 24-Mar-07 22:14 honeyhive/models/operations/updateconfiguration.py
+-rw-r--r--  2.0 unx     1049 b- defN 24-Mar-07 22:14 honeyhive/models/operations/updatedatapoint.py
+-rw-r--r--  2.0 unx      755 b- defN 24-Mar-07 22:14 honeyhive/models/operations/updateproject.py
+-rw-r--r--  2.0 unx      760 b- defN 24-Mar-07 22:14 honeyhive/models/operations/updatetool.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Nov-16 16:25 honeyhive/utils/__init__.py
+-rw-r--r--  2.0 unx    36037 b- defN 24-Apr-12 16:06 honeyhive/utils/langchain_tracer.py
+-rw-r--r--  2.0 unx    26678 b- defN 24-Apr-12 16:06 honeyhive/utils/llamaindex_tracer.py
+-rw-r--r--  2.0 unx     3778 b- defN 24-Mar-07 22:14 honeyhive/utils/retries.py
+-rw-r--r--  2.0 unx    24449 b- defN 24-Apr-12 16:06 honeyhive/utils/tracer.py
+-rw-r--r--  2.0 unx    29904 b- defN 24-Mar-07 22:14 honeyhive/utils/utils.py
+-rw-r--r--  2.0 unx     1067 b- defN 24-Apr-12 16:07 honeyhive-0.1.92.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    10104 b- defN 24-Apr-12 16:07 honeyhive-0.1.92.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-12 16:07 honeyhive-0.1.92.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-12 16:07 honeyhive-0.1.92.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-12 16:07 honeyhive-0.1.92.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    15540 b- defN 24-Apr-12 16:07 honeyhive-0.1.92.dist-info/RECORD
+156 files, 460982 bytes uncompressed, 111810 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -42,14 +42,20 @@
 
 Filename: honeyhive/models/__init__.py
 Comment: 
 
 Filename: honeyhive/models/components/__init__.py
 Comment: 
 
+Filename: honeyhive/models/components/chatcompletionrequest.py
+Comment: 
+
+Filename: honeyhive/models/components/chatcompletionresponse.py
+Comment: 
+
 Filename: honeyhive/models/components/configuration.py
 Comment: 
 
 Filename: honeyhive/models/components/createdatapointrequest.py
 Comment: 
 
 Filename: honeyhive/models/components/createdatasetrequest.py
@@ -63,44 +69,164 @@
 
 Filename: honeyhive/models/components/datapoint.py
 Comment: 
 
 Filename: honeyhive/models/components/dataset.py
 Comment: 
 
+Filename: honeyhive/models/components/datasetresponse.py
+Comment: 
+
 Filename: honeyhive/models/components/datasetupdate.py
 Comment: 
 
+Filename: honeyhive/models/components/deleteresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/evaluation.py
+Comment: 
+
+Filename: honeyhive/models/components/evaluationloggingquery.py
+Comment: 
+
+Filename: honeyhive/models/components/evaluationupdaterequest.py
+Comment: 
+
 Filename: honeyhive/models/components/event.py
 Comment: 
 
+Filename: honeyhive/models/components/feedbackquery.py
+Comment: 
+
+Filename: honeyhive/models/components/feedbackresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/finetunedmodelresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/generatequery.py
+Comment: 
+
+Filename: honeyhive/models/components/generation.py
+Comment: 
+
+Filename: honeyhive/models/components/generationloggingquery.py
+Comment: 
+
+Filename: honeyhive/models/components/generationresponse.py
+Comment: 
+
 Filename: honeyhive/models/components/metric.py
 Comment: 
 
+Filename: honeyhive/models/components/metriccomputerequest.py
+Comment: 
+
+Filename: honeyhive/models/components/metriccomputeresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/metriccreaterequest.py
+Comment: 
+
+Filename: honeyhive/models/components/metriccreateresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/metricdeleteresponse.py
+Comment: 
+
 Filename: honeyhive/models/components/metricedit.py
 Comment: 
 
+Filename: honeyhive/models/components/metricresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/metricupdaterequest.py
+Comment: 
+
+Filename: honeyhive/models/components/metricupdateresponse.py
+Comment: 
+
 Filename: honeyhive/models/components/project.py
 Comment: 
 
+Filename: honeyhive/models/components/promptcreationquery.py
+Comment: 
+
+Filename: honeyhive/models/components/promptresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/promptupdatequery.py
+Comment: 
+
 Filename: honeyhive/models/components/security.py
 Comment: 
 
+Filename: honeyhive/models/components/sessionendresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/sessioneventquery.py
+Comment: 
+
+Filename: honeyhive/models/components/sessioneventresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/sessioneventupdate.py
+Comment: 
+
+Filename: honeyhive/models/components/sessionfeedback.py
+Comment: 
+
+Filename: honeyhive/models/components/sessionstartquery.py
+Comment: 
+
 Filename: honeyhive/models/components/sessionstartrequest.py
 Comment: 
 
+Filename: honeyhive/models/components/sessionstartresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/sessiontrace.py
+Comment: 
+
+Filename: honeyhive/models/components/successresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/successtraceresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/taskcreationquery.py
+Comment: 
+
+Filename: honeyhive/models/components/taskresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/taskupdatequery.py
+Comment: 
+
+Filename: honeyhive/models/components/taskupdateresponse.py
+Comment: 
+
 Filename: honeyhive/models/components/tool.py
 Comment: 
 
 Filename: honeyhive/models/components/toolupdate.py
 Comment: 
 
+Filename: honeyhive/models/components/traceevent.py
+Comment: 
+
 Filename: honeyhive/models/components/updatedatapointrequest.py
 Comment: 
 
+Filename: honeyhive/models/components/updateresponse.py
+Comment: 
+
+Filename: honeyhive/models/components/uploaddataset.py
+Comment: 
+
 Filename: honeyhive/models/errors/__init__.py
 Comment: 
 
 Filename: honeyhive/models/errors/sdkerror.py
 Comment: 
 
 Filename: honeyhive/models/operations/__init__.py
@@ -117,20 +243,38 @@
 
 Filename: honeyhive/models/operations/createtool.py
 Comment: 
 
 Filename: honeyhive/models/operations/delete_datasets.py
 Comment: 
 
+Filename: honeyhive/models/operations/delete_datasets_name_.py
+Comment: 
+
+Filename: honeyhive/models/operations/delete_evaluations_id_.py
+Comment: 
+
 Filename: honeyhive/models/operations/delete_events_event_id_.py
 Comment: 
 
+Filename: honeyhive/models/operations/delete_fine_tuned_models_id_.py
+Comment: 
+
 Filename: honeyhive/models/operations/delete_metrics.py
 Comment: 
 
+Filename: honeyhive/models/operations/delete_prompts_id_.py
+Comment: 
+
+Filename: honeyhive/models/operations/delete_session_session_id_.py
+Comment: 
+
+Filename: honeyhive/models/operations/delete_tasks.py
+Comment: 
+
 Filename: honeyhive/models/operations/deleteconfiguration.py
 Comment: 
 
 Filename: honeyhive/models/operations/deletedatapoint.py
 Comment: 
 
 Filename: honeyhive/models/operations/deleteproject.py
@@ -141,17 +285,47 @@
 
 Filename: honeyhive/models/operations/deletetool.py
 Comment: 
 
 Filename: honeyhive/models/operations/get_datasets.py
 Comment: 
 
+Filename: honeyhive/models/operations/get_evaluations.py
+Comment: 
+
+Filename: honeyhive/models/operations/get_evaluations_id_.py
+Comment: 
+
+Filename: honeyhive/models/operations/get_fine_tuned_models.py
+Comment: 
+
+Filename: honeyhive/models/operations/get_fine_tuned_models_id_.py
+Comment: 
+
+Filename: honeyhive/models/operations/get_generations.py
+Comment: 
+
 Filename: honeyhive/models/operations/get_metrics.py
 Comment: 
 
+Filename: honeyhive/models/operations/get_prompts.py
+Comment: 
+
+Filename: honeyhive/models/operations/get_session.py
+Comment: 
+
+Filename: honeyhive/models/operations/get_session_session_id_.py
+Comment: 
+
+Filename: honeyhive/models/operations/get_session_session_id_export.py
+Comment: 
+
+Filename: honeyhive/models/operations/get_tasks.py
+Comment: 
+
 Filename: honeyhive/models/operations/getconfigurations.py
 Comment: 
 
 Filename: honeyhive/models/operations/getdatapoint.py
 Comment: 
 
 Filename: honeyhive/models/operations/getdatapoints.py
@@ -162,35 +336,89 @@
 
 Filename: honeyhive/models/operations/getsession.py
 Comment: 
 
 Filename: honeyhive/models/operations/gettools.py
 Comment: 
 
+Filename: honeyhive/models/operations/post_chat.py
+Comment: 
+
 Filename: honeyhive/models/operations/post_datasets.py
 Comment: 
 
+Filename: honeyhive/models/operations/post_evaluations.py
+Comment: 
+
 Filename: honeyhive/models/operations/post_events.py
 Comment: 
 
+Filename: honeyhive/models/operations/post_feedback.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_fine_tuned_models.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_generations.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_generations_log.py
+Comment: 
+
 Filename: honeyhive/models/operations/post_metrics.py
 Comment: 
 
+Filename: honeyhive/models/operations/post_metrics_compute.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_prompts.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_session_session_id_end.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_session_session_id_event.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_session_session_id_feedback.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_session_session_id_traces.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_session_start.py
+Comment: 
+
+Filename: honeyhive/models/operations/post_tasks.py
+Comment: 
+
 Filename: honeyhive/models/operations/processeventtrace.py
 Comment: 
 
 Filename: honeyhive/models/operations/put_datasets.py
 Comment: 
 
+Filename: honeyhive/models/operations/put_evaluations_id_.py
+Comment: 
+
 Filename: honeyhive/models/operations/put_events.py
 Comment: 
 
 Filename: honeyhive/models/operations/put_metrics.py
 Comment: 
 
+Filename: honeyhive/models/operations/put_prompts_id_.py
+Comment: 
+
+Filename: honeyhive/models/operations/put_session_session_id_.py
+Comment: 
+
+Filename: honeyhive/models/operations/put_tasks.py
+Comment: 
+
 Filename: honeyhive/models/operations/startsession.py
 Comment: 
 
 Filename: honeyhive/models/operations/updateconfiguration.py
 Comment: 
 
 Filename: honeyhive/models/operations/updatedatapoint.py
@@ -216,26 +444,26 @@
 
 Filename: honeyhive/utils/tracer.py
 Comment: 
 
 Filename: honeyhive/utils/utils.py
 Comment: 
 
-Filename: honeyhive-0.1.91.dist-info/LICENSE.md
+Filename: honeyhive-0.1.92.dist-info/LICENSE.md
 Comment: 
 
-Filename: honeyhive-0.1.91.dist-info/METADATA
+Filename: honeyhive-0.1.92.dist-info/METADATA
 Comment: 
 
-Filename: honeyhive-0.1.91.dist-info/WHEEL
+Filename: honeyhive-0.1.92.dist-info/WHEEL
 Comment: 
 
-Filename: honeyhive-0.1.91.dist-info/entry_points.txt
+Filename: honeyhive-0.1.92.dist-info/entry_points.txt
 Comment: 
 
-Filename: honeyhive-0.1.91.dist-info/top_level.txt
+Filename: honeyhive-0.1.92.dist-info/top_level.txt
 Comment: 
 
-Filename: honeyhive-0.1.91.dist-info/RECORD
+Filename: honeyhive-0.1.92.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## honeyhive/utils/langchain_tracer.py

```diff
@@ -7,20 +7,23 @@
 from abc import ABC
 import json
 import os
 import re
 import datetime
 from enum import Enum
 import inspect
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, ConfigDict, Field, validator
 from typing import Any, Dict, Optional, Union, List, Tuple, Callable
 from datetime import timedelta
 import uuid
 import requests
+import random
 
+from requests.adapters import HTTPAdapter
+from urllib3.util.retry import Retry
 from langchain.callbacks.tracers.base import BaseTracer, TracerException
 from langchain.callbacks.tracers.schemas import (
     TracerSession,
     Run,
 )
 from langchain.input import get_colored_text
 
@@ -42,14 +45,15 @@
     def __init__(
         self,
         project: str,
         name: Optional[str] = None,
         source: Optional[str] = None,
         user_properties: Optional[Dict[str, Any]] = None,
         api_key: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
     ):
         """Initialize the HoneyHive tracer."""
         super().__init__()
         if self._env_api_key:
             api_key = self._env_api_key
         elif not api_key:
             raise ValueError(
@@ -59,31 +63,69 @@
         if api_key:
             self._headers["Authorization"] = f"Bearer {api_key}"
 
         self.project = project
         self.source = source if source is not None else "langchain"
         self.name = name
         self.user_properties = user_properties
-
+        self.metadata = metadata
+        self.eval_info = None
+        if self.source == "evaluation":
+            try:
+                if self.metadata and "run_id" in self.metadata:
+                    self.eval_info = {"run_id": self.metadata["run_id"]}
+                elif self.metadata and "dataset_name" in self.metadata:
+                    project_res = requests_retry_session().get(
+                        url=f"{self._base_url}/projects",
+                        headers=self._headers,
+                        params={"name": self.project},
+                    )
+                    if project_res.status_code == 200:
+                        project_id = project_res.json()[0]["_id"]
+                        dataset_res = requests_retry_session().get(
+                            url=f"{self._base_url}/datasets",
+                            headers=self._headers,
+                            params={
+                                "name": self.metadata["dataset_name"],
+                                "project": project_id,
+                            },
+                        )
+                        if dataset_res.status_code == 200:
+                            dataset = dataset_res.json()["testcases"][0]
+                            dataset_id = dataset["_id"]
+                            datapoint_ids = dataset["datapoints"]
+                            if "run_name" in self.metadata:
+                                run_name = self.metadata["run_name"]
+                            else:
+                                run_name = self.name
+                            self.eval_info = {
+                                "dataset_id": dataset_id,
+                                "datapoint_ids": datapoint_ids,
+                                "project_id": project_id,
+                                "run_name": run_name,
+                            }
+            except:
+                pass
         if api_key is not None:
             self._headers["Authorization"] = "Bearer " + api_key
 
     def _start_new_session(self, inputs):
-        body = {
+        session_body = {
             "project": self.project,
             "source": self.source,
             "session_id": self.session_id,
             "session_name": self.name,
             "user_properties": self.user_properties,
+            "metadata": self.metadata,
             "inputs": inputs,
         }
-        requests.post(
+        requests_retry_session().post(
             url=f"{self._base_url}/session/start",
             headers=self._headers,
-            json=body,
+            json=session_body,
         )
 
     def _persist_run(self, run: Run) -> None:
         """Persist a run."""
         try:
             logs = self._convert_run_to_logs(run=run)
             if self.project is not None:
@@ -187,28 +229,62 @@
     def _post_trace(self, logs: List[Log]) -> None:
         """Post a trace to the HoneyHive API"""
         root_log = logs[0].dict()
         self.final_outputs = root_log["outputs"]
         self.session_id = str(uuid.uuid4())
         self._set_parent_ids(root_log, self.session_id)
         self._start_new_session(root_log["inputs"])
-        trace_response = requests.post(
+        trace_response = requests_retry_session().post(
             url=f"{self._base_url}/session/{self.session_id}/traces",
             json={"logs": [root_log]},
             headers=self._headers,
         )
         if trace_response.status_code != 200:
             raise TracerException(
                 f"Failed to post trace to HoneyHive with status code {trace_response.status_code}"
             )
-        requests.put(
+        requests_retry_session().put(
             url=f"{self._base_url}/events",
             json={"event_id": self.session_id, "outputs": self.final_outputs},
             headers=self._headers,
         )
+        if self.eval_info:
+            try:
+                if "run_id" in self.eval_info:
+                    run_res = requests_retry_session().get(
+                        url=f"{self._base_url}/runs/{self.eval_info['run_id']}",
+                        headers=self._headers,
+                    )
+                    event_ids = run_res.json()["evaluation"]["event_ids"]
+                    event_ids.append(self.session_id)
+                    requests_retry_session().put(
+                        url=f"{self._base_url}/runs/{self.eval_info['run_id']}",
+                        json={"event_ids": event_ids},
+                        headers=self._headers,
+                    )
+                else:
+                    body = {
+                        "event_ids": [self.session_id],
+                        "dataset_id": self.eval_info["dataset_id"],
+                        "datapoint_ids": self.eval_info["datapoint_ids"],
+                        "project": self.eval_info["project_id"],
+                        "status": "completed",
+                        "name": self.eval_info["run_name"],
+                    }
+                    if "config" in root_log:
+                        body["configuration"] = root_log["config"]
+                    run_res = requests_retry_session().post(
+                        url=f"{self._base_url}/runs",
+                        headers=self._headers,
+                        json=body,
+                    )
+                    run_id = run_res.json()["run_id"]
+                    self.eval_info["run_id"] = run_id
+            except:
+                pass
 
     def _set_parent_ids(self, trace, session_id) -> None:
         def crawl(node):
             if node is None:
                 return
             node["session_id"] = session_id
             self.final_outputs = node["outputs"]
@@ -315,25 +391,26 @@
                         tool["name"], tool["func"]
                     )
                     if "func" in tool
                     else None,
                 )
                 for tool in run.serialized["tools"]
             ],
-            model_config=self._create_model_config_from_params(
+            model=self._create_model_config_from_params(
                 params=run.serialized["agent"]["llm_chain"]["llm"],
                 prompt_details=run.serialized["agent"]["llm_chain"]["prompt"],
             ),
             other=AgentOther(
                 max_iterations=run.serialized["max_iterations"],
                 stop=run.serialized["early_stopping_method"],
                 output_parser=run.serialized["agent"]["output_parser"]["_type"],
             ),
         )
         return Log(
+            source=self.source,
             project=self.project,
             children=None,
             event_name=event_name,
             event_type="chain",
             event_id=str(uuid.uuid4()),
             parent_id=parent_id,
             config=config,
@@ -359,14 +436,15 @@
         """Converts LC generic chain run to HH log."""
         if parent_log is not None:
             parent_id = parent_log.event_id
         else:
             parent_id = None
         config = Config(name=event_name)
         return Log(
+            source=self.source,
             project=self.project,
             event_name=event_name,
             event_type="generic",
             config=config,
             event_id=str(uuid.uuid4()),
             parent_id=parent_id,
             inputs=self._convert_chain_inputs_to_text(inputs=run.inputs),
@@ -402,14 +480,15 @@
             parent_id = parent_log.event_id
         else:
             parent_id = None
         description = (
             run.serialized["description"] if run.run_type != "retriever" else None
         )
         return Log(
+            source=self.source,
             project=self.project,
             children=None,
             event_name=event_name,
             event_type="tool",
             event_id=str(uuid.uuid4()),
             parent_id=parent_id,
             config=ToolConfig(
@@ -528,14 +607,15 @@
                         output = generation["text"]
                     else:
                         raise NotImplementedError
                     logs.append(
                         # TODO: add token usage
                         # TODO: chat serialization doesn't include messages array
                         Log(
+                            source=self.source,
                             project=self.project,
                             children=None,
                             event_name=event_name,
                             event_type="model",
                             event_id=str(uuid.uuid4()),
                             parent_id=parent_id,
                             config=config,
@@ -546,14 +626,15 @@
                             duration=duration,
                             metadata=metadata,
                         )
                     )
         else:
             logs = [
                 Log(
+                    source=self.source,
                     project=self.project,
                     children=None,
                     event_name=event_name,
                     event_type="model",
                     event_id=str(uuid.uuid4()),
                     parent_id=parent_id,
                     config=config,
@@ -590,14 +671,23 @@
     name: Optional[str] = None
 
 
 class Config(BaseModel):
     type: str = "generic"
     name: Optional[str] = None
     description: Optional[str] = None
+    model_config = ConfigDict(protected_namespaces=())
+
+
+class LLMConfig(Config):
+    type: str = "model"
+    model_name: Optional[str] = None
+    api_base: Optional[str] = None
+    class_name: Optional[str] = None
+    api_version: Optional[str] = None
 
 
 class ModelConfig(Config):
     provider: str = Field(
         title="Model provider",
         description="The company providing the underlying model service.",
     )
@@ -692,15 +782,15 @@
     stop: Optional[Union[str, List[str]]]
     output_parser: Optional[str]
 
 
 class AgentConfig(Config):
     agent_class: str
     tools: List[ToolConfig]
-    model_config: ModelConfig
+    model: ModelConfig
     other: AgentOther
     type: str = "agent"
 
 
 class Log(BaseModel):
     project: Optional[str] = Field(
         title="Project name",
@@ -833,8 +923,54 @@
 def config_to_dict(config):
     # Handle config field
     if config:
         return config.dict()
     return None
 
 
+def requests_retry_session(
+    retries=8,
+    backoff_factor=0.3,
+    status_forcelist=(400, 500, 502, 503, 504),
+    session=None,
+    jitter_base=0.1,
+):
+    """
+    Creates a requests session with retry logic including exponential backoff with jitter.
+
+    Args:
+        retries (int): Number of retries.
+        backoff_factor (float): A base factor to apply for exponential backoff.
+        status_forcelist (tuple): A set of HTTP status codes that we should force a retry on.
+        session (requests.Session, optional): Use an existing session if provided, otherwise create a new one.
+
+    Returns:
+        requests.Session: A requests session configured with retry logic including jitter.
+    """
+    session = session or requests.Session()
+    retry = Retry(
+        total=retries,
+        read=retries,
+        connect=retries,
+        backoff_factor=backoff_factor,
+        status_forcelist=status_forcelist,
+        allowed_methods=["GET", "PUT", "POST"],
+        raise_on_status=False,
+    )
+
+    def backoff_with_jitter(retry, *args, **kwargs):
+        # Calculate the normal backoff
+        backoff_value = retry.get_backoff_time()
+        # Apply jitter by randomizing the backoff time
+        jittered_backoff = backoff_value + random.uniform(0, jitter_base)
+        return jittered_backoff
+
+    # Override the backoff method
+    retry.get_backoff_time = backoff_with_jitter
+
+    adapter = HTTPAdapter(max_retries=retry)
+    session.mount("http://", adapter)
+    session.mount("https://", adapter)
+    return session
+
+
 __all__ = ["HoneyHiveLangChainTracer"]
```

## honeyhive/utils/llamaindex_tracer.py

```diff
@@ -1,29 +1,40 @@
 # pylint: skip-file
+import json
 import os
 import uuid
 from collections import defaultdict
 from datetime import datetime
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import requests
 from llama_index.core.callbacks.base import BaseCallbackHandler
-from llama_index.core.callbacks.schema import TIMESTAMP_FORMAT, CBEvent, CBEventType
+from llama_index.core.callbacks.schema import (
+    TIMESTAMP_FORMAT,
+    CBEvent,
+    CBEventType,
+    LEAF_EVENTS,
+)
 from llama_index.core.callbacks.token_counting import get_llm_token_counts
 from llama_index.core.utilities.token_counting import TokenCounter
 
-from .langchain_tracer import Config, Log, log_to_dict
+from .langchain_tracer import (
+    Config,
+    LLMConfig,
+    Log,
+    log_to_dict,
+    requests_retry_session,
+)
 
 
 class HHEventType(str, Enum):
     MODEL = "model"
     CHAIN = "chain"
     TOOL = "tool"
-    GENERIC = "generic"
 
 
 class HoneyHiveLlamaIndexTracer(BaseCallbackHandler):
     _base_url: str = "https://api.honeyhive.ai"
     _headers: Dict[str, Any] = {"Content-Type": "application/json"}
     # Retrieve the API key from the environment variable
     _env_api_key = os.getenv("HONEYHIVE_API_KEY")
@@ -34,14 +45,15 @@
         name: Optional[str] = None,
         source: Optional[str] = None,
         user_properties: Optional[Dict[str, Any]] = None,
         tokenizer: Optional[TokenCounter] = None,
         event_starts_to_ignore: Optional[List[CBEventType]] = None,
         event_ends_to_ignore: Optional[List[CBEventType]] = None,
         api_key: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
     ) -> None:
         if self._env_api_key:
             api_key = self._env_api_key
         elif not api_key:
             raise ValueError(
                 "HoneyHive API key is not set! Please set the HONEYHIVE_API_KEY environment variable or pass in the api_key value."
             )
@@ -58,26 +70,67 @@
             TokenCounter(tokenizer=tokenizer) if tokenizer else TokenCounter()
         )
 
         self.name = name
         self.project = project
         self.source = source
         self.user_properties = user_properties
+        self.metadata = metadata
+        self.eval_info = None
+        self.root_event_ids = []
+        if self.source == "evaluation":
+            try:
+                if self.metadata and "run_id" in self.metadata:
+                    self.eval_info = {"run_id": self.metadata["run_id"]}
+                elif self.metadata and "dataset_name" in self.metadata:
+                    project_res = requests_retry_session().get(
+                        url=f"{self._base_url}/projects",
+                        headers=self._headers,
+                        params={"name": self.project},
+                    )
+                    if project_res.status_code == 200:
+                        project_id = project_res.json()[0]["_id"]
+                        dataset_res = requests_retry_session().get(
+                            url=f"{self._base_url}/datasets",
+                            headers=self._headers,
+                            params={
+                                "name": self.metadata["dataset_name"],
+                                "project": project_id,
+                            },
+                        )
+                        if dataset_res.status_code == 200:
+                            dataset = dataset_res.json()["testcases"][0]
+                            dataset_id = dataset["_id"]
+                            datapoint_ids = dataset["datapoints"]
+                            if "run_name" in self.metadata:
+                                run_name = self.metadata["run_name"]
+                            else:
+                                run_name = self.name
+                            self.eval_info = {
+                                "dataset_id": dataset_id,
+                                "datapoint_ids": datapoint_ids,
+                                "project_id": project_id,
+                                "run_name": run_name,
+                            }
+            except:
+                pass
+        self.session_id = None
 
     def _start_new_session(self, inputs):
         body = {
             "project": self.project,
             "source": self.source,
             "session_name": self.name,
             "session_id": self.session_id,
             "user_properties": self.user_properties,
+            "metadata": self.metadata,
             "inputs": inputs,
         }
 
-        requests.post(
+        res = requests_retry_session().post(
             url=f"{self._base_url}/session/start",
             headers=self._headers,
             json=body,
         )
 
     def on_event_start(
         self,
@@ -126,68 +179,60 @@
     def end_trace(
         self,
         trace_id: Optional[str] = None,
         trace_map: Optional[Dict[str, List[str]]] = None,
     ) -> None:
         self._trace_map = trace_map or defaultdict(list)
         self._end_time = datetime.now()
-
         self.log_trace()
 
     def log_trace(self) -> None:
         try:
-            child_nodes = self._trace_map.get("root")
-            if child_nodes:
-                root_span = self._convert_event_pair_to_log(
-                    self._event_pairs_by_id.get(child_nodes[0]),
-                    trace_id=self._cur_trace_id if len(child_nodes) > 1 else None,
-                )
-                if len(child_nodes) == 1:
-                    child_nodes = self._trace_map.get(child_nodes[0])
-                    root_span = self._build_trace(child_nodes, root_span)
-                else:
-                    root_span = self._build_trace(child_nodes, root_span)
-                if root_span and root_span.event_type == "chain":
-                    self._post_trace(root_span)
+            events = []
+            for event_list in self._trace_map.values():
+                events.extend(event_list)
+            events = set(events)
+            event_map = {}
+            for event in events:
+                event_pair = self._event_pairs_by_id[event]
+                event_log = self._convert_event_pair_to_log(event_pair)
+                event_map[event] = event_log
+            for event_id, child_event_ids in self._trace_map.items():
+                if event_id == "root":
+                    continue
+                parent_log = event_map[event_id]
+                for child_event_id in child_event_ids:
+                    child_log = event_map[child_event_id]
+                    child_log.parent_id = parent_log.event_id
+                    if parent_log.children is None:
+                        parent_log.children = [child_log]
+                    else:
+                        parent_log.children += [child_log]
+            root_events = []
+            for event_id in self._trace_map["root"]:
+                root_events.append(event_map[event_id])
+            root_events.sort(key=lambda event: event.start_time)
+            for event in root_events:
+                self._post_trace(event)
+
         except Exception:
             # Silently ignore errors to not break user code
             pass
 
-    def _build_trace(
-        self, events: List[str], span: Log, parent_id: Optional[str] = None
-    ) -> Log:
-        """Build the trace tree from the trace map."""
-        for child_event in events:
-            child_span = self._convert_event_pair_to_log(
-                self._event_pairs_by_id[child_event], parent_id=parent_id
-            )
-            child_span = self._build_trace(
-                self._trace_map[child_event], child_span, child_span.event_id
-            )
-            if span.children is None:
-                span.children = [child_span]
-            else:
-                span.children.append(child_span)
-        return span
-
     def _convert_event_pair_to_log(
         self,
         event_pair: List[CBEvent],
         parent_id: Optional[str] = None,
         trace_id: Optional[str] = None,
     ) -> Log:
         """Convert a pair of events to a HoneyHive log."""
-        start_time_us, end_time_us, end_time = self._get_time_in_us(event_pair)
+        start_time_us, end_time_us = self._get_time_in_us(event_pair)
 
-        if trace_id is None:
-            event_type = event_pair[0].event_type
-            span_kind = self._map_event_type(event_type)
-        else:
-            event_type = trace_id  # type: ignore
-            span_kind = "generic"
+        event_type = event_pair[0].event_type
+        span_kind = self._map_event_type(event_type)
 
         root_log = Log(
             project=self.project,
             source=self.source,
             event_id=str(uuid.uuid4()),
             inputs={},
             outputs={},
@@ -207,98 +252,197 @@
         root_log.outputs = outputs
 
         return root_log
 
     def _map_event_type(self, event_type: CBEventType) -> str:
         """Map a CBEventType to a HoneyHive event type."""
         if event_type in [
-            CBEventType.EMBEDDING,
             CBEventType.LLM,
-            CBEventType.SYNTHESIZE,
+            CBEventType.EMBEDDING,
+            CBEventType.AGENT_STEP,
+            CBEventType.RERANKING,
         ]:
             hh_event_type = HHEventType.MODEL
         elif event_type in [
-            CBEventType.QUERY,
+            CBEventType.CHUNKING,
+            CBEventType.NODE_PARSING,
             CBEventType.TREE,
-            CBEventType.SUB_QUESTION,
+            CBEventType.TEMPLATING,
+            CBEventType.FUNCTION_CALL,
+            CBEventType.EXCEPTION,
         ]:
-            hh_event_type = HHEventType.CHAIN
-        elif event_type == CBEventType.RETRIEVE:
             hh_event_type = HHEventType.TOOL
         else:
-            hh_event_type = HHEventType.GENERIC
+            hh_event_type = HHEventType.CHAIN
 
         return hh_event_type
 
     def _add_payload_to_log(
         self, span: Log, event_pair: List[CBEvent]
     ) -> Tuple[Optional[Dict[str, Any]], Optional[Dict[str, Any]], Log]:
         """Add the event's payload to the span."""
         assert len(event_pair) == 2
         event_type = event_pair[0].event_type
         inputs = None
         outputs = {}
 
         if event_type == CBEventType.NODE_PARSING:
-            # TODO: disabled full detailed inputs/outputs due to UI lag
             inputs, outputs = self._handle_node_parsing_payload(event_pair)
         elif event_type == CBEventType.LLM:
             inputs, outputs, span = self._handle_llm_payload(event_pair, span)
         elif event_type == CBEventType.QUERY:
             inputs, outputs = self._handle_query_payload(event_pair)
         elif event_type == CBEventType.EMBEDDING:
-            inputs, outputs = self._handle_embedding_payload(event_pair)
+            inputs, outputs, span = self._handle_embedding_payload(event_pair, span)
         elif event_type == CBEventType.RETRIEVE:
             inputs, outputs = self._handle_retrieve_payload(event_pair)
+        elif event_type == CBEventType.SYNTHESIZE:
+            inputs, outputs = self._handle_synthesize_payload(event_pair)
+        elif event_type == CBEventType.TEMPLATING:
+            inputs, outputs = self._handle_templating_payload(event_pair)
+        elif event_type == CBEventType.TREE:
+            inputs, outputs = self._handle_tree_payload(event_pair)
+        elif event_type == CBEventType.SUB_QUESTION:
+            inputs, outputs = self._handle_sub_question_payload(event_pair)
+        elif event_type == CBEventType.FUNCTION_CALL:
+            inputs, outputs = self._handle_function_call_payload(event_pair)
+        elif event_type == CBEventType.RERANKING:
+            inputs, outputs, span = self._handle_reranking_payload(event_pair, span)
+        elif event_type == CBEventType.EXCEPTION:
+            inputs, outputs = self._handle_exception_payload(event_pair)
+        elif event_type == CBEventType.AGENT_STEP:
+            inputs, outputs = self._handle_agent_step_payload(event_pair)
 
         return inputs, outputs, span
 
+    def _handle_agent_step_payload(
+        self, event_pair: List[CBEvent]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        # TODO: Implement this
+        inputs = event_pair[0].payload
+        outputs = event_pair[-1].payload
+        return inputs or {}, outputs or {}
+
+    def _handle_exception_payload(
+        self, event_pair: List[CBEvent]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        # TODO: Implement this
+        inputs = event_pair[0].payload
+        outputs = event_pair[-1].payload
+        return inputs or {}, outputs or {}
+
+    def _handle_reranking_payload(
+        self, event_pair: List[CBEvent], span: Log
+    ) -> Tuple[Dict[str, Any], Dict[str, Any], Log]:
+        input_payload = event_pair[0].payload
+        outputs = event_pair[-1].payload
+
+        inputs = {}
+        if "nodes" in input_payload:
+            inputs["nodes"] = input_payload["nodes"]
+        if "query_str" in input_payload:
+            inputs["query_str"] = input_payload["query_str"]
+        if "top_k" in input_payload:
+            inputs["top_k"] = input_payload["top_k"]
+
+        if "model_name" in input_payload:
+            config = LLMConfig()
+            config.model_name = input_payload["model_name"]
+            span.config = config
+
+        return inputs, outputs or {}, span
+
+    def _handle_function_call_payload(
+        self, event_pair: List[CBEvent]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        # TODO: Implement this
+        inputs = event_pair[0].payload
+        outputs = event_pair[-1].payload
+        return inputs or {}, outputs or {}
+
+    def _handle_sub_question_payload(
+        self, event_pair: List[CBEvent]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        # TODO: Implement this
+        inputs = event_pair[0].payload
+        outputs = event_pair[-1].payload
+        return inputs or {}, outputs or {}
+
+    def _handle_tree_payload(
+        self, event_pair: List[CBEvent]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        # TODO: Implement this
+        inputs = event_pair[0].payload
+        outputs = event_pair[-1].payload
+        return inputs or {}, outputs or {}
+
     def _handle_retrieve_payload(
         self, event_pair: List[CBEvent]
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         inputs = {"query_str": event_pair[0].payload["query_str"]}
         chunks = []
         for node in event_pair[1].payload["nodes"]:
             chunks.append({"score": node.score, "text": node.node.text})
         outputs = {"chunks": chunks}
         return inputs, outputs
 
-    def _handle_node_parsing_payload(
+    def _handle_templating_payload(
         self, event_pair: List[CBEvent]
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
-        """Handle the payload of a NODE_PARSING event."""
         inputs = event_pair[0].payload
         outputs = event_pair[-1].payload
+        return inputs or {}, outputs or {}
 
-        if inputs and "documents" in inputs:
-            documents = inputs.pop("documents")
-            inputs["num_documents"] = len(documents)
-
-        if outputs and "nodes" in outputs:
-            nodes = outputs.pop("nodes")
-            outputs["num_nodes"] = len(nodes)
+    def _handle_synthesize_payload(
+        self, event_pair: List[CBEvent]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        inputs = event_pair[0].payload
+        outputs = event_pair[-1].payload
+        return inputs or {}, outputs or {}
 
+    def _handle_node_parsing_payload(
+        self, event_pair: List[CBEvent]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        inputs = event_pair[0].payload
+        outputs = event_pair[-1].payload
         return inputs or {}, outputs or {}
 
     def _handle_llm_payload(
         self, event_pair: List[CBEvent], span: Log
     ) -> Tuple[Dict[str, Any], Dict[str, Any], Log]:
         """Handle the payload of a LLM event."""
-        inputs = event_pair[0].payload
+        input_payload = event_pair[0].payload
         outputs = event_pair[-1].payload
 
-        assert isinstance(inputs, dict) and isinstance(outputs, dict)
+        inputs = {}
 
         # Get `original_template` from Prompt
-        if "formatted_prompt" in inputs:
-            inputs["formatted_prompt"] = inputs["formatted_prompt"]
+        if "formatted_prompt" in input_payload:
+            inputs["formatted_prompt"] = input_payload["formatted_prompt"]
 
         # Format messages
-        if "messages" in inputs:
-            inputs["messages"] = "\n".join([str(x) for x in inputs["messages"]])
+        if "messages" in input_payload:
+            inputs["chat_history"] = []
+            for message in input_payload["messages"]:
+                role, content = str(message).split(":", 1)
+                inputs["chat_history"].append({"role": role, "content": content})
+
+        if "serialized" in input_payload:
+            config = LLMConfig()
+            if input_payload["serialized"].get("model"):
+                config.model_name = input_payload["serialized"]["model"]
+            if input_payload["serialized"].get("model_name"):
+                config.model_name = input_payload["serialized"]["model_name"]
+            if input_payload["serialized"].get("api_base"):
+                config.api_base = input_payload["serialized"]["api_base"]
+            if input_payload["serialized"].get("api_version"):
+                config.api_version = input_payload["serialized"]["api_version"]
+            if input_payload["serialized"].get("class_name"):
+                config.class_name = input_payload["serialized"]["class_name"]
+            span.config = config
 
         token_counts = get_llm_token_counts(self.tokenizer, outputs)
         metadata = {
             "formatted_prompt_tokens_count": token_counts.prompt_token_count,
             "prediction_tokens_count": token_counts.completion_token_count,
             "total_tokens_used": token_counts.total_token_count,
         }
@@ -314,84 +458,219 @@
 
     def _handle_query_payload(
         self, event_pair: List[CBEvent]
     ) -> Tuple[Optional[Dict[str, Any]], Dict[str, Any]]:
         """Handle the payload of a QUERY event."""
         inputs = event_pair[0].payload
         outputs = event_pair[-1].payload
-
-        if outputs:
-            response = outputs["response"]
-
-            if type(response).__name__ == "Response":
-                response = response.response
-            elif type(response).__name__ == "StreamingResponse":
-                response = response.get_response().response
-        else:
-            response = " "
-
-        outputs = {"response": response}
-
         return inputs, outputs
 
     def _handle_embedding_payload(
         self,
         event_pair: List[CBEvent],
-    ) -> Tuple[Optional[Dict[str, Any]], Dict[str, Any]]:
-        event_pair[0].payload
+        span: Log,
+    ) -> Tuple[Optional[Dict[str, Any]], Dict[str, Any], Log]:
+        input_payload = event_pair[0].payload
         outputs = event_pair[-1].payload
 
         chunks = []
         if outputs:
             chunks = outputs.get("chunks", [])
 
-        return {}, {"chunks": chunks}
+        inputs = {}
+        if "serialized" in input_payload:
+            config = LLMConfig()
+            if input_payload["serialized"].get("model"):
+                config.model_name = input_payload["serialized"]["model"]
+            if input_payload["serialized"].get("model_name"):
+                config.model_name = input_payload["serialized"]["model_name"]
+            if input_payload["serialized"].get("api_base"):
+                config.api_base = input_payload["serialized"]["api_base"]
+            if input_payload["serialized"].get("api_version"):
+                config.api_version = input_payload["serialized"]["api_version"]
+            if input_payload["serialized"].get("class_name"):
+                config.class_name = input_payload["serialized"]["class_name"]
+            span.config = config
+
+        inputs["chunks"] = chunks
+
+        return inputs, {}, span
 
     def _get_time_in_us(self, event_pair: List[CBEvent]) -> Tuple[int, int]:
         """Get the start and end time of an event pair in microseconds."""
         start_time = datetime.strptime(event_pair[0].time, TIMESTAMP_FORMAT)
         end_time = datetime.strptime(event_pair[1].time, TIMESTAMP_FORMAT)
 
         start_time_in_ms = int(
             (start_time - datetime(1970, 1, 1)).total_seconds() * 1000000
         )
         end_time_in_ms = int(
             (end_time - datetime(1970, 1, 1)).total_seconds() * 1000000
         )
 
-        return start_time_in_ms, end_time_in_ms, end_time
+        return start_time_in_ms, end_time_in_ms
 
     def _post_trace(self, root_log: Log) -> None:
+        self.root_event_ids.append(root_log.event_id)
         root_log = log_to_dict(root_log)
         self.final_outputs = root_log["outputs"]
-        self.session_id = str(uuid.uuid4())
-        self._set_parent_ids(root_log, self.session_id)
-        self._start_new_session(root_log["inputs"])
-        trace_response = requests.post(
+        first_trace = False
+        if self.session_id is None:
+            first_trace = True
+            self.session_id = str(uuid.uuid4())
+            self._start_new_session(root_log["inputs"])
+        self._crawl(root_log, self.session_id)
+
+        trace_response = requests_retry_session().post(
             url=f"{self._base_url}/session/{self.session_id}/traces",
             json={"logs": [root_log]},
             headers=self._headers,
         )
         if trace_response.status_code != 200:
             raise Exception(
                 f"Failed to post trace to HoneyHive with status code {trace_response.status_code}"
             )
-        requests.put(
-            url=f"{self._base_url}/events/{self.session_id}/traces",
-            json={"event_id": self.session_id, "outputs": self.final_outputs},
+        requests_retry_session().put(
+            url=f"{self._base_url}/events",
+            json={
+                "event_id": self.session_id,
+                "outputs": self.final_outputs,
+                "children_ids": self.root_event_ids,
+            },
             headers=self._headers,
         )
+        if self.eval_info and first_trace:
+            try:
+                if "run_id" in self.eval_info:
+                    run_res = requests_retry_session().get(
+                        url=f"{self._base_url}/runs/{self.eval_info['run_id']}",
+                        headers=self._headers,
+                    )
+                    event_ids = run_res.json()["evaluation"]["event_ids"]
+                    event_ids.append(self.session_id)
+                    requests_retry_session().put(
+                        url=f"{self._base_url}/runs/{self.eval_info['run_id']}",
+                        json={"event_ids": event_ids},
+                        headers=self._headers,
+                    )
+                else:
+                    body = {
+                        "event_ids": [self.session_id],
+                        "dataset_id": self.eval_info["dataset_id"],
+                        "datapoint_ids": self.eval_info["datapoint_ids"],
+                        "project": self.eval_info["project_id"],
+                        "status": "completed",
+                        "name": self.eval_info["run_name"],
+                    }
+                    if "config" in root_log:
+                        body["configuration"] = root_log["config"]
+                    run_res = requests_retry_session().post(
+                        url=f"{self._base_url}/runs",
+                        headers=self._headers,
+                        json=body,
+                    )
+                    run_id = run_res.json()["run_id"]
+                    self.eval_info["run_id"] = run_id
+            except:
+                pass
+
+    def _parse_chat_history(self, chat_string):
+        # Split the string into lines
+        lines = chat_string.split("\n")
+
+        # This list will store our parsed chat history
+        chat_history = []
+
+        # Temporary variables to hold current role and content
+        current_role = None
+        content = []
+
+        # Helper function to add an entry to chat history
+        def add_entry(role, content):
+            if content:
+                chat_history.append(
+                    {"role": role, "content": "\n".join(content).strip()}
+                )
+
+        # Iterate through each line to process the content
+        for line in lines:
+            # Check if the line starts a new role section
+            if line.startswith(("system:", "user:", "assistant:")):
+                # If there is an existing role and content, save it
+                if current_role is not None:
+                    add_entry(current_role, content)
+
+                # Reset for the new role
+                parts = line.split(":", 1)
+                current_role = parts[0].strip()
+                content = [parts[1].strip()] if len(parts) > 1 else []
+            else:
+                # Continue accumulating content for the current role
+                content.append(line)
+
+        # Don't forget to add the last accumulated content to the chat history
+        add_entry(current_role, content)
+
+        return chat_history
 
-    def _set_parent_ids(self, trace, session_id) -> None:
+    def _crawl(self, trace, session_id) -> None:
         def crawl(node):
             if node is None:
                 return
             node["session_id"] = session_id
             self.final_outputs = node["outputs"]
             if node["children"]:
+                """
+                We do a pattern-match for the following pattern in the event tree:
+                synthesize
+                  llm
+                  templating
+
+                We then replace this pattern with a single event that has all of the information from these events rolled into one.
+                TODO: Look into replacing this workaround if the instrumentation from the LlamaIndex side changes.
+                """
+                if (
+                    len(node["children"]) == 2
+                    and node["event_name"] == CBEventType.SYNTHESIZE
+                ):
+                    child1, child2 = node["children"][0], node["children"][1]
+                    pattern = set([CBEventType.TEMPLATING, CBEventType.LLM])
+                    child_event_names = set(
+                        [child1["event_name"], child2["event_name"]]
+                    )
+                    if (
+                        pattern == child_event_names
+                        and not child1["children"]
+                        and not child2["children"]
+                    ):
+                        if child1["event_name"] == CBEventType.LLM:
+                            llm_event = child1
+                            templating_event = child2
+                        else:
+                            llm_event = child2
+                            templating_event = child1
+                        node["children"] = None
+                        node["outputs"] = llm_event.get("outputs")
+                        node["config"] = llm_event["config"]
+                        inputs = {}
+                        if "chat_history" in llm_event["inputs"]:
+                            inputs["chat_history"] = llm_event["inputs"]["chat_history"]
+                        if "template" in templating_event["inputs"]:
+                            node["config"]["template"] = self._parse_chat_history(
+                                templating_event["inputs"]["template"]
+                            )
+                        if "template_vars" in templating_event["inputs"]:
+                            template_vars = templating_event["inputs"]["template_vars"]
+                            if "query_str" in template_vars:
+                                inputs["query_str"] = template_vars["query_str"]
+                            if "context_str" in template_vars:
+                                inputs["context_str"] = template_vars["context_str"]
+                        node["inputs"] = inputs
+                        node["event_type"] = HHEventType.MODEL
+                        return
                 for child in node["children"]:
                     child["parent_id"] = node["event_id"]
                     crawl(child)
 
         crawl(trace)
 
     def finish(self) -> None:
```

## honeyhive/utils/tracer.py

```diff
@@ -6,14 +6,15 @@
 import traceback
 import datetime
 import inspect
 import requests
 import openai
 
 from pathlib import Path
+from .langchain_tracer import requests_retry_session
 
 sys.path.append(str(Path(__file__).resolve().parent.parent))
 import honeyhive
 
 
 class HoneyHiveTraceContextManager:
     def __init__(self, tracer):
@@ -42,15 +43,15 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.end_time = time.time()
         sys.settrace(self.original_trace_function)
         self.prepare_input()
         self.prepare_output()
         self.prepare_error(exc_type, exc_val)
-        self.tracer.log_event_with_data(self.event_data)
+        self.event_data = self.tracer.log_event_with_data(self.event_data)
 
     def prepare_input(self):
         # prepare input, output, metadata, duration, error
         if "kwargs" in self.first_call_value:
             temp = dict(self.first_call_value["kwargs"])
             del self.first_call_value["kwargs"]
             for key, value in temp.items():
@@ -126,39 +127,44 @@
             if self.event_data["event_name"] == "":
                 self.event_data["event_name"] = frame.f_code.co_name
         elif event == "return":
             self.last_return_value = arg
 
         return self.general_trace_call
 
+    def get_output(self):
+        return self.event_data["output"]
+
 
 class HoneyHiveTracer:
     def __init__(
         self, project, name, source, api_key, user_properties={}, show_trace=False
     ):
         self._base_url = "https://api.honeyhive.ai"
         self._headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {api_key}",
         }
-        self.sdk = honeyhive.HoneyHive(bearer_auth=api_key)
-        res = self.sdk.session.start_session(
-            {
-                "session": {
-                    "project": project,
-                    "session_name": name,
-                    "source": source,
-                    "user_properties": user_properties,
-                }
+        body = {
+            "session": {
+                "project": project,
+                "session_name": name,
+                "source": source,
+                "user_properties": user_properties,
             }
+        }
+
+        res = requests_retry_session().post(
+            url=f"{self._base_url}/session/start",
+            headers=self._headers,
+            json=body,
         )
-        if res.object is not None:
-            self.session_id = res.object.session_id
-        else:
-            raise Exception("Unable to start session")
+        data = res.json()
+        self.session_id = data["session_id"]
+
         self.events = []
         self.project = project
         self.source = source
         self.event_id = None
         self.event_type = "model"
         self.event_name = ""
         self.config = {"provider": "", "endpoint": ""}
@@ -367,18 +373,18 @@
 
     def log_event(self):
         # print("Logging event")
         if self.show_trace:
             self.print_event()
 
         if type(self.input) != dict:
-            self.input = { "input": self.input }
+            self.input = {"input": self.input}
         if type(self.output) != dict:
-            self.output = { "role": "assistant", "content": self.output }
-        
+            self.output = {"role": "assistant", "content": self.output}
+
         event = {
             "event_name": self.event_name,
             "event_type": self.event_type,
             "project": self.project,
             "source": self.source,
             "config": self.config,
             "inputs": self.input,
@@ -387,15 +393,15 @@
             "duration": self.duration,
             "metadata": self.metadata,
             "user_properties": self.user_properties,
             "parent_id": self.session_id,
             "session_id": self.session_id,
         }
 
-        res = requests.post(
+        res = requests_retry_session().post(
             url=f"{self._base_url}/events",
             json={"event": event},
             headers=self._headers,
         )
 
         # reset the event
         self.event_id = None
@@ -425,61 +431,59 @@
                 # if there is, don't overwrite it
                 if not hasattr(self, key) or getattr(self, key) is None:
                     setattr(self, key, value)
 
         # check if "provider" and "endpoint" are in config
         if self.config.get("provider") == "openai":
             if self.config.get("endpoint") == "streaming":
-                self.output = {
-                    "role": "assistant",
-                    "content": None
-                }
+                self.output = {"role": "assistant", "content": None}
                 func_call = {
                     "name": None,
                     "arguments": "",
                 }
-                
+
                 for chunk in event_data["output"]:
                     if not chunk.choices:
                         continue
                     delta = chunk.choices[0].delta
 
                     if delta.content:
                         if not self.output.get("content"):
                             self.output["content"] = ""
-                        
+
                         self.output["content"] += delta.content
                     elif delta.tool_calls:
                         delta = delta.tool_calls[0]
                         if delta.function.name:
                             func_call["name"] = delta.function.name
-                        
+
                         if delta.function.arguments:
                             func_call["arguments"] += delta.function.arguments
-                
+
                 if func_call["arguments"] != "":
                     func_call["arguments"] = json.loads(func_call["arguments"])
                 if func_call["name"]:
-                    self.output["tool_calls"] = [{
-                        "type": "function",
-                        "function": func_call
-                    }]
+                    self.output["tool_calls"] = [
+                        {"type": "function", "function": func_call}
+                    ]
             else:
                 self.output = event_data["output"].choices[0].message
             self.duration = event_data["duration"]
-        
+
         # check for pydantic models
         try:
             self.output = self.output.model_dump()
             # drop any fields whose value is None from self.output
             self.output = {k: v for k, v in self.output.items() if v is not None}
         except:
             pass
 
+        event_data["output"] = self.output
         self.log_event()
+        return event_data
 
     def set_model_context(
         self,
         event_name,
         input,
         func,
         prompt_template="",
```

## Comparing `honeyhive-0.1.91.dist-info/LICENSE.md` & `honeyhive-0.1.92.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `honeyhive-0.1.91.dist-info/METADATA` & `honeyhive-0.1.92.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeyhive
-Version: 0.1.91
+Version: 0.1.92
 Summary: The HoneyHive SDK for Python
 Author: HoneyHive
 Author-email: support@honeyhive.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.honeyhive.ai/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


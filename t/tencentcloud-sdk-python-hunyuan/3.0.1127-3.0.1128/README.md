# Comparing `tmp/tencentcloud-sdk-python-hunyuan-3.0.1127.tar.gz` & `tmp/tencentcloud-sdk-python-hunyuan-3.0.1128.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1127.tar", last modified: Wed Apr 10 20:46:57 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1128.tar", last modified: Fri Apr 12 09:51:11 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127.tar` & `tencentcloud-sdk-python-hunyuan-3.0.1128.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/v20230901/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/v20230901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25912 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/v20230901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/v20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5163 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/v20230901/hunyuan_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/setup.py
--rw-r--r--   0 root         (0) root         (0)      749 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud_sdk_python_hunyuan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      539 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-10 20:46:57.000000 tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-12 09:51:10.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 09:51:10.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/v20230901/
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-12 09:51:10.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/v20230901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    30308 2024-04-12 09:51:10.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/v20230901/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 09:51:10.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/v20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5295 2024-04-12 09:51:10.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/v20230901/hunyuan_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-12 09:51:10.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/setup.py
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-12 09:51:10.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud_sdk_python_hunyuan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-12 09:51:11.000000 tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1128/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1127
+Version: 3.0.1128
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1127'
+__version__ = '3.0.1128'
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/v20230901/errorcodes.py` & `tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/v20230901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/v20230901/models.py` & `tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/v20230901/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,32 +23,51 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Messages: 聊天上下文信息。
 说明：
-1.长度最多为40, 按对话时间从旧到新在数组中排列。
-2.Message的Role当前可选值：system、user、assistant，其中，system角色是可选的，如果存在，必须位于列表的最开始。user和assistant需要交替出现(一问一答)，最后一个为user提问, 且Content不能为空。
-3.Messages中Content总长度不超过16000 token，超过则会截断最前面的内容，只保留尾部内容。建议不超过4000 token。
+1. 长度最多为 40，按对话时间从旧到新在数组中排列。
+2. Message 的 Role 当前可选值：system、user、assistant。其中，system 角色是可选的，如果存在，必须位于列表的最开始。此外，user 和 assistant 需交替出现（一问一答），以 user 提问开始和结束，且 Content 不能为空。Role 的顺序示例：[system（可选） user assistant user assistant user ...]。
+3. Messages 中 Content 总长度不超过 16000 Token，超过则会截断最前面的内容，只保留尾部内容。建议不超过 4000 Token。
         :type Messages: list of Message
         :param _TopP: 说明：
-1.影响输出文本的多样性，取值越大，生成文本的多样性越强。
-2.默认1.0，取值区间为[0.0, 1.0]。
-3.非必要不建议使用, 不合理的取值会影响效果。
+1. 影响输出文本的多样性，取值越大，生成文本的多样性越强。
+2. 默认 1.0，取值区间为 [0.0, 1.0]。
+3. 非必要不建议使用，不合理的取值会影响效果。
         :type TopP: float
         :param _Temperature: 说明：
-1.较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
-2.默认1.0，取值区间为[0.0，2.0]。
-3.非必要不建议使用,不合理的取值会影响效果。
+1. 较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
+2. 默认 1.0，取值区间为 [0.0，2.0]。
+3. 非必要不建议使用，不合理的取值会影响效果。
         :type Temperature: float
+        :param _Stream: 流式调用开关。
+说明：
+1. 未传值时默认为流式调用。
+2. 流式调用时以 SSE 协议增量返回结果。
+3. 非流式调用时接口响应耗时较长，非必要不建议使用。
+4. 非流式调用时只返回一次最终结果，调用方式与普通 HTTP 请求无异。
+        :type Stream: bool
+        :param _StreamModeration: 流式输出审核开关。
+说明：
+1. 当 Stream 字段值为 true 时，该字段有效。
+2. 未传值时默认不使用流式输出审核。
+3. 如果值为 true，将对输出内容进行分段审核，审核通过的内容流式输出返回。如果出现审核不过，响应中的 finish_reason 值为 sensitive。
+4. 如果值为 false，则需要审核完所有输出内容后再返回结果。
+
+注意：
+当选择流式输出审核时，可能会出现部分内容已输出，但中间某一段响应中的 finish_reason 值为 sensitive，此时说明安全审核未通过。如果业务场景有实时文字上屏的需求，需要自行撤回已上屏的内容，并建议自定义替换为一条提示语，如 “这个问题我不方便回答，不如我们换个话题试试”，以保障终端体验。
+        :type StreamModeration: bool
         """
         self._Messages = None
         self._TopP = None
         self._Temperature = None
+        self._Stream = None
+        self._StreamModeration = None
 
     @property
     def Messages(self):
         return self._Messages
 
     @Messages.setter
     def Messages(self, Messages):
@@ -66,24 +85,42 @@
     def Temperature(self):
         return self._Temperature
 
     @Temperature.setter
     def Temperature(self, Temperature):
         self._Temperature = Temperature
 
+    @property
+    def Stream(self):
+        return self._Stream
+
+    @Stream.setter
+    def Stream(self, Stream):
+        self._Stream = Stream
+
+    @property
+    def StreamModeration(self):
+        return self._StreamModeration
+
+    @StreamModeration.setter
+    def StreamModeration(self, StreamModeration):
+        self._StreamModeration = StreamModeration
+
 
     def _deserialize(self, params):
         if params.get("Messages") is not None:
             self._Messages = []
             for item in params.get("Messages"):
                 obj = Message()
                 obj._deserialize(item)
                 self._Messages.append(obj)
         self._TopP = params.get("TopP")
         self._Temperature = params.get("Temperature")
+        self._Stream = params.get("Stream")
+        self._StreamModeration = params.get("StreamModeration")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -93,22 +130,22 @@
 class ChatProResponse(AbstractModel):
     """ChatPro返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Created: unix 时间戳，单位为秒。
+        :param _Created: Unix 时间戳，单位为秒。
         :type Created: int
-        :param _Usage: token统计信息。
-按照总token数量计费。
+        :param _Usage: Token 统计信息。
+按照总 Token 数量计费。
         :type Usage: :class:`tencentcloud.hunyuan.v20230901.models.Usage`
         :param _Note: 免责声明。
         :type Note: str
-        :param _Id: 本轮对话的id。
+        :param _Id: 本轮对话的 ID。
         :type Id: str
         :param _Choices: 回复内容。
         :type Choices: list of Choice
         :param _ErrorMsg: 错误信息。
 如果流式返回中服务处理异常，返回该错误信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ErrorMsg: :class:`tencentcloud.hunyuan.v20230901.models.ErrorMsg`
@@ -204,32 +241,52 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Messages: 聊天上下文信息。
 说明：
-1.长度最多为40, 按对话时间从旧到新在数组中排列。
-2.Message的Role当前可选值：user、assistant，其中，user和assistant需要交替出现(一问一答)，最后一个为user提问, 且Content不能为空。
-3.Messages中Content总长度不超过16000 token，超过则会截断最前面的内容，只保留尾部内容。建议不超过4000 token。
+1. 长度最多为 40，按对话时间从旧到新在数组中排列。
+2. Message 的 Role 当前可选值：user、assistant。其中，user 和 assistant 需交替出现（一问一答），以 user 提问开始和结束，且 Content 不能为空。Role 的顺序示例：[user assistant user assistant user ...]。
+3. Messages 中 Content 总长度不超过 16000 Token，超过则会截断最前面的内容，只保留尾部内容。建议不超过 4000 Token。
+
         :type Messages: list of Message
         :param _TopP: 说明：
-1.影响输出文本的多样性，取值越大，生成文本的多样性越强。
-2.默认1.0，取值区间为[0.0, 1.0]。
-3.非必要不建议使用, 不合理的取值会影响效果。
+1. 影响输出文本的多样性，取值越大，生成文本的多样性越强。
+2. 默认 1.0，取值区间为 [0.0, 1.0]。
+3. 非必要不建议使用，不合理的取值会影响效果。
         :type TopP: float
         :param _Temperature: 说明：
-1.较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
-2.默认1.0，取值区间为[0.0，2.0]。
-3.非必要不建议使用,不合理的取值会影响效果。
+1. 较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
+2. 默认 1.0，取值区间为 [0.0，2.0]。
+3. 非必要不建议使用，不合理的取值会影响效果。
         :type Temperature: float
+        :param _Stream: 流式调用开关。
+说明：
+1. 未传值时默认为流式调用。
+2. 流式调用时以 SSE 协议增量返回结果。
+3. 非流式调用时接口响应耗时较长，非必要不建议使用。
+4. 非流式调用时只返回一次最终结果，调用方式与普通 HTTP 请求无异。
+        :type Stream: bool
+        :param _StreamModeration: 流式输出审核开关。
+说明：
+1. 当 Stream 字段值为 true 时，该字段有效。
+2. 未传值时默认不使用流式输出审核。
+3. 如果值为 true，将对输出内容进行分段审核，审核通过的内容流式输出返回。如果出现审核不过，响应中的 finish_reason 值为 sensitive。
+4. 如果值为 false，则需要审核完所有输出内容后再返回结果。
+
+注意：
+当选择流式输出审核时，可能会出现部分内容已输出，但中间某一段响应中的 finish_reason 值为 sensitive，此时说明安全审核未通过。如果业务场景有实时文字上屏的需求，需要自行撤回已上屏的内容，并建议自定义替换为一条提示语，如 “这个问题我不方便回答，不如我们换个话题试试”，以保障终端体验。
+        :type StreamModeration: bool
         """
         self._Messages = None
         self._TopP = None
         self._Temperature = None
+        self._Stream = None
+        self._StreamModeration = None
 
     @property
     def Messages(self):
         return self._Messages
 
     @Messages.setter
     def Messages(self, Messages):
@@ -247,24 +304,42 @@
     def Temperature(self):
         return self._Temperature
 
     @Temperature.setter
     def Temperature(self, Temperature):
         self._Temperature = Temperature
 
+    @property
+    def Stream(self):
+        return self._Stream
+
+    @Stream.setter
+    def Stream(self, Stream):
+        self._Stream = Stream
+
+    @property
+    def StreamModeration(self):
+        return self._StreamModeration
+
+    @StreamModeration.setter
+    def StreamModeration(self, StreamModeration):
+        self._StreamModeration = StreamModeration
+
 
     def _deserialize(self, params):
         if params.get("Messages") is not None:
             self._Messages = []
             for item in params.get("Messages"):
                 obj = Message()
                 obj._deserialize(item)
                 self._Messages.append(obj)
         self._TopP = params.get("TopP")
         self._Temperature = params.get("Temperature")
+        self._Stream = params.get("Stream")
+        self._StreamModeration = params.get("StreamModeration")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -274,22 +349,22 @@
 class ChatStdResponse(AbstractModel):
     """ChatStd返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Created: unix 时间戳，单位为秒。
+        :param _Created: Unix 时间戳，单位为秒。
         :type Created: int
-        :param _Usage: token统计信息。
-按照总token数量计费。
+        :param _Usage: Token 统计信息。
+按照总 Token 数量计费。
         :type Usage: :class:`tencentcloud.hunyuan.v20230901.models.Usage`
         :param _Note: 免责声明。
         :type Note: str
-        :param _Id: 本轮对话的id。
+        :param _Id: 本轮对话的 ID。
         :type Id: str
         :param _Choices: 回复内容。
         :type Choices: list of Choice
         :param _ErrorMsg: 错误信息。
 如果流式返回中服务处理异常，返回该错误信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ErrorMsg: :class:`tencentcloud.hunyuan.v20230901.models.ErrorMsg`
@@ -383,21 +458,26 @@
 class Choice(AbstractModel):
     """返回的回复, 支持多个
 
     """
 
     def __init__(self):
         r"""
-        :param _FinishReason: 流式结束标志位，为 stop 则表示尾包。
+        :param _FinishReason: 结束标志位，为 stop 则表示尾包。
         :type FinishReason: str
-        :param _Delta: 返回值。
+        :param _Delta: 增量返回值，流式调用时使用该字段。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Delta: :class:`tencentcloud.hunyuan.v20230901.models.Delta`
+        :param _Message: 返回值，非流式调用时使用该字段。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: :class:`tencentcloud.hunyuan.v20230901.models.Message`
         """
         self._FinishReason = None
         self._Delta = None
+        self._Message = None
 
     @property
     def FinishReason(self):
         return self._FinishReason
 
     @FinishReason.setter
     def FinishReason(self, FinishReason):
@@ -407,20 +487,31 @@
     def Delta(self):
         return self._Delta
 
     @Delta.setter
     def Delta(self, Delta):
         self._Delta = Delta
 
+    @property
+    def Message(self):
+        return self._Message
+
+    @Message.setter
+    def Message(self, Message):
+        self._Message = Message
+
 
     def _deserialize(self, params):
         self._FinishReason = params.get("FinishReason")
         if params.get("Delta") is not None:
             self._Delta = Delta()
             self._Delta._deserialize(params.get("Delta"))
+        if params.get("Message") is not None:
+            self._Message = Message()
+            self._Message._deserialize(params.get("Message"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -805,23 +896,23 @@
         self._TokenCount = params.get("TokenCount")
         self._CharacterCount = params.get("CharacterCount")
         self._Tokens = params.get("Tokens")
         self._RequestId = params.get("RequestId")
 
 
 class Message(AbstractModel):
-    """会话内容,  按对话时间序排列，长度最多为40
+    """单条消息
 
     """
 
     def __init__(self):
         r"""
         :param _Role: 角色
         :type Role: str
-        :param _Content: 消息的内容
+        :param _Content: 消息内容
         :type Content: str
         """
         self._Role = None
         self._Content = None
 
     @property
     def Role(self):
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud/hunyuan/v20230901/hunyuan_client.py` & `tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud/hunyuan/v20230901/hunyuan_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 class HunyuanClient(AbstractClient):
     _apiVersion = '2023-09-01'
     _endpoint = 'hunyuan.tencentcloudapi.com'
     _service = 'hunyuan'
 
 
     def ChatPro(self, request):
-        """腾讯混元大模型高级版是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口为SSE协议。
+        """腾讯混元大模型高级版是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
 
-         1.本接口暂不支持返回图片内容。
-         2.默认单账号限制并发数为5路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
-         3.请使用SDK调用本接口 ，每种开发语言的SDK GitHub仓库examples/hunyuan/v20230901/目录下有提供示例供参考。
+         1. 本接口暂不支持返回图片内容。
+         2. 默认单账号限制并发数为 5 路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
+         3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。
 
         :param request: Request instance for ChatPro.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatProRequest`
         :rtype: :class:`tencentcloud.hunyuan.v20230901.models.ChatProResponse`
 
         """
         try:
@@ -45,19 +45,19 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChatStd(self, request):
-        """腾讯混元大模型标准版是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口为SSE协议。
+        """腾讯混元大模型标准版是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
 
-         1.本接口暂不支持返回图片内容。
-         2.默认单账号限制并发数为5路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
-         3.请使用SDK调用本接口 ，每种开发语言的SDK GitHub仓库examples/hunyuan/v20230901/目录下有提供示例供参考。
+         1. 本接口暂不支持返回图片内容。
+         2. 默认单账号限制并发数为 5 路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
+         3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。
 
         :param request: Request instance for ChatStd.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatStdRequest`
         :rtype: :class:`tencentcloud.hunyuan.v20230901.models.ChatStdResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/setup.py` & `tencentcloud-sdk-python-hunyuan-3.0.1128/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hunyuan',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1127"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1128"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hunyuan SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/README.rst` & `tencentcloud-sdk-python-hunyuan-3.0.1128/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1127
+Version: 3.0.1128
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1127/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-hunyuan-3.0.1128/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*


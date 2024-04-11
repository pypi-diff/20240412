# Comparing `tmp/prodpadlm_client-0.1.1.3.1.tar.gz` & `tmp/prodpadlm_client-0.1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodpadlm_client-0.1.1.3.1.tar", last modified: Mon Apr  8 08:04:07 2024, max compression
+gzip compressed data, was "prodpadlm_client-0.1.1.4.tar", last modified: Thu Apr 11 23:51:51 2024, max compression
```

## Comparing `prodpadlm_client-0.1.1.3.1.tar` & `prodpadlm_client-0.1.1.4.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 08:04:07.388563 prodpadlm_client-0.1.1.3.1/
--rw-rw-rw-   0        0        0     1727 2024-04-08 08:04:07.386563 prodpadlm_client-0.1.1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1413 2024-04-08 07:39:29.000000 prodpadlm_client-0.1.1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 08:04:07.342179 prodpadlm_client-0.1.1.3.1/prodpadlm_client/
--rw-rw-rw-   0        0        0       49 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client/__init__.py
--rw-rw-rw-   0        0        0    10761 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-08 08:04:07.376972 prodpadlm_client-0.1.1.3.1/prodpadlm_client/client_types/
--rw-rw-rw-   0        0        0        0 2024-04-08 08:03:15.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client/client_types/__init__.py
--rw-rw-rw-   0        0        0     3112 2024-04-08 01:09:30.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client/client_types/messages.py
-drwxrwxrwx   0        0        0        0 2024-04-08 08:04:07.383165 prodpadlm_client-0.1.1.3.1/prodpadlm_client/resources/
--rw-rw-rw-   0        0        0        0 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client/resources/__init__.py
--rw-rw-rw-   0        0        0     2814 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client/resources/api.py
-drwxrwxrwx   0        0        0        0 2024-04-08 08:04:07.371728 prodpadlm_client-0.1.1.3.1/prodpadlm_client.egg-info/
--rw-rw-rw-   0        0        0     1727 2024-04-08 08:04:06.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2024-04-08 08:04:07.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 08:04:06.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-08 08:04:06.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-08 08:04:06.000000 prodpadlm_client-0.1.1.3.1/prodpadlm_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 08:04:07.389558 prodpadlm_client-0.1.1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      895 2024-04-08 08:03:24.000000 prodpadlm_client-0.1.1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.488406 prodpadlm_client-0.1.1.4/
+-rw-rw-rw-   0        0        0    11556 2024-04-08 06:33:36.000000 prodpadlm_client-0.1.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    15472 2024-04-11 23:51:51.485396 prodpadlm_client-0.1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1413 2024-04-08 07:39:29.000000 prodpadlm_client-0.1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.400010 prodpadlm_client-0.1.1.4/prodpadlm_client/
+-rw-rw-rw-   0        0        0       49 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/__init__.py
+-rw-rw-rw-   0        0        0    10775 2024-04-11 22:04:07.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.476251 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/
+-rw-rw-rw-   0        0        0        0 2024-04-08 08:03:15.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-10 11:04:40.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/_types.py
+-rw-rw-rw-   0        0        0     3112 2024-04-08 01:09:30.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/messages.py
+-rw-rw-rw-   0        0        0     2052 2024-04-11 22:01:54.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/stream_messages.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.481260 prodpadlm_client-0.1.1.4/prodpadlm_client/resources/
+-rw-rw-rw-   0        0        0        0 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/resources/__init__.py
+-rw-rw-rw-   0        0        0     6250 2024-04-11 22:39:06.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/resources/api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.484064 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/
+-rw-rw-rw-   0        0        0    15472 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      958 2024-04-11 23:51:37.000000 prodpadlm_client-0.1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 23:51:51.488406 prodpadlm_client-0.1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      938 2024-04-11 22:47:39.000000 prodpadlm_client-0.1.1.4/setup.py
```

### Comparing `prodpadlm_client-0.1.1.3.1/PKG-INFO` & `prodpadlm_client-0.1.1.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: prodpadlm_client
-Version: 0.1.1.3.1
-Summary: Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡
-Author: Ayo Kehinde Samuel
-License: Apache 2.0
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-
 # ProdPadLM - Client
 
 Production LaunchPad for Language Models [Client] is a robust service designed to seamlessly integrate the ProdPadLM server into applications. It is built with support for Langchain, a powerful language processing tool, making it an ideal choice for applications that require advanced language model capabilities.
 
 ## Features
 
 - **Seamless Integration**: ProdPadLM - Client is designed to easily integrate with your existing applications, reducing the need for extensive code changes.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prodpadlm_client-0.1.1.3.1/prodpadlm_client/client.py` & `prodpadlm_client-0.1.1.4/prodpadlm_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,149 +525,150 @@
 000020c0: 2d3e 2049 7465 7261 746f 725b 4368 6174  -> Iterator[Chat
 000020d0: 4765 6e65 7261 7469 6f6e 4368 756e 6b5d  GenerationChunk]
 000020e0: 3a0d 0a20 2020 2020 2020 2070 6172 616d  :..        param
 000020f0: 7320 3d20 7365 6c66 2e5f 666f 726d 6174  s = self._format
 00002100: 5f70 6172 616d 7328 6d65 7373 6167 6573  _params(messages
 00002110: 3d6d 6573 7361 6765 732c 2073 746f 703d  =messages, stop=
 00002120: 7374 6f70 2c20 2a2a 6b77 6172 6773 290d  stop, **kwargs).
-00002130: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00002140: 6c66 2e5f 636c 6965 6e74 2e6d 6573 7361  lf._client.messa
-00002150: 6765 732e 7374 7265 616d 282a 2a70 6172  ges.stream(**par
-00002160: 616d 7329 2061 7320 7374 7265 616d 3a0d  ams) as stream:.
-00002170: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00002180: 2074 6578 7420 696e 2073 7472 6561 6d2e   text in stream.
-00002190: 7465 7874 5f73 7472 6561 6d3a 0d0a 2020  text_stream:..  
-000021a0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-000021b0: 756e 6b20 3d20 4368 6174 4765 6e65 7261  unk = ChatGenera
-000021c0: 7469 6f6e 4368 756e 6b28 6d65 7373 6167  tionChunk(messag
-000021d0: 653d 4149 4d65 7373 6167 6543 6875 6e6b  e=AIMessageChunk
-000021e0: 2863 6f6e 7465 6e74 3d74 6578 7429 290d  (content=text)).
-000021f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002200: 2069 6620 7275 6e5f 6d61 6e61 6765 723a   if run_manager:
-00002210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002220: 2020 2020 2020 7275 6e5f 6d61 6e61 6765        run_manage
-00002230: 722e 6f6e 5f6c 6c6d 5f6e 6577 5f74 6f6b  r.on_llm_new_tok
-00002240: 656e 2874 6578 742c 2063 6875 6e6b 3d63  en(text, chunk=c
-00002250: 6875 6e6b 290d 0a20 2020 2020 2020 2020  hunk)..         
-00002260: 2020 2020 2020 2079 6965 6c64 2063 6875         yield chu
-00002270: 6e6b 0d0a 0d0a 2020 0d0a 0d0a 2020 2020  nk....  ....    
-00002280: 6465 6620 5f66 6f72 6d61 745f 6f75 7470  def _format_outp
-00002290: 7574 2873 656c 662c 2064 6174 613a 2041  ut(self, data: A
-000022a0: 6e79 2c20 2a2a 6b77 6172 6773 3a20 416e  ny, **kwargs: An
-000022b0: 7929 202d 3e20 4368 6174 5265 7375 6c74  y) -> ChatResult
-000022c0: 3a0d 0a20 2020 2020 2020 2064 6174 615f  :..        data_
-000022d0: 6469 6374 203d 2064 6174 612e 6d6f 6465  dict = data.mode
-000022e0: 6c5f 6475 6d70 2829 0d0a 2020 2020 2020  l_dump()..      
-000022f0: 2020 636f 6e74 656e 7420 3d20 6461 7461    content = data
-00002300: 5f64 6963 745b 2263 6f6e 7465 6e74 225d  _dict["content"]
-00002310: 0d0a 2020 2020 2020 2020 6c6c 6d5f 6f75  ..        llm_ou
-00002320: 7470 7574 203d 207b 0d0a 2020 2020 2020  tput = {..      
-00002330: 2020 2020 2020 6b3a 2076 2066 6f72 206b        k: v for k
-00002340: 2c20 7620 696e 2064 6174 615f 6469 6374  , v in data_dict
-00002350: 2e69 7465 6d73 2829 2069 6620 6b20 6e6f  .items() if k no
-00002360: 7420 696e 2028 2263 6f6e 7465 6e74 222c  t in ("content",
-00002370: 2022 726f 6c65 222c 2022 7479 7065 2229   "role", "type")
-00002380: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-00002390: 2020 2020 2069 6620 6c65 6e28 636f 6e74       if len(cont
-000023a0: 656e 7429 203d 3d20 3120 616e 6420 636f  ent) == 1 and co
-000023b0: 6e74 656e 745b 305d 5b22 7479 7065 225d  ntent[0]["type"]
-000023c0: 203d 3d20 2274 6578 7422 3a0d 0a20 2020   == "text":..   
-000023d0: 2020 2020 2020 2020 206d 7367 203d 2041           msg = A
-000023e0: 494d 6573 7361 6765 2863 6f6e 7465 6e74  IMessage(content
-000023f0: 3d63 6f6e 7465 6e74 5b30 5d5b 2274 6578  =content[0]["tex
-00002400: 7422 5d29 0d0a 2020 2020 2020 2020 656c  t"])..        el
-00002410: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00002420: 206d 7367 203d 2041 494d 6573 7361 6765   msg = AIMessage
-00002430: 2863 6f6e 7465 6e74 3d63 6f6e 7465 6e74  (content=content
-00002440: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00002450: 2822 6d73 673a 2022 2c6d 7367 290d 0a20  ("msg: ",msg).. 
-00002460: 2020 2020 2020 2072 6574 7572 6e20 4368         return Ch
-00002470: 6174 5265 7375 6c74 280d 0a20 2020 2020  atResult(..     
-00002480: 2020 2020 2020 2067 656e 6572 6174 696f         generatio
-00002490: 6e73 3d5b 4368 6174 4765 6e65 7261 7469  ns=[ChatGenerati
-000024a0: 6f6e 286d 6573 7361 6765 3d6d 7367 295d  on(message=msg)]
-000024b0: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
-000024c0: 6c6d 5f6f 7574 7075 743d 6c6c 6d5f 6f75  lm_output=llm_ou
-000024d0: 7470 7574 2c0d 0a20 2020 2020 2020 2029  tput,..        )
-000024e0: 0d0a 0d0a 2020 2020 6465 6620 5f67 656e  ....    def _gen
-000024f0: 6572 6174 6528 0d0a 2020 2020 2020 2020  erate(..        
-00002500: 7365 6c66 2c0d 0a20 2020 2020 2020 206d  self,..        m
-00002510: 6573 7361 6765 733a 204c 6973 745b 4261  essages: List[Ba
-00002520: 7365 4d65 7373 6167 655d 2c0d 0a20 2020  seMessage],..   
-00002530: 2020 2020 2073 746f 703a 204f 7074 696f       stop: Optio
-00002540: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 203d  nal[List[str]] =
-00002550: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00002560: 7275 6e5f 6d61 6e61 6765 723a 204f 7074  run_manager: Opt
-00002570: 696f 6e61 6c5b 4361 6c6c 6261 636b 4d61  ional[CallbackMa
-00002580: 6e61 6765 7246 6f72 4c4c 4d52 756e 5d20  nagerForLLMRun] 
-00002590: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-000025a0: 202a 2a6b 7761 7267 733a 2041 6e79 2c0d   **kwargs: Any,.
-000025b0: 0a20 2020 2029 202d 3e20 4368 6174 5265  .    ) -> ChatRe
-000025c0: 7375 6c74 3a0d 0a20 2020 2020 2020 2070  sult:..        p
-000025d0: 6172 616d 7320 3d20 7365 6c66 2e5f 666f  arams = self._fo
-000025e0: 726d 6174 5f70 6172 616d 7328 6d65 7373  rmat_params(mess
-000025f0: 6167 6573 3d6d 6573 7361 6765 732c 2073  ages=messages, s
-00002600: 746f 703d 7374 6f70 2c20 2a2a 6b77 6172  top=stop, **kwar
-00002610: 6773 290d 0a20 2020 2020 2020 2069 6620  gs)..        if 
-00002620: 7365 6c66 2e73 7472 6561 6d69 6e67 3a0d  self.streaming:.
-00002630: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00002640: 6561 6d5f 6974 6572 203d 2073 656c 662e  eam_iter = self.
-00002650: 5f73 7472 6561 6d28 0d0a 2020 2020 2020  _stream(..      
-00002660: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00002670: 7373 6167 6573 2c20 7374 6f70 3d73 746f  ssages, stop=sto
-00002680: 702c 2072 756e 5f6d 616e 6167 6572 3d72  p, run_manager=r
-00002690: 756e 5f6d 616e 6167 6572 2c20 2a2a 6b77  un_manager, **kw
-000026a0: 6172 6773 0d0a 2020 2020 2020 2020 2020  args..          
-000026b0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-000026c0: 2020 2020 2072 6574 7572 6e20 6765 6e65       return gene
-000026d0: 7261 7465 5f66 726f 6d5f 7374 7265 616d  rate_from_stream
-000026e0: 2873 7472 6561 6d5f 6974 6572 290d 0a20  (stream_iter).. 
-000026f0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00002700: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00002710: 2073 656c 662e 5f63 6c69 656e 742e 6372   self._client.cr
-00002720: 6561 7465 282a 2a70 6172 616d 7329 0d0a  eate(**params)..
-00002730: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002740: 656c 662e 5f66 6f72 6d61 745f 6f75 7470  elf._format_outp
-00002750: 7574 2864 6174 612c 202a 2a6b 7761 7267  ut(data, **kwarg
-00002760: 7329 0d0a 2020 2020 0d0a 2020 2020 6173  s)..    ..    as
-00002770: 796e 6320 6465 6620 5f61 6765 6e65 7261  ync def _agenera
-00002780: 7465 280d 0a20 2020 2020 2020 2073 656c  te(..        sel
-00002790: 662c 0d0a 2020 2020 2020 2020 6d65 7373  f,..        mess
-000027a0: 6167 6573 3a20 4c69 7374 5b42 6173 654d  ages: List[BaseM
-000027b0: 6573 7361 6765 5d2c 0d0a 2020 2020 2020  essage],..      
-000027c0: 2020 7374 6f70 3a20 4f70 7469 6f6e 616c    stop: Optional
-000027d0: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
-000027e0: 6e65 2c0d 0a20 2020 2020 2020 2072 756e  ne,..        run
-000027f0: 5f6d 616e 6167 6572 3a20 4f70 7469 6f6e  _manager: Option
-00002800: 616c 5b41 7379 6e63 4361 6c6c 6261 636b  al[AsyncCallback
-00002810: 4d61 6e61 6765 7246 6f72 4c4c 4d52 756e  ManagerForLLMRun
-00002820: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-00002830: 2020 202a 2a6b 7761 7267 733a 2041 6e79     **kwargs: Any
-00002840: 2c0d 0a20 2020 2029 202d 3e20 4368 6174  ,..    ) -> Chat
-00002850: 5265 7375 6c74 3a0d 0a20 2020 2020 2020  Result:..       
-00002860: 2070 6172 616d 7320 3d20 7365 6c66 2e5f   params = self._
-00002870: 666f 726d 6174 5f70 6172 616d 7328 6d65  format_params(me
-00002880: 7373 6167 6573 3d6d 6573 7361 6765 732c  ssages=messages,
-00002890: 2073 746f 703d 7374 6f70 2c20 2a2a 6b77   stop=stop, **kw
-000028a0: 6172 6773 290d 0a20 2020 2020 2020 2069  args)..        i
-000028b0: 6620 7365 6c66 2e73 7472 6561 6d69 6e67  f self.streaming
-000028c0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000028d0: 7472 6561 6d5f 6974 6572 203d 2073 656c  tream_iter = sel
-000028e0: 662e 5f61 7374 7265 616d 280d 0a20 2020  f._astream(..   
-000028f0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00002900: 7361 6765 732c 2073 746f 703d 7374 6f70  sages, stop=stop
-00002910: 2c20 7275 6e5f 6d61 6e61 6765 723d 7275  , run_manager=ru
-00002920: 6e5f 6d61 6e61 6765 722c 202a 2a6b 7761  n_manager, **kwa
-00002930: 7267 730d 0a20 2020 2020 2020 2020 2020  rgs..           
-00002940: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00002950: 7265 7475 726e 2061 7761 6974 2061 6765  return await age
-00002960: 6e65 7261 7465 5f66 726f 6d5f 7374 7265  nerate_from_stre
-00002970: 616d 2873 7472 6561 6d5f 6974 6572 290d  am(stream_iter).
-00002980: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00002990: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000029a0: 203d 2061 7761 6974 2073 656c 662e 5f61   = await self._a
-000029b0: 7379 6e63 5f63 6c69 656e 742e 6372 6561  sync_client.crea
-000029c0: 7465 282a 2a70 6172 616d 7329 0d0a 2020  te(**params)..  
-000029d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000029e0: 662e 5f66 6f72 6d61 745f 6f75 7470 7574  f._format_output
-000029f0: 2864 6174 612c 202a 2a6b 7761 7267 7329  (data, **kwargs)
-00002a00: 0d0a 0d0a 200d 0a0d 0a                   .... ....
+00002130: 0a20 2020 2020 2020 2066 6f72 2073 7472  .        for str
+00002140: 6561 6d20 696e 2073 656c 662e 5f63 6c69  eam in self._cli
+00002150: 656e 742e 7374 7265 616d 282a 2a70 6172  ent.stream(**par
+00002160: 616d 7329 3a0d 0a20 2020 2020 2020 2020  ams):..         
+00002170: 2020 2077 6974 6820 7374 7265 616d 2061     with stream a
+00002180: 7320 7374 726d 3a0d 0a20 2020 2020 2020  s strm:..       
+00002190: 2020 2020 2020 2020 2066 6f72 2074 6578           for tex
+000021a0: 7420 696e 2073 7472 6d2e 7465 7874 5f73  t in strm.text_s
+000021b0: 7472 6561 6d3a 0d0a 2020 2020 2020 2020  tream:..        
+000021c0: 2020 2020 2020 2020 2020 2020 6368 756e              chun
+000021d0: 6b20 3d20 4368 6174 4765 6e65 7261 7469  k = ChatGenerati
+000021e0: 6f6e 4368 756e 6b28 6d65 7373 6167 653d  onChunk(message=
+000021f0: 4149 4d65 7373 6167 6543 6875 6e6b 2863  AIMessageChunk(c
+00002200: 6f6e 7465 6e74 3d74 6578 7429 290d 0a20  ontent=text)).. 
+00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002220: 2020 2069 6620 7275 6e5f 6d61 6e61 6765     if run_manage
+00002230: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00002240: 2020 2020 2020 2020 2020 2020 7275 6e5f              run_
+00002250: 6d61 6e61 6765 722e 6f6e 5f6c 6c6d 5f6e  manager.on_llm_n
+00002260: 6577 5f74 6f6b 656e 2874 6578 742c 2063  ew_token(text, c
+00002270: 6875 6e6b 3d63 6875 6e6b 290d 0a20 2020  hunk=chunk)..   
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2079 6965 6c64 2063 6875 6e6b 0d0a 0d0a   yield chunk....
+000022a0: 2020 0d0a 0d0a 2020 2020 6465 6620 5f66    ....    def _f
+000022b0: 6f72 6d61 745f 6f75 7470 7574 2873 656c  ormat_output(sel
+000022c0: 662c 2064 6174 613a 2041 6e79 2c20 2a2a  f, data: Any, **
+000022d0: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
+000022e0: 4368 6174 5265 7375 6c74 3a0d 0a20 2020  ChatResult:..   
+000022f0: 2020 2020 2064 6174 615f 6469 6374 203d       data_dict =
+00002300: 2064 6174 612e 6d6f 6465 6c5f 6475 6d70   data.model_dump
+00002310: 2829 0d0a 2020 2020 2020 2020 636f 6e74  ()..        cont
+00002320: 656e 7420 3d20 6461 7461 5f64 6963 745b  ent = data_dict[
+00002330: 2263 6f6e 7465 6e74 225d 0d0a 2020 2020  "content"]..    
+00002340: 2020 2020 6c6c 6d5f 6f75 7470 7574 203d      llm_output =
+00002350: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00002360: 6b3a 2076 2066 6f72 206b 2c20 7620 696e  k: v for k, v in
+00002370: 2064 6174 615f 6469 6374 2e69 7465 6d73   data_dict.items
+00002380: 2829 2069 6620 6b20 6e6f 7420 696e 2028  () if k not in (
+00002390: 2263 6f6e 7465 6e74 222c 2022 726f 6c65  "content", "role
+000023a0: 222c 2022 7479 7065 2229 0d0a 2020 2020  ", "type")..    
+000023b0: 2020 2020 7d0d 0a20 2020 2020 2020 2069      }..        i
+000023c0: 6620 6c65 6e28 636f 6e74 656e 7429 203d  f len(content) =
+000023d0: 3d20 3120 616e 6420 636f 6e74 656e 745b  = 1 and content[
+000023e0: 305d 5b22 7479 7065 225d 203d 3d20 2274  0]["type"] == "t
+000023f0: 6578 7422 3a0d 0a20 2020 2020 2020 2020  ext":..         
+00002400: 2020 206d 7367 203d 2041 494d 6573 7361     msg = AIMessa
+00002410: 6765 2863 6f6e 7465 6e74 3d63 6f6e 7465  ge(content=conte
+00002420: 6e74 5b30 5d5b 2274 6578 7422 5d29 0d0a  nt[0]["text"])..
+00002430: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00002440: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
+00002450: 2041 494d 6573 7361 6765 2863 6f6e 7465   AIMessage(conte
+00002460: 6e74 3d63 6f6e 7465 6e74 290d 0a20 2020  nt=content)..   
+00002470: 2020 2020 2072 6574 7572 6e20 4368 6174       return Chat
+00002480: 5265 7375 6c74 280d 0a20 2020 2020 2020  Result(..       
+00002490: 2020 2020 2067 656e 6572 6174 696f 6e73       generations
+000024a0: 3d5b 4368 6174 4765 6e65 7261 7469 6f6e  =[ChatGeneration
+000024b0: 286d 6573 7361 6765 3d6d 7367 295d 2c0d  (message=msg)],.
+000024c0: 0a20 2020 2020 2020 2020 2020 206c 6c6d  .            llm
+000024d0: 5f6f 7574 7075 743d 6c6c 6d5f 6f75 7470  _output=llm_outp
+000024e0: 7574 2c0d 0a20 2020 2020 2020 2029 0d0a  ut,..        )..
+000024f0: 0d0a 2020 2020 6465 6620 5f67 656e 6572  ..    def _gener
+00002500: 6174 6528 0d0a 2020 2020 2020 2020 7365  ate(..        se
+00002510: 6c66 2c0d 0a20 2020 2020 2020 206d 6573  lf,..        mes
+00002520: 7361 6765 733a 204c 6973 745b 4261 7365  sages: List[Base
+00002530: 4d65 7373 6167 655d 2c0d 0a20 2020 2020  Message],..     
+00002540: 2020 2073 746f 703a 204f 7074 696f 6e61     stop: Optiona
+00002550: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
+00002560: 6f6e 652c 0d0a 2020 2020 2020 2020 7275  one,..        ru
+00002570: 6e5f 6d61 6e61 6765 723a 204f 7074 696f  n_manager: Optio
+00002580: 6e61 6c5b 4361 6c6c 6261 636b 4d61 6e61  nal[CallbackMana
+00002590: 6765 7246 6f72 4c4c 4d52 756e 5d20 3d20  gerForLLMRun] = 
+000025a0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 202a  None,..        *
+000025b0: 2a6b 7761 7267 733a 2041 6e79 2c0d 0a20  *kwargs: Any,.. 
+000025c0: 2020 2029 202d 3e20 4368 6174 5265 7375     ) -> ChatResu
+000025d0: 6c74 3a0d 0a20 2020 2020 2020 2070 6172  lt:..        par
+000025e0: 616d 7320 3d20 7365 6c66 2e5f 666f 726d  ams = self._form
+000025f0: 6174 5f70 6172 616d 7328 6d65 7373 6167  at_params(messag
+00002600: 6573 3d6d 6573 7361 6765 732c 2073 746f  es=messages, sto
+00002610: 703d 7374 6f70 2c20 2a2a 6b77 6172 6773  p=stop, **kwargs
+00002620: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00002630: 6c66 2e73 7472 6561 6d69 6e67 3a0d 0a20  lf.streaming:.. 
+00002640: 2020 2020 2020 2020 2020 2073 7472 6561             strea
+00002650: 6d5f 6974 6572 203d 2073 656c 662e 5f73  m_iter = self._s
+00002660: 7472 6561 6d28 0d0a 2020 2020 2020 2020  tream(..        
+00002670: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
+00002680: 6167 6573 2c20 7374 6f70 3d73 746f 702c  ages, stop=stop,
+00002690: 2072 756e 5f6d 616e 6167 6572 3d72 756e   run_manager=run
+000026a0: 5f6d 616e 6167 6572 2c20 2a2a 6b77 6172  _manager, **kwar
+000026b0: 6773 0d0a 2020 2020 2020 2020 2020 2020  gs..            
+000026c0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+000026d0: 2020 2072 6574 7572 6e20 6765 6e65 7261     return genera
+000026e0: 7465 5f66 726f 6d5f 7374 7265 616d 2873  te_from_stream(s
+000026f0: 7472 6561 6d5f 6974 6572 290d 0a20 2020  tream_iter)..   
+00002700: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00002710: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
+00002720: 656c 662e 5f63 6c69 656e 742e 6372 6561  elf._client.crea
+00002730: 7465 282a 2a70 6172 616d 7329 0d0a 2020  te(**params)..  
+00002740: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002750: 662e 5f66 6f72 6d61 745f 6f75 7470 7574  f._format_output
+00002760: 2864 6174 612c 202a 2a6b 7761 7267 7329  (data, **kwargs)
+00002770: 0d0a 2020 2020 0d0a 2020 2020 6173 796e  ..    ..    asyn
+00002780: 6320 6465 6620 5f61 6765 6e65 7261 7465  c def _agenerate
+00002790: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
+000027a0: 0d0a 2020 2020 2020 2020 6d65 7373 6167  ..        messag
+000027b0: 6573 3a20 4c69 7374 5b42 6173 654d 6573  es: List[BaseMes
+000027c0: 7361 6765 5d2c 0d0a 2020 2020 2020 2020  sage],..        
+000027d0: 7374 6f70 3a20 4f70 7469 6f6e 616c 5b4c  stop: Optional[L
+000027e0: 6973 745b 7374 725d 5d20 3d20 4e6f 6e65  ist[str]] = None
+000027f0: 2c0d 0a20 2020 2020 2020 2072 756e 5f6d  ,..        run_m
+00002800: 616e 6167 6572 3a20 4f70 7469 6f6e 616c  anager: Optional
+00002810: 5b41 7379 6e63 4361 6c6c 6261 636b 4d61  [AsyncCallbackMa
+00002820: 6e61 6765 7246 6f72 4c4c 4d52 756e 5d20  nagerForLLMRun] 
+00002830: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00002840: 202a 2a6b 7761 7267 733a 2041 6e79 2c0d   **kwargs: Any,.
+00002850: 0a20 2020 2029 202d 3e20 4368 6174 5265  .    ) -> ChatRe
+00002860: 7375 6c74 3a0d 0a20 2020 2020 2020 2070  sult:..        p
+00002870: 6172 616d 7320 3d20 7365 6c66 2e5f 666f  arams = self._fo
+00002880: 726d 6174 5f70 6172 616d 7328 6d65 7373  rmat_params(mess
+00002890: 6167 6573 3d6d 6573 7361 6765 732c 2073  ages=messages, s
+000028a0: 746f 703d 7374 6f70 2c20 2a2a 6b77 6172  top=stop, **kwar
+000028b0: 6773 290d 0a20 2020 2020 2020 2069 6620  gs)..        if 
+000028c0: 7365 6c66 2e73 7472 6561 6d69 6e67 3a0d  self.streaming:.
+000028d0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+000028e0: 6561 6d5f 6974 6572 203d 2073 656c 662e  eam_iter = self.
+000028f0: 5f61 7374 7265 616d 280d 0a20 2020 2020  _astream(..     
+00002900: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00002910: 6765 732c 2073 746f 703d 7374 6f70 2c20  ges, stop=stop, 
+00002920: 7275 6e5f 6d61 6e61 6765 723d 7275 6e5f  run_manager=run_
+00002930: 6d61 6e61 6765 722c 202a 2a6b 7761 7267  manager, **kwarg
+00002940: 730d 0a20 2020 2020 2020 2020 2020 2029  s..            )
+00002950: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00002960: 7475 726e 2061 7761 6974 2061 6765 6e65  turn await agene
+00002970: 7261 7465 5f66 726f 6d5f 7374 7265 616d  rate_from_stream
+00002980: 2873 7472 6561 6d5f 6974 6572 290d 0a20  (stream_iter).. 
+00002990: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000029a0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+000029b0: 2061 7761 6974 2073 656c 662e 5f61 7379   await self._asy
+000029c0: 6e63 5f63 6c69 656e 742e 6372 6561 7465  nc_client.create
+000029d0: 282a 2a70 6172 616d 7329 0d0a 2020 2020  (**params)..    
+000029e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000029f0: 5f66 6f72 6d61 745f 6f75 7470 7574 2864  _format_output(d
+00002a00: 6174 612c 202a 2a6b 7761 7267 7329 0d0a  ata, **kwargs)..
+00002a10: 0d0a 200d 0a0d 0a                        .. ....
```

### Comparing `prodpadlm_client-0.1.1.3.1/prodpadlm_client/client_types/messages.py` & `prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/messages.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.3.1/setup.py` & `prodpadlm_client-0.1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,21 @@
     """Read the README file."""
     return (Path(__file__).parent / "README.md").read_text(encoding="UTF-8")
 
 requirements = [
     "pydantic-settings",
     "langchain==0.1.14",
     "langchain-core==0.1.40",
+    "httpcore==1.0.5",
+    "httpx==0.27.0"
 ]
 
 setup(
     name='prodpadlm_client',
-    version='0.1.1.3.1',
+    version='0.1.1.4',
     description='Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡',
     author='Ayo Kehinde Samuel',
     packages=find_packages(),
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     license_files="LICENSE.txt",
```


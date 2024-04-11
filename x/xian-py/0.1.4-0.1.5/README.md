# Comparing `tmp/xian_py-0.1.4.tar.gz` & `tmp/xian_py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xian_py-0.1.4.tar", max compression
+gzip compressed data, was "xian_py-0.1.5.tar", max compression
```

## Comparing `xian_py-0.1.4.tar` & `xian_py-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4472 2024-02-21 22:59:58.766214 xian_py-0.1.4/README.md
--rw-r--r--   0        0        0      344 2024-04-08 22:25:42.732388 xian_py-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4755 2024-02-21 22:59:58.766680 xian_py-0.1.4/xian_py/encoding.py
--rw-r--r--   0        0        0     2320 2024-02-21 22:59:58.766767 xian_py-0.1.4/xian_py/formating.py
--rw-r--r--   0        0        0     3683 2024-04-08 21:58:17.489646 xian_py-0.1.4/xian_py/transactions.py
--rw-r--r--   0        0        0      387 2024-04-08 21:58:01.758197 xian_py-0.1.4/xian_py/utils.py
--rw-r--r--   0        0        0     1906 2024-02-21 22:59:58.767011 xian_py-0.1.4/xian_py/wallet.py
--rw-r--r--   0        0        0     6593 2024-04-08 22:25:24.966190 xian_py-0.1.4/xian_py/xian.py
--rw-r--r--   0        0        0     7299 2024-02-21 22:59:58.767235 xian_py-0.1.4/xian_py/xian_datetime.py
--rw-r--r--   0        0        0     4683 2024-02-21 22:59:58.767344 xian_py-0.1.4/xian_py/xian_decimal.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 xian_py-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4472 2024-02-21 22:59:58.766214 xian_py-0.1.5/README.md
+-rw-r--r--   0        0        0      344 2024-04-11 23:27:32.259119 xian_py-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4755 2024-02-21 22:59:58.766680 xian_py-0.1.5/xian_py/encoding.py
+-rw-r--r--   0        0        0      198 2024-04-10 23:20:44.689826 xian_py-0.1.5/xian_py/exception.py
+-rw-r--r--   0        0        0     2320 2024-02-21 22:59:58.766767 xian_py-0.1.5/xian_py/formating.py
+-rw-r--r--   0        0        0     4115 2024-04-11 22:45:16.756569 xian_py-0.1.5/xian_py/transactions.py
+-rw-r--r--   0        0        0      387 2024-04-08 21:58:01.758197 xian_py-0.1.5/xian_py/utils.py
+-rw-r--r--   0        0        0     1906 2024-02-21 22:59:58.767011 xian_py-0.1.5/xian_py/wallet.py
+-rw-r--r--   0        0        0     6774 2024-04-11 23:21:17.001237 xian_py-0.1.5/xian_py/xian.py
+-rw-r--r--   0        0        0     7299 2024-02-21 22:59:58.767235 xian_py-0.1.5/xian_py/xian_datetime.py
+-rw-r--r--   0        0        0     4683 2024-02-21 22:59:58.767344 xian_py-0.1.5/xian_py/xian_decimal.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 xian_py-0.1.5/PKG-INFO
```

### Comparing `xian_py-0.1.4/README.md` & `xian_py-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.4/xian_py/encoding.py` & `xian_py-0.1.5/xian_py/encoding.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.4/xian_py/formating.py` & `xian_py-0.1.5/xian_py/formating.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.4/xian_py/transactions.py` & `xian_py-0.1.5/xian_py/transactions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import requests
 import json
 
 from xian_py.wallet import Wallet
 from xian_py.utils import decode_dict, decode_str
 from xian_py.formating import format_dictionary, check_format_of_payload
+from xian_py.exception import XianException
 from xian_py.encoding import encode
+
 from typing import Dict, Any
 
 
 def get_nonce(node_url: str, address: str) -> int:
     """
     Return next nonce for given address
     :param node_url: Node URL in format 'http://<IP>:<Port>'
     :param address: Wallet address for which the nonce will be returned
     :return: Next unused nonce
     """
-    r = requests.post(f'{node_url}/abci_query?path="/get_next_nonce/{address}"')
+    try:
+        r = requests.post(f'{node_url}/abci_query?path="/get_next_nonce/{address}"')
+        r.raise_for_status()
+    except Exception as e:
+        raise XianException(e)
+
     data = r.json()['result']['response']['value']
 
     # Data is None
     if data == 'AA==':
         return 0
 
     nonce = decode_str(data)
@@ -30,15 +37,19 @@
     """
     Return transaction either with encoded or decoded content
     :param node_url: Node URL in format 'http://<IP>:<Port>'
     :param tx_hash: Hash of transaction that gets retrieved
     :param decode: If TRUE, returned JSON data will be decoded
     :return: Transaction data in JSON
     """
-    r = requests.get(f'{node_url}/tx?hash=0x{tx_hash}')
+    try:
+        r = requests.get(f'{node_url}/tx?hash=0x{tx_hash}')
+    except Exception as e:
+        raise XianException(e)
+
     data = r.json()
 
     if decode and 'result' in data:
         decoded = decode_dict(data['result']['tx'])
         data['result']['tx'] = decoded
 
         if data['result']['tx_result']['data'] is not None:
@@ -89,34 +100,39 @@
         }
     }
 
     tx = encode(format_dictionary(tx))
     return json.loads(tx)
 
 
-def broadcast_tx(
-        node_url: str,
-        tx: Dict[str, Any],
-        decode: bool = True) -> Dict[str, Any]:
+def broadcast_tx_sync(node_url: str, tx: Dict[str, Any]) -> Dict[str, Any]:
     """
-    Broadcast transaction to the network
+    Submits a transaction to be included in the blockchain and returns
+    the response from CheckTx. Does not wait for DeliverTx result.
     :param node_url: Node URL in format 'http://<IP>:<Port>'
     :param tx: Transaction data in JSON format (dict)
-    :param decode: If TRUE, returned JSON data will be decoded
     :return: Broadcast data in JSON
     """
     payload = json.dumps(tx).encode().hex()
-    r = requests.post(f'{node_url}/broadcast_tx_commit?tx="{payload}"')
 
-    # TODO: If statuscode != 200, set error as JSON data or raise exception?
+    try:
+        r = requests.post(f'{node_url}/broadcast_tx_sync?tx="{payload}"')
+    except Exception as e:
+        raise XianException(e)
 
     data = r.json()
+    return data
 
-    # For example if tx already exists in cache
-    if 'error' in data:
-        return data
-
-    if decode and data['result']['tx_result']['data']:
-        decoded = decode_str(data['result']['tx_result']['data'])
-        data['result']['tx_result']['data'] = json.loads(decoded)
 
-    return data
+def broadcast_tx_async(node_url: str, tx: Dict[str, Any]):
+    """
+    Submits a transaction to be included in the blockchain and returns
+    immediately. Does not wait for CheckTx or DeliverTx results.
+    :param node_url: Node URL in format 'http://<IP>:<Port>'
+    :param tx: Transaction data in JSON format (dict)
+    """
+    payload = json.dumps(tx).encode().hex()
+
+    try:
+        requests.post(f'{node_url}/broadcast_tx_async?tx="{payload}"')
+    except Exception as e:
+        raise XianException(e)
```

### Comparing `xian_py-0.1.4/xian_py/wallet.py` & `xian_py-0.1.5/xian_py/wallet.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.4/xian_py/xian.py` & `xian_py-0.1.5/xian_py/xian.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,81 @@
 import ast
 import requests
+
 import xian_py.utils as utl
 import xian_py.transactions as tr
 
+from xian_py.exception import XianException
 from xian_py.wallet import Wallet
-from typing import Dict, Any
+
+from typing import Dict, Any, Optional
 
 
 class Xian:
     def __init__(self, node_url: str, chain_id: str, wallet: Wallet = None):
         self.wallet = wallet if wallet else Wallet()
         self.chain_id = chain_id
         self.node_url = node_url
 
     def get_tx(self, tx_hash: str) -> Dict[str, Any]:
         """ Return transaction data """
-        return tr.get_tx(self.node_url, tx_hash)
+
+        data = tr.get_tx(self.node_url, tx_hash)
+
+        if 'error' in data:
+            data['success'] = False
+            data['message'] = data['error']['data']
+        elif data['result']['tx_result']['code'] == 0:
+            data['success'] = True
+        else:
+            data['success'] = False
+            data['message'] = data['result']['tx_result']['data']['result']
+
+        return data
 
     def get_balance(
             self,
             address: str = None,
             contract: str = 'currency') -> int | float:
         """ Return balance for given address and token contract """
 
         address = address if address else self.wallet.public_key
 
-        with requests.get(f'{self.node_url}/abci_query?path="/get/{contract}.balances:{address}"') as r:
-            balance_byte_string = r.json()['result']['response']['value']
-
-            # Decodes to 'None'
-            if balance_byte_string == 'AA==':
-                return 0
+        try:
+            r = requests.get(f'{self.node_url}/abci_query?path="/get/{contract}.balances:{address}"')
+        except Exception as e:
+            raise XianException(e)
+            
+        balance_byte_string = r.json()['result']['response']['value']
+
+        # Decodes to 'None'
+        if balance_byte_string == 'AA==':
+            return 0
 
-            balance = utl.decode_str(balance_byte_string)
+        balance = utl.decode_str(balance_byte_string)
 
-            if balance.isdigit():
-                balance = int(balance)
+        if balance.isdigit():
+            balance = int(balance)
+        else:
+            if float(balance).is_integer():
+                balance = int(float(balance))
             else:
-                if float(balance).is_integer():
-                    balance = int(float(balance))
-                else:
-                    balance = float(balance)
+                balance = float(balance)
 
-            return balance
+        return balance
 
     def send_tx(
             self,
             contract: str,
             function: str,
             kwargs: dict,
             stamps: int | str = 500,
-            chain_id: str = None) -> Dict[str, Any]:
-        """
-        Send a transaction to the network
-        :returns:
-        - success - Boolean. True if successful
-        - data - String. Transaction hash
-        """
+            chain_id: str = None,
+            synchronous: bool = True) -> Optional[Dict[str, Any]]:
+        """ Send a transaction to the network """
 
         if chain_id is None:
             if self.chain_id:
                 chain_id = self.chain_id
 
         tx = tr.create_tx(
             contract=contract,
@@ -71,100 +86,98 @@
             private_key=self.wallet.private_key,
             nonce=tr.get_nonce(
                 self.node_url,
                 self.wallet.public_key
             )
         )
 
-        data = tr.broadcast_tx(self.node_url, tx)
+        if synchronous:
+            data = tr.broadcast_tx_sync(self.node_url, tx)
 
-        result = {
-            'success': None,
-            'tx_hash': None,
-            'result': None,
-            'data': data
-        }
+            result = {
+                'success': None,
+                'message': None,
+                'tx_hash': None,
+                'response': data
+            }
+
+            if 'error' in data:
+                result['success'] = False
+                result['message'] = data['error']['data']
+            elif data['result']['code'] == 0:
+                result['success'] = True
+                result['tx_hash'] = data['result']['hash']
+            else:
+                result['success'] = False
+                result['message'] = data['result']['log']
+                result['tx_hash'] = data['result']['hash']
 
-        if 'error' in data:
-            result['success'] = False
-            result['result'] = data['error']['data']
+            return result
 
-        elif data['result']['check_tx']['code'] == 1:
-            result['success'] = False
-            result['tx_hash'] = data['result']['hash']
-            result['result'] = 'Transaction check not successful'
-
-        elif data['result']['tx_result']['code'] == 1:
-            result['success'] = False
-            result['tx_hash'] = data['result']['hash']
-            result['result'] = 'Transaction delivery not successful'
-
-        elif data['result']['tx_result']['data']['status'] == 1:
-            result['success'] = False
-            result['tx_hash'] = data['result']['hash']
-            result['result'] = data['result']['tx_result']['data']['result']
         else:
-            result['success'] = True
-            result['tx_hash'] = data['result']['hash']
-            result['result'] = data['result']['tx_result']['data']['result']
-
-        return result
+            tr.broadcast_tx_async(self.node_url, tx)
 
     def send(
             self,
             amount: int | float | str,
             to_address: str,
             token: str = "currency",
             stamps: int | str = 100,
-            chain_id: str = None) -> Dict[str, Any]:
-        """
-        Send a token to a given address
-        :returns:
-        - success - Boolean. True if successful
-        - data - String. Transaction hash
-        """
-
-        kwargs = {"amount": float(amount), "to": to_address}
-        return self.send_tx(token, "transfer", kwargs, stamps, chain_id)
+            chain_id: str = None,
+            synchronous: bool = True) -> Optional[Dict[str, Any]]:
+        """ Send a token to a given address """
+
+        return self.send_tx(
+            token,
+            "transfer",
+            {"amount": float(amount), "to": to_address},
+            stamps,
+            chain_id,
+            synchronous
+        )
 
     def get_contract_data(
             self,
             contract: str,
             variable: str,
             *keys: str) -> None | int | float | dict | str:
         """ Retrieve contract data and decode it """
 
         path = f'/get/{contract}.{variable}'
         path = f'{path}:{":".join(keys)}' if keys else path
 
-        with requests.get(f'{self.node_url}/abci_query?path="{path}"') as r:
-            byte_string = r.json()['result']['response']['value']
-
-            # Decodes to 'None'
-            if byte_string == 'AA==':
-                return None
-
-            data = utl.decode_str(byte_string)
-
-            try:
-                return int(data)
-            except:
-                pass
-            try:
-                if float(data).is_integer():
-                    return int(float(data))
-                return float(data)
-            except:
-                pass
-            try:
-                return ast.literal_eval(data)
-            except:
-                pass
+        try:
+            r = requests.get(f'{self.node_url}/abci_query?path="{path}"')
+        except Exception as e:
+            raise XianException(e)
+
+        byte_string = r.json()['result']['response']['value']
+
+        # Decodes to 'None'
+        if byte_string == 'AA==':
+            return None
+
+        data = utl.decode_str(byte_string)
+
+        try:
+            return int(data)
+        except:
+            pass
+        try:
+            if float(data).is_integer():
+                return int(float(data))
+            return float(data)
+        except:
+            pass
+        try:
+            return ast.literal_eval(data)
+        except:
+            pass
 
-            return data
+        return data
 
     def get_approved_amount(
             self,
             contract: str,
             address: str = None,
             token: str = 'currency') -> int | float:
         """ Retrieve approved token amount for a contract """
@@ -177,40 +190,53 @@
         return value
 
     def approve(
             self,
             contract: str,
             token: str = "currency",
             amount: int | float | str = 900000000000,
-            chain_id: str = None) -> Dict[str, Any]:
+            chain_id: str = None,
+            synchronous: bool = True) -> Optional[Dict[str, Any]]:
         """ Approve smart contract to spend max token amount """
 
-        kwargs = {"amount": float(amount), "to": contract}
-        return self.send_tx(token, "approve", kwargs, 50, chain_id)
+        return self.send_tx(
+            token,
+            "approve",
+            {"amount": float(amount), "to": contract},
+            50,
+            chain_id,
+            synchronous
+        )
 
     def submit_contract(
             self,
             name: str,
             code: str,
             stamps: int | str = 1000,
-            chain_id: str = None) -> Dict[str, Any]:
-        """
-        Deploy a contract to the network
-        :returns:
-        - success - Boolean. True if successful
-        - data - String. Transaction hash
-        """
-
-        kwargs = {"name": name, "code": code}
-        return self.send_tx('submission', 'submit_contract', kwargs, stamps, chain_id)
+            chain_id: str = None,
+            synchronous: bool = True) -> Optional[Dict[str, Any]]:
+        """ Deploy a contract to the network """
+
+        return self.send_tx(
+            'submission',
+            'submit_contract',
+            {"name": name, "code": code},
+            stamps,
+            chain_id,
+            synchronous
+        )
 
     def get_nodes(self) -> list:
         """ Retrieve list of nodes from the network """
 
-        r = requests.post(f'{self.node_url}/net_info')
+        try:
+            r = requests.post(f'{self.node_url}/net_info')
+        except Exception as e:
+            raise XianException(e)
+
         peers = r.json()['result']['peers']
 
         ips = list()
 
         for peer in peers:
             ips.append(peer['remote_ip'])
```

### Comparing `xian_py-0.1.4/xian_py/xian_datetime.py` & `xian_py-0.1.5/xian_py/xian_datetime.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.4/xian_py/xian_decimal.py` & `xian_py-0.1.5/xian_py/xian_decimal.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.4/PKG-INFO` & `xian_py-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xian-py
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python tools to interact with the Xian blockchain
 License: MIT
 Author: endogen
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


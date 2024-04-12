# Comparing `tmp/MercadoBitcoinBalance-1.1.tar.gz` & `tmp/mercadobitcoinbalance-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MercadoBitcoinBalance-1.1.tar", last modified: Tue Nov 28 16:54:58 2023, max compression
+gzip compressed data, was "mercadobitcoinbalance-1.2.tar", last modified: Fri Apr 12 21:19:33 2024, max compression
```

## Comparing `MercadoBitcoinBalance-1.1.tar` & `mercadobitcoinbalance-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    35149 2023-11-28 12:45:31.000000 MercadoBitcoinBalance-1.1/LICENSE
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/MercadoBitcoinBalance.egg-info/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    44921 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/MercadoBitcoinBalance.egg-info/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)      336 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/MercadoBitcoinBalance.egg-info/SOURCES.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/MercadoBitcoinBalance.egg-info/dependency_links.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       66 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/MercadoBitcoinBalance.egg-info/entry_points.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)        7 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/MercadoBitcoinBalance.egg-info/requires.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       22 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/MercadoBitcoinBalance.egg-info/top_level.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)    44921 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)     3397 2023-11-28 16:53:43.000000 MercadoBitcoinBalance-1.1/README.md
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1126 2023-11-28 16:47:19.000000 MercadoBitcoinBalance-1.1/pyproject.toml
--rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/setup.cfg
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-11-28 16:54:58.000000 MercadoBitcoinBalance-1.1/src/
--rw-r--r--   0 aviram    (1000) aviram    (1000)     4597 2023-11-28 15:12:28.000000 MercadoBitcoinBalance-1.1/src/__init__.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    11481 2023-11-28 16:27:55.000000 MercadoBitcoinBalance-1.1/src/__main__.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-12 21:19:33.000000 mercadobitcoinbalance-1.2/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    35149 2023-11-28 19:52:03.000000 mercadobitcoinbalance-1.2/LICENSE
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-12 21:19:32.000000 mercadobitcoinbalance-1.2/MercadoBitcoinBalance.egg-info/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    44909 2024-04-12 21:19:30.000000 mercadobitcoinbalance-1.2/MercadoBitcoinBalance.egg-info/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      336 2024-04-12 21:19:31.000000 mercadobitcoinbalance-1.2/MercadoBitcoinBalance.egg-info/SOURCES.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2024-04-12 21:19:30.000000 mercadobitcoinbalance-1.2/MercadoBitcoinBalance.egg-info/dependency_links.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       66 2024-04-12 21:19:30.000000 mercadobitcoinbalance-1.2/MercadoBitcoinBalance.egg-info/entry_points.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)        7 2024-04-12 21:19:30.000000 mercadobitcoinbalance-1.2/MercadoBitcoinBalance.egg-info/requires.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       22 2024-04-12 21:19:30.000000 mercadobitcoinbalance-1.2/MercadoBitcoinBalance.egg-info/top_level.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    44909 2024-04-12 21:19:33.000000 mercadobitcoinbalance-1.2/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     3385 2023-12-17 05:45:36.000000 mercadobitcoinbalance-1.2/README.md
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1126 2024-04-12 21:19:22.000000 mercadobitcoinbalance-1.2/pyproject.toml
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2024-04-12 21:19:33.000000 mercadobitcoinbalance-1.2/setup.cfg
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-12 21:19:33.000000 mercadobitcoinbalance-1.2/src/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     4597 2023-11-28 19:52:03.000000 mercadobitcoinbalance-1.2/src/__init__.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    11481 2023-11-28 19:52:03.000000 mercadobitcoinbalance-1.2/src/__main__.py
```

### Comparing `MercadoBitcoinBalance-1.1/LICENSE` & `mercadobitcoinbalance-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MercadoBitcoinBalance-1.1/MercadoBitcoinBalance.egg-info/PKG-INFO` & `mercadobitcoinbalance-1.2/MercadoBitcoinBalance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MercadoBitcoinBalance
-Version: 1.1
+Version: 1.2
 Summary: Calcula, salva e reporta seu saldo do Mercado Bitcoin
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -702,19 +702,21 @@
 - Calcula saldo consolidado
 - Atualiza um CSV caso o saldo tenha mudado
 - Manda o saldo atual por e-mail ou Telegram junto com algumas estatísticas
 
 ## Como usá-lo
 
 Instale:
+
 ```shell
-pip install MercadoBitcoinBalance
+pip install MercadoBitcoinBalance --user
 ```
 
 Use:
+
 ```shell
 balancemb \
     --mb-id 06…05 \
     --mb-secret 10…19 \
     --csv-threshold 1 \
     --csv balances.txt \
     --csv-fund-name 'Nome arbitrário do fundo' \
@@ -747,31 +749,32 @@
 
 > Current balance: **36,576.22 BRL**.
 >
 > Previous balance: **34,595.72 BRL**.
 >
 > Variation: **1,980.50 BRL**.
 >
-> Percent change: **5.72%**.
+> Percent change: **5\.72%**.
 >
 > Historycal growth: **4%** in **0m2d**.
 >
 > Brakedown by tokens and coins:
-> | 	| Total (BRL) |
-> ------|--------------
-> | **brl**	 | 36,229.86 BRL |
-> | **abfy** | 336.42 BRL |
-> | **psgft** | 9.40 BRL |
-> | **wemix** | 0.54 BRL |
+>
+> |  | Total (BRL) |
+> |--|-------------|
+> | **brl** | 36,229.86 BRL |
+> | **abfy** | 336\.42 BRL |
+> | **psgft** | 9\.40 BRL |
+> | **wemix** | 0\.54 BRL |
 
 Eu rodo isso a cada meia hora via crontab, assim:
 
 ```crontab
-*/30 * * * * balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
-15 20 * * * cd $HOME/Notebooks/MercadoBitcoinBalance && ./balancemb.py --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
 ```
 
 Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando e-mail mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
 Além do mais, todo dia às 20:15 manda o saldo atual.
 
 É necessário Python 3, Pandas e nada mais para rodar este programa.
```

### Comparing `MercadoBitcoinBalance-1.1/PKG-INFO` & `mercadobitcoinbalance-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MercadoBitcoinBalance
-Version: 1.1
+Version: 1.2
 Summary: Calcula, salva e reporta seu saldo do Mercado Bitcoin
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -702,19 +702,21 @@
 - Calcula saldo consolidado
 - Atualiza um CSV caso o saldo tenha mudado
 - Manda o saldo atual por e-mail ou Telegram junto com algumas estatísticas
 
 ## Como usá-lo
 
 Instale:
+
 ```shell
-pip install MercadoBitcoinBalance
+pip install MercadoBitcoinBalance --user
 ```
 
 Use:
+
 ```shell
 balancemb \
     --mb-id 06…05 \
     --mb-secret 10…19 \
     --csv-threshold 1 \
     --csv balances.txt \
     --csv-fund-name 'Nome arbitrário do fundo' \
@@ -747,31 +749,32 @@
 
 > Current balance: **36,576.22 BRL**.
 >
 > Previous balance: **34,595.72 BRL**.
 >
 > Variation: **1,980.50 BRL**.
 >
-> Percent change: **5.72%**.
+> Percent change: **5\.72%**.
 >
 > Historycal growth: **4%** in **0m2d**.
 >
 > Brakedown by tokens and coins:
-> | 	| Total (BRL) |
-> ------|--------------
-> | **brl**	 | 36,229.86 BRL |
-> | **abfy** | 336.42 BRL |
-> | **psgft** | 9.40 BRL |
-> | **wemix** | 0.54 BRL |
+>
+> |  | Total (BRL) |
+> |--|-------------|
+> | **brl** | 36,229.86 BRL |
+> | **abfy** | 336\.42 BRL |
+> | **psgft** | 9\.40 BRL |
+> | **wemix** | 0\.54 BRL |
 
 Eu rodo isso a cada meia hora via crontab, assim:
 
 ```crontab
-*/30 * * * * balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
-15 20 * * * cd $HOME/Notebooks/MercadoBitcoinBalance && ./balancemb.py --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
 ```
 
 Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando e-mail mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
 Além do mais, todo dia às 20:15 manda o saldo atual.
 
 É necessário Python 3, Pandas e nada mais para rodar este programa.
```

### Comparing `MercadoBitcoinBalance-1.1/README.md` & `mercadobitcoinbalance-1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 - Calcula saldo consolidado
 - Atualiza um CSV caso o saldo tenha mudado
 - Manda o saldo atual por e-mail ou Telegram junto com algumas estatísticas
 
 ## Como usá-lo
 
 Instale:
+
 ```shell
-pip install MercadoBitcoinBalance
+pip install MercadoBitcoinBalance --user
 ```
 
 Use:
+
 ```shell
 balancemb \
     --mb-id 06…05 \
     --mb-secret 10…19 \
     --csv-threshold 1 \
     --csv balances.txt \
     --csv-fund-name 'Nome arbitrário do fundo' \
@@ -51,31 +53,32 @@
 
 > Current balance: **36,576.22 BRL**.
 >
 > Previous balance: **34,595.72 BRL**.
 >
 > Variation: **1,980.50 BRL**.
 >
-> Percent change: **5.72%**.
+> Percent change: **5\.72%**.
 >
 > Historycal growth: **4%** in **0m2d**.
 >
 > Brakedown by tokens and coins:
-> | 	| Total (BRL) |
-> ------|--------------
-> | **brl**	 | 36,229.86 BRL |
-> | **abfy** | 336.42 BRL |
-> | **psgft** | 9.40 BRL |
-> | **wemix** | 0.54 BRL |
+>
+> |  | Total (BRL) |
+> |--|-------------|
+> | **brl** | 36,229.86 BRL |
+> | **abfy** | 336\.42 BRL |
+> | **psgft** | 9\.40 BRL |
+> | **wemix** | 0\.54 BRL |
 
 Eu rodo isso a cada meia hora via crontab, assim:
 
 ```crontab
-*/30 * * * * balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
-15 20 * * * cd $HOME/Notebooks/MercadoBitcoinBalance && ./balancemb.py --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
 ```
 
 Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando e-mail mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
 Além do mais, todo dia às 20:15 manda o saldo atual.
 
 É necessário Python 3, Pandas e nada mais para rodar este programa.
```

### Comparing `MercadoBitcoinBalance-1.1/pyproject.toml` & `mercadobitcoinbalance-1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "MercadoBitcoinBalance"
-version = '1.1'
+version = '1.2'
 description = "Calcula, salva e reporta seu saldo do Mercado Bitcoin"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 authors = [
     { name = "Avi Alkalay", email = "avi@unix.sh" },
 ]
```

### Comparing `MercadoBitcoinBalance-1.1/src/__init__.py` & `mercadobitcoinbalance-1.2/src/__init__.py`

 * *Files identical despite different names*

### Comparing `MercadoBitcoinBalance-1.1/src/__main__.py` & `mercadobitcoinbalance-1.2/src/__main__.py`

 * *Files identical despite different names*


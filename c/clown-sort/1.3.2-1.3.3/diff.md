# Comparing `tmp/clown_sort-1.3.2.tar.gz` & `tmp/clown_sort-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.3.2.tar", max compression
+gzip compressed data, was "clown_sort-1.3.3.tar", max compression
```

## Comparing `clown_sort-1.3.2.tar` & `clown_sort-1.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1911 2023-04-16 21:20:52.124000 clown_sort-1.3.2/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.3.2/LICENSE
--rw-r--r--   0        0        0     7434 2023-04-14 22:57:58.586571 clown_sort-1.3.2/README.md
--rw-r--r--   0        0        0     3294 2023-04-16 21:18:44.118253 clown_sort-1.3.2/clown_sort/__init__.py
--rw-r--r--   0        0        0     6991 2023-04-14 22:38:02.184270 clown_sort-1.3.2/clown_sort/config.py
--rw-r--r--   0        0        0     7530 2023-04-16 21:19:30.844002 clown_sort-1.3.2/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4260 2023-04-16 21:12:34.135691 clown_sort-1.3.2/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     1317 2023-04-16 20:55:13.426378 clown_sort-1.3.2/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0     9805 2023-04-16 21:08:33.938145 clown_sort-1.3.2/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3109 2023-04-14 22:23:25.165083 clown_sort-1.3.2/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     6638 2023-04-16 06:02:13.380652 clown_sort-1.3.2/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3298 2023-04-14 23:18:26.928346 clown_sort-1.3.2/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1455 2023-02-27 03:16:08.096928 clown_sort-1.3.2/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.3.2/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-02-27 01:29:17.019569 clown_sort-1.3.2/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.3.2/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.3.2/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      345 2023-04-16 20:51:08.331725 clown_sort-1.3.2/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1558 2023-04-16 21:20:52.127337 clown_sort-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     8995 1970-01-01 00:00:00.000000 clown_sort-1.3.2/setup.py
--rw-r--r--   0        0        0     8798 1970-01-01 00:00:00.000000 clown_sort-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1999 2023-04-24 00:48:38.955951 clown_sort-1.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.3.3/LICENSE
+-rw-r--r--   0        0        0     7617 2023-04-16 21:33:01.097803 clown_sort-1.3.3/README.md
+-rw-r--r--   0        0        0     3294 2023-04-16 21:18:44.118253 clown_sort-1.3.3/clown_sort/__init__.py
+-rw-r--r--   0        0        0     6991 2023-04-14 22:38:02.184270 clown_sort-1.3.3/clown_sort/config.py
+-rw-r--r--   0        0        0     7530 2023-04-16 21:19:30.844002 clown_sort-1.3.3/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4260 2023-04-16 21:12:34.135691 clown_sort-1.3.3/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     1330 2023-04-24 00:42:15.932759 clown_sort-1.3.3/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0     9805 2023-04-16 21:08:33.938145 clown_sort-1.3.3/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3109 2023-04-14 22:23:25.165083 clown_sort-1.3.3/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     7489 2023-04-24 00:44:38.181699 clown_sort-1.3.3/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3298 2023-04-14 23:18:26.928346 clown_sort-1.3.3/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1455 2023-02-27 03:16:08.096928 clown_sort-1.3.3/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.3.3/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-02-27 01:29:17.019569 clown_sort-1.3.3/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.3.3/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.3.3/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      345 2023-04-16 20:51:08.331725 clown_sort-1.3.3/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1558 2023-04-24 00:48:38.962489 clown_sort-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9177 1970-01-01 00:00:00.000000 clown_sort-1.3.3/setup.py
+-rw-r--r--   0        0        0     8981 1970-01-01 00:00:00.000000 clown_sort-1.3.3/PKG-INFO
```

### Comparing `clown_sort-1.3.2/CHANGELOG.md` & `clown_sort-1.3.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # NEXT RELEASE
 
+### 1.3.3
+* Handle more unparseable PDF issues more gracefully
+* New crypto sort rules
+
 ### 1.3.2
 * Make `--rescan-sorted` respect `--all` flag
 * Don't append empty string to images that no text was extracted from
 * More crypto sort rules
 
 ### 1.3.1
 * Handle unparseable PDFs with a warning instead of a crash.
```

### Comparing `clown_sort-1.3.2/LICENSE` & `clown_sort-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/README.md` & `clown_sort-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,17 @@
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
 ```
 pipx install clown_sort
 ```
 
-Some (not many) PDFs require the `pycryptodome` package. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with:
+Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pycryptodome]`.
 
-```sh
-pipx install clown_sort[pycryptodome]
-```
+Updating to the latest version can be accomplished with `pipx upgrade clown_sort`.
 
 
 ### Configuring With `.clown_sort` File
 If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
 
 1. The current directory
 2. Your home directory
```

### Comparing `clown_sort-1.3.2/clown_sort/__init__.py` & `clown_sort-1.3.3/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/config.py` & `clown_sort-1.3.3/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/filename_extractor.py` & `clown_sort-1.3.3/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/files/image_file.py` & `clown_sort-1.3.3/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/files/pdf_file.py` & `clown_sort-1.3.3/clown_sort/files/pdf_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._extracted_text = None
 
         try:
             pdf_reader = PdfReader(self.file_path)
             self._extracted_text = '\\n\\n'.join([page.extract_text() for page in pdf_reader.pages])
         except DependencyError:
             log_optional_module_warning('pycryptodome')
-        except KeyError:
+        except (KeyError, TypeError):
             # TODO: failure on KeyError: '/Root' seems to have been fixed but not released yet
             # https://github.com/py-pdf/pypdf/pull/1784
             log.warn("Failed to parse PDF!")
 
         if self._extracted_text is not None:
             self._extracted_text = self._extracted_text.strip()
```

### Comparing `clown_sort-1.3.2/clown_sort/files/sortable_file.py` & `clown_sort-1.3.3/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/sort_selector.py` & `clown_sort-1.3.3/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.3.3/clown_sort/sorting_rules/crypto.csv`

 * *Files 11% similar despite different names*

```diff
@@ -5,113 +5,122 @@
 Aave,aave
 AAX,\baax
 Arbitrum,Arbitrum|[$#]ARB\b
 Amber Group,Amber[-_\s]*Group|\btiantian\b|\bkullander\b|\btony[-_\s]*he\b|\bbo[-_\s]*shen\b
 Aptos,\bAptos\b
 Art,occult
 Avalanche,\bAvax|AVAX\b|avalanche
-Banks,SEBA[^a-z]|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group|\$FRC
+Banks,SEBA[^a-z]|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group|\$FRC|Commercium[-_\s]*Financial
 Bankless,Bankless
 Biconomy,Biconomy|Omchain
 Binary Options,binary[-_\s]*options
 Binance,binance|biconomy|\bbnb|bsc|cz|bifinity|binaryx|billance|changpeng|joselito|paysafe|SwipeIO|Swipe\s*Wallet|keyway|\bkey[-_\s]*vision|TrustWallet|BUSD|\boztures|Kaiser[-_\s]*Ng|InvestByBit
 Bitdeer,Bitdeer
 BitGet,Bitget
 Bitmain,Bitmain
 Bitstamp,Bitstamp
-Bittrex,Bittrex|Ritchie[-_\s]*Lai
+Bittrex,Bittrex|Ritchie[-_\s]*Lai|Kiran[-_\s]*Raj|John[-_\s]*Roth
 Bitzlato,Bitzlato
-Blockchain8,Blockchain8|tom[-_\s]*emmer|ritchie[-_\s]*torres|repritchie|Warren[-_\s]*Davidson|Byron[-_\s]*Donalds|Ted[-_\s]*Budd|Josh[-_\s]*Gotheimer|Jake[-_\s]*Auchincloss|Darren[-_\s]*Soto|ro[-_\s]*khanna|KMSmithDC|Kristin[-_\s]*Smith\b
+Blockchain8,Blockchain8|tom[-_\s]*emmer|ritchie[-_\s]*torres|repritchie|Warren[-_\s]*Davidson|Byron[-_\s]*Donalds|Ted[-_\s]*Budd|Josh[-_\s]*Gotheimer|Jake[-_\s]*Auchincloss|Darren[-_\s]*Soto|ro[-_\s]*khanna|KMSmithDC|Kristin[-_\s]*Smith\b|Warren[-_\s]*Davidson
 Blockchain Capital,Blockchain[-_\s]*Capital|\bbrock\b|brockpierce
 BlockFi,BlockFi
+Blockstream,Blockstream
 Bored Ape Yacht Club,BAYC|Bored[-_\s]*Ape|yuga[-_\s]*labs
 Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi|Max[-_\s]*Keiser|Cowboy[-_\s]*Crypto|minimalcsgo
+Broettes,Nicole[-_\s]*Behnam
 Bybit,\bBybit\b|Ben[-_\s]*Zhou|InvestByBit
-Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson
+Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
 Cathie Wood,Cathie\s*Wood|\bARK(F|G|K|\s*Innovation|\s*Invest)
 Celsius,celsius|mashinsky|levity[-_\s]*and[-_\s]*love|celsian
 Circle,[@#]circle|usdc|circle[-_\s]*internet|disparte|\ballaire|jerallaire
-Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b
-Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk|OPNX|flexusd
+CMCC Global,CMCC[-_\s]*Global
+Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b|Asiff[-_\s]*Hirji|\bbalaji|Fred[-_\s]*Ehrsam
+Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk|OPNX|flexusd|Leslie[-_\s]*Lamb|dougpolkvids
 CompoundFi,compoundfi|leshner|\bgonen\b
 Cross River Bank,CRB|Cross[-_\s]*River|Prestige[-_\s]*Capital|bae[-_\s]*communications|Zenfi|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim
 Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s
-CUBI,\$CUBI|Customers[-_\s]*Ban(k|corp)
+CUBI,\bCUBI\b|Customers[-_\s]*Ban(k|corp)
 Custodia,custodia|caitlin[-_\s]*long
+dalle,craiyon
 DCG,DCG|digital\s*currency\s*group|sh?ill?bert|Grayscale|GBTC
 DWF,DWF|Andrey[-_\s]*Grachev|\bgrachev\b
+Effective Altruism,\bEA\b|effective[-_\s]*altruism
 El Salvador,El[-_\s]*Salvador|Bukele|Max[-_\s]*Keiser
-EOS,\bEOS\b|\bBlumer\b|Stan|@B1\b|Block[-_\.\s]One
+EOS,\bEOS\b|\bBlumer\b|\bLarimer\b|@B1\b|Block[-_\.\s]One
 Euler Finance,\beuler\b
 FalconX,falconx
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
 Friedlander Group,Friedlander|Agro[-_\s]*Bank|all\s*year\*m|\bbrock\b|brockpierce|litvishhocker
 FTX,FTX|FTT|SBF|Trabucco|Bankman|Ellison|Nishad|Alameda|Moonstone|friedberg|autism\s*capital
+Galaxy Digital,novogratz|Alex[-_\s]*Thorn
 Gelato Network,Gelato[-_\s]*Network|\bSorbet[-_\s]*Finance|@gitpusha|hilmar[-_\s]*x|\bmistx\b|@_alchemistcoin|@ChaosLabs_NFT|Arrakis[-_\s]*Finance|Dave[-_\s]*Leibowitz|Hilmar[-_\s]*Orth|joehquak
 Gemini,Gemini|winklev|@cameron
 Genesis,Genesis|Michael\s?Moro
 Goldfinch,goldfinch
 Hex,\bHex\b|[#$]Hex|Pulsechain|Richard\s*Heart|Hexican
-Hoo,Hoo[-_\s]*Exchange|#Hoo\s|Rexy\s*(Hoo|Wang)
-Huobi,huobi
+Hoo,Hoo[-_\s]*(Research|Exchange)|[#$]Hoo\b|Rexy\s*(Hoo|Wang)|\bhoo\b
+Huobi,huobi|jiao_newlife|jiaojiao|Leon[-_\s]*Li
 Jump Trading,Jump[-_\s]*Trading|@jump_
 Justin Sun,justin[-_\s]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina
 Kazakhstan,kazakhstan|Freedom[-_\s]*Holding|\balmaty|Timor[-_\s]*Turlov|\bFFIN[-_\s]*brokerage
-Kinesis,kinesis|kvt|ABX|KAG
+Kinesis,kinesis|\bKVT\b|\bABX\b|\bKAG\b
 Kraken,kraken|payward
 KuCoin,kucoin
 LBRY,LBRY|\bLBC\b
-Lexpunk Army,lexpunk|gabriel[-_\s]*shapiro
+Lexpunk Army,lexpunk|gabriel[-_\s]*shapiro|_gabrielShapir0|\blex_node\b
 Lifeboat Foundation,Lifeboat[-_\s]*Foundation
 North Korea,lazarus|North\s*Korea|pyongyang
 Paul LeRoux,leroux
+Polygon Labs,polygon[-_\s]*labs|ryan[-_\s]*watt\b|@Fwiz|Rebecca[-_\s]*Rettig|[#$]DOT\b
 MakerDAO,makerdao|[$#\s]DAI[^\w]
 Marathon,\$MARA|marathon
-Matthew Roszak,\broszak|matthewroszak
-Mario Nawfal,marionawfal
+Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s]*Cheng
+Mario Nawfal,mario[-_\s]*nawfal
 Messari,Ryan\s*Selkis|twobitidiot|messari|@robustus|Dan[-_\s]*McArdle
 Memes,\smeme
 Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s]*Stewart
-Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*Commercial
+Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*(Bank|Commercial)
 Founders Bank,Michael[-_\s]*Bianchi|Founders[-_\s]*Bank
 Miles Guo,\bguo\b|hcoin|himalaya[-_\s]*exchange|bannon|fjb|miles[-_\s]*kwok|brother[-_\s]*seven|kin[-_\s]*ming[-_\s]*je|william[-_\s]*je\b|\bHaoyun\b
 Miners,bitcoin[-_\s]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s]*Scientific|Iris[-_\s]*Energy|Blockstream
 Moonpay,moonpay
 MSTR,Saylor|MSTR
 Near Protocol,NEAR[-_\s]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s]*Rettig
 Nexo,Nexo
 NFTs,crypto[-_\s]*punk|pudgy[-_\s]*penguin
 OKX,oke?[cx]|star[-_\s]*xu
 Olympus DAO,\bOlympus\b|\bOHM\b
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea
-Paxful,paxful|Ray[-_\s]*Youssef|Artur[-_\s]*Schaback
+PAG,\bpag\b
+Paradigm,Fred[-_\s]*Ehrsam|paradigm\b
+Paxful,paxful|Ray[-_\s]*(Youssef|Savant)|Artur[-_\s]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
 Payrnet,payrnet|railsr|railsbank
 Pi,\$PI[^\w]|Pi[-_\s]*Network
 Prime Trust,Prime[-\s_]?Trust
 PVBC,PVBC|BankProv
 Quadriga,Quadriga|Gerald[-_\s]*Cotten
 Revolut,revolut[^\w]
 Ripple,XRP|garlinghouse|\bripple\b
-RIOT,\$RIOT|Riot[-\s_]*Block
+RIOT,[$#]RIOT\b|Riot[-\s_]*(Block|Platform)|Bioptix
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
 SEC,\bSEC(\b|Gov)|Gensler|Securities.{0,6}Exchange.{0,6}Commission
 Signature Bank,SBNY|Signature[-_\s]*Bank|Signet
 Silicon Valley Bank,si?vb|Silicon[-_\s]*Valley[-_\s]*Bank
 Silk Road,Silk[-_\s]*Road|\bulbricht|\bDPR\b
-Silvergate,\$SI|Silvergate|Alan\s*Lane|Eisele|[\s#]SEN[^\w]|Rebecca[-_\s]*Rettig
+Silvergate,\$SI|Silvergate|Alan\s*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s]*Rettig
 Solana,Solana|Serum
 Symbolic Capital,Symbolic[-_\s]*Capital|Lev[-_\s]Livnev
 TerraLuna,luna\b|do[-_\s]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s]*Foundation\b
-Tether,tether|usdt|paolo|friedberg|hoegner|Noble\s?Bank|Deltec[^\']|bitfinex[^e]|\bbrock\b|brockpierce|Capital[-_\s]*Union|Noblex|SJMBT
+Tether,tether|usdt|paolo|friedberg|hoegner|Noble\s?Bank|Deltec[^\']|b(e|i)tfinex[^e]|\bbrock\b|brockpierce|Capital[-_\s]*Union|Noblex|SJMBT|Global[-_\s]*Trad(ing|e)[-_\s]*Solutions|ifinex|BFXNA|BFXWW|[$#]Leo\b
 Tornado Cash,tornado\s*cash
 Transactive Systems UAB,Transactive
 Tron,\btron\b|tron(block|\s*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
 VCs,venture[-_\s]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s]*sacks|\bthiel\b|sequoia|founders[-_\s]*fund|Valar[-_\s]*Ventures|6th[-_\s]*Man[-_\s]*Ventures|Northzone|Warburg[-_\s]*Serres|Alan[-_\s]*Howard|Tiger[-_\s]*Global
 Voyager,voyager
@@ -122,10 +131,11 @@
 Wallet Addresses Dash,X[1–9A-HJ-NP-Za-km-z]{33}
 Wallet Addresses Doge,\sD[a-zA-Z0–9_.-]{33}
 Wallet Addresses Ethereum,0x[a-fA-F0–9]{40}
 Wallet Addresses Monero,[48][0–9AB][1–9A-HJ-NP-Za-km-z]{93}
 Wallet Addresses Polkadot,1[0–9a-zA-Z]{47}
 Wallet Addresses Ripple,r[0–9a-zA-Z]{33}
 Wallet Addresses Stellar,G[0–9A-Z]{40,60}\b
+Waves,sasha35625|sasha\.waves|\bvires|sasha[-_\s]*ivanov|boris[-_\s]*titov|[$#]waves\b
 Wintermute,wintermute|\bbebop\b
-Wirecard,wirecard|\bmarsalek\b
-Wyre,wyre
+Wirecard,wirecard|\bmarsalek\b|\bBafin\b
+Wyre,\bwyre|sendwyre
```

### Comparing `clown_sort-1.3.2/clown_sort/util/argument_parser.py` & `clown_sort-1.3.3/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/util/constants.py` & `clown_sort-1.3.3/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/util/filesystem_helper.py` & `clown_sort-1.3.3/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/clown_sort/util/rich_helper.py` & `clown_sort-1.3.3/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.2/pyproject.toml` & `clown_sort-1.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.3.2"
+version = "1.3.3"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.3.2/setup.py` & `clown_sort-1.3.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 entry_points = \
 {'console_scripts': ['set_screenshot_timestamps = '
                      'clown_sort:set_screenshot_timestamps',
                      'sort_screenshots = clown_sort:sort_screenshots']}
 
 setup_kwargs = {
     'name': 'clown-sort',
-    'version': '1.3.2',
+    'version': '1.3.3',
     'description': 'Sort screenshots based on rules or through individual review.',
-    'long_description': '# CLOWN SORT\nSometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can\'t find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.\n\nClown Sort[^1] solves this.\n\n\n## What It Do\nIt sorts screenshots, PDFs, etc. based on their name and/or their textual contents into folders based on a list of rules. The contents of the tweet/reddit post/whatever are prepended to the filename and the `ImageDescription` EXIF tag is set to the OCR text. As you can configure your own arbitrary rules and run it against any set of images it works on many things other than screenshots of social media clowns, though the default configuration is for cryptocurrency clowns.\n\nFor example this screenshot of a tweet by a noteworthy cryptocurrency "reporter"[^2] on the eve of FTX\'s implosion:\n\n![](doc/larry_cermak_on_alameda_and_ftx.png)\n\nWould be renamed from `Screen Shot 2023-02-17 at 7.11.37 PM.png` to\n\n```\nTweet by @lawmaster: "I will say though before this thread gets taken over: 1. I do believe Alameda has the size to easily buy Binance\\\'s FIT OTC 2. I think the chance of FTX insolvency is near" Screen Shot 2023-02-17 at 7.11.37 PM.png\n```\n\nOther stuff that happens:\n* The `ImageDescription` EXIF tag will be written (for images).\n* All timestamps will be preserved.\n* Files that match multiple patterns will be copied to multiple destination folders.\n* The original file will be moved into a `Processed/` directory after it has been handled.\n\nNote also that:\n* This works on images that are more substantive than just self-clowning screenshots.\n* So far only Tweets and Reddit screenshots have special handling beyond OCR text extraction.\n* PDFs can be sorted by contents or filename, e.g. a PDF named `Norton Anthology of Crypto Bro Poetry.pdf` containing iambic verse like _["Fuck u justin sun  and fuck ur dick face... u all play with investing and money of the people !!!!"](https://universeodon.com/@cryptadamist/109642431382653023)_ by the noted bard JOKER_OF_CRYPTO will be copied to the `Justin Sun/` folder but not renamed.\n* Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.\n\n## Quick Start\n```sh\n# Installation with pipx is preferred if you have it but you can also use pip which comes standard\n# on almost all systems. pipx is only a noticeably better answer if you\'re a python programmer who\n# is concerned about side effects of pip upgrading system python packages.\npip install clown_sort\n\n# Get help\nsort_screenshots -h\n\n# Dry run with default cryptocurrency sort rules (dry runs don\'t actually move anything,\n# they just show you what will happen if you run again with the --execute flag)\nsort_screenshots\n\n# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots\nsort_screenshots --execute\n\n# Sort a different directory of screenshots\nsort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute\n\n# Sort with custom rules\nsort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute\n\n# Sort pdfs\nsort_screenshots -f \'.*pdf$\' -e\n```\n\n# Setup\n[pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.\n```\npipx install clown_sort\n```\n\nSome (not many) PDFs require the `pycryptodome` package. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with:\n\n```sh\npipx install clown_sort[pycryptodome]\n```\n\n\n### Configuring With `.clown_sort` File\nIf there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:\n\n1. The current directory\n2. Your home directory\n\nSee [the example](.clown_sort.example) for more information on what can be configured this way.\n\n### Optional Components\nIf you want to use the popup window to manually tag you _may_ need to install:\n* Python TK: `brew install python-tk@3.10` (if you don\'t have [homebrew](https://brew.sh/) you need to install it to run `brew install`)\n\nNot required for standard PNG, JPG, etc. images but you may optionally install `exiftool` for other file types if you want excessive debugging.\n* ExifTool: `brew install exiftool` or download from https://exiftool.org\n\n\n# Usage\nThe default is for the tool to run in "dry run" mode, meaning it doesn\'t actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**\n\nWhile every effort has been made to use Python\'s cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.\n\n### Help Screen\n![](doc/sort_screenshots_help.png)\n\n(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)\n\n### Custom Sorting Rules\nThe default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you\'re not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.\n\n### Example Output (Automated Sorting)\n![](doc/output_example.png)\n\n\n## Manually Sorting (Experimental)\n**This is an experimental feature.** It\'s only been tested on macOS.\n\nIf you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.\n\nTo use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:\n```sh\npipx install clown_sort[PySimpleGUI]\n```\n\n![](doc/manual_select_box.png)\n\n\n# Contributing\nFeel free to file issues or open pull requests.\n\nThis package is managed with [Python Poetry](http://python-poetry.org/). To get going:\n1. Install Poetry.\n1. `git clone` this repo.\n1. `cd clown_sort`\n1. `poetry install`\n1. Optional components can be install with `poetry install -E pdf -E gui`\n\nOnly requirement is that tests should pass before you open it, which you can check with\n\n```\npytest\n```\n\n[^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.\n\n[^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried\'s various scams as part of his commitment to "unrivaled transparency".\n',
+    'long_description': '# CLOWN SORT\nSometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can\'t find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.\n\nClown Sort[^1] solves this.\n\n\n## What It Do\nIt sorts screenshots, PDFs, etc. based on their name and/or their textual contents into folders based on a list of rules. The contents of the tweet/reddit post/whatever are prepended to the filename and the `ImageDescription` EXIF tag is set to the OCR text. As you can configure your own arbitrary rules and run it against any set of images it works on many things other than screenshots of social media clowns, though the default configuration is for cryptocurrency clowns.\n\nFor example this screenshot of a tweet by a noteworthy cryptocurrency "reporter"[^2] on the eve of FTX\'s implosion:\n\n![](doc/larry_cermak_on_alameda_and_ftx.png)\n\nWould be renamed from `Screen Shot 2023-02-17 at 7.11.37 PM.png` to\n\n```\nTweet by @lawmaster: "I will say though before this thread gets taken over: 1. I do believe Alameda has the size to easily buy Binance\\\'s FIT OTC 2. I think the chance of FTX insolvency is near" Screen Shot 2023-02-17 at 7.11.37 PM.png\n```\n\nOther stuff that happens:\n* The `ImageDescription` EXIF tag will be written (for images).\n* All timestamps will be preserved.\n* Files that match multiple patterns will be copied to multiple destination folders.\n* The original file will be moved into a `Processed/` directory after it has been handled.\n\nNote also that:\n* This works on images that are more substantive than just self-clowning screenshots.\n* So far only Tweets and Reddit screenshots have special handling beyond OCR text extraction.\n* PDFs can be sorted by contents or filename, e.g. a PDF named `Norton Anthology of Crypto Bro Poetry.pdf` containing iambic verse like _["Fuck u justin sun  and fuck ur dick face... u all play with investing and money of the people !!!!"](https://universeodon.com/@cryptadamist/109642431382653023)_ by the noted bard JOKER_OF_CRYPTO will be copied to the `Justin Sun/` folder but not renamed.\n* Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.\n\n## Quick Start\n```sh\n# Installation with pipx is preferred if you have it but you can also use pip which comes standard\n# on almost all systems. pipx is only a noticeably better answer if you\'re a python programmer who\n# is concerned about side effects of pip upgrading system python packages.\npip install clown_sort\n\n# Get help\nsort_screenshots -h\n\n# Dry run with default cryptocurrency sort rules (dry runs don\'t actually move anything,\n# they just show you what will happen if you run again with the --execute flag)\nsort_screenshots\n\n# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots\nsort_screenshots --execute\n\n# Sort a different directory of screenshots\nsort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute\n\n# Sort with custom rules\nsort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute\n\n# Sort pdfs\nsort_screenshots -f \'.*pdf$\' -e\n```\n\n# Setup\n[pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.\n```\npipx install clown_sort\n```\n\nSome (not many) PDFs require the `pycryptodome` package to be parsed. If you don\'t have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pycryptodome]`.\n\nUpdating to the latest version can be accomplished with `pipx upgrade clown_sort`.\n\n\n### Configuring With `.clown_sort` File\nIf there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:\n\n1. The current directory\n2. Your home directory\n\nSee [the example](.clown_sort.example) for more information on what can be configured this way.\n\n### Optional Components\nIf you want to use the popup window to manually tag you _may_ need to install:\n* Python TK: `brew install python-tk@3.10` (if you don\'t have [homebrew](https://brew.sh/) you need to install it to run `brew install`)\n\nNot required for standard PNG, JPG, etc. images but you may optionally install `exiftool` for other file types if you want excessive debugging.\n* ExifTool: `brew install exiftool` or download from https://exiftool.org\n\n\n# Usage\nThe default is for the tool to run in "dry run" mode, meaning it doesn\'t actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**\n\nWhile every effort has been made to use Python\'s cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.\n\n### Help Screen\n![](doc/sort_screenshots_help.png)\n\n(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)\n\n### Custom Sorting Rules\nThe default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you\'re not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.\n\n### Example Output (Automated Sorting)\n![](doc/output_example.png)\n\n\n## Manually Sorting (Experimental)\n**This is an experimental feature.** It\'s only been tested on macOS.\n\nIf you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.\n\nTo use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:\n```sh\npipx install clown_sort[PySimpleGUI]\n```\n\n![](doc/manual_select_box.png)\n\n\n# Contributing\nFeel free to file issues or open pull requests.\n\nThis package is managed with [Python Poetry](http://python-poetry.org/). To get going:\n1. Install Poetry.\n1. `git clone` this repo.\n1. `cd clown_sort`\n1. `poetry install`\n1. Optional components can be install with `poetry install -E pdf -E gui`\n\nOnly requirement is that tests should pass before you open it, which you can check with\n\n```\npytest\n```\n\n[^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.\n\n[^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried\'s various scams as part of his commitment to "unrivaled transparency".\n',
     'author': 'Michel de Cryptadamus',
     'author_email': 'michel@cryptadamus.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/michelcrypt4d4mus/clown_sort',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `clown_sort-1.3.2/PKG-INFO` & `clown_sort-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.3.2
+Version: 1.3.3
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -90,19 +90,17 @@
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
 ```
 pipx install clown_sort
 ```
 
-Some (not many) PDFs require the `pycryptodome` package. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with:
+Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pycryptodome]`.
 
-```sh
-pipx install clown_sort[pycryptodome]
-```
+Updating to the latest version can be accomplished with `pipx upgrade clown_sort`.
 
 
 ### Configuring With `.clown_sort` File
 If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
 
 1. The current directory
 2. Your home directory
```


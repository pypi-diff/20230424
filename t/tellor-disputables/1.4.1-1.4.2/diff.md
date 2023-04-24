# Comparing `tmp/tellor_disputables-1.4.1.tar.gz` & `tmp/tellor_disputables-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellor_disputables-1.4.1.tar", max compression
+gzip compressed data, was "tellor_disputables-1.4.2.tar", max compression
```

## Comparing `tellor_disputables-1.4.1.tar` & `tellor_disputables-1.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     9401 2023-04-06 18:49:29.235626 tellor_disputables-1.4.1/README.md
--rw-r--r--   0        0        0      308 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/disputer-config.yaml
--rw-r--r--   0        0        0      995 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8930 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/src/tellor_disputables/__init__.py
--rw-r--r--   0        0        0     2661 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/src/tellor_disputables/alerts.py
--rw-r--r--   0        0        0     7573 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/src/tellor_disputables/cli.py
--rw-r--r--   0        0        0     3390 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/src/tellor_disputables/config.py
--rw-r--r--   0        0        0    13677 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/src/tellor_disputables/data.py
--rw-r--r--   0        0        0     5596 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/src/tellor_disputables/disputer.py
--rw-r--r--   0        0        0     3491 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/src/tellor_disputables/utils.py
--rw-r--r--   0        0        0      152 2023-04-06 18:49:29.239626 tellor_disputables-1.4.1/vars.example.sh
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 tellor_disputables-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     9401 2023-04-24 16:28:23.336368 tellor_disputables-1.4.2/README.md
+-rw-r--r--   0        0        0      368 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/disputer-config.yaml
+-rw-r--r--   0        0        0      996 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9235 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/src/tellor_disputables/__init__.py
+-rw-r--r--   0        0        0     2661 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/src/tellor_disputables/alerts.py
+-rw-r--r--   0        0        0     7573 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/src/tellor_disputables/cli.py
+-rw-r--r--   0        0        0     4057 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/src/tellor_disputables/config.py
+-rw-r--r--   0        0        0    17690 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/src/tellor_disputables/data.py
+-rw-r--r--   0        0        0     6493 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/src/tellor_disputables/disputer.py
+-rw-r--r--   0        0        0     3491 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/src/tellor_disputables/utils.py
+-rw-r--r--   0        0        0      152 2023-04-24 16:28:23.344368 tellor_disputables-1.4.2/vars.example.sh
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 tellor_disputables-1.4.2/PKG-INFO
```

### Comparing `tellor_disputables-1.4.1/README.md` & `tellor_disputables-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tellor_disputables-1.4.1/pyproject.toml` & `tellor_disputables-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tellor-disputables"
-version = "1.4.1"
+version = "1.4.2"
 description = "dashboard & text alerts for disputable values reported to Tellor oracles"
 authors = ["tallywiesenberg <info@tellor.io>"]
 license = "MIT"
 packages = [{ include = "tellor_disputables", from = "src" }]
 include = ["vars.example.sh", "README.md", "disputer-config.yaml"]
 
 [tool.poetry.dependencies]
@@ -13,15 +13,15 @@
 web3 = "^5.27.0"
 pandas = "^1.4.1"
 tabulate = "^0.8.9"
 pytest-asyncio = "^0.19.0"
 click = "^8.1.3"
 pydantic = "^1.10.2"
 python-box = "^7.0.1"
-telliot-feeds = "^0.1.7"
+telliot-feeds = "^0.1.10"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.0"
 black = "^22.3.0"
 pre-commit = "^2.17.0"
 mypy = "^0.942"
 types-python-dateutil = "^2.8.10"
```

### Comparing `tellor_disputables-1.4.1/src/tellor_disputables/__init__.py` & `tellor_disputables-1.4.2/src/tellor_disputables/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Tellor Disputables - CLI dashboard & alerts for potential
 bad values reported to Tellor oracles."""
 from hexbytes import HexBytes
 from telliot_feeds import feeds
+from telliot_feeds.queries.mimicry.nft_market_index import MimicryNFTMarketIndex
+from telliot_feeds.queries.price.spot_price import SpotPrice
 from web3.datastructures import AttributeDict
 
 WAIT_PERIOD = 7  # seconds between checks for new events
 
 ALWAYS_ALERT_QUERY_TYPES = ("AutopayAddresses", "TellorOracleAddress")
 
+QUERY_TYPES = (SpotPrice, MimicryNFTMarketIndex)
+
 DATAFEED_LOOKUP = {
+    "486e2149f25d46bb39a27f5e0c81be9b6f193abf46c0d49314b8d1dd104cd53b": feeds.mimicry_nft_market_index_usd_feed,
     "0d12ad49193163bbbeff4e6db8294ced23ff8605359fd666799d4e25a3aa0e3a": feeds.ampl_usd_vwap_feed,
     "35e083af947a4cf3bc053440c3b4f753433c76acab6c8b1911ee808104b72e85": feeds.bct_usd_feed.bct_usd_median_feed,
     "a6f013ee236804827b77696d350e9f0ac3e879328f2a3021d473a0b778ad78ac": feeds.btc_usd_feed.btc_usd_median_feed,
     "d913406746edf7891a09ffb9b26a12553bbf4d25ecf8e530ec359969fe6a7a9c": feeds.dai_usd_feed.dai_usd_median_feed,
     "ba3452d8acca69e530308515f4a0cb01da604dd077801db619800e7d3a7b5f8c": feeds.eth_jpy_feed.eth_jpy_median_feed,
     "83a7f3d48786ac2667503a61e8c415438ed2922eb86a2906e4ee66d9a2ce4992": feeds.eth_usd_feed.eth_usd_median_feed,
     "7239909c0aa5d3e89efb2dce06c80811e93ab18413110b8c0435ee32c52cc4fb": feeds.idle_usd_feed.idle_usd_median_feed,
```

### Comparing `tellor_disputables-1.4.1/src/tellor_disputables/alerts.py` & `tellor_disputables-1.4.2/src/tellor_disputables/alerts.py`

 * *Files identical despite different names*

### Comparing `tellor_disputables-1.4.1/src/tellor_disputables/cli.py` & `tellor_disputables-1.4.2/src/tellor_disputables/cli.py`

 * *Files identical despite different names*

### Comparing `tellor_disputables-1.4.1/src/tellor_disputables/config.py` & `tellor_disputables-1.4.2/src/tellor_disputables/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 from typing import Any
 from typing import List
 from typing import Optional
 
 import yaml
 from box import Box
 from telliot_feeds.feeds import DataFeed
+from telliot_feeds.feeds import DATAFEED_BUILDER_MAPPING
 
 from tellor_disputables import DATAFEED_LOOKUP
 from tellor_disputables.data import Metrics
 from tellor_disputables.data import MonitoredFeed
 from tellor_disputables.data import Threshold
+from tellor_disputables.utils import get_logger
+
+logger = get_logger(__name__)
 
 
 @dataclass
 class AutoDisputerConfig:
 
     monitored_feeds: Optional[List[MonitoredFeed]]
 
@@ -56,45 +60,54 @@
 
         monitored_feeds = []
 
         for i in range(len(self.box.feeds)):
             try:
                 # parse query type from YAML
                 try:
-                    query_id = self.box.feeds[i].query_id[2:]
+                    if hasattr(self.box.feeds[i], "query_id"):
+                        query_id = self.box.feeds[i].query_id[2:]
+                        datafeed: DataFeed[Any] = DATAFEED_LOOKUP[query_id]
+                    elif hasattr(self.box.feeds[i], "query_type"):
+                        query_type = self.box.feeds[i].query_type
+                        datafeed = DATAFEED_BUILDER_MAPPING[query_type]
+                    else:
+                        logger.error("Invalid query id or query type provided in disputer-config.yaml")
                 except AttributeError as e:
-                    logging.error(f"Python Box attribute error: {e}")
+                    logger.error(f"Python Box attribute error: {e}")
                     return None
                 except TypeError as e:
-                    logging.error(f"Python Box attribute error: {e}")
+                    logger.error(f"Python Box type error: {e}")
                     return None
 
-                datafeed: DataFeed[Any] = DATAFEED_LOOKUP[query_id]
             except KeyError:
-                logging.error(f"No corresponding datafeed found for query id: {query_id}\n")
+                logger.error(f"No corresponding datafeed found for query id: {query_id}\n")
                 return None
 
             try:
                 # parse query type from YAML
                 try:
                     threshold_type = self.box.feeds[i].threshold.type
-                    threshold_amount = self.box.feeds[i].threshold.amount
+                    if threshold_type.lower() == "equality":
+                        threshold_amount = None
+                    else:
+                        threshold_amount = self.box.feeds[i].threshold.amount
                 except AttributeError as e:
                     logging.error(f"Python Box attribute error: {e}")
                     return None
                 except TypeError as e:
                     logging.error(f"Python Box attribute error: {e}")
                     return None
 
                 threshold: Threshold = Threshold(Metrics[threshold_type], amount=threshold_amount)
             except KeyError:
                 logging.error(f"Unsupported threshold: {threshold}\n")
                 return None
 
-            monitored_feeds.append(MonitoredFeed(datafeed, threshold, query_id))
+            monitored_feeds.append(MonitoredFeed(datafeed, threshold))
 
         return monitored_feeds
 
 
 if __name__ == "__main__":
 
     print(AutoDisputerConfig())
```

### Comparing `tellor_disputables-1.4.1/src/tellor_disputables/data.py` & `tellor_disputables-1.4.2/src/tellor_disputables/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Get and parse NewReport events from Tellor oracles."""
 import asyncio
+import math
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
+import eth_abi
 from chained_accounts import ChainedAccount
+from clamfig import deserialize
+from clamfig.base import Registry
 from telliot_core.apps.telliot_config import TelliotConfig
 from telliot_core.contract.contract import Contract
 from telliot_core.directory import contract_directory
 from telliot_core.model.base import Base
 from telliot_feeds.datafeed import DataFeed
+from telliot_feeds.datasource import DataSource
 from telliot_feeds.queries.abi_query import AbiQuery
 from telliot_feeds.queries.json_query import JsonQuery
-from telliot_feeds.queries.price.spot_price import SpotPrice
 from telliot_feeds.queries.query import OracleQuery
 from web3 import Web3
 from web3._utils.events import get_event_data
 from web3.types import LogReceipt
 
 from tellor_disputables import ALWAYS_ALERT_QUERY_TYPES
 from tellor_disputables import DATAFEED_LOOKUP
@@ -69,50 +73,80 @@
             if self.amount is None:
                 raise ValueError(f"{self.metric} threshold selected, amount cannot be None")
 
             if self.amount < 0:
                 raise ValueError(f"{self.metric} threshold selected, amount cannot be negative")
 
 
+Reportable = Union[str, bytes, float, int, tuple[Any], None]
+
+
 @dataclass
 class MonitoredFeed(Base):
     feed: DataFeed[Any]
     threshold: Threshold
-    query_id: Optional[str] = None
 
     async def is_disputable(
         self,
-        reported_val: Union[str, bytes, float, int, None],
+        cfg: TelliotConfig,
+        reported_val: Reportable,
     ) -> Optional[bool]:
         """Check if the reported value is disputable."""
         if reported_val is None:
             logger.error("Need reported value to check disputability")
             return None
 
-        trusted_val, _ = await general_fetch_new_datapoint(self.feed)
-        if not trusted_val:
-            logger.warning("trusted val was " + str(trusted_val))
-            return None
+        if get_query_type(self.feed.query) == "EVMCall":
+
+            if not isinstance(reported_val, tuple):
+                return True
 
-        if isinstance(trusted_val, (str, int, float, bytes)):
+            block_timestamp = reported_val[1]
+            cfg.main.chain_id = self.feed.query.chainId
+
+            block_number = get_block_number_at_timestamp(cfg, block_timestamp)
+
+            trusted_val, _ = await general_fetch_new_datapoint(self.feed, block_number)
+
+            if trusted_val is None:
+                logger.warning("trusted val was " + str(trusted_val))
+                return None
+
+        else:
+            trusted_val, _ = await general_fetch_new_datapoint(self.feed)
+
+            if trusted_val is None:
+                logger.warning("trusted val was " + str(trusted_val))
+                return None
+
+        if isinstance(reported_val, (str, bytes, float, int, tuple)) and isinstance(
+            trusted_val, (str, bytes, float, int, tuple)
+        ):
 
             if self.threshold.metric == Metrics.Percentage:
 
-                if isinstance(trusted_val, (str, bytes)) or isinstance(reported_val, (str, bytes)):
+                if not trusted_val:
+                    logger.warning(
+                        f"Telliot val for {self.feed.query} found to be 0. Reported value was {reported_val!r}"
+                        "Please double check telliot value before disputing."
+                    )
+                    return None
+
+                if isinstance(trusted_val, (str, bytes, tuple)) or isinstance(reported_val, (str, bytes, tuple)):
                     logger.error("Cannot evaluate percent difference on text/addresses/bytes")
                     return None
                 if self.threshold.amount is None:
                     logger.error("Please set a threshold amount to measure percent difference")
                     return None
                 percent_diff: float = (reported_val - trusted_val) / trusted_val
                 return float(abs(percent_diff)) >= self.threshold.amount
 
             elif self.threshold.metric == Metrics.Range:
 
-                if isinstance(trusted_val, (str, bytes)) or isinstance(reported_val, (str, bytes)):
+                if isinstance(trusted_val, (str, bytes, tuple)) or isinstance(reported_val, (str, bytes, tuple)):
                     logger.error("Cannot evaluate range on text/addresses/bytes")
 
                 if self.threshold.amount is None:
                     logger.error("Please set a threshold amount to measure range")
                     return None
                 range_: float = abs(reported_val - trusted_val)
                 return range_ >= self.threshold.amount
@@ -123,27 +157,30 @@
                 if (
                     (isinstance(reported_val, str))
                     and (isinstance(trusted_val, str))
                     and reported_val.startswith("0x")
                     and trusted_val.startswith("0x")
                 ):
                     return trusted_val.lower() != reported_val.lower()
-                return trusted_val != reported_val
+                return bool(trusted_val != reported_val)
 
             else:
                 logger.error("Attemping comparison with unknown threshold metric")
                 return None
         else:
-            logger.error("Unable to fetch new datapoint from feed")
+            logger.error(
+                f"Unable to compare telliot val {trusted_val!r} of type {type(trusted_val)}"
+                f"with reported val {reported_val!r} of type {type(reported_val)}"
+            )
             return None
 
 
-async def general_fetch_new_datapoint(feed: DataFeed) -> Optional[Any]:
+async def general_fetch_new_datapoint(feed: DataFeed, *args: Any) -> Optional[Any]:
     """Fetch a new datapoint from a datafeed."""
-    return await feed.source.fetch_new_datapoint()
+    return await feed.source.fetch_new_datapoint(*args)
 
 
 def get_contract_info(chain_id: int, name: str) -> Tuple[Optional[str], Optional[str]]:
     """Get the contract address and ABI for the given chain ID."""
 
     contracts = contract_directory.find(chain_id=chain_id, name=name)
 
@@ -304,27 +341,48 @@
         try:
             return q_type.get_query_from_data(query_data)
         except ValueError:
             pass
     return None
 
 
+def get_source_from_data(query_data: bytes) -> Optional[DataSource]:
+    """Recreate an oracle query from the `query_data` field"""
+    try:
+        query_type, encoded_param_values = eth_abi.decode_abi(["string", "bytes"], query_data)
+    except OverflowError:
+        logger.error("OverflowError while decoding query data.")
+        return None
+    try:
+        cls = Registry.registry[query_type]
+    except KeyError:
+        logger.error(f"Unsupported query type: {query_type}")
+        return None
+    params_abi = cls.abi
+    param_names = [p["name"] for p in params_abi]
+    param_types = [p["type"] for p in params_abi]
+    param_values = eth_abi.decode_abi(param_types, encoded_param_values)
+
+    params = dict(zip(param_names, param_values))
+
+    if query_type != "SpotPrice":
+        query_type += "Source"
+
+    return deserialize({"type": query_type, **params})
+
+
 async def parse_new_report_event(
     cfg: TelliotConfig,
     log: LogReceipt,
     confidence_threshold: float,
     monitored_feeds: List[MonitoredFeed],
     see_all_values: bool = False,
 ) -> Optional[NewReport]:
     """Parse a NewReport event."""
 
-    q_ids_to_monitored_feeds = {
-        monitored_feed.feed.query.query_id.hex(): monitored_feed for monitored_feed in monitored_feeds
-    }
-
     chain_id = cfg.main.chain_id
     endpoint = cfg.endpoints.find(chain_id=chain_id)[0]
 
     new_report = NewReport()
 
     if not endpoint:
         logger.error(f"Unable to find a suitable endpoint for chain_id {chain_id}")
@@ -340,45 +398,69 @@
 
         codec = w3.codec
         event_data = get_event_data(codec, NEW_REPORT_ABI, log)
 
     q = get_query_from_data(event_data.args._queryData)
 
     if q is None:
-        logger.error("Unable to form query from query data")
+        logger.error("Unable to form query from queryData of query type" + new_report.query_type)
         return None
 
     new_report.tx_hash = event_data.transactionHash.hex()
     new_report.chain_id = endpoint.web3.eth.chain_id
     new_report.query_id = "0x" + event_data.args._queryId.hex()
     new_report.query_type = get_query_type(q)
-    new_report.value = q.value_type.decode(event_data.args._value)
     new_report.link = get_tx_explorer_url(tx_hash=new_report.tx_hash, cfg=cfg)
     new_report.submission_timestamp = event_data.args._time  # in unix time
 
+    try:
+        new_report.value = q.value_type.decode(event_data.args._value)
+    except eth_abi.exceptions.DecodingError:
+        new_report.value = event_data.args._value
+
+    # if query of event matches a query type of the monitored feeds, fill the query parameters
+
+    monitored_feed = None
+
+    for mf in monitored_feeds:
+
+        if get_query_type(mf.feed.query) == new_report.query_type:
+
+            if new_report.query_type == "SpotPrice":
+
+                mf.feed = DATAFEED_LOOKUP[new_report.query_id[2:]]
+
+            else:
+
+                source = get_source_from_data(event_data.args._queryData)
+
+                if source is None:
+                    logger.error("Unable to form source from queryData of query type" + new_report.query_type)
+                    return None
+
+                mf.feed = DataFeed(query=q, source=source)
+
+            monitored_feed = mf
+
     if new_report.query_type in ALWAYS_ALERT_QUERY_TYPES:
         new_report.status_str = "❗❗❗❗ VERY IMPORTANT DATA SUBMISSION ❗❗❗❗"
         return new_report
 
-    if new_report.query_id not in q_ids_to_monitored_feeds:  # TODO ensure both has 0x or none have 0x
+    if monitored_feed is not None:
+        monitored_query_id = monitored_feed.feed.query.query_id.hex()
+    else:
+        monitored_query_id = None
+
+    if (new_report.query_id[2:] != monitored_query_id) or (not monitored_feed):
 
         # build a monitored feed for all feeds not auto-disputing for
         threshold = Threshold(metric=Metrics.Percentage, amount=confidence_threshold)
         monitored_feed = MonitoredFeed(DATAFEED_LOOKUP[new_report.query_id[2:]], threshold)
-    else:
-        monitored_feed = q_ids_to_monitored_feeds[new_report.query_id]
 
-    if isinstance(q, SpotPrice):
-        new_report.asset = q.asset.upper()
-        new_report.currency = q.currency.upper()
-    else:
-        logger.error("unsupported query type")
-        return None
-
-    disputable = await monitored_feed.is_disputable(new_report.value)
+    disputable = await monitored_feed.is_disputable(cfg, new_report.value)
     if disputable is None:
 
         if see_all_values:
 
             new_report.status_str = disputable_str(disputable, new_report.query_id)
             new_report.disputable = disputable
 
@@ -387,7 +469,47 @@
             logger.info("unable to check disputability")
             return None
     else:
         new_report.status_str = disputable_str(disputable, new_report.query_id)
         new_report.disputable = disputable
 
         return new_report
+
+
+def get_block_number_at_timestamp(cfg: TelliotConfig, timestamp: int) -> Optional[int]:
+
+    try:
+        endpoint = cfg.get_endpoint()
+        endpoint.connect()
+    except ValueError as e:
+        logger.error(f"Unable to connect to endpoint on chain_id {cfg.main.chain_id}: " + str(e))
+        return None
+
+    w3 = endpoint.web3
+
+    current_block = w3.eth.block_number
+    start_block = 0
+    end_block = current_block
+
+    while start_block <= end_block:
+        midpoint = math.floor((start_block + end_block) / 2)
+        block = w3.eth.get_block(midpoint)
+
+        if block.timestamp == timestamp:
+            return midpoint
+        elif block.timestamp < timestamp:
+            start_block = midpoint + 1
+        else:
+            end_block = midpoint - 1
+
+    # If we haven't found an exact match, interpolate between adjacent blocks
+    block_a = w3.eth.get_block(end_block)
+    block_b = w3.eth.get_block(start_block)
+
+    block_delta = block_b.number - block_a.number
+    timestamp_delta = block_b.timestamp - block_a.timestamp
+    target_delta = timestamp - block_a.timestamp
+
+    estimated_block_delta = target_delta * block_delta / timestamp_delta
+    estimated_block_number = block_a.number + estimated_block_delta
+
+    return int(estimated_block_number)
```

### Comparing `tellor_disputables-1.4.1/src/tellor_disputables/disputer.py` & `tellor_disputables-1.4.2/src/tellor_disputables/disputer.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,26 +19,46 @@
 ) -> str:
     """Main dispute logic for auto-disputer"""
 
     if not disp_cfg.monitored_feeds:
         logger.info("Currently not auto-dispuing on any feeds. See ./disputer-config.yaml")
         return ""
 
-    meant_to_dispute = new_report.query_id[2:] in [feed.feed.query.query_id.hex() for feed in disp_cfg.monitored_feeds]
+    disputable_query_ids = []
+    for feed in disp_cfg.monitored_feeds:
+        try:
+            disputable_query_id = feed.feed.query.query_id.hex()
+        except Exception:
+            pass
+        disputable_query_ids.append(disputable_query_id)
+
+    meant_to_dispute = new_report.query_id[2:] in disputable_query_ids
 
     if not meant_to_dispute:
         logger.info("Found disputable new report outside selected Monitored Feeds, skipping dispute")
         return ""
 
     if account is None:
         logger.info("No account provided, skipping eligible dispute")
         return ""
 
     cfg.main.chain_id = new_report.chain_id
 
+    try:
+        endpoint = cfg.get_endpoint()
+    except ValueError:
+        logger.error(f"Unable to dispute: can't find an endpoint on chain id {new_report.chain_id}")
+        return ""
+
+    try:
+        endpoint.connect()
+    except ValueError:
+        logger.error(f"Unable to dispute: can't connect to endpoint on chain id {new_report.chain_id}")
+        return ""
+
     token = get_contract(cfg, name="trb-token", account=account)
     governance = get_contract(cfg, name="tellor-governance", account=account)
 
     if token is None:
         logger.error("Unable to find token contract")
         return ""
 
@@ -64,44 +84,56 @@
     logger.info("Dispute Fee: " + str(dispute_fee / 1e18) + " TRB")
 
     # if balanceOf(user) < disputeFee, log "need more tokens to initiate dispute"
     if user_token_balance < dispute_fee:
         logger.info("User balance is below dispute fee: need more tokens to initiate dispute")
         return ""
 
+    try:
+        acc_nonce = endpoint.web3.eth.get_transaction_count(Web3.toChecksumAddress(account.address))
+    except Exception as e:
+        logger.error(f"Unable to dispute: could not retrieve account nonce: {e}")
+        return ""
+
     # write approve(governance contract, disputeFee) and log "token approved" if successful
     gas_price = await fetch_gas_price()
     tx_receipt, status = await token.write(
-        "approve", spender=governance.address, amount=dispute_fee * 100, gas_limit=60000, legacy_gas_price=gas_price
+        "approve",
+        spender=governance.address,
+        amount=dispute_fee * 100,
+        gas_limit=60000,
+        legacy_gas_price=gas_price,
+        acc_nonce=acc_nonce,
     )
 
     if not status.ok:
         logger.error("unable to approve tokens for dispute fee: " + status.error)
         return ""
 
     logger.info("Approval Tx Hash: " + str(tx_receipt.transactionHash.hex()))
 
     tx_receipt, status = await governance.write(
         func_name="beginDispute",
         _queryId=new_report.query_id,
         _timestamp=new_report.submission_timestamp,
         gas_limit=800000,
         legacy_gas_price=gas_price,
+        acc_nonce=acc_nonce + 1,
     )
 
     if not status.ok:
         logger.error(
             f"unable to begin dispute on {new_report.query_id}"
             + f"at submission timestamp {new_report.submission_timestamp}:"
             + status.error
         )
         return ""
 
     new_report.status_str += ": disputed!"
-    explorer = cfg.get_endpoint().explorer
+    explorer = endpoint.explorer
     if not explorer:
         dispute_tx_link = str(tx_receipt.transactionHash.hex())
     else:
         dispute_tx_link = explorer + str(tx_receipt.transactionHash.hex())
 
     logger.info("Dispute Tx Link: " + dispute_tx_link)
     return "Dispute Tx Link: " + dispute_tx_link
```

### Comparing `tellor_disputables-1.4.1/src/tellor_disputables/utils.py` & `tellor_disputables-1.4.2/src/tellor_disputables/utils.py`

 * *Files identical despite different names*

### Comparing `tellor_disputables-1.4.1/PKG-INFO` & `tellor_disputables-1.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellor-disputables
-Version: 1.4.1
+Version: 1.4.2
 Summary: dashboard & text alerts for disputable values reported to Tellor oracles
 License: MIT
 Author: tallywiesenberg
 Author-email: info@tellor.io
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,10 +12,10 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pytest-asyncio (>=0.19.0,<0.20.0)
 Requires-Dist: python-box (>=7.0.1,<8.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
-Requires-Dist: telliot-feeds (>=0.1.7,<0.2.0)
+Requires-Dist: telliot-feeds (>=0.1.10,<0.2.0)
 Requires-Dist: twilio (>=7.7.0,<8.0.0)
 Requires-Dist: web3 (>=5.27.0,<6.0.0)
```


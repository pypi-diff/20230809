# Comparing `tmp/minswap_py-0.2.1.tar.gz` & `tmp/minswap_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minswap_py-0.2.1.tar", max compression
+gzip compressed data, was "minswap_py-0.3.0.tar", max compression
```

## Comparing `minswap_py-0.2.1.tar` & `minswap_py-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-01-23 21:36:51.427567 minswap_py-0.2.1/LICENSE
--rw-r--r--   0        0        0     1325 2023-07-09 00:06:49.111301 minswap_py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2526 2023-07-09 00:10:54.817138 minswap_py-0.2.1/README.md
--rw-r--r--   0        0        0      170 2023-06-29 13:18:21.012654 minswap_py-0.2.1/src/minswap/__init__.py
--rw-r--r--   0        0        0    18209 2023-07-08 23:42:48.126153 minswap_py-0.2.1/src/minswap/addr.py
--rw-r--r--   0        0        0    30826 2023-06-29 13:17:59.623510 minswap_py-0.2.1/src/minswap/assets.py
--rw-r--r--   0        0        0      397 2023-06-29 13:18:21.014655 minswap_py-0.2.1/src/minswap/models/__init__.py
--rw-r--r--   0        0        0    95901 2023-06-29 13:17:59.626508 minswap_py-0.2.1/src/minswap/models/blockfrost_models.py
--rw-r--r--   0        0        0     9044 2023-06-29 13:17:59.627509 minswap_py-0.2.1/src/minswap/models/common.py
--rw-r--r--   0        0        0    12574 2023-07-08 23:54:30.655576 minswap_py-0.2.1/src/minswap/pools.py
--rw-r--r--   0        0        0    13458 2023-06-29 13:17:59.630510 minswap_py-0.2.1/src/minswap/transactions.py
--rw-r--r--   0        0        0     9145 2023-06-29 13:17:59.631509 minswap_py-0.2.1/src/minswap/utils.py
--rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 minswap_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-01-23 21:36:51.427567 minswap_py-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1259 2023-08-09 02:19:27.448512 minswap_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4197 2023-08-09 02:05:57.192739 minswap_py-0.3.0/README.md
+-rw-r--r--   0        0        0      195 2023-08-09 02:02:17.605720 minswap_py-0.3.0/src/minswap/__init__.py
+-rw-r--r--   0        0        0    18952 2023-07-30 19:21:28.386994 minswap_py-0.3.0/src/minswap/addr.py
+-rw-r--r--   0        0        0    30826 2023-06-29 13:17:59.623510 minswap_py-0.3.0/src/minswap/assets.py
+-rw-r--r--   0        0        0      606 2023-08-09 00:41:54.140557 minswap_py-0.3.0/src/minswap/models/__init__.py
+-rw-r--r--   0        0        0    95901 2023-06-29 13:17:59.626508 minswap_py-0.3.0/src/minswap/models/blockfrost_models.py
+-rw-r--r--   0        0        0    15383 2023-08-09 00:42:20.866577 minswap_py-0.3.0/src/minswap/models/common.py
+-rw-r--r--   0        0        0    14376 2023-07-31 17:03:02.034385 minswap_py-0.3.0/src/minswap/pools.py
+-rw-r--r--   0        0        0    13458 2023-06-29 13:17:59.630510 minswap_py-0.3.0/src/minswap/transactions.py
+-rw-r--r--   0        0        0     9835 2023-07-21 01:21:44.717368 minswap_py-0.3.0/src/minswap/utils.py
+-rw-r--r--   0        0        0    23884 2023-08-09 01:41:09.688806 minswap_py-0.3.0/src/minswap/wallets.py
+-rw-r--r--   0        0        0     5148 1970-01-01 00:00:00.000000 minswap_py-0.3.0/PKG-INFO
```

### Comparing `minswap_py-0.2.1/LICENSE` & `minswap_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minswap_py-0.2.1/src/minswap/addr.py` & `minswap_py-0.3.0/src/minswap/addr.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 Attributes:
     POOL: Mainnet pool address.
     POOL_TEST: Testnet pool address.
     ORDER: Mainnet pool address.
     ORDER_TEST: Testnet pool address.
 """
 import logging
+import os
 import time
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from multiprocessing import cpu_count
 from pathlib import Path
 from typing import List, Optional, Tuple
 
-import blockfrost
 import numpy
 import pandas
 import vaex
-from dotenv import dotenv_values
+from dotenv import load_dotenv
 from pyarrow import TimestampScalar
 
 from minswap.models import Address, PoolTransactionReference
-from minswap.utils import get_utxo, save_timestamp
+from minswap.utils import BlockfrostBackend, get_utxo, save_timestamp
+
+load_dotenv()
 
 logger = logging.getLogger(__name__)
 
-POOL = [
+POOL_MAIN = [
     Address(
         bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxz2j2c79gy9l76sdg0xwhd7r0c0kna0tycz4y5s6mlenh8pq0xmsha"  # noqa
     ),
     Address(
         bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxzfgf0jgfz5xdvg2pges20usxhw8zwnkggheqrxwmxd6huuqss46eh"  # noqa
     ),
     Address(
@@ -44,24 +46,46 @@
     Address(
         bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxz2jyskd3y6etkv8ye450545xu6q4jfq5hv4e0uxwkpf8lsq048y90"  # noqa
     ),
     Address(
         bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxztnqm37tpj0q63s0qns5wfe4flqzqqg55760472n7yt4v8skpaj3k"  # noqa
     ),
 ]
-ORDER = Address(
+ORDER_MAIN = Address(
     bech32="addr1zxn9efv2f6w82hagxqtn62ju4m293tqvw0uhmdl64ch8uw6j2c79gy9l76sdg0xwhd7r0c0kna0tycz4y5s6mlenh8pq6s3z70"  # noqa
 )
-
-POOL_TEST = Address(
-    bech32="addr_test1zrsnz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxzvrajt8r8wqtygrfduwgukk73m5gcnplmztc5tl5ngy0upqs8q93k"  # noqa
+STAKE_ORDER_MAIN = Address(
+    bech32="addr1zxn9efv2f6w82hagxqtn62ju4m293tqvw0uhmdl64ch8uw6j2c79gy9l76sdg0xwhd7r0c0kna0tycz4y5s6mlenh8pq6s3z70"  # noqa
 )
+
+POOL_TEST = [
+    Address(
+        bech32="addr_test1zrsnz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxzvrajt8r8wqtygrfduwgukk73m5gcnplmztc5tl5ngy0upqs8q93k"  # noqa
+    )
+]
 ORDER_TEST = Address(
     bech32="addr_test1zzn9efv2f6w82hagxqtn62ju4m293tqvw0uhmdl64ch8uwurajt8r8wqtygrfduwgukk73m5gcnplmztc5tl5ngy0upq932hcy"  # noqa
 )
+STAKE_ORDER_TEST = Address(
+    bech32="addr_test1zzn9efv2f6w82hagxqtn62ju4m293tqvw0uhmdl64ch8uwurajt8r8wqtygrfduwgukk73m5gcnplmztc5tl5ngy0upq932hcy"  # noqa
+)
+
+if os.environ.get("NETWORK", "mainnet").lower() == "mainnet":
+    POOL = POOL_MAIN
+    ORDER = ORDER_MAIN
+    STAKE_ORDER = STAKE_ORDER_MAIN
+elif os.environ.get("NETWORK", None) == "preprod":
+    POOL = POOL_TEST
+    ORDER = ORDER_TEST
+    STAKE_ORDER = STAKE_ORDER_TEST
+else:
+    raise ValueError(
+        f"The NETWORK environment variable was set to {os.environ.get('NETWORK')}. "
+        + "Must be one of ['main', 'preprod']."
+    )
 
 # Policies
 FACTORY_POLICY_ID = "13aa2accf2e1561723aa26871e071fdf32c867cff7e7d50ad470d62f"
 FACTORY_ASSET_NAME = "4d494e53574150"
 LP_POLICY_ID = "e4214b7cce62ac6fbba385d164df48e157eae5863521b4b67ca71d86"
 POOL_NFT_POLICY_ID = "0be55d262b29f564998ff81efe21bdc0022621c12f15af08d0f2ddb1"
 
@@ -236,18 +260,15 @@
         page: The index of paginated results to return. Defaults to 1.
         count: The total number of results to return. Defaults to 100.
         order: Must be "asc" or "desc". Defaults to "desc".
 
     Returns:
         A list of `PoolHistory` items.
     """
-    env = dotenv_values()
-    api = blockfrost.BlockFrostApi(env["PROJECT_ID"])
-
-    txs = api.address_transactions(
+    txs = BlockfrostBackend.api().address_transactions(
         pol_addr, count=count, page=page, order=order, return_type="json"
     )
 
     tx = [PoolTransactionReference.parse_obj(tx) for tx in txs]
 
     return tx
```

### Comparing `minswap_py-0.2.1/src/minswap/assets.py` & `minswap_py-0.3.0/src/minswap/assets.py`

 * *Files identical despite different names*

### Comparing `minswap_py-0.2.1/src/minswap/models/blockfrost_models.py` & `minswap_py-0.3.0/src/minswap/models/blockfrost_models.py`

 * *Files identical despite different names*

### Comparing `minswap_py-0.2.1/src/minswap/pools.py` & `minswap_py-0.3.0/src/minswap/pools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Functions for processing minswap pools.
 
 This mostly reflects the pool functionality in the minswap-blockfrostadapter.
 """
 import logging
+import math
 from concurrent.futures import ThreadPoolExecutor
 from decimal import Decimal
 from typing import List, Optional, Tuple, Union
 
 from pydantic import BaseModel, root_validator
 
 from minswap import addr
 from minswap.assets import naturalize_assets
-from minswap.models import AddressUtxoContent  # type: ignore[attr-defined]
 from minswap.models import (
+    AddressUtxoContent,
     AddressUtxoContentItem,
     AssetIdentity,
     Assets,
     AssetTransaction,
     Output,
+    PoolDatum,
     TxContentUtxo,
 )
 from minswap.utils import BlockfrostBackend
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
@@ -53,22 +55,22 @@
         )
         logger.debug(message)
         raise InvalidPool(message)
 
     # Check to make sure the pool has 1 factory token
     for asset in utxo.amount:
         has_factory: bool = (
-            f"{addr.FACTORY_POLICY_ID}{addr.FACTORY_ASSET_NAME}" == asset.unit
+            f"{addr.FACTORY_POLICY_ID}{addr.FACTORY_ASSET_NAME}" == asset
         )
         if has_factory:
             break
     if not has_factory:
         message = "Pool must have 1 factory token."
         logger.debug(message)
-        logger.debug(f"asset.unit={asset.unit}")
+        logger.debug(f"asset.unit={asset}")
         logger.debug(f"factory={addr.FACTORY_POLICY_ID}{addr.FACTORY_ASSET_NAME}")
         raise InvalidPool(message)
 
 
 def is_valid_pool_output(utxo: AddressUtxoContentItem):
     """Determine if a utxo contains a pool identifier."""
     try:
@@ -83,23 +85,32 @@
 
     tx_index: int
     tx_hash: str
     assets: Assets
     pool_nft: Assets
     minswap_nft: Assets
     datum_hash: str
+    lp_total: int
+    root_k_last: int
 
     class Config:  # noqa: D106
         allow_mutation = False
         extra = "forbid"
 
     @root_validator(pre=True)
     def translate_address(cls, values):  # noqa: D102
         assets = values["assets"]
 
+        raw_datum = BlockfrostBackend.api().script_datum(
+            values["datum_hash"], return_type="json"
+        )["json_value"]
+        pool_datum = PoolDatum.from_dict(raw_datum)
+        values["lp_total"] = pool_datum.total_liquidity
+        values["root_k_last"] = pool_datum.root_k_last
+
         # Find the NFT that assigns the pool a unique id
         nfts = [asset for asset in assets if asset.startswith(addr.POOL_NFT_POLICY_ID)]
         if len(nfts) != 1:
             raise ValueError("A pool must have one pool NFT token.")
         pool_nft = Assets(**{nfts[0]: assets.__root__.pop(nfts[0])})
         values["pool_nft"] = pool_nft
 
@@ -209,15 +220,15 @@
 
         Raises:
             NotImplementedError: Only ADA pool TVL is implemented.
         """
         if self.unit_a != "lovelace":
             raise NotImplementedError("tvl for non-ADA pools is not implemented.")
 
-        tvl = (Decimal(self.reserve_a) / Decimal(10**6)).quantize(
+        tvl = 2 * (Decimal(self.reserve_a) / Decimal(10**6)).quantize(
             1 / Decimal(10**6)
         )
 
         return tvl
 
     def get_amount_out(self, asset: Assets) -> Tuple[Assets, float]:
         """Get the output asset amount given an input asset amount.
@@ -226,30 +237,30 @@
             asset: An asset with a defined quantity.
 
         Returns:
             A tuple where the first value is the estimated asset returned from the swap
                 and the second value is the price impact ratio.
         """
         assert len(asset) == 1, "Asset should only have one token."
-        assert asset.unit in [
+        assert asset.unit() in [
             self.unit_a,
             self.unit_b,
         ], f"Asset {asset.unit} is invalid for pool {self.unit_a}-{self.unit_b}"
 
-        if asset.unit == self.unit_a:
+        if asset.unit() == self.unit_a:
             reserve_in, reserve_out = self.reserve_a, self.reserve_b
             unit_out = self.unit_b
         else:
             reserve_in, reserve_out = self.reserve_b, self.reserve_a
             unit_out = self.unit_a
 
         # Calculate the amount out
         numerator: int = asset.quantity() * 997 * reserve_out
         denominator: int = asset.quantity() * 997 + reserve_in * 1000
-        amount_out = Assets(unit=unit_out, quantity=numerator // denominator)
+        amount_out = Assets(**{unit_out: numerator // denominator})
 
         # Calculate the price impact
         price_numerator: int = (
             reserve_out * asset.quantity() * denominator * 997
             - numerator * reserve_in * 1000
         )
         price_denominator: int = reserve_out * asset.quantity() * denominator * 1000
@@ -289,14 +300,57 @@
             - asset.quantity() * denominator * reserve_in * 1000
         )
         price_denominator: int = reserve_out * numerator * 1000
         price_impact: float = price_numerator / price_denominator
 
         return amount_in, price_impact
 
+    def get_zap_in_lp(self, asset: Assets) -> Tuple[Assets, float]:
+        """Calculate the estimate LP received for zapping in an amount of asset.
+
+        Args:
+            asset: An asset with a defined quantity.
+
+        Returns:
+            The estimated amount of lp received for the zap in quantity.
+        """
+        assert len(asset) == 1, "Asset should only have one token."
+        assert asset.unit() in [
+            self.unit_a,
+            self.unit_b,
+        ], f"Asset {asset.unit} is invalid for pool {self.unit_a}-{self.unit_b}"
+        if asset.unit() == self.unit_a:
+            reserve_in, reserve_out = self.reserve_a, self.reserve_b
+        else:
+            reserve_in, reserve_out = self.reserve_b, self.reserve_a
+
+        quantity_in = (
+            math.sqrt(
+                1997**2 * reserve_in**2
+                + 4 * 997 * 1000 * asset.quantity() * reserve_in
+            )
+            - 1997 * reserve_in
+        ) / (2 * 997)
+        asset_in = Assets(**{asset.unit(): quantity_in})
+
+        asset_out, price_impact = self.get_amount_out(asset_in)
+
+        # This number appears to be incorrect
+        # https://github.com/minswap/blockfrost-adapter/pull/7/files#r1279439474
+        total_lp = self.lp_total
+
+        quantity_lp = (asset_out.quantity() * total_lp) / (
+            reserve_out - asset_out.quantity()
+        )
+
+        lp_out = Assets(**{self.lp_token: int(quantity_lp)})
+
+        # TODO: Make sure price impact is correct
+        return lp_out, price_impact
+
 
 def get_pools(
     return_non_pools: bool = False,
 ) -> Union[List[PoolState], tuple[List[PoolState], List[AddressUtxoContentItem]]]:
     """Get a list of all pools.
 
     Args:
@@ -328,15 +382,15 @@
 
     for utxo in utxos:
         if is_valid_pool_output(utxo):
             pools.append(
                 PoolState(
                     tx_hash=utxo.tx_hash,
                     tx_index=utxo.output_index,
-                    assets=Assets(values=utxo.amount),
+                    assets=utxo.amount,
                     datum_hash=utxo.data_hash,
                 )
             )
         else:
             non_pools.append(utxo)
 
     if return_non_pools:
@@ -366,17 +420,17 @@
     if pool_utxo is None:
         return None
 
     check_valid_pool_output(pool_utxo)
 
     out_state = PoolState(
         tx_hash=tx_hash,
-        tx_index=utxo.output_index,
-        assets=Assets(values=utxo.amount),
-        datum_hash=utxo.data_hash,
+        tx_index=pool_utxo.output_index,
+        assets=pool_utxo.amount,
+        datum_hash=pool_utxo.data_hash,
     )
 
     return out_state
 
 
 def get_pool_by_id(pool_id: str) -> Optional[PoolState]:
     """Latest `PoolState` of a pool.
```

### Comparing `minswap_py-0.2.1/src/minswap/transactions.py` & `minswap_py-0.3.0/src/minswap/transactions.py`

 * *Files identical despite different names*

### Comparing `minswap_py-0.2.1/src/minswap/utils.py` & `minswap_py-0.3.0/src/minswap/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,296 +1,318 @@
-"""Utility functions."""
-import logging
-import os
-import time
-from datetime import datetime
-from pathlib import Path
-from threading import Lock
-from typing import Callable, List, Optional, Union
-
-import blockfrost
-import pandas
-import vaex
-from dotenv import load_dotenv
-
-import minswap
-
-logger = logging.getLogger(__name__)
-
-CACHE_GLOB = "[0-9][0-9][0-9][0-9][0-9][0-9].arrow"
-
-# Load the project information
-load_dotenv()
-PROJECT_ID = os.environ["PROJECT_ID"]
-MAX_CALLS = int(os.environ["MAX_CALLS"])
-call_lock = Lock()
-
-
-class BlockfrostCallLimit(Exception):
-    """Error when the Blockfrost call limit is reached."""
-
-
-class BlockfrostBackend:
-    """A class to enforce stall calls to Blockfrost when a rate limit is hit."""
-
-    last_call: float = time.time()
-    num_limit_calls: float = 0.0
-    max_limit_calls: int = 500
-    total_calls = 0
-    max_total_calls = MAX_CALLS
-    backoff_time: int = 10
-    _api = blockfrost.BlockFrostApi(PROJECT_ID)
-
-    @classmethod
-    def remaining_calls(cls) -> int:
-        """Remaining calls before rate limit."""
-        return cls.max_total_calls - cls.total_calls
-
-    @classmethod
-    def reset_total_calls(cls) -> None:
-        """Reset the call count."""
-        cls.total_calls = 0
-
-    @classmethod
-    def _limiter(cls):
-        with call_lock:
-            cls.num_limit_calls += 1
-            cls.total_calls += 1
-            if cls.total_calls >= cls.max_total_calls:
-                raise BlockfrostCallLimit(
-                    f"Made {cls.total_calls}, "
-                    + f"only {cls.max_total_calls} are allowed."
-                )
-            elif cls.num_limit_calls >= cls.max_limit_calls:
-                logger.warning(
-                    "At or near blockfrost rate limit. "
-                    + f"Waiting {cls.backoff_time}s..."
-                )
-                time.sleep(cls.backoff_time)
-                logger.info("Finished sleeping, resuming...")
-
-        now = time.time()
-        cls.num_limit_calls = max(0, cls.num_limit_calls - (now - cls.last_call) * 10)
-        cls.last_call = now
-
-    @classmethod
-    def api(cls):
-        """Blockfrost API with rate limits."""
-        cls._limiter()
-        return cls._api
-
-    @classmethod
-    def rate_limit(cls, func):
-        """Wrap with rate limit.
-
-        This can probably be removed. It might have utility in the future for
-        customizing imposing rate limits on a function.
-
-        """
-
-        def wrapper(*args, **kwargs):
-            cls._limiter()
-            try:
-                return func(*args, **kwargs)
-            except blockfrost.ApiError:
-                print(f"cls.num_limit_calls: {cls.num_limit_calls}")
-                raise
-
-        return wrapper
-
-
-def save_timestamp(
-    basepath: Path, arg_num: int, kwarg_key: str, func: Optional[Callable] = None
-) -> Callable:
-    """Timestamp cache decorator.
-
-    Args:
-        basepath: Path to save the timestamp to.
-        arg_num: Argument position that should be used to append to basepath.
-        kwarg_key: Alternative to arg_num, in case kwarg is supplied instead of an arg.
-        func: Function to wrap. Defaults to None.
-
-    Returns:
-        Wrapped function that will have a timestamp dumped to disk.
-    """
-    if func is None:
-        return lambda x: save_timestamp(
-            basepath=basepath, arg_num=arg_num, kwarg_key=kwarg_key, func=x
-        )
-
-    def wrapper(*args, **kwargs):
-        if len(args) - 1 >= arg_num:
-            key = args[arg_num]
-        else:
-            key = kwargs[kwarg_key]
-
-        if hasattr(key, "id"):
-            identifier = key.id
-        else:
-            identifier = key
-
-        path = basepath.joinpath(identifier)
-
-        path.mkdir(exist_ok=True, parents=True)
-
-        with open(path.joinpath("TIMESTAMP"), "w") as fw:
-            fw.write(str(time.time()))
-
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-def load_timestamp(path: Path) -> datetime:
-    """Load a timestamp for a cache.
-
-    Args:
-        path: Path to cache.
-
-    Returns:
-        A datetime object for when the function was called.
-    """
-    with open(path.joinpath("TIMESTAMP")) as fr:
-        timestamp = datetime.utcfromtimestamp(float(fr.read()))
-
-    return timestamp
-
-
-def _get_cache(cache_path: Path, glob: str = CACHE_GLOB) -> Optional[vaex.DataFrame]:
-    if len(list(cache_path.glob(glob))) > 0:
-        df = vaex.open(cache_path.joinpath(glob))
-    else:
-        df = None
-
-    return df
-
-
-def _cache_timestamp_data(
-    data: Union[
-        List[minswap.models.PoolTransactionReference],
-        List[minswap.models.Transaction],
-        List[pandas.DataFrame],
-    ],
-    cache_path: Path,
-    hash_filter: bool = False,
-) -> Union[
-    List[minswap.models.PoolTransactionReference],
-    List[minswap.models.Transaction],
-    List[pandas.DataFrame],
-]:
-    """Cache a list of objects.
-
-    This is a utility function to cache a list of objects containing a timestamp. It
-    searches the list for a change in the timestamp month, caches data for the first
-    occurring month, and returns the rest.
-
-    Args:
-        data: A list of objects containing a time element.
-        cache_path: The path to where the data should be stored.
-
-    Raises:
-        TypeError: `data` must be one of [PoolTransactionReference, pandas.DataFrame]
-
-    Returns:
-        _description_
-    """
-    # Convert data to a vaex dataframe
-    if isinstance(
-        data[0], (minswap.models.PoolTransactionReference, minswap.models.Transaction)
-    ):
-        if data[0].block_time.month == data[-1].block_time.month:
-            index = len(data)
-        else:
-            for index in range(len(data) - 1):
-                if data[index].block_time.month != data[index + 1].block_time.month:
-                    index += 1
-                    break
-        df = pandas.DataFrame([d.dict() for d in data[:index]])
-    elif isinstance(data[0], pandas.DataFrame):
-        if data[0].block_time[0].month == data[-1].block_time[0].month:  # type: ignore
-            index = len(data)
-        else:
-            for index in range(len(data) - 1):
-                if (
-                    data[index].block_time[0].month  # type:ignore
-                    != data[index + 1].block_time[0].month  # type: ignore
-                ):
-                    index += 1
-                    break
-        df = pandas.concat(data, ignore_index=True)
-    else:
-        raise TypeError(
-            "Transactions should be one of [pydantic.BaseModel, pandas.DataFrame]"
-        )
-
-    df["block_time"] = df.block_time.astype("datetime64[s]")
-    df.sort_values(by="block_time", inplace=True)
-
-    # Define the output path
-    cache_name = (
-        f"{df.block_time[0].year}" + f"{str(df.block_time[0].month).zfill(2)}.arrow"
-    )
-    path = cache_path.joinpath(cache_name)
-
-    # If the cache exists, append to it
-    if path.exists():
-        cache_df = pandas.read_feather(path)
-        tmp_path = path.with_name(path.name.replace(".arrow", "_temp.arrow"))
-        if hash_filter:
-            unique_hashes = list(
-                set(df.hash.values.tolist()) - set(cache_df.hash.values.tolist())
-            )
-            filtered = df[df.hash.isin(unique_hashes)]
-        else:
-            threshold = cache_df.block_time.astype("datetime64[s]").values[-1]
-            filtered = df[df.block_time > threshold]
-
-        logger.info(len(filtered))
-        if len(filtered) > 0:
-            pandas.concat([cache_df, filtered], ignore_index=True).sort_values(
-                by="block_time"
-            ).reset_index(drop=True).to_feather(tmp_path)
-            path.unlink()
-            tmp_path.rename(path)
-
-    # Otherwise, just dump the whole dataframe to cache
-    else:
-        df.sort_values(by="block_time", inplace=True)
-        df.reset_index(drop=True, inplace=True)
-        df.to_feather(path)
-
-    return data[index:]
-
-
-def get_utxo(
-    tx_hash: str,
-) -> pandas.DataFrame:
-    """Get a list of pool history transactions.
-
-    This returns a pandas dataframe containing all inputs and UTXOs for a particular
-    transaction.
-
-    Args:
-        pool_id: The unique pool id.
-        page: The index of paginated results to return. Defaults to 1.
-        count: The total number of results to return. Defaults to 100.
-        order: Must be "asc" or "desc". Defaults to "desc".
-
-    Returns:
-        A list of `PoolHistory` items.
-    """
-    tx = BlockfrostBackend.api().transaction_utxos(tx_hash, return_type="json")
-
-    # TODO: Need to create a pydantic model for this
-    df = (
-        pandas.concat(
-            [pandas.DataFrame(tx["inputs"]), pandas.DataFrame(tx["outputs"])],
-            keys=["input", "output"],
-        )
-        .reset_index(level=0)
-        .reset_index(drop=True)
-    )
-
-    df.rename(columns={"level_0": "side"}, inplace=True)
-    df["hash"] = tx["hash"]
-
-    return df
+"""Utility functions."""
+import logging
+import os
+import time
+from datetime import datetime
+from pathlib import Path
+from threading import Lock
+from typing import Callable, List, Optional, Union
+
+import blockfrost
+import pandas
+import vaex
+from dotenv import load_dotenv
+
+import minswap
+
+logger = logging.getLogger(__name__)
+
+CACHE_GLOB = "[0-9][0-9][0-9][0-9][0-9][0-9].arrow"
+
+# Load the project information
+load_dotenv()
+PROJECT_ID = os.environ["PROJECT_ID"]
+MAX_CALLS = int(os.environ["MAX_CALLS"])
+call_lock = Lock()
+
+
+class BlockfrostCallLimit(Exception):
+    """Error when the Blockfrost call limit is reached."""
+
+
+class BlockfrostBackend:
+    """A class to enforce stall calls to Blockfrost when a rate limit is hit."""
+
+    last_call: float = time.time()
+    num_limit_calls: float = 0.0
+    max_limit_calls: int = 500
+    total_calls = 0
+    max_total_calls = MAX_CALLS
+    backoff_time: int = 10
+    _api_url = getattr(blockfrost.ApiUrls, os.environ["NETWORK"]).value
+    _api = blockfrost.BlockFrostApi(PROJECT_ID, base_url=_api_url)
+    _network_parameters: minswap.models.EpochParamContent = (
+        minswap.models.EpochParamContent.parse_obj(
+            _api.epoch_latest_parameters(return_type="json")
+        )
+    )
+    _epoch_infos: minswap.models.EpochContent = minswap.models.EpochContent.parse_obj(
+        _api.epoch_latest(return_type="json")
+    )
+
+    @classmethod
+    def remaining_calls(cls) -> int:
+        """Remaining calls before rate limit."""
+        return cls.max_total_calls - cls.total_calls
+
+    @classmethod
+    def reset_total_calls(cls) -> None:
+        """Reset the call count."""
+        cls.total_calls = 0
+
+    @classmethod
+    def _limiter(cls):
+        with call_lock:
+            cls.num_limit_calls += 1
+            cls.total_calls += 1
+            if cls.total_calls >= cls.max_total_calls:
+                raise BlockfrostCallLimit(
+                    f"Made {cls.total_calls}, "
+                    + f"only {cls.max_total_calls} are allowed."
+                )
+            elif cls.num_limit_calls >= cls.max_limit_calls:
+                logger.warning(
+                    "At or near blockfrost rate limit. "
+                    + f"Waiting {cls.backoff_time}s..."
+                )
+                time.sleep(cls.backoff_time)
+                logger.info("Finished sleeping, resuming...")
+
+        now = time.time()
+        cls.num_limit_calls = max(0, cls.num_limit_calls - (now - cls.last_call) * 10)
+        cls.last_call = now
+
+    @classmethod
+    def api(cls) -> blockfrost.BlockFrostApi:
+        """Blockfrost API with rate limits."""
+        cls._limiter()
+        return cls._api
+
+    @classmethod
+    def rate_limit(cls, func):
+        """Wrap with rate limit.
+
+        This can probably be removed. It might have utility in the future for
+        customizing imposing rate limits on a function.
+
+        """
+
+        def wrapper(*args, **kwargs):
+            cls._limiter()
+            try:
+                return func(*args, **kwargs)
+            except blockfrost.ApiError:
+                print(f"cls.num_limit_calls: {cls.num_limit_calls}")
+                raise
+
+        return wrapper
+
+    @classmethod
+    def protocol_parameters(cls) -> minswap.models.EpochParamContent:
+        """Cardano protocol parameters."""
+        if int(time.time()) > cls._epoch_infos.end_time:
+            cls._epoch_infos = minswap.models.EpochContent.parse_obj(
+                cls.api().epoch_latest(return_type="json")
+            )
+            cls._network_parameters = minswap.models.EpochParamContent.parse_obj(
+                cls.api().epoch_latest_parameters(return_type="json")
+            )
+
+        return cls._network_parameters
+
+
+def save_timestamp(
+    basepath: Path, arg_num: int, kwarg_key: str, func: Optional[Callable] = None
+) -> Callable:
+    """Timestamp cache decorator.
+
+    Args:
+        basepath: Path to save the timestamp to.
+        arg_num: Argument position that should be used to append to basepath.
+        kwarg_key: Alternative to arg_num, in case kwarg is supplied instead of an arg.
+        func: Function to wrap. Defaults to None.
+
+    Returns:
+        Wrapped function that will have a timestamp dumped to disk.
+    """
+    if func is None:
+        return lambda x: save_timestamp(
+            basepath=basepath, arg_num=arg_num, kwarg_key=kwarg_key, func=x
+        )
+
+    def wrapper(*args, **kwargs):
+        if len(args) - 1 >= arg_num:
+            key = args[arg_num]
+        else:
+            key = kwargs[kwarg_key]
+
+        if hasattr(key, "id"):
+            identifier = key.id
+        else:
+            identifier = key
+
+        path = basepath.joinpath(identifier)
+
+        path.mkdir(exist_ok=True, parents=True)
+
+        with open(path.joinpath("TIMESTAMP"), "w") as fw:
+            fw.write(str(time.time()))
+
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def load_timestamp(path: Path) -> datetime:
+    """Load a timestamp for a cache.
+
+    Args:
+        path: Path to cache.
+
+    Returns:
+        A datetime object for when the function was called.
+    """
+    with open(path.joinpath("TIMESTAMP")) as fr:
+        timestamp = datetime.utcfromtimestamp(float(fr.read()))
+
+    return timestamp
+
+
+def _get_cache(cache_path: Path, glob: str = CACHE_GLOB) -> Optional[vaex.DataFrame]:
+    if len(list(cache_path.glob(glob))) > 0:
+        df = vaex.open(cache_path.joinpath(glob))
+    else:
+        df = None
+
+    return df
+
+
+def _cache_timestamp_data(
+    data: Union[
+        List[minswap.models.PoolTransactionReference],
+        List[minswap.models.Transaction],
+        List[pandas.DataFrame],
+    ],
+    cache_path: Path,
+    hash_filter: bool = False,
+) -> Union[
+    List[minswap.models.PoolTransactionReference],
+    List[minswap.models.Transaction],
+    List[pandas.DataFrame],
+]:
+    """Cache a list of objects.
+
+    This is a utility function to cache a list of objects containing a timestamp. It
+    searches the list for a change in the timestamp month, caches data for the first
+    occurring month, and returns the rest.
+
+    Args:
+        data: A list of objects containing a time element.
+        cache_path: The path to where the data should be stored.
+
+    Raises:
+        TypeError: `data` must be one of [PoolTransactionReference, pandas.DataFrame]
+
+    Returns:
+        _description_
+    """
+    # Convert data to a vaex dataframe
+    if isinstance(
+        data[0], (minswap.models.PoolTransactionReference, minswap.models.Transaction)
+    ):
+        if data[0].block_time.month == data[-1].block_time.month:
+            index = len(data)
+        else:
+            for index in range(len(data) - 1):
+                if data[index].block_time.month != data[index + 1].block_time.month:
+                    index += 1
+                    break
+        df = pandas.DataFrame([d.dict() for d in data[:index]])
+    elif isinstance(data[0], pandas.DataFrame):
+        if data[0].block_time[0].month == data[-1].block_time[0].month:  # type: ignore
+            index = len(data)
+        else:
+            for index in range(len(data) - 1):
+                if (
+                    data[index].block_time[0].month  # type:ignore
+                    != data[index + 1].block_time[0].month  # type: ignore
+                ):
+                    index += 1
+                    break
+        df = pandas.concat(data, ignore_index=True)
+    else:
+        raise TypeError(
+            "Transactions should be one of [pydantic.BaseModel, pandas.DataFrame]"
+        )
+
+    df["block_time"] = df.block_time.astype("datetime64[s]")
+    df.sort_values(by="block_time", inplace=True)
+
+    # Define the output path
+    cache_name = (
+        f"{df.block_time[0].year}" + f"{str(df.block_time[0].month).zfill(2)}.arrow"
+    )
+    path = cache_path.joinpath(cache_name)
+
+    # If the cache exists, append to it
+    if path.exists():
+        cache_df = pandas.read_feather(path)
+        tmp_path = path.with_name(path.name.replace(".arrow", "_temp.arrow"))
+        if hash_filter:
+            unique_hashes = list(
+                set(df.hash.values.tolist()) - set(cache_df.hash.values.tolist())
+            )
+            filtered = df[df.hash.isin(unique_hashes)]
+        else:
+            threshold = cache_df.block_time.astype("datetime64[s]").values[-1]
+            filtered = df[df.block_time > threshold]
+
+        logger.info(len(filtered))
+        if len(filtered) > 0:
+            pandas.concat([cache_df, filtered], ignore_index=True).sort_values(
+                by="block_time"
+            ).reset_index(drop=True).to_feather(tmp_path)
+            path.unlink()
+            tmp_path.rename(path)
+
+    # Otherwise, just dump the whole dataframe to cache
+    else:
+        df.sort_values(by="block_time", inplace=True)
+        df.reset_index(drop=True, inplace=True)
+        df.to_feather(path)
+
+    return data[index:]
+
+
+def get_utxo(
+    tx_hash: str,
+) -> pandas.DataFrame:
+    """Get a list of pool history transactions.
+
+    This returns a pandas dataframe containing all inputs and UTXOs for a particular
+    transaction.
+
+    Args:
+        pool_id: The unique pool id.
+        page: The index of paginated results to return. Defaults to 1.
+        count: The total number of results to return. Defaults to 100.
+        order: Must be "asc" or "desc". Defaults to "desc".
+
+    Returns:
+        A list of `PoolHistory` items.
+    """
+    tx = BlockfrostBackend.api().transaction_utxos(tx_hash, return_type="json")
+
+    # TODO: Need to create a pydantic model for this
+    df = (
+        pandas.concat(
+            [pandas.DataFrame(tx["inputs"]), pandas.DataFrame(tx["outputs"])],
+            keys=["input", "output"],
+        )
+        .reset_index(level=0)
+        .reset_index(drop=True)
+    )
+
+    df.rename(columns={"level_0": "side"}, inplace=True)
+    df["hash"] = tx["hash"]
+
+    return df
```


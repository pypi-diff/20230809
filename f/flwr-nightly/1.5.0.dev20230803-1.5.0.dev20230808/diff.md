# Comparing `tmp/flwr_nightly-1.5.0.dev20230803.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230808.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230803.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230808.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230803.tar` & `flwr_nightly-1.5.0.dev20230808.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    11358 2023-08-03 23:00:53.081812 flwr_nightly-1.5.0.dev20230803/LICENSE
--rw-r--r--   0        0        0    10808 2023-08-03 23:00:53.085812 flwr_nightly-1.5.0.dev20230803/README.md
--rw-r--r--   0        0        0     5422 2023-08-03 23:01:13.509818 flwr_nightly-1.5.0.dev20230803/pyproject.toml
--rw-r--r--   0        0        0      952 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    14058 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     7677 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     7209 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4954 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     7345 2023-08-03 23:00:53.617709 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6380 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     4693 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5318 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     9050 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1875 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1791 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1889 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3459 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    18804 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3861 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3906 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4877 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5653 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     7295 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     6182 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     7505 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2183 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     8232 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0    10889 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26229 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6120 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2227 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1054 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5686 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6408 2023-08-03 23:00:53.621708 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4650 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11501 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6313 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     2546 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2876 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3934 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4897 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15958 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6774 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19294 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4833 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1647 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4654 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     6995 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5893 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6740 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7014 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11522 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9991 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8286 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2708 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5428 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7126 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     6026 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3519 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7079 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6343 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10154 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5478 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5672 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7762 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5471 2023-08-03 23:00:53.625707 flwr_nightly-1.5.0.dev20230803/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    13163 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230803/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-08 23:00:56.096177 flwr_nightly-1.5.0.dev20230808/LICENSE
+-rw-r--r--   0        0        0    10808 2023-08-08 23:00:56.096177 flwr_nightly-1.5.0.dev20230808/README.md
+-rw-r--r--   0        0        0     5420 2023-08-08 23:01:12.336396 flwr_nightly-1.5.0.dev20230808/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    14058 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7677 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     7209 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4954 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     7345 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6380 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     4693 2023-08-08 23:00:56.568184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5318 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     9050 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1875 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1791 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1889 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3459 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    18804 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3861 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3906 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4877 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5653 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7295 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     6182 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     7505 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2183 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8232 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0    10889 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26229 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6120 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2227 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1054 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5686 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6408 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4650 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11738 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6313 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     2546 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2876 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3934 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4897 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15958 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6774 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19294 2023-08-08 23:00:56.572184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4833 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1647 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4654 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     6995 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5893 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6740 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7014 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11522 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9991 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8286 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2708 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5428 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7126 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     6026 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3519 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7079 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6343 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10154 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5478 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5672 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7762 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5471 2023-08-08 23:00:56.576184 flwr_nightly-1.5.0.dev20230808/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    13163 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230808/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230803/LICENSE` & `flwr_nightly-1.5.0.dev20230808/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/README.md` & `flwr_nightly-1.5.0.dev20230808/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/pyproject.toml` & `flwr_nightly-1.5.0.dev20230808/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230803"
+version = "1.5.0-dev20230808"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
@@ -78,15 +78,15 @@
 [tool.poetry.extras]
 simulation = ["ray", "pydantic"]
 rest = ["requests", "starlette", "uvicorn"]
 
 [tool.poetry.group.dev.dependencies]
 types-dataclasses = "==0.6.6"
 types-protobuf = "==3.19.18"
-types-requests = "==2.28.11.17"
+types-requests = "==2.31.0.2"
 types-setuptools = "==68.0.0.3"
 clang-format = "==16.0.3"
 isort = "==5.11.5"
 black = { version = "==23.3.0", extras = ["jupyter"] }
 docformatter = "==1.7.5"
 mypy = "==1.4.0"
 pylint = "==2.13.9"
```

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,18 @@
         # compatibility with popular cloud providers. Mobile Flower clients may
         # choose to increase this value if their server environment allows
         # long-running idle TCP connections.
         ("grpc.keepalive_time_ms", keepalive_time_ms),
         # Setting this to zero will allow sending unlimited keepalive pings in between
         # sending actual data frames.
         ("grpc.http2.max_pings_without_data", 0),
+        # Is it permissible to send keepalive pings from the client without
+        # any outstanding streams. More explanation here:
+        # https://github.com/adap/flower/pull/2197
+        ("grpc.keepalive_permit_without_calls", 0),
     ]
 
     server = grpc.server(
         concurrent.futures.ThreadPoolExecutor(max_workers=max_concurrent_workers),
         # Set the maximum number of concurrent RPCs this server will service before
         # returning RESOURCE_EXHAUSTED status, or None to indicate no limit.
         maximum_concurrent_rpcs=max_concurrent_workers,
```

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230808/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230803/PKG-INFO` & `flwr_nightly-1.5.0.dev20230808/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230803
+Version: 1.5.0.dev20230808
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230803 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230808 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.dev Requires-Python: >=3.7,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

